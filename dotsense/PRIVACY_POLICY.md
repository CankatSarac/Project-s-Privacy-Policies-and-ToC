# DOTSENSE APP PRIVACY POLICY

**Effective Date:** April 27, 2026
**Last Updated:** April 27, 2026

## Introduction

Welcome to DotSense ("DotSense", "we", "our", or "us"). DotSense is a
mobile application that helps people learn braille through structured
lessons, flash cards, word practice, speed drills, and free typing.

This Privacy Policy explains what information we collect, how we use
it, with whom we share it, and the rights you have over your data.

By creating an account or using DotSense, you confirm that you have
read and understood this Privacy Policy.

## 1. INFORMATION WE COLLECT

### 1.1 Information you provide

You can use DotSense as a guest without creating an account. If you
choose to sign in for cloud sync, we collect:

- An account identifier from your sign-in provider (Apple ID or Google
  account user ID).
- Your email address, if your sign-in provider releases it. Apple Sign
  In may return a private relay address; we accept and store it as-is.
- A display name (optional, you can change or remove it at any time).

We do **not** ask for, collect, or store your password. Authentication
is delegated to Apple and Google; we never see your credentials.

### 1.2 Learning data

While you use DotSense we collect data that exists only because you
use the app:

- Lesson progress, completion state, and per-letter mastery scores.
- Flash card answers, word practice results, and speed drill timings.
- Daily challenge state, streak count, and activity timestamps.
- App-internal analytics events (for example: "lesson_started",
  "flash_card_answered", "speed_drill_completed") with the timestamp
  and a small set of context fields.

This data is stored under your account in Google Firebase Firestore in
a structure that only you can read or write. See section 4.

### 1.3 Information collected automatically

When you use DotSense we may automatically collect:

- Device information (device model, operating system version, app
  version, language and region).
- Approximate, IP-derived country (for service operation; we do not
  store precise location).
- Crash and performance information when the app fails or behaves
  unexpectedly.

We do not collect your precise GPS location. We do not access your
contacts, camera, microphone, photos, or health data.

### 1.4 Information we do **not** collect

- We do not run third-party advertising and we do not collect data for
  advertising purposes.
- We do not use third-party analytics SDKs that build a cross-app
  profile of you. Our analytics live inside your own Firestore
  document and are tied to your account, not to a marketing identifier.
- We do not sell your personal information.

## 2. HOW WE USE YOUR INFORMATION

We use the information described above to:

- Provide and operate the app, including authentication and cloud
  sync of your learning progress.
- Calculate streaks, mastery scores, and daily challenges.
- Diagnose crashes, fix bugs, and improve performance.
- Understand which lessons and modes are working and which need
  improvement, in aggregate.
- Communicate service updates, important changes to this Privacy
  Policy, and to respond to support requests.
- Detect and prevent fraud, abuse, and violations of our Terms of
  Service.
- Comply with legal obligations.

We do not use your learning data or progress to train external machine
learning models, and we do not share it with third parties for that
purpose.

## 3. LEGAL BASES (GDPR / UK GDPR)

If you are in the European Economic Area, the United Kingdom, or
another jurisdiction with similar laws, we rely on these legal bases:

- **Performance of a contract** when you sign in: we need your
  identifier to give you the account features.
- **Legitimate interests** for service operation, security, and
  product improvement, balanced against your rights.
- **Consent** where required (for example, for any future optional
  marketing communication, which we will explicitly ask for).
- **Legal obligation** when the law requires us to retain or disclose
  information.

You can withdraw consent or object to processing at any time
(see section 7).

## 4. WHO PROCESSES YOUR DATA (SUBPROCESSORS)

DotSense is a small operation. We use the following service providers
to run the app. They process data on our behalf and only as instructed:

- **Google Firebase (Firebase Authentication, Cloud Firestore)** —
  account authentication and cloud storage of your account document
  and learning data. Google acts as our data processor.
- **Apple App Store / Apple Sign In** — distribution and the Apple
  Sign In flow. Apple is the controller of its own services.
- **Google Play Store / Google Sign In** — distribution and the Google
  Sign In flow. Google is the controller of its own services.
- **Hosting of this Privacy Policy and our Terms of Service** —
  GitHub Pages or an equivalent static host. No personal information
  is collected by the hosting provider beyond standard server logs.

