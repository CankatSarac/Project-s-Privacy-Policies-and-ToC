# PLANTMEDIC — PRIVACY POLICY

**Effective Date:** May 15, 2026
**Last Updated:** May 15, 2026

---

## Introduction

PlantMedic is a mobile application that identifies common plant diseases from a photograph of the affected leaf or area and suggests treatment plans. The core disease-classification model runs **on your device** using TensorFlow Lite; treatment-plan content is sourced from a bundled SQLite database shipped with the app.

This policy explains exactly what is processed, what stays on your device, and what is transmitted elsewhere.

Contact: **cankatsarac@gmail.com**

---

## 1. ⚠️ NOT VETERINARY OR AGRICULTURAL EXPERT ADVICE

PlantMedic is informational. It is not veterinary, agronomic, agricultural-extension, or commercial-crop advice. Treatment-plan suggestions are general guidance based on a bundled reference database; they are not tailored to your soil, climate, regulations, or commercial cultivation requirements. Consult a qualified agronomist or agricultural-extension service for any commercial, regulated, or high-stakes plant-care decision.

---

## 2. WHAT WE COLLECT

### 2.1 On your device

- **Plant photographs you capture or pick** — used as input to the on-device classifier.
- **Classification results** (predicted disease label, confidence) — stored in your local SQLite database for history.
- **Treatment plan progress** (which steps you marked as done).
- **App preferences and onboarding state.**

All of the above is stored in app-private local storage on your device.

### 2.2 Cloud calls (optional)

The app's dependencies include the Rork Toolkit AI SDK. In the current build, classification runs **on-device only** through the bundled TFLite model. If a future release adds a cloud-AI fallback for difficult identifications, the app will transmit only the plant photograph (no other personal content) and we will update this Privacy Policy before activating that flow.

### 2.3 Information we do NOT collect

- No account, no login.
- No name, email, phone number, contacts, microphone, or location data despite some related libraries appearing in our dependencies.
- No advertising SDKs or advertising identifiers.
- No third-party analytics SDKs.
- No backend operated by us in the current version.
- We do not sell, rent, or trade data.

---

## 3. THIRD PARTIES

- **Apple App Store / Google Play Store** — distribution. Platform store policies apply.
- **No other third parties in the current version.** The on-device TFLite model is bundled at install time; no inference traffic leaves your device.

---

## 4. LEGAL BASIS (GDPR / UK GDPR)

| Data | Legal basis |
|---|---|
| Camera capture and photo selection | **Consent** (Art. 6(1)(a)). |
| On-device classification and history | Held on your device by you; we do not access. |

---

## 5. CHILDREN'S PRIVACY

PlantMedic is not directed at children under 13 (or under 16 in the EEA). We do not knowingly collect personal data from children.

---

## 6. YOUR RIGHTS

- **Access:** All data is on your device.
- **Delete:** Uninstall the app to permanently delete the local SQLite database and image cache. Use in-app delete for individual scans.
- **Withdraw consent for camera:** revoke permission in OS settings.
- **EEA / UK:** lodge a complaint with your local supervisory authority.
- **California (CCPA / CPRA):** know, delete, correct, opt-out of sale/sharing (we do not), limit sensitive PI use, non-discrimination.

---

## 7. RETENTION

All scan history and preferences are kept on-device until you uninstall or delete them in-app.

---

## 8. CHANGES

Material changes — particularly any change that introduces a cloud-AI call — will be communicated via in-app notice on the next launch.

---

## 9. CONTACT

**Controller:** Cankat Saraç (sole proprietor)
**Email:** cankatsarac@gmail.com
**Postal address:** [INSERT POSTAL ADDRESS]

---

*This Privacy Policy applies to the PlantMedic mobile application available on the Apple App Store and Google Play Store.*
