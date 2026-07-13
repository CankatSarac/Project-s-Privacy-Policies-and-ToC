# WITNESS — PRIVACY POLICY

**Effective Date:** May 15, 2026
**Last Updated:** May 15, 2026

---

## Introduction

Witness ("we," "us," or "our") is a mobile application that lets you have a short, voiced conversation with a simulation of yourself at age 80. The app takes a single selfie, ages it via an AI image model, briefly samples the sound of your voice to choose an appropriate premade older voice, and synthesizes spoken replies through a third-party text-to-speech service.

Because Witness processes facial imagery and voice — which can constitute **biometric or special-category personal data** under GDPR (Article 9) and several US state laws (notably the Illinois Biometric Information Privacy Act) — this Privacy Policy is written with extra care. Read Sections 1, 4, and 7 carefully before you decide whether to use the app.

If you have questions or concerns, contact us at: **cankatsarac@gmail.com**

---

## 1. WHAT WITNESS PROCESSES, AND WHERE IT GOES

### 1.1 Selfie photograph

When you accept the camera permission, the app takes a single still photograph of your face. The app then sends that photograph **once per onboarding** to an AI image-editing service (currently fal.ai, model family "fal-ai/gemini-25-flash-image/edit") to produce an aged portrait of you. The aged portrait is downloaded back to your device and cached locally; the original selfie is **not stored** on the device beyond what is needed to complete the upload, and is **not stored on our servers** (we do not operate any).

Where the photograph travels:

- Your device → fal.ai service endpoint at `fal.run` and `queue.fal.run`.
- fal.ai processes the photograph to produce the aged portrait and may store it temporarily in its own storage layer for the duration of the inference job.
- The aged portrait is returned to your device and cached on disk under the app's private storage area.