We do not use third-party advertising networks, third-party analytics
SDKs, or third-party crash-reporting SDKs at the time of this update.
If we add any in the future we will update this Privacy Policy and
notify users in-app before the new processing starts.

## 5. DATA SECURITY

We use the following measures to protect your data:

- All network traffic between the app and our backend is encrypted in
  transit (TLS 1.2+).
- Data at rest in Firebase is encrypted by Google.
- Firestore security rules restrict every document to its owner: only
  the authenticated user with the matching account ID can read or
  write their own data.
- Authentication is delegated to Apple and Google; we do not store
  passwords.
- We follow the principle of least privilege for any administrative
  access to backend systems.

No system is perfectly secure. If you believe your account has been
compromised, contact us immediately at the address in section 12.

## 6. DATA RETENTION AND DELETION

We retain your account and learning data for as long as your account
is active. If you have not signed in to DotSense for 24 months, we
may treat the account as inactive and schedule it for deletion after
notifying the email address on file (if any).

You can delete your account at any time:

- **In-app:** open the Profile tab and choose "Delete account". This
  removes your account record, all subcollections under your account,
  and your authentication record from our backend within 30 days.
- **By email:** write to the address in section 12 from the email
  address associated with your account, asking us to delete your data.

After deletion:

- Personal account data is removed from active systems within 30 days.
- Standard backups may retain copies for up to 90 days, after which
  they are overwritten in the normal backup rotation.
- Aggregated, fully-anonymized statistics that cannot be linked back
  to you may be retained.

## 7. YOUR RIGHTS

Depending on where you live you may have some or all of these rights:

- Access a copy of the personal information we hold about you.
- Correct inaccurate or incomplete information.
- Delete your account and associated data.
- Restrict or object to certain processing.
- Receive a portable copy of your data in a structured format.
- Withdraw consent for any consent-based processing.
- Lodge a complaint with your local data protection authority.

To exercise any of these rights, write to us at the address in
section 12. We will respond within 30 days. We may need to verify your
identity before acting on a request.

## 8. CHILDREN

DotSense is intended for general audiences and is rated 4+ in the
Apple App Store and "Everyone" in the Google Play Store. The content
itself is appropriate for children, but the **account features** are
not.

- The app may be used in guest mode by users of any age. No account
  is required and no personal information is sent to our servers in
  guest mode (other than device-level information automatically sent
  by app store services).
- Account creation requires the user to be at least 13 years old (or
  the minimum age of digital consent in their country, whichever is
  higher; for example, 16 in some EU member states).
- We do not knowingly collect personal information from children
  under those thresholds. If you are a parent or guardian and believe
  your child has created an account, contact us at the address in
  section 12 and we will delete the account.

## 9. INTERNATIONAL DATA TRANSFERS

Our backend (Firebase) is operated by Google and may store data in
data centers outside your country, including in the United States.
When data is transferred from the European Economic Area, the United
Kingdom, or Switzerland to a country without an adequacy decision, we
rely on Standard Contractual Clauses or equivalent safeguards offered
by Google.

## 10. CALIFORNIA PRIVACY RIGHTS (CCPA / CPRA)

If you are a California resident, you have these rights:

- **Right to know** what personal information we have collected about
  you, the categories of sources, the business purpose, and the
  categories of third parties we share it with.
- **Right to delete** personal information we have collected about
  you, subject to legal exceptions.
- **Right to correct** inaccurate personal information.
- **Right to opt out of "sale" or "sharing"** of personal information.
  We do not sell or share personal information as those terms are
  defined under California law.
- **Right to non-discrimination** for exercising your rights.

To exercise these rights, contact us at the address in section 12.

## 11. CHANGES TO THIS POLICY

We may update this Privacy Policy from time to time. When we do we
will:

- Update the **Last Updated** date at the top.
- Post the new policy at the same URL.
- For material changes, notify you in-app on next launch and, where we
  have your email address, by email.

Continued use of DotSense after a change becomes effective means you
accept the updated policy. If you do not accept the change, you can
stop using the app and delete your account.

## 12. CONTACT US

If you have questions, complaints, or requests regarding this Privacy
Policy or our handling of your personal information:

**Email:** cankatsarac@gmail.com
**Operator:** Cankat Saraç

We aim to respond to substantive requests within 30 days.

---

This Privacy Policy is effective as of the date stated above and
governs our collection, use, and disclosure of information in the
DotSense mobile application.
