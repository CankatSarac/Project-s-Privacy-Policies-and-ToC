# WAYPOINT — PRIVACY POLICY

**Effective Date:** May 15, 2026
**Last Updated:** May 15, 2026

---

## Introduction

Waypoint ("we," "us," or "our") is a mobile application that surfaces global supply-chain risk alerts and disruptions. We classify publicly reported incidents (port closures, geopolitical events, weather disruptions, shortages, cyber events, labor disputes) and deliver them as filtered, prioritized alerts.

This Privacy Policy explains what we collect, why, where it goes, and your rights.

Contact: **cankatsarac@gmail.com**

---

## 1. WHAT WE COLLECT

### 1.1 Information you provide

- **Email address** (entered during onboarding) — used to subscribe you to alert emails and digests via our backend service.
- **Filter preferences** (regions, categories, severities you care about).
- **Bookmarks and dismissed alerts** — your interaction with the alerts feed.

### 1.2 Automatically collected

- **Push notification token** (when you grant notification permission and we register your device with our backend, including for background remote notifications).
- **Device-level information** sent by Apple/Google during normal app distribution and platform billing (we do not retain this beyond standard platform analytics that we cannot opt out of).

### 1.3 What we do NOT collect

- We do not collect your name, phone number, address, contacts, or social graph.
- We do not collect location data. The `expo-location` library appears in our dependencies but the app does not call any location API.
- We do not use advertising SDKs or advertising identifiers (IDFA / GAID).
- We do not use third-party analytics SDKs (Mixpanel, Amplitude, Firebase Analytics, PostHog, etc.).
- We do not sell, rent, or trade your data.

---

## 2. HOW DATA IS STORED

| Data | Where |
|---|---|
| Email address | Your device (preferences cache) + our backend email subscriber list |
| Filter preferences, bookmarks, dismissed alerts | Your device only (local storage) |
| Push notification token | Our backend, mapped to your subscription, until you uninstall or revoke notification permission |

We operate a minimal backend that delivers alerts and email digests. Beyond your email address, your push token, and aggregate non-identifying analytics about alert delivery (e.g., delivery success rate), we do not retain user-identifying data.

---

## 3. LEGAL BASIS (GDPR / UK GDPR)

| Data | Legal basis |
|---|---|
| Email address and push token | **Performance of a contract** (Article 6(1)(b) GDPR) — necessary to deliver the alert subscription you requested. |
| Local preferences | Held on your device by you; we do not access. |
| Email digests beyond service notifications | **Consent** (Article 6(1)(a)) — you can unsubscribe from each email. |

---

## 4. THIRD PARTIES

### 4.1 Waypoint backend
Our own backend service (operated by Cankat Saraç) that fetches and classifies supply-chain incidents from public news and data sources and delivers alerts to your device. Stores your email address, push token, and aggregate analytics. Hosted in [cloud region — currently the United States or European Union; consult our most recent infrastructure disclosure].

### 4.2 Rork Toolkit (NLP Classification)
The app integrates with the Rork Toolkit AI relay for natural-language classification of incident summaries. The app does **not** send your email, push token, or any identifier tied to you to Rork — only the public alert text being classified, when classification happens client-side. Refer to [https://rork.com](https://rork.com).

### 4.3 Apple Push Notification Service / Firebase Cloud Messaging
Used to deliver push notifications. Apple and Google control these services and receive only the push token + notification payload necessary for delivery.

### 4.4 Apple App Store / Google Play Store
Distribution and platform analytics that we cannot opt out of. See their policies.

---

## 5. DEVICE PERMISSIONS

- **Notifications:** required to deliver real-time alerts. You can disable at any time in OS settings.
- **Internet:** required to fetch alerts and email subscriptions.
- No camera, microphone, location, contacts, photo library, or other sensor permissions are requested.

---

## 6. RETENTION

| Item | Retention |
|---|---|
| Email address (backend) | Until you unsubscribe (link in every email) or request deletion. |
| Push token (backend) | Until you uninstall or revoke notification permission, at which point the token is invalidated by Apple/Google and removed from our records. |
| Local preferences and bookmarks | Until you uninstall the app or use the in-app reset. |
| Backend logs | Up to 30 days of operational logs (delivery success, error rates). No personal content in payloads beyond email address. |

---

## 7. YOUR RIGHTS

- **Access:** email cankatsarac@gmail.com to receive a copy of your email/push token record.
- **Delete:** email cankatsarac@gmail.com to delete your subscription, or click the unsubscribe link in any email digest, or uninstall the app to revoke the push token.
- **Correct:** update your email by re-entering it in the app.
- **Object / withdraw consent:** unsubscribe at any time.

### 7.1 EEA / UK rights
You have the right to lodge a complaint with your local supervisory authority (ICO, CNIL, BfDI, AEPD, KVKK, etc.).

### 7.2 California rights (CCPA / CPRA)
California residents have the right to know, delete, correct, opt out of the sale/sharing of personal information (which we do not do), limit the use of sensitive personal information, and non-discrimination.

---

## 8. CHILDREN'S PRIVACY

Waypoint is intended for professional users — supply-chain operators, analysts, and managers. We do not knowingly collect data from children under 13 (or 16 in the EEA). If you believe a child has provided an email address to us, contact us and we will delete it.

---

## 9. CONFIDENTIALITY OF YOUR USE

The alerts that Waypoint surfaces are publicly reported events. We do **not** ask you to upload any internal supply-chain, supplier, or commercial data. Your bookmarks and filter preferences (which categories or regions you watch) remain on your device and are not transmitted to our backend.

---

## 10. INTERNATIONAL DATA TRANSFERS

Where your email address or push token is processed in a jurisdiction other than your country of residence, we and our processors rely on Standard Contractual Clauses or equivalent safeguards under GDPR Article 46 where applicable.

---

## 11. SECURITY

All backend traffic uses HTTPS (TLS). Email addresses are stored in a database accessible only via authenticated backend services. We follow the principle of least privilege for administrative access.

No system is perfectly secure. If you believe your email address has been used by someone else, contact us at cankatsarac@gmail.com.

---

## 12. CHANGES

Material changes are communicated via in-app notice on the next launch and, where we have your email address, by email. The "Last Updated" date reflects the most recent revision.

---

## 13. CONTACT

**Controller:** Cankat Saraç (sole proprietor)
**Email:** cankatsarac@gmail.com
**Postal address:** [INSERT POSTAL ADDRESS]

We aim to respond to verified requests within 30 days.

---

*This Privacy Policy applies to the Waypoint mobile application available on the Apple App Store and Google Play Store.*
