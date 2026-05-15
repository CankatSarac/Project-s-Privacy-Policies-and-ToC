# THE LAST PAGE — PRIVACY POLICY

**Effective Date:** May 15, 2026
**Last Updated:** May 15, 2026

---

## Introduction

The Last Page ("we," "us," or "our") is a mobile application that helps you preserve the closing words of every book you finish. You take a photograph of the last page, the app identifies the book, and you write down the final sentence that mattered. Your library of endings builds itself, ending by ending.

We take privacy seriously, and this app was designed around a single principle: **the words and feelings you write down for each book are sacred and never leave your device.** This Privacy Policy explains exactly what data is processed, where it lives, what is and is not sent off your device, and what rights you have over it.

If you have questions or concerns, contact us at: **cankatsarac@gmail.com**

---

## 1. DATA WE COLLECT AND WHY

### 1.1 Data You Create While Using the App

| Data | Purpose | Storage |
|------|---------|---------|
| **Final sentence** you save for each book | The core experience — your private record of the words that mattered | **On-device only** |
| **Feeling / note** you save for each book | Your private reflection on the ending | **On-device only** |
| **Photograph of the last page** of each book | Visual record, plus single-use input to the book identification service (see Section 4.1) | **On-device only** (a temporary copy is sent for identification — see 4.1) |
| **Book metadata** (title, author, cover, Open Library identifier) | Build your shelf, display book covers | **On-device only** |
| **Finished-at timestamp** for each ending | Order your shelf chronologically | **On-device only** |
| **App preferences and onboarding state** | Personalization and navigation | **On-device only** |
| **Notification opt-in flag** | Decide whether to schedule the biweekly local reminder | **On-device only** |
| **Premium subscription status** | Feature gating (managed by RevenueCat — see Section 4.2) | **On-device** cache; **on RevenueCat** for entitlement record |

### 1.2 Data We Do NOT Collect

- We do not collect your name, email address, phone number, or any account credentials. The app has no login.
- We do not collect or use precise GPS or coarse location, despite any platform-permission entry. The app does not call location APIs.
- We do not collect biometric data.
- We do not collect contacts.
- We do not use advertising SDKs, advertising identifiers, or ad networks.
- We do not use analytics SDKs (Firebase Analytics, Mixpanel, Amplitude, Segment, PostHog, etc.).
- We do not run crash-reporting tools that transmit identifiable data to third-party servers.
- We do not share, sell, or rent your data to anyone.

---

## 2. HOW YOUR DATA IS STORED

**All of the personal content described in Section 1.1 — your sentences, your feelings, the photographs of your last pages, your book list, and your settings — is stored exclusively on your device using local storage (AsyncStorage on iOS and Android). It is never transmitted to our servers (we do not run any), never uploaded to the cloud, and never synchronized across devices.**

This architecture means:
- **No account is required** to use The Last Page.
- **No data breach on our servers** can expose your library, because we hold none of it.
- **We cannot read your sentences, feelings, or photos**, even if legally compelled, because we do not possess them.
- **Uninstalling the app permanently deletes all your data.**

The only exceptions, both narrow, are described in Sections 4.1 (book identification) and 4.2 (subscription processing).

---

## 3. LEGAL BASIS FOR PROCESSING (GDPR / UK GDPR)

If you are located in the European Economic Area (EEA), the United Kingdom, or Switzerland, we process data under the following legal bases:

| Data Category | Legal Basis |
|---------------|-------------|
| Sentences, feelings, photos stored on your device | You act as the sole data subject and sole controller of this data on your own device. We do not process it. |
| Book identification request (photo sent once for AI identification) | **Performance of a contract / your explicit request** (Article 6(1)(b) GDPR) — necessary to provide the identification feature you triggered |
| Open Library metadata queries | **Legitimate interest** (Article 6(1)(f) GDPR) — providing the book lookup you requested, with no personal data transmitted |
| Premium subscription | **Performance of a contract** (Article 6(1)(b) GDPR) — required to deliver the subscription you purchased |

---

## 4. THIRD PARTIES

The Last Page deliberately keeps third-party processing to the minimum needed to deliver the features you trigger. The third parties below are the only ones who ever receive any data related to your use of the app.

### 4.1 Book Identification — AI Vision Service (Rork Toolkit / Google Gemini)

