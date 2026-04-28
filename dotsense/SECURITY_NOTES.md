# DOTSENSE SECURITY AND COMPLIANCE NOTES

**Last Updated:** April 27, 2026
**Audience:** the operator (Cankat) and any future contributor.
**Status:** internal engineering notes, not a published legal document.

This file is the developer-side companion to PRIVACY_POLICY.md and
TERMS_OF_SERVICE.md. It captures the actions that have to be true on
the codebase and the cloud project for the published legal claims to
hold up. Treat it as a living checklist.

---

## 1. Open items that block clean publication

These need to be closed before pointing the App Store / Play Store at
the live policy URLs.

- [ ] Confirm a governing-law jurisdiction in TERMS_OF_SERVICE.md
      section 12 (replace the `[GOVERNING LAW JURISDICTION]`
      placeholder). Default options to discuss with counsel:
      - Country of residence of the operator.
      - England and Wales (broadly enforceable, common in app ToS).
      - Delaware, USA (common, but only sensible if there is a US
        legal entity).
- [ ] Decide and register the support / privacy email addresses
      (`cankatsarac@gmail.com`, `cankatsarac@gmail.com`,
      `cankatsarac@gmail.com`). If the `dotsense.app` domain is not
      yet owned, either register it or replace these with addresses
      on a domain you do own. Apple and Google will reject privacy
      contacts that bounce.
- [ ] Decide whether DotSense is operated as a sole proprietorship,
      a limited company, or under another entity. If a limited
      company exists, replace "Cankat Saraç" with the company name
      and registered address in both legal documents and in the
      App Store Connect / Play Console submission forms.
- [ ] Confirm whether iPad support is going to ship at launch. If
      yes, set `expo.ios.supportsTablet = true` in `app.json` and
      include the iPad screenshots; if no, remove the iPad
      screenshots to avoid review confusion.
- [ ] Decide whether to keep `NSUserTrackingUsageDescription` in
      `app.json`. As of this writing the project does not include
      `expo-tracking-transparency` and does not call the ATT API.
      If no SDK is going to request the ATT prompt, **remove** the
      key — leaving it in implies a tracking intent that does not
      match the privacy policy. If a future SDK needs ATT, add the
      key back at that time and update the privacy policy.

## 2. Backend posture (Firebase)

What is true today and what to keep true.

- [x] Firestore rules deny everything except per-user owned reads
      and writes (`request.auth.uid == userId`). Confirmed in
      `expo/firestore.rules`.
- [x] Account deletion is allowed from the rules so the in-app
      "Delete account" flow can run.
- [x] The `events` subcollection is append-only (`update: false`)
      and only the owner can read, create, and delete its entries.
- [ ] Add an emulator-based test for the rules (`firebase emulators:exec
      --only firestore "<rules-test-runner>"`). At minimum cover:
      - User A cannot read User B's `users/{B}` document.
      - User A cannot write to User B's `events`.
      - An anonymous request fails on every path.
      - Account-create requires `request.resource.data.uid == userId`.
      Run the suite in CI on every PR that touches `firestore.rules`.
- [ ] Add a "delete-account" Cloud Function (or admin script) that
      cascades deletion of subcollections (`events` and any future
      ones). Firestore does not cascade by itself, and the policy
      promises a 30-day deletion window. The client-side delete
      removes the parent document but can leave subcollections
      orphaned.
- [ ] Verify that Firebase Auth users are deleted alongside the
      Firestore document. The Firestore "Delete user data" extension
      (or a Cloud Function trigger on `onUserDelete`) is the cleanest
      path; pick one and document it here once installed.
- [ ] Lock the Firebase project's "Authorized domains" list to the
      domains actually used (custom auth handlers, web preview).
- [ ] Set Firestore "Time to live" policies on any future log /
      event collections that should not be retained indefinitely.
- [ ] Enable **App Check** before public launch. Without App Check,
      Firestore rules accept any authenticated client, including a
      curl script with a valid ID token. App Check forces requests
      to come from an attested copy of your app.
- [ ] Restrict the Firebase Web API key in the Google Cloud Console
      ("API restrictions" + "Application restrictions"). Even though
      Firebase web keys are not secrets, restriction limits abuse.

## 3. Mobile client posture (Expo)

- [ ] Privacy manifest (`PrivacyInfo.xcprivacy`): the `app.json`
      already includes `NSPrivacyAccessedAPITypes` for UserDefaults,
      SystemBootTime, DiskSpace, and FileTimestamp. Verify each one
      is actually used by a dependency (Expo lists them
      automatically) and that the reason codes are still the ones
      Apple expects. Re-check with `npx expo-doctor` after every
      Expo SDK upgrade.
- [ ] Apple Sign In: confirm the "Sign in with Apple" button is the
      first option offered if any third-party social login is
      offered, per Apple Guideline 4.8. As of today the only social
      logins planned are Apple and Google, which is compliant.
- [ ] Account deletion in-app: must be reachable in two taps from
      a primary screen and must actually delete (Apple Guideline
      5.1.1(v) and Play Console "Account deletion" requirement).
      Verify the button is on the Profile screen and that it
      triggers the cascading deletion described above.
- [ ] Do not log PII to the console in production. Wrap any
      `console.log` that touches the user object behind a `__DEV__`
      check, or strip them with the Babel `react-native-paper-redact`
      pattern (a simple Babel plugin that drops `console.*` in prod).