We do not control fal.ai's retention practices for transient inference data. fal.ai's terms of service and privacy policy are the authoritative source for how they handle the image once it arrives. See [https://fal.ai](https://fal.ai) for their published documentation.

### 1.2 Voice sample

When you accept the microphone permission, the app records approximately **ten seconds of your voice**. The recording is processed to detect the apparent gender of the speaker, and that gender selection is used to pick a **premade older voice** from ElevenLabs (a default voice that belongs to ElevenLabs, not your cloned voice).

**Witness does not clone your voice.** The synthesized replies you hear are spoken by ElevenLabs's stock older-voice library, not by an imitation of you. The original ten-second voice sample is held in memory long enough to perform the gender heuristic and is not retained after that.

If the future cost structure ever allows voice cloning, we will update this Privacy Policy to disclose it and require your explicit, separate consent before any cloning request is made.

### 1.3 Conversation text

The text of your conversation (your messages and the replies the future self produces) is sent to a large language model (currently GPT-4o, accessed through the Rork Toolkit relay endpoint) so that the future self can answer in context. We do **not** store the conversation transcript on our servers — see Section 6 (Retention) for what is held on your device and for how long.

### 1.4 Subscription state

If you subscribe to Witness Pro, RevenueCat receives transaction identifiers, subscription status, platform identifiers (Apple App Store or Google Play), and an anonymous RevenueCat user identifier so that your entitlement can be restored across reinstalls. RevenueCat does not receive your selfie, voice sample, conversation text, or any other in-app content.

### 1.5 What Witness does **not** collect

- We do not require you to create an account; the app has no login screen.
- We do not collect your name, email address, phone number, or contacts.
- We do not collect precise or coarse location. The `expo-location` library is bundled with our build but the app does not call any location APIs.
- We do not use advertising SDKs, advertising identifiers (IDFA / GAID), or any cross-app tracking.
- We do not use analytics SDKs (Firebase Analytics, Mixpanel, Amplitude, PostHog, etc.).
- We do not sell, rent, or share your data with data brokers.

---

## 2. HOW YOUR DATA IS STORED

What is kept on your device (in app-private local storage and the cache directory):

- The aged portrait image (a cached file URI).
- The selected premade voice ID (a string).
- The date of your last conversation (for the "return visit" experience).
- Optional bio and social-handle context if you have shared them for the Pro contextual mode.
- Notification opt-in flag.

These items remain on your device until you uninstall the app or use an in-app reset, whichever happens first.

What is **not** kept on our servers (we operate none):

- Your selfie.
- Your voice sample.
- Your conversation transcripts.
- Any identifier tied to you.

---

## 3. LEGAL BASIS FOR PROCESSING (GDPR / UK GDPR)

If you are located in the European Economic Area, the United Kingdom, or Switzerland, we process data on the following legal bases:

| Data Category | Legal Basis |
|---|---|
| Selfie photograph and ten-second voice sample (biometric / special-category data within the meaning of Article 9 GDPR, to the extent applicable) | **Explicit consent** under Article 9(2)(a) GDPR. You provide this consent affirmatively by accepting the camera and microphone permission prompts and proceeding through the onboarding screen. You may withdraw consent at any time by uninstalling the app or by using the in-app reset option, which deletes the cached aged portrait. |
| Conversation text | **Performance of a contract / your explicit request** under Article 6(1)(b) GDPR — necessary to deliver the conversational experience you initiated. |
| Subscription processing | **Performance of a contract** under Article 6(1)(b) GDPR. |

We act as the **controller** for the design of these data flows. fal.ai, ElevenLabs, OpenAI (for the GPT-4o calls via Rork), Rork (the relay), and RevenueCat act as our **processors** or as independent controllers of their own services; refer to their published terms for their own role determinations.

---

## 4. BIOMETRIC DATA — SPECIAL NOTICE

The selfie photograph and the voice recording can constitute biometric data under several frameworks:

- **GDPR / UK GDPR Article 9** — special category if used "for the purpose of uniquely identifying a natural person." Witness does not use the selfie or voice to identify or authenticate you; we use the selfie only as the input to a generative aging transformation, and the voice only to pick a premade older voice through a gender heuristic. We treat the processing as falling within Article 9 out of an abundance of caution, and we obtain explicit consent.
- **Illinois Biometric Information Privacy Act (BIPA), 740 ILCS 14** — if you are an Illinois resident, you have additional statutory rights regarding the collection and storage of biometric identifiers and biometric information.
- **Texas Capture or Use of Biometric Identifier Act, Tex. Bus. & Com. Code §503.001** — if you are a Texas resident, similar protections apply.
- **Washington's biometric law, RCW 19.375** — applies to Washington residents.

What you are consenting to:

- **Capture:** the app captures a single selfie and a ten-second voice sample on your device.
- **Use:** the selfie is sent once to fal.ai to produce an aged portrait. The voice sample is processed locally to detect apparent gender; the resulting label is used to pick a premade voice ID. The original voice sample is not retained.
- **Storage:** only the aged portrait and the selected premade voice ID are persisted on your device. The original selfie and original voice sample are not persisted.
- **Disclosure:** the selfie travels off-device to fal.ai for inference; otherwise no biometric content leaves your device.
- **Retention:** until you uninstall the app or reset within the app, the aged portrait stays cached on your device. We retain nothing.
- **Withdrawal:** you may withdraw consent at any time by uninstalling the app or resetting the session in app.

If you do not consent to biometric processing as described above, **do not proceed past the onboarding screen.**

---

## 5. THIRD PARTIES

The third-party services below are the only ones who receive any data from your use of Witness.

### 5.1 fal.ai (Image Aging)
Receives a single selfie photograph during onboarding. Used solely to produce the aged portrait. See [https://fal.ai](https://fal.ai) for their terms and privacy practices.

### 5.2 ElevenLabs (Text-to-Speech)
Receives the text of the future self's reply (not your message) and the selected premade voice ID. Returns an audio file that is played back and cached on your device. ElevenLabs receives no biometric audio from you because we do not transmit your voice sample to them. See [https://elevenlabs.io/privacy](https://elevenlabs.io/privacy).

### 5.3 Rork Toolkit (AI Relay) → OpenAI (GPT-4o)
The Rork Toolkit is a relay service that forwards the conversation text to OpenAI's GPT-4o for response generation. We have a service relationship with Rork; we do not have a direct contractual relationship with OpenAI. Refer to Rork's terms at [https://rork.com](https://rork.com) and OpenAI's API data-use terms at [https://openai.com/policies/api-data-usage-policies](https://openai.com/policies/api-data-usage-policies). Per OpenAI's policies (current at the time of writing), paid API inputs and outputs are not used to train OpenAI's models.

### 5.4 RevenueCat (Subscription Management)
Processes subscription transactions and entitlement records. Does not receive selfies, voice samples, or conversation content. See [https://www.revenuecat.com/privacy](https://www.revenuecat.com/privacy).

### 5.5 Apple App Store / Google Play
Distribution and platform billing. See [https://www.apple.com/legal/privacy/](https://www.apple.com/legal/privacy/) and [https://policies.google.com/privacy](https://policies.google.com/privacy).

### 5.6 No Other Third Parties
We do not use advertising networks, advertising identifiers, third-party analytics SDKs, social login providers, or third-party crash reporters that transmit identifiable data externally.

---

## 6. DATA RETENTION

| Item | Retention |
|---|---|
| Original selfie file | Not retained beyond the upload to fal.ai during onboarding. |
| Aged portrait | Cached on your device until you uninstall, reset within the app, or clear the app's storage. |
| Voice sample | Held briefly in memory for gender detection; not persisted. |
| Conversation text (transmitted to GPT-4o) | Not stored by us. May be retained transiently by Rork and/or OpenAI per their policies. |
| Synthesized audio replies | Cached on your device for replay. |
| Subscription records (RevenueCat) | Retained for as long as necessary to provide the subscription and meet Apple/Google billing-audit requirements, typically up to 7 years. |
| Local app preferences (bio, social handles, notification flag) | Persist on your device until uninstall or in-app reset. |

---

## 7. YOUR RIGHTS

### 7.1 Rights for All Users

- **Access:** all in-app data is visible to you in the app. We do not hold a server-side copy.
- **Delete:** uninstall the app, or use the in-app reset, to permanently delete the cached aged portrait and all local preferences.
- **Correct:** edit any bio or social-handle entries directly in the app.
- **Withdraw consent:** uninstalling the app withdraws all consents granted under Section 4.

### 7.2 EEA / UK Residents (GDPR / UK GDPR)

You additionally have the right to:

- Object to processing.
- Receive a portable copy of any data we hold about you. (In practice, we hold none beyond the RevenueCat subscription record tied to your platform receipt.)
- Lodge a complaint with your local supervisory authority (ICO in the UK, CNIL in France, BfDI in Germany, AEPD in Spain, KVKK in Türkiye, etc.).

### 7.3 California Residents (CCPA / CPRA)

California residents have the right to know, delete, correct, opt out of the sale/sharing of personal information (which we do not do), limit the use of sensitive personal information, and non-discrimination for exercising these rights.

### 7.4 Illinois, Texas, Washington Residents (Biometric Laws)

You have the additional rights described in Section 4. To exercise them, contact us at the address in Section 11.

---

## 8. CHILDREN'S PRIVACY

Witness is not directed at children under 13 years of age, and the EEA minimum is 16. We do not knowingly process biometric data of children. If you are a parent or guardian and believe your child has used the app, contact us and we will assist in deleting any locally cached content; because nothing is stored on our servers, uninstalling the app is sufficient to permanently remove the data.

---

## 9. INTERNATIONAL DATA TRANSFERS

The selfie, voice processing metadata, and conversation text may be processed in jurisdictions other than your country of residence (typically the United States and the European Union). Where transfers from the EEA / UK to a country without an adequacy decision occur via our service providers, we rely on those providers' transfer mechanisms — including the European Commission's Standard Contractual Clauses where applicable, and their participation in the EU–US Data Privacy Framework where applicable.

---

## 10. CHANGES TO THIS POLICY

We may update this Privacy Policy. Material changes — particularly any change that would broaden what biometric data is transmitted off the device, or any change in the AI provider that processes the selfie — will be communicated via an in-app notice on the next launch. The "Last Updated" date at the top reflects the most recent revision.

If a future update would introduce voice cloning of your real voice or any other materially new biometric processing, we will obtain fresh, explicit consent before performing it. Continued use of Witness after a policy update constitutes acceptance of the updated policy in respect of non-material changes only.

---

## 11. CONTACT

For privacy questions, biometric-rights requests, complaints, or any other concern:

**Controller:** Cankat Saraç (sole proprietor)
**Email:** cankatsarac@gmail.com
**Postal address:** [INSERT POSTAL ADDRESS]

We aim to respond to verified requests within 30 days.

---

*This Privacy Policy applies to the Witness mobile application available on the Apple App Store and Google Play Store.*