When you take or pick a photograph of the last page of a book, the app sends **only that photograph** to an AI vision model (currently Google Gemini 2.5 Flash, accessed through the Rork Toolkit hosted endpoint) for the sole purpose of identifying the book's title and author. The model is invoked **once per book** and is given a strict instruction to return only `{title, author, confidence}` as JSON.

What is sent:
- The photograph of the last page (as a temporary base64-encoded image in the API request body).

What is **NEVER** sent:
- Your saved sentence.
- Your saved feeling or note.
- Any other ending, book, or library content.
- Any identifier tied to you (no account, no email, no device ID is passed in the request body).

The response (title, author, confidence) is used only to look up canonical metadata in Open Library and is then discarded.

Note: As with any HTTP request, the underlying network connection exposes your IP address to the receiving server. We do not control how the upstream model provider handles transient inference data; you should treat their policies as the authoritative reference for how the photograph is processed once it arrives:

- Rork Toolkit: see [https://rork.com](https://rork.com) for the operator's published terms.
- Google Gemini API: [https://ai.google.dev/gemini-api/terms](https://ai.google.dev/gemini-api/terms) and [https://policies.google.com/privacy](https://policies.google.com/privacy).

If you do not wish to send any photograph to an AI service, you may identify books manually via title search instead of using the camera capture flow.

### 4.2 RevenueCat (Subscription Management)

The Last Page uses **RevenueCat** to manage in-app subscriptions and entitlements. When you start a free trial or purchase a premium subscription, RevenueCat processes:

- Transaction identifiers from Apple App Store or Google Play.
- Subscription status and entitlement records.
- Platform identifiers and a RevenueCat-assigned anonymous user identifier.
- Device identifiers associated with your subscription on the relevant platform.

RevenueCat does **not** receive any of your sentences, feelings, photographs, book list, or any other in-app content.

RevenueCat Privacy Policy: [https://www.revenuecat.com/privacy](https://www.revenuecat.com/privacy)

### 4.3 Open Library (Book Metadata)

The Last Page queries the public **Open Library** search API at `openlibrary.org` to retrieve canonical book metadata (title, author, cover image, work identifier). Queries contain only the search terms (a title, an author, or an ISBN) — never your sentence, feeling, photograph, or any account-style identifier.

As with any web request, your IP address is visible to Open Library's servers. Open Library is operated by the Internet Archive: [https://archive.org/about/terms.php](https://archive.org/about/terms.php).

### 4.4 Apple App Store / Google Play Store

Your in-app purchases, subscription renewals, restoration, and refunds are processed by Apple or Google according to your platform. Their privacy policies govern this processing:

- Apple Privacy Policy: [https://www.apple.com/legal/privacy/](https://www.apple.com/legal/privacy/)
- Google Privacy Policy: [https://policies.google.com/privacy](https://policies.google.com/privacy)

### 4.5 No Other Third Parties

We do not use:
- Advertising networks or advertising identifiers (IDFA, GAID).
- Analytics platforms (Firebase Analytics, Mixpanel, Amplitude, Segment, PostHog, etc.).
- Social login providers.
- Server-side cloud storage for your library content.
- Third-party crash reporting services that transmit identifiable data externally.

---

## 5. DEVICE PERMISSIONS

The Last Page requests only the permissions strictly required to deliver the features you trigger.

| Permission | When Requested | Why |
|------------|----------------|-----|
| **Camera** | When you choose to capture a last page in the app | To take the photograph of the last page used for book identification (Section 4.1) and visual record |
| **Photo Library** | When you choose to pick an existing photo of a last page | So you can select a photograph you have already taken |
| **Notifications** | When you opt in to the biweekly reminder | To deliver a single local "did a book end this week?" nudge every 14 days |

All three are optional. The app remains usable for manually entered endings and book lookups without granting camera, photo library, or notification access.

Photographs taken or selected through the app are stored on your device. A copy is transmitted only once, only for the identification step described in Section 4.1.

---

## 6. NOTIFICATIONS

The Last Page sends only **local notifications**. There are no push notifications. There is no push token. We do not run a notification server.

If you opt in, the app schedules a single biweekly reminder ("Did a book end this week?") using the device's local notification scheduler. The schedule is re-armed on the device. No notification content, identifier, or scheduling metadata is transmitted to us or any third party.

You can disable the nudge at any time from the app's settings, or from your operating system's notification settings.

---

## 7. CHILDREN'S PRIVACY

The Last Page is not directed at children under 13 years of age. We do not knowingly collect personal information from children under 13.

For users in the European Economic Area, the minimum age is 16 unless verifiable parental consent has been obtained, in line with Article 8 GDPR and applicable national digital-age-of-consent rules.

If you are a parent or guardian and believe your child has used the app, please contact us at cankatsarac@gmail.com. Because all in-app content is local to the device, you can permanently delete it by uninstalling the app or by using the in-app delete option.

---

## 8. YOUR RIGHTS

### 8.1 Rights for All Users

- **Access:** You can view every ending you have saved at any time inside the app. There is no off-device copy for us to share.
- **Deletion:** You can delete an individual ending from within the app, or delete all data by uninstalling the app. Both are immediate and permanent.
- **Correction:** You can edit or replace any saved ending directly in the app.
- **Portability:** Because all data is stored locally on your device, you already have full possession of your data. Premium users can additionally export their library as a PDF keepsake.

### 8.2 Additional Rights for EEA / UK Residents (GDPR / UK GDPR)

You have the right to:

- **Withdraw consent** at any time (delete the relevant ending, revoke OS-level permissions, uninstall the app).
- **Object to processing** — since processing on our side is limited to subscription handling and the one-time identification request you trigger, you exercise this right by not using those features.
- **Lodge a complaint** with your local supervisory authority (e.g., ICO in the UK, CNIL in France, BfDI in Germany, AEPD in Spain, KVKK in Türkiye).

### 8.3 Rights for California Residents (CCPA / CPRA)

California residents have the right to:

- **Know** what personal information is collected — see Section 1.
- **Delete** personal information — uninstall the app, or use in-app deletion controls.
- **Opt out of the sale or sharing of personal information** — we do not sell or share personal information for cross-context behavioral advertising.
- **Non-discrimination** — we will not discriminate against you for exercising your privacy rights.

To exercise CCPA rights, contact: cankatsarac@gmail.com

---

## 9. DATA SECURITY

Although your library never leaves your device, we still take reasonable steps to promote data security:

- Local storage relies on platform-level protections provided by iOS and Android for app-private storage.
- No unencrypted personal data is transmitted over the network. All third-party calls described in Section 4 use HTTPS (TLS).
- The app does not request system permissions beyond those listed in Section 5.
- We follow secure coding practices and keep dependencies updated.

The security of your device, lock screen, and any cloud backup you enable through iOS or Android is your responsibility. We recommend enabling device-level encryption and a strong passcode. If you enable iCloud or Google Drive device backups, photographs and AsyncStorage data may be included in those backups, governed by Apple's or Google's privacy terms — not ours.

---

## 10. DATA RETENTION

Because all in-app content is stored locally on your device, you control retention entirely:

- **Active use:** Data persists until you delete it or uninstall the app.
- **App uninstall:** All data is permanently and immediately deleted.
- **Per-ending delete:** Available from within the app.

We do not retain any copies of your library on our servers.

**Identification requests** (Section 4.1) are transient and not retained by us. We do not control how the upstream model provider handles transient inference data; refer to their terms.

**RevenueCat subscription records** are retained for as long as necessary to provide subscription services and comply with Apple/Google billing requirements.

---

## 11. INTERNATIONAL DATA TRANSFERS

Because your sentences, feelings, photographs, and book list do not leave your device, there are no international transfers of that data.

When the identification request, Open Library lookup, or subscription event is processed, the receiving service may operate servers in jurisdictions outside your country of residence (typically the United States and the European Union). Those transfers are governed by the receiving service's privacy terms and their own compliance with applicable data transfer mechanisms (including EU Standard Contractual Clauses where applicable).

---

## 12. CHANGES TO THIS POLICY

We may update this Privacy Policy from time to time. Material changes will be communicated via an in-app notice on the app's next launch after the change. The "Last Updated" date at the top will reflect the most recent revision.

Continued use of The Last Page after a policy update constitutes acceptance of the updated policy. If you do not accept material changes, you should discontinue use and uninstall the app, which will delete all of your data.

---

## 13. CONTACT US

For any privacy-related questions, requests, or concerns:

**Email:** cankatsarac@gmail.com
**Developer:** Cankat Saraç

We will respond to all verified requests within 30 days.

---

*This Privacy Policy applies to The Last Page mobile application available on the Apple App Store and Google Play Store.*
