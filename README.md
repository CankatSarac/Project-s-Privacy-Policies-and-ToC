# Project Legal Documents

Central home for the privacy policies and terms of service of apps
built by **Cankat Saraç**. Each subfolder is one app. Each app has its
own `PRIVACY_POLICY.md` and `TERMS_OF_SERVICE.md`.

## Apps

### Pledge

Personal habit-tracking and goal-keeping app.

- [Privacy Policy](./pledge/PRIVACY_POLICY.md)
- [Terms of Service](./pledge/TERMS_OF_SERVICE.md)

### NameStory

Name-discovery app that returns demographic predictions, meaning, and cultural context for any first name.

- [Privacy Policy](./namestory/PRIVACY_POLICY.md)
- [Terms of Service](./namestory/TERMS_OF_SERVICE.md)

### Socrates Pocket

Reflective self-inquiry app that asks Socratic questions — never gives answers. No accounts, local-only storage, AI-generated questions.

- [Privacy Policy](./socrates-pocket/PRIVACY_POLICY.md)
- [Terms of Service](./socrates-pocket/TERMS_OF_SERVICE.md)

### The Stranger

Travel companion / fictional encounter app. See policies for current data flows.

- [Privacy Policy](./the-stranger/PRIVACY_POLICY.md)
- [Terms of Service](./the-stranger/TERMS_OF_SERVICE.md)

### DotSense

Braille learning app: structured lessons, flash cards, word practice, speed drills, and free typing. Optional Apple / Google sign-in for cloud sync via Firebase. No advertising, no third-party analytics SDK.

- [Privacy Policy](./dotsense/PRIVACY_POLICY.md)
- [Terms of Service](./dotsense/TERMS_OF_SERVICE.md)
- [Security & compliance notes](./dotsense/SECURITY_NOTES.md) (internal)

### Finite

Mortality-awareness app that generates a personalized statistical estimate of remaining days of life based on actuarial tables, date of birth, biological sex, country, lifestyle factors, and self-reported medical conditions. All health data is stored exclusively on-device (no backend). Includes daily reflection journaling, letters to loved ones, family countdown, and home screen widgets. Premium subscription managed via RevenueCat.

**⚠️ Contains special-category health data under GDPR. No data leaves the user's device. Strong medical disclaimer required.**

- [Privacy Policy](./finite/PRIVACY_POLICY.md)
- [Terms of Service](./finite/TERMS_OF_SERVICE.md)

### The Last Page (endpage)

Personal reading library that preserves the closing line of every book you finish. You photograph the last page, an AI vision model identifies the book (title and author only), Open Library returns canonical metadata, and you write the final sentence and feeling that mattered. All sentences, feelings, photos, and shelves are stored exclusively on-device. The single off-device transmission is the last-page photo sent once for identification — the user's sentence and feeling never leave the device. Premium subscription (monthly, annual, lifetime) managed via RevenueCat.

**Sends one image per book to a third-party AI vision service (Google Gemini via Rork Toolkit) for identification. Disclosed in Privacy Policy §4.1. No analytics, no advertising SDKs, no account.**

- [Privacy Policy](./endpage/PRIVACY_POLICY.md)
- [Terms of Service](./endpage/TERMS_OF_SERVICE.md)

### Witness

A short conversation with a simulation of your 80-year-old future self. Takes a single selfie and a 10-second voice sample; the selfie is sent once to fal.ai for image aging, and the voice sample is processed on-device for apparent-gender detection (used to pick a premade ElevenLabs older voice — no voice cloning). Conversation text is sent to GPT-4o via the Rork Toolkit. Premium subscription managed via RevenueCat.

**⚠️ Processes biometric data (face image, voice sample). GDPR Article 9 / BIPA / CUBI / RCW 19.375 disclosures included. Explicit consent flow required at onboarding.**

- [Privacy Policy](./witness/PRIVACY_POLICY.md)
- [Terms of Service](./witness/TERMS_OF_SERVICE.md)

### Waypoint

Supply-chain risk-alert app. Delivers classified alerts (port closures, geopolitical events, weather, shortages, cyber, labor) sourced from public news/data. Backend operated by Cankat Saraç stores email address (for digest emails) and push token (for notifications). No commercial data uploaded by users.

- [Privacy Policy](./waypoint/PRIVACY_POLICY.md)
- [Terms of Service](./waypoint/TERMS_OF_SERVICE.md)

### Tide — Ocean Breathing

Ocean-paced breathing companion. Optionally uses approximate location to find the nearest coast; pulls live wave data from the public Open-Meteo Marine API. No backend operated by us. No accounts.

- [Privacy Policy](./tide/PRIVACY_POLICY.md)
- [Terms of Service](./tide/TERMS_OF_SERVICE.md)

### WikiChess

Single-player puzzle game: navigate Wikipedia by clicking inline links to reach a target article. Reads Wikipedia REST + MediaWiki Action API. No accounts, no backend, no analytics, no AI.

