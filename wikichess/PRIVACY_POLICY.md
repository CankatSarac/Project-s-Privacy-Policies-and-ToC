# WIKICHESS — PRIVACY POLICY

**Effective Date:** May 15, 2026
**Last Updated:** May 15, 2026

---

## Introduction

WikiChess is a mobile puzzle game where you navigate Wikipedia by clicking inline links to reach a target article in as few hops as possible. Daily challenges, streaks, and duels included.

This Privacy Policy explains what we use, where it goes, and your rights.

Contact: **cankatsarac@gmail.com**

---

## 1. WHAT WE COLLECT

### 1.1 Information stored locally on your device

- Match history (challenges played, hop counts, completion times).
- Personal-best statistics and streak count.
- Daily-challenge state.
- App preferences and onboarding state.

All of the above is stored in app-private local storage on your device. No account is required.

### 1.2 Information we do NOT collect

- We do not require you to create an account; there is no login.
- We do not collect your name, email address, phone number, contacts, photos, microphone audio, camera images, or any sensor data.
- We do not collect location data despite some related libraries appearing in our dependencies.
- We do not use advertising SDKs or advertising identifiers (IDFA / GAID).
- We do not use third-party analytics SDKs that transmit identifiable events. The app contains a local analytics scaffold (`analytics.ts`) which logs events to the developer console in development mode and is a no-op in production. **No production telemetry is transmitted in the current version.**
- We do not sell, rent, or trade any data.
- We do not operate a backend that holds user data.

---

## 2. THIRD-PARTY DATA SOURCES

### 2.1 Wikipedia (Wikimedia Foundation)

The core gameplay loop loads article content and links from Wikipedia's public REST API and MediaWiki Action API at `en.wikipedia.org`. The app sends article titles and standard MediaWiki query parameters and receives article content (titles, extracts, links, thumbnails). As with any HTTP request, your IP address is visible to Wikimedia's servers. See the [Wikimedia Foundation Privacy Policy](https://foundation.wikimedia.org/wiki/Policy:Privacy_policy) for their handling of request metadata.

### 2.2 Apple App Store / Google Play Store

Distribution only. Platform store policies apply.

### 2.3 No other third parties

We do not use Rork, Anthropic, OpenAI, Google Gemini, ElevenLabs, fal.ai, RevenueCat, Firebase, Supabase, or any other backend or AI service in the current version of WikiChess.

---

## 3. LEGAL BASIS (GDPR / UK GDPR)

| Data | Legal basis |
|---|---|
| Local match history and preferences | Held on your device by you; we do not access or process. |
| Wikipedia article requests | **Legitimate interest** (Art. 6(1)(f) GDPR) — providing the gameplay you requested. |

---

## 4. CHILDREN'S PRIVACY

WikiChess is suitable for general audiences. Wikipedia content can include topics that may not be suitable for very young children, depending on the article they navigate to. Parental discretion is advised. We do not knowingly collect personal data from anyone, including children. Since we have no backend, you can permanently delete all locally stored data by uninstalling the app.

---

## 5. YOUR RIGHTS

- **Access:** All data is on your device and visible in the app.
- **Delete:** Uninstall the app, or use the in-app reset, to permanently clear match history and preferences.
- **Lodge a complaint** (EEA / UK residents) with your local supervisory authority.
- **California residents (CCPA / CPRA):** rights to know, delete, correct, opt out of sale/sharing (we do not sell or share), limit sensitive PI use (we collect none), and non-discrimination.

---

## 6. RETENTION

| Item | Retention |
|---|---|
| Match history and preferences | On-device until uninstall or in-app reset. |
| Wikipedia API requests | Transient. Not retained by us. Refer to Wikimedia for their retention. |

---

## 7. CHANGES

Material changes are communicated via in-app notice on the next launch.

---

## 8. CONTACT

**Controller:** Cankat Saraç (sole proprietor)
**Email:** cankatsarac@gmail.com
**Postal address:** [INSERT POSTAL ADDRESS]

---

*This Privacy Policy applies to the WikiChess mobile application available on the Apple App Store and Google Play Store.*