- [ ] Do not store secrets in the JS bundle. Anything bundled into
      a React Native app is extractable. Treat the Firebase web
      config as public-but-restricted. Treat anything else (server
      keys, signing secrets, third-party tokens) as off-limits.
- [ ] Use EAS Secrets (`eas secret:create`) for any build-time
      secrets, never commit `.env*` files. Add `.env*` to
      `.gitignore` if not already.
- [ ] Pin Expo SDK and React Native to known-good versions. Run
      `npx expo-doctor` and `bun audit` (or `npm audit`) on every
      release branch.
- [ ] Enable a dependency-update bot (Renovate or Dependabot)
      against the `expo/` package.json. Critical CVEs in transitive
      dependencies are the most common quiet security failure on
      Expo apps.
- [ ] Crash and error reporting: the app currently has no crash
      reporter. Decide whether to add Sentry or Crashlytics before
      a wider release. Whichever is chosen:
      - Configure it to scrub user identifiers from error reports.
      - Update PRIVACY_POLICY.md section 4 to list the new
        subprocessor before turning the SDK on for end users.

## 4. Authentication and account hygiene

- [x] No passwords are stored (Apple Sign In, Google Sign In only).
- [ ] Apple Sign In: support email-relay addresses and never
      require the user to "verify" by sending mail to the relay
      address; Apple's relay can break unverified flows.
- [ ] Implement re-authentication before destructive actions
      (delete account). Firebase requires a recent login for
      `deleteUser()`. Surface a clear "sign in again to confirm"
      step rather than swallowing the error.
- [ ] Rate limit sign-in attempts at the Firebase Auth level
      (Firebase Auth has built-in rate limiting; do not disable
      it). Watch the Firebase project quotas in production.
- [ ] Decide on a session policy: Firebase Auth refresh tokens are
      long-lived by default. For a learning app that is acceptable.
      If high-risk features are added later, force re-auth on a
      schedule.

## 5. App store privacy declarations

These are the labels that must match the policy.

### Apple App Privacy ("nutrition label")

For the launch build, declare:

- **Data Used to Track You:** none.
- **Data Linked to You:**
  - **Identifiers** — User ID (Firebase Auth UID, Apple/Google
    sub-identifier). Linked. Used for App Functionality.
  - **Contact Info** — Email address. Linked. Used for App
    Functionality. Optional (can be Apple relay).
  - **User Content** — Other User Content (lesson progress,
    drill answers). Linked. Used for App Functionality.
  - **Usage Data** — Product Interaction (analytics events).
    Linked. Used for Analytics.
  - **Diagnostics** — Crash Data, Performance Data (only if a
    crash SDK is added). Linked. Used for App Functionality.
- **Data Not Collected:** none of the other categories
  (Health, Financial, Location, Sensitive Info, Browsing
  History, Search History, Contacts, Other User Content beyond
  what is listed above).

### Google Play "Data safety" form

Mirror the above. Pay attention to the encryption-in-transit
question (yes), the data-deletion request mechanism question
(yes, in-app + email), and the third-party-sharing question
(no advertising, no analytics-vendor sharing, only Google as
the backend operator).

## 6. Incident response (small-team minimum)

- [ ] Maintain a private incident log (`incidents.md`, not in this
      repo) with date, severity, scope, mitigation, and root cause
      for any security incident that affects user data.
- [ ] If user data is exposed, applicable law may require
      notification within 72 hours (GDPR Art. 33). Have a draft
      notification ready: who is affected, what was exposed, what
      mitigation, what users should do.
- [ ] Provide a `cankatsarac@gmail.com` mailbox and monitor it.
      Add a `/.well-known/security.txt` on the web property when
      one exists.

## 7. Yearly review

- [ ] Re-read PRIVACY_POLICY.md and TERMS_OF_SERVICE.md every 12
      months and bump the "Last Updated" line if anything changed.
- [ ] Re-confirm subprocessors (currently Firebase + Apple + Google
      + GitHub Pages). Add or remove from section 4 of the privacy
      policy as needed.
- [ ] Re-run `npx expo-doctor` and audit dependencies.
- [ ] Re-verify the Firestore rules tests still pass.
- [ ] Re-check the Apple App Privacy and Google Play Data Safety
      forms against what the app actually does.

---

## Appendix A: rejection-prone things to double-check before submission

Apple and Google reject for these often:

- Privacy policy URL returns 404, redirects, or shows a parking page.
- Privacy policy URL is on a free site that injects ads (Carrd, free
  Wix tier, Notion published page that breaks for crawlers).
- Privacy policy email address bounces.
- "Account deletion" in the app is hidden behind more than two taps,
  or requires a support email and is not actually self-serve.
- The App Privacy / Data Safety form contradicts the policy text
  (e.g. policy says "no analytics" but the form declares analytics
  collection — or vice versa).
- The app uses `NSUserTrackingUsageDescription` without ever calling
  the ATT API, or calls the ATT API but does not declare tracking
  in the privacy form.
- Sign in with Apple is required for account creation but is not
  shown alongside other social sign-in options as the first option.

If the URL pattern is `https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/dotsense/PRIVACY_POLICY`,
test in an incognito window from a different network before pasting
it into App Store Connect.
