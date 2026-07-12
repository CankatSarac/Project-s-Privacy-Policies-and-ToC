# MERIDIAN — PRIVACY POLICY

**Effective Date:** May 15, 2026
**Last Updated:** May 15, 2026

---

## Introduction

Meridian is a mobile application that calculates the exact moment of solar noon at your location and supports a daily reflection practice anchored to that moment. The app uses your location, schedules local notifications, and (when enabled) syncs reflections to a cloud backend operated by Cankat Saraç on Google Firebase.

This Privacy Policy explains exactly what is collected, where it goes, and your rights.

Contact: **cankatsarac@gmail.com**

---

## 1. WHAT WE COLLECT

### 1.1 Location data

To calculate the exact moment of solar noon at your position, the app reads your device coordinates (latitude and longitude). Per the app's in-app disclosure: *"Meridian uses your location only to calculate the exact moment of solar noon where you stand."*

What happens to your coordinates depends on whether you are signed in (see Section 2):

- **Signed out (default):** Coordinates are used in memory to compute the solar-noon time and are persisted only as part of your local app state on the device. They are not transmitted to our backend.
- **Signed in (optional cloud sync):** Coordinates may be stored in a Firebase Firestore document scoped to your user ID under `users/{uid}/locations/`, so that your noon times can be retrieved on other devices you sign in to. Each user's document is readable and writable only by that authenticated user, enforced by Firestore security rules.

### 1.2 Reflections (journal entries)

If you write a reflection, the text is stored on your device. If you have enabled cloud sync (Section 2), the reflection is also stored in your Firestore subtree at `users/{uid}/journal/`, accessible only to your authenticated user.

### 1.3 Anonymous events (pre-auth telemetry)

The app may write a small set of anonymous diagnostic events (for example, "welcome_screen_viewed", "app_opened") to a write-only Firestore collection `anonymous_events`. These events do not include your user ID, your location, or your reflections. They are write-only at the database level: even we cannot read them back from the client. They are used in aggregate to understand whether onboarding and app-open flows are functioning.

### 1.4 Authentication and entitlement state

If you sign in (Firebase Authentication), we store the email address or auth identifier supplied by your sign-in method (e.g., Apple Sign In private relay address). If you subscribe to Meridian Plus, an entitlement record is stored at `users/{uid}/entitlements/`.

### 1.5 Notifications

If you opt in, Meridian schedules local notifications to alert you near solar noon. The app does not send push notifications from a server in the current version.

### 1.6 What we do NOT collect

- No name (unless you provide one in your auth provider's account).
- No contacts, photos, microphone, or camera.
- No advertising SDKs or advertising identifiers (IDFA / GAID).
- No third-party analytics SDKs (Firebase Analytics is **not** enabled in this app; the `anonymous_events` collection is our own write-only diagnostic stream).
- We do not sell, rent, or trade data.

---

## 2. CLOUD SYNC AND HOW DATA IS STORED

The app supports **two modes**:

- **Local-only mode** (default for users who do not sign in): all reflections and locations remain on your device.
- **Cloud-sync mode** (when you sign in via Firebase Authentication): reflections, locations, and entitlement records are mirrored to a Firestore subtree owned by your authenticated user (`users/{uid}/{...}`). Firestore security rules guarantee that only the authenticated user with that UID can read or write that subtree.

You can sign out at any time. Signing out stops further sync but does not delete already-synced cloud records. To delete cloud records, see Section 6 (Your Rights).

---

## 3. LEGAL BASIS (GDPR / UK GDPR)

| Data | Legal basis |
|---|---|
| Location (in-memory calculation, signed out) | **Consent** (Art. 6(1)(a) GDPR) — granted when you accept location permission. |
| Location and reflections (cloud sync, signed in) | **Performance of a contract** (Art. 6(1)(b) GDPR) — to deliver the cross-device sync you signed up for. |
| Authentication identifier | **Performance of a contract** (Art. 6(1)(b) GDPR). |
| Anonymous events | **Legitimate interest** (Art. 6(1)(f) GDPR) — operational telemetry, not associated with any user identifier. |

---

## 4. THIRD PARTIES

### 4.1 Google Firebase (Cloud Backend)
Firebase Authentication, Firestore, and related infrastructure operated by Google. Acts as our processor for personal data stored under your authenticated user subtree. See [https://firebase.google.com/support/privacy](https://firebase.google.com/support/privacy) and Google's standard data processing terms.

### 4.2 Apple Sign In / Google Sign In
If you sign in, the auth provider you choose is the controller of its own sign-in flow. Your sign-in identifier (or Apple Private Relay email) is shared with us to maintain your account in Firebase Authentication.

### 4.3 Apple App Store / Google Play Store
Distribution and platform billing.

### 4.4 No other third parties
The current version does not call Rork, OpenAI, Anthropic, Gemini, ElevenLabs, fal.ai, RevenueCat, Supabase, or any advertising or third-party analytics service.

---

## 5. CHILDREN'S PRIVACY

Meridian is not directed at children under 13 (or under 16 in the EEA without verifiable parental consent). We do not knowingly collect personal data from children. If you are a parent or guardian and believe your child has signed in, please contact us and we will delete the account and any associated data.

---

## 6. YOUR RIGHTS

- **Access:** locally stored data is visible in the app. For your Firestore subtree, you can export reflections via in-app export (where available) or by contacting us.
- **Delete:** uninstall the app to remove local data. To delete your cloud records, use the in-app "Delete account" option, or email cankatsarac@gmail.com. Account deletion removes your `users/{uid}/...` subtree and your Firebase Authentication record within 30 days.
- **Correct:** edit your reflections directly in the app.
- **Withdraw consent for location:** revoke location permission in OS settings.
- **EEA / UK:** lodge a complaint with your local supervisory authority.
- **California (CCPA / CPRA):** know, delete, correct, opt-out of sale/sharing (we do not sell or share), limit sensitive PI use, non-discrimination.

---

## 7. DATA SECURITY

- All Firebase traffic is encrypted in transit (TLS 1.2+).
- Firestore data is encrypted at rest by Google.
- Firestore security rules restrict every user's documents to that user only.
- Authentication is delegated to Apple, Google, or other sign-in providers; we do not store passwords.

---

## 8. INTERNATIONAL DATA TRANSFERS

Firebase operates data centers globally, including in the United States. Where data is transferred from the EEA / UK to a country without an adequacy decision, we rely on Google's Standard Contractual Clauses (Article 46 GDPR) or equivalent safeguards.

---

## 9. RETENTION

| Item | Retention |
|---|---|
| Local app data | On-device until uninstall. |
| Firestore user subtree | Until you delete your account or request deletion. |
| Firebase Authentication record | Until you delete your account. Inactive accounts (no sign-in for 24 months) may be flagged for deletion notice. |
| Anonymous events | Up to 365 days for operational analysis; not linked to any user identifier. |

---

## 10. CHANGES

Material changes are communicated via in-app notice on the next launch and by email where we have your email address.

---

## 11. CONTACT

**Controller:** Cankat Saraç (sole proprietor)
**Email:** cankatsarac@gmail.com
**Postal address:** [INSERT POSTAL ADDRESS]

---

*This Privacy Policy applies to the Meridian mobile application available on the Apple App Store and Google Play Store.*
