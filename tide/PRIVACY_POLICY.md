# TIDE — OCEAN BREATHING — PRIVACY POLICY

**Effective Date:** May 15, 2026
**Last Updated:** May 15, 2026

---

## Introduction

Tide is a mobile application that guides your breathing to the rhythm of the real ocean. The app calculates tidal phases, optionally pulls live marine data from a public weather API, and animates a breathing pace that matches the wave action at the nearest coast.

This policy explains what data we use, where it goes, and your rights.

Contact: **cankatsarac@gmail.com**

---

## 1. WHAT TIDE USES

### 1.1 Your approximate location (optional)

If you grant location permission, Tide reads your device coordinates (latitude and longitude). The coordinates are used **only on your device** to find the nearest coastline point from a bundled list of named coasts shipped with the app. The coordinates themselves are not stored on our servers; only the resulting **selected coast identifier** (e.g., `pt-lisbon`) is persisted on your device.

If you do not grant location permission, Tide uses a curated default coast (Lisbon, Portugal). The app remains fully usable without location.

### 1.2 Coast and breathing preferences

Saved locally on your device:

- Selected coast identifier.
- Breathing pace preference, theme preference, reduce-motion preference.
- Recent breathing sessions for streak counting.

### 1.3 What we do **not** collect

- No account, no login, no email address.
- No name, phone number, contacts, photos, microphone, or camera access.
- No advertising SDKs or identifiers.
- No analytics SDKs (Firebase, Mixpanel, Amplitude, PostHog, etc.).
- No backend operated by us — we have no servers that hold user data.

---

## 2. HOW DATA IS STORED

All preferences and session history are stored exclusively on your device using local storage. We do not have a backend; uninstalling the app permanently deletes all data.

---

## 3. THIRD-PARTY DATA SOURCES

### 3.1 Open-Meteo Marine API
For live wave and swell data near your selected coast, the app calls the public **Open-Meteo Marine API** at `marine-api.open-meteo.com`. Open-Meteo is a free public weather API that does not require an API key or account. The app sends only the latitude and longitude of the **selected coast** (not necessarily your device location — a coastline point) and receives wave data in response. Open-Meteo's privacy policy: [https://open-meteo.com/en/terms](https://open-meteo.com/en/terms).

If you have explicit location permission granted and the nearest coast is within 500 km, the coastline lat/lon used in the API call corresponds to a curated coastline point near you, not your precise device location.

As with any HTTP request, your IP address is visible to Open-Meteo's servers.

### 3.2 Apple App Store / Google Play Store
Distribution only. See their privacy policies.

### 3.3 No other third parties
We do not use Rork, Anthropic, OpenAI, Google Gemini, ElevenLabs, or any other AI provider in the current version, despite some related SDKs being present in the codebase.

---

## 4. LEGAL BASIS (GDPR / UK GDPR)

| Data | Legal basis |
|---|---|
| Approximate location (when granted) | **Consent** (Art. 6(1)(a) GDPR) and **performance of your request** (Art. 6(1)(b)). |
| Marine API request to Open-Meteo | **Legitimate interest** (Art. 6(1)(f)) — providing the breathing rhythm you asked for. |

---

## 5. CHILDREN'S PRIVACY

Tide is suitable for general audiences but is not directed at children under 13 (or 16 in the EEA). We do not knowingly collect personal data from anyone. Since the app stores nothing on our servers, you can permanently delete all locally stored data by uninstalling the app.

---

## 6. YOUR RIGHTS

- **Access:** All data is on your device and visible in the app.
- **Delete:** Uninstall the app, or use the in-app reset, to permanently clear preferences and session history.
- **Withdraw consent for location:** Revoke location permission in your OS settings at any time. The app continues to work using the curated default coast.
- **Lodge a complaint** (EEA / UK residents) with your local supervisory authority.
- **California (CCPA / CPRA):** rights to know, delete, correct, opt out of sale/sharing (we do not sell or share), limit sensitive PI use (we collect none), and non-discrimination.

---

## 7. RETENTION

| Item | Retention |
|---|---|
| Coast / preference / session data | On-device until uninstall or in-app reset. |
| Marine API requests | Transient. Not retained by us. Refer to Open-Meteo for their retention. |

---

## 8. CHANGES

Material changes are communicated via in-app notice on the next launch.

---

## 9. CONTACT

**Controller:** Cankat Saraç (sole proprietor)
**Email:** cankatsarac@gmail.com
**Postal address:** [INSERT POSTAL ADDRESS]

---

*This Privacy Policy applies to the Tide — Ocean Breathing mobile application available on the Apple App Store and Google Play Store.*