- [Privacy Policy](./wikichess/PRIVACY_POLICY.md)
- [Terms of Service](./wikichess/TERMS_OF_SERVICE.md)

### Untold

AI-assisted apology composer. Two modes: apologies you'll send today (5 tonal tiers) and apologies you'll never deliver. Draft text is sent to the Rork Toolkit AI relay; output is shown in the app and optionally saved locally. Premium subscription managed via RevenueCat.

- [Privacy Policy](./untold/PRIVACY_POLICY.md)
- [Terms of Service](./untold/TERMS_OF_SERVICE.md)

### Chronicle

Historical timeline trivia in themed packs. Daily challenges, streaks, achievements, weekly tournament. Premium content via Chronicle Pass (RevenueCat). No backend operated by us beyond entitlement.

- [Privacy Policy](./chronicle/PRIVACY_POLICY.md)
- [Terms of Service](./chronicle/TERMS_OF_SERVICE.md)

### Mind the Lane

Three-lane memory-practice runner for iOS. Gameplay history, personal trends, settings, and generated result cards are processed on-device. No account, backend, advertising, analytics, or tracking in the current release. The folder retains the project's legacy `emoji-lane-run` slug so existing public links remain stable.

- [Privacy Policy](./emoji-lane-run/PRIVACY_POLICY.md)
- [Terms of Service](./emoji-lane-run/TERMS_OF_SERVICE.md)

### Glow — Kindness Map

Map-based journal of small acts of kindness. Optional location and photo attachment per entry. All entries stored on-device. No accounts, no backend, no analytics, no AI in current version.

- [Privacy Policy](./glow/PRIVACY_POLICY.md)
- [Terms of Service](./glow/TERMS_OF_SERVICE.md)

### MathStory

Interactive math stories in a fictional kingdom. Designed to be safe for child users — no account, no personal information collected, no advertising, no third-party SDKs in current version.

**⚠️ Possibly child-directed audience. COPPA / GDPR Art. 8 considerations included.**

- [Privacy Policy](./mathstory/PRIVACY_POLICY.md)
- [Terms of Service](./mathstory/TERMS_OF_SERVICE.md)

### Meridian

Solar-noon calculator with daily reflection practice. Uses location to compute solar noon. Optional cloud sync via Firebase Authentication + Firestore for users who sign in (reflections and locations are stored under their own UID with security-rule isolation). Local notifications, no push server.

- [Privacy Policy](./meridian/PRIVACY_POLICY.md)
- [Terms of Service](./meridian/TERMS_OF_SERVICE.md)

### Blink — One Sec Video

One-second daily video capture, assembled into a time-lapse year. Clips stored on-device only. No accounts, no backend, no analytics, no AI in current version.

**Captures camera video, which is biometric content kept on-device. User-shared clips are user's responsibility.**

- [Privacy Policy](./blink/PRIVACY_POLICY.md)
- [Terms of Service](./blink/TERMS_OF_SERVICE.md)

### PlantMedic

Plant-disease identification with on-device TensorFlow Lite classifier and bundled treatment-plan database (SQLite). All inference is on-device in the current version; no cloud AI calls.

**⚠️ Informational only. Not agronomic, veterinary, medical, or regulatory advice. Strong disclaimer for pesticide/herbicide use.**

- [Privacy Policy](./plantmedic/PRIVACY_POLICY.md)
- [Terms of Service](./plantmedic/TERMS_OF_SERVICE.md)

### SkinWatch

Skin-lesion screening using the ABCDE framework. Photo sent once per scan to the Rork Toolkit relay → upstream multimodal AI model. Returns screening output only, not a diagnosis. Scan history stored locally on device.

**⚠️ Health-related and biometric data. GDPR Article 9 / HIPAA-related notice / MDR / FDA disclaimers required. Explicit consent flow at scan time. Strong medical disclaimer.**

- [Privacy Policy](./skinwatch/PRIVACY_POLICY.md)
- [Terms of Service](./skinwatch/TERMS_OF_SERVICE.md)

### Compass (Urban Refuge)

Directory of nearby community services (shelter, food, healthcare, legal aid, etc.). Reads from a Supabase read-only backend with no per-user identifier. Optional location and microphone (voice search). Designed for vulnerable users — no account, no demographic intake, no off-device search history.

**Vulnerable-user audience. Designed for minimal data collection.**

- [Privacy Policy](./compass/PRIVACY_POLICY.md)
- [Terms of Service](./compass/TERMS_OF_SERVICE.md)

### Face Recall

Memory practice game for learning names and faces: study packs, timed recall tests, streaks, and personal trend reports. Custom face packs are built from photos chosen on-device and are never uploaded. Pro subscription via StoreKit (Apple). Optional Game Center leaderboard. No advertising, no third-party analytics SDK.

- [Privacy Policy](./face-recall/PRIVACY_POLICY.md)
- [Terms of Service](./face-recall/TERMS_OF_SERVICE.md)

### Emoji Lane Run

Local-first memory practice game with optional household profiles. Gameplay is stored on-device; no user account and no application backend.

