# SKINWATCH — PRIVACY POLICY

**Effective Date:** May 15, 2026
**Last Updated:** May 15, 2026

---

## Introduction

SkinWatch is a mobile application that screens a single photograph of a skin lesion against the ABCDE framework (Asymmetry, Border, Color, Diameter, Evolution) commonly used in dermatology education. The screening is performed by a multimodal AI model. **The output is not a diagnosis. It is a signal designed to help you decide whether to consult a dermatologist.**

Because SkinWatch processes images that may include identifiable skin and body areas, and because the screening relates to health, this Privacy Policy is written with extra care. Read it fully before using the App.

Contact: **cankatsarac@gmail.com**

---

## 1. ⚠️ HEALTH-DATA AND BIOMETRIC NOTICE

Photographs of skin can:

- Constitute **health-related personal data** under GDPR Article 9 to the extent they reveal information about a person's physical condition (a lesion, a possible disease).
- Constitute **biometric data** under several frameworks if the image incidentally captures features that can identify the person (face, distinctive marks).
- Be regulated under **HIPAA** in the United States if processed in certain healthcare contexts (SkinWatch is **not** a covered entity or business associate under HIPAA; do not use SkinWatch as a clinical health record).
- Be regulated under **EU MDR (Regulation (EU) 2017/745)** if marketed for a medical purpose. SkinWatch is **not** marketed as a medical device and is not CE-marked or FDA-cleared.

We treat skin photographs as sensitive special-category data and apply explicit-consent processing under Article 9(2)(a) GDPR.

---

## 2. WHAT WE PROCESS

### 2.1 Skin lesion photograph

When you accept the camera or photo-library permission and choose to scan a lesion, the photograph is sent **once per scan** to the Rork Toolkit AI relay endpoint for ABCDE screening. The relay forwards the image to an underlying multimodal AI model. The model returns ABCDE scores, a risk category (low / moderate / high / urgent), a confidence value, a plain-language summary, and short flags.

The photograph is sent only for the purpose of producing the screening output. The image itself is **not stored** on a server operated by us (we operate none beyond the relay) and is **not retained** by us after the scan completes.

### 2.2 Body area and notes (optional)

You may optionally tag the body area (e.g., "back of forearm") and add a short note (e.g., "appeared two months ago, slight itch"). This optional text is sent alongside the image to inform the screening prompt.

### 2.3 Scan history (on your device)

Each scan's image URI, ABCDE result, risk category, confidence, and timestamp are stored in your device's local storage. They are not transmitted to any backend operated by us.

### 2.4 Information we do NOT collect

- No account, no login.
- No name, email address, phone number, contacts, microphone, or location data despite some related libraries appearing in our dependencies.
- No advertising SDKs or advertising identifiers.
- No third-party analytics SDKs.
- We do not sell, rent, or trade data.

---

## 3. THIRD PARTIES

### 3.1 Rork Toolkit (AI Relay) → upstream multimodal AI model
The lesion image, body-area tag, and optional notes are transmitted to the Rork Toolkit relay endpoint, which forwards the request to a multimodal AI model (currently a Gemini- or GPT-family model, depending on Rork's configuration at request time) for ABCDE screening.

We have a service relationship with Rork; we do not have a direct contractual relationship with the underlying model provider. Refer to:
- Rork: [https://rork.com](https://rork.com)
- Google Generative AI: [https://ai.google.dev/gemini-api/terms](https://ai.google.dev/gemini-api/terms)
- OpenAI API: [https://openai.com/policies/api-data-usage-policies](https://openai.com/policies/api-data-usage-policies)

Per the published terms of these providers (current at the time of writing), paid API inputs and outputs are not used to train their models.

### 3.2 Apple App Store / Google Play Store
Distribution only.

### 3.3 No other third parties.

---

## 4. LEGAL BASIS (GDPR / UK GDPR)

| Data | Legal basis |
|---|---|
| Skin lesion photograph (health-related, special-category) | **Explicit consent** (Art. 9(2)(a) GDPR), granted when you accept the camera/photo-library permission and proceed through the scan flow. |
| Optional body-area tag and notes | **Explicit consent** (Art. 9(2)(a) GDPR). |
| Local scan history | Held on your device by you; we do not access. |

---

## 5. CONSENT WITHDRAWAL

You can withdraw consent at any time by:

- Revoking the camera and photo-library permissions in OS settings.
- Deleting individual scans within the app.
- Uninstalling the app, which permanently deletes the local scan history.

---

## 6. CHILDREN'S PRIVACY

SkinWatch is not directed at children under 13 (or under 16 in the EEA). Photographs of minors should only be submitted by a parent or legal guardian; submission by the guardian is treated as the guardian's processing of health-related data of the minor for whom they are responsible. The guardian remains solely responsible for the appropriateness of submitting such an image.

---

## 7. YOUR RIGHTS

- **Access:** all scans and history are on your device.
- **Delete:** uninstall the app, or delete individual scans in-app.
- **Withdraw consent:** revoke permissions or uninstall.
- **EEA / UK:** lodge a complaint with your local supervisory authority.
- **California (CCPA / CPRA):** know, delete, correct, opt-out of sale/sharing (we do not), limit sensitive PI use, non-discrimination.
- **Illinois / Texas / Washington biometric laws:** to the extent that an incidental face or identifying mark appears in a scan, the additional protections of BIPA, CUBI, or RCW 19.375 apply. Contact us to exercise those rights.

---

## 8. RETENTION

| Item | Retention |
|---|---|
| Lesion photograph (off-device upload) | Transient. Not retained by us. Upstream model providers may retain transient inference data per their terms. |
| Local scan history (on-device) | Until you uninstall the app or delete the scan in-app. |

---

## 9. INTERNATIONAL DATA TRANSFERS

When the screening request is processed by the upstream AI provider, transfer may occur to a jurisdiction other than your country of residence (typically the United States or the European Union). Where transfers from the EEA / UK to a country without an adequacy decision occur, we rely on the provider's Standard Contractual Clauses or equivalent safeguards.

---

## 10. CHANGES

Material changes — particularly any change in the AI provider that receives lesion images, or any change in retention behavior — will be communicated via in-app notice on the next launch.

---

## 11. CONTACT

**Controller:** Cankat Saraç (sole proprietor)
**Email:** cankatsarac@gmail.com
**Postal address:** [INSERT POSTAL ADDRESS]

---

*This Privacy Policy applies to the SkinWatch mobile application available on the Apple App Store and Google Play Store.*
