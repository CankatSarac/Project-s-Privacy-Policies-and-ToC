# COMPASS (URBAN REFUGE) — PRIVACY POLICY

**Effective Date:** May 15, 2026
**Last Updated:** May 15, 2026

---

## Introduction

Compass (originally branded "Urban Refuge") is a mobile application that helps you find nearby community services — shelter, food assistance, healthcare, legal aid, and similar resources — by location and category.

This Privacy Policy is written with extra care because the App may be used by people in vulnerable situations. Read it before using the App.

Contact: **cankatsarac@gmail.com**

---

## 1. WHY THIS POLICY MATTERS

Compass is sometimes used by people who are unhoused, displaced, undocumented, escaping violence, or otherwise in a position where data exposure could cause real harm. We have designed Compass to minimize what is collected, what is stored, and what is shared.

---

## 2. WHAT WE COLLECT

### 2.1 Your approximate location (optional)

If you grant location permission, Compass reads your device coordinates to display nearby community services. The coordinates are used **only in memory** during a session and are **not transmitted** to a server operated by us. The Supabase backend (Section 4.1) returns service listings filtered server-side using only the approximate region you query, not your precise device coordinates.

If you do not grant location permission, you can search by city, region, or service type instead.

### 2.2 Locally stored on your device

- Service bookmarks (which listings you saved for later).
- Recent searches.
- App preferences, language selection, and onboarding state.
- Cached service data for offline access.

### 2.3 Microphone (optional)

If you grant microphone permission, you can perform a voice search. The voice recording is processed for speech-to-text **on your device** where the platform permits, or sent to the operating system's transcription service. The resulting text is sent to the Supabase backend as a search query. Per the App's permission text: *"Urban Refuge uses your microphone for voice search."*

### 2.4 What we do NOT collect

- No account, no login.
- No name, email address, phone number, immigration status, citizenship status, age, gender, household composition, or any demographic detail.
- No photos or contacts.
- We do not associate your queries with any persistent identifier on our backend.
- We do not use advertising SDKs or advertising identifiers (IDFA / GAID).
- We do not use third-party analytics SDKs.
- We do not sell, rent, or trade data.

---

## 3. HOW DATA IS STORED

| Item | Where |
|---|---|
| Bookmarks, recent searches, preferences | Your device only (local storage). |
| Service listings (read-only) | Supabase backend, served to your device on request. |
| Search queries | Transient. Sent to Supabase to retrieve results, not retained against you. |

We do not store who you are. Standard Supabase server-side request logs may exist for operational purposes; see Section 4.1.

---

## 4. THIRD PARTIES

### 4.1 Supabase (Read-Only Backend)
Compass reads its directory of community services from a Supabase project operated by Cankat Saraç. The app uses a public, read-only anonymous key (`auth: { persistSession: false }`); the App does not authenticate users to the backend, so no per-user identifier is sent. Supabase may log standard server-side request metadata (IP address, timestamp, query parameters) for up to 30 days for abuse-prevention and reliability purposes. See [https://supabase.com/privacy](https://supabase.com/privacy).

### 4.2 Apple App Store / Google Play Store
Distribution only.

### 4.3 No other third parties.
We do not use Rork, OpenAI, Anthropic, Gemini, RevenueCat, Firebase, advertising networks, or third-party analytics SDKs in the current version, despite some related SDKs appearing in dependencies.

---

## 5. LEGAL BASIS (GDPR / UK GDPR)

| Data | Legal basis |
|---|---|
| Location (when granted) | **Consent** (Art. 6(1)(a) GDPR). |
| Microphone (when granted) | **Consent** (Art. 6(1)(a) GDPR). |
| Search queries to Supabase | **Performance of a contract / your explicit request** (Art. 6(1)(b) GDPR). |
| Local preferences | Held on your device by you; we do not access. |

---

## 6. SAFETY-CONSCIOUS DESIGN CHOICES

To protect users who may be in vulnerable situations:

- **No account.** You cannot be linked across sessions by anything we control.
- **No demographic intake.** We never ask whether you are unhoused, undocumented, fleeing violence, or anything similar.
- **No off-device search history.** Recent searches are kept on your device only.
- **Quick-clear.** You can clear bookmarks and recent searches in one tap.
- **Service-quality is not personalized.** The backend does not tailor results to who you are because the backend does not know who you are.

---

## 7. CHILDREN'S PRIVACY

Compass is intended for adults but may be used by minors who are themselves in a crisis. We do not knowingly collect personal data from anyone, including children. No personally identifying information is required to use the App.

---

## 8. YOUR RIGHTS

- **Access:** all local data is visible in the app.
- **Delete:** uninstall the app, or use the in-app "clear all" option.
- **Withdraw consent:** revoke location or microphone permissions in OS settings.
- **EEA / UK:** lodge a complaint with your local supervisory authority.
- **California (CCPA / CPRA):** know, delete, correct, opt-out of sale/sharing (we do not), limit sensitive PI use, non-discrimination.

---

## 9. INTERNATIONAL DATA TRANSFERS

Supabase may operate data centers outside your country of residence. Where transfers from the EEA / UK occur, we rely on Supabase's published transfer mechanisms, including Standard Contractual Clauses where applicable.

---

## 10. RETENTION

| Item | Retention |
|---|---|
| Local app data | On-device until uninstall or in-app clear. |
| Supabase server logs (operational) | Per Supabase's standard retention, typically up to 30 days. |

We retain no user-identifying data on our own systems.

---

## 11. CHANGES

Material changes are communicated via in-app notice on the next launch.

---

## 12. CONTACT

**Controller:** Cankat Saraç (sole proprietor)
**Email:** cankatsarac@gmail.com
**Postal address:** [INSERT POSTAL ADDRESS]

---

*This Privacy Policy applies to the Compass mobile application (originally branded Urban Refuge) available on the Apple App Store and Google Play Store.*