- [Privacy Policy](./emoji-lane-run/PRIVACY_POLICY.md)
- [Terms of Service](./emoji-lane-run/TERMS_OF_SERVICE.md)

### Sediment

Local-first reflective game and breathing/attention companion. Gameplay, observations, and time capsules are stored on the device.

- [Privacy Policy](./sediment/PRIVACY_POLICY.md)
- [Terms of Service](./sediment/TERMS_OF_SERVICE.md)

### Spot the Swap

Local-first visual comparison and brain-training game. No user account and no application backend.

- [Privacy Policy](./spot-the-swap/PRIVACY_POLICY.md)
- [Terms of Service](./spot-the-swap/TERMS_OF_SERVICE.md)

## How these are hosted

These documents are served as a public static site via GitHub Pages
(or an equivalent host). App Store Connect and Google Play Console
require publicly reachable URLs in every store listing, and the live
URLs for each app are set in that app's store submission.

Typical URL pattern once GitHub Pages is enabled on this repo:

```
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/pledge/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/pledge/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/namestory/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/namestory/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/socrates-pocket/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/socrates-pocket/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/the-stranger/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/the-stranger/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/dotsense/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/dotsense/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/finite/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/finite/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/endpage/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/endpage/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/witness/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/witness/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/waypoint/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/waypoint/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/tide/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/tide/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/wikichess/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/wikichess/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/untold/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/untold/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/chronicle/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/chronicle/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/glow/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/glow/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/mathstory/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/mathstory/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/meridian/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/meridian/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/blink/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/blink/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/plantmedic/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/plantmedic/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/skinwatch/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/skinwatch/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/compass/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/compass/TERMS_OF_SERVICE
```

To enable GitHub Pages on this repo:

1. Push this repo to GitHub if not already pushed.
2. On GitHub, go to the repo → **Settings** → **Pages**.
3. Set **Source** to **Deploy from a branch**.
4. Pick **main** (or your default branch) and **/ (root)** folder.
5. Save. Within a minute or two the URLs above resolve.

## Adding a new app

1. Create a new subfolder named after the app, lowercase and hyphenated (e.g. `myapp/`).
2. Drop in `PRIVACY_POLICY.md` and `TERMS_OF_SERVICE.md`, mirroring the
   structure of the existing `endpage/` or `finite/` folders.
3. Update this README with a link to the new app's documents.
4. Commit and push.

## Maintenance

Every legal document in this repository includes an **Effective Date**
and **Last Updated** line at the top. Bump both of them whenever a
document is edited, and notify affected app users through in-app
messaging or email on their next app launch.

Review each document at least once a year regardless of whether
anything has changed.

## Known follow-ups (engineer / counsel review)

The following items were flagged during the May 2026 build-out and should be
reviewed by a qualified attorney in the operator's jurisdiction before any
App Store submission relies on them:

1. **Postal address:** Several policies include `[INSERT POSTAL ADDRESS]`
   placeholders next to the controller contact. Replace with the real
   address required by GDPR Art. 13(1)(a), KVKK Aydınlatma Yükümlülüğü
   Tebliği, and (where applicable) the German Telemediengesetz
   Impressum requirement.
2. **Governing law and arbitration clauses:** All policies elect the
   Republic of Türkiye and ISTAC for non-EU / non-UK users. Confirm with
   counsel that this election is appropriate and enforceable for each
   target market.
3. **Locally drifted i18n content (Socrates Pocket):** The Socrates
   Pocket website previously served localized policy stubs via
   `next-intl` message files in 10 languages. The English routes have
   been rebound to render the canonical `socrates-pocket/PRIVACY_POLICY.md`
   and `socrates-pocket/TERMS_OF_SERVICE.md`. Non-English translations
   should be re-generated from these canonical sources before launching
   non-English locales.
4. **Cloud sync promise (endpage):** The endpage App Store listing copy
   advertises "cloud sync across iPhone and iPad" as a Premium feature,
   but cloud sync is not implemented in the current `endpage-library-mobile`
   codebase. Either ship the feature, defer the marketing claim, or qualify
   it as "coming soon" before submitting to Apple — a refund-risk under
   EU Unfair Commercial Practices Directive otherwise.
5. **Witness — biometric consent UI:** The Witness policy describes explicit
   consent for biometric processing. Confirm that the app's onboarding screen
   actually presents the required affirmative-consent UI (BIPA / CUBI /
   RCW 19.375) before submitting the first US build.
6. **SkinWatch — medical-device classification:** The SkinWatch policy
   states the app is not a medical device. Confirm with counsel that the
   App Store listing copy and any marketing materials match this position
   in every market (FDA, MDR, MHRA).
7. **MathStory — child-audience submission:** If MathStory will be
   submitted to the App Store's "Made for Kids" category or Google Play
   Designed for Families, additional disclosures and the Apple Kids
   Category requirements apply beyond what this policy covers.
8. **Compass / Supabase — server-log retention:** Confirm the Supabase
   project's actual server-log retention matches the "up to 30 days"
   statement in the Compass Privacy Policy.
