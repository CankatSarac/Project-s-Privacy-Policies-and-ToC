# FINITE APP — PRIVACY POLICY

**Effective Date:** April 28, 2026
**Last Updated:** April 28, 2026

---

## Introduction

Finite ("we," "us," or "our") is a mobile application that helps you reflect on the finite nature of your time by generating a personalized statistical estimate of days remaining in your life based on actuarial data.

We take privacy seriously. This Privacy Policy explains exactly what data we collect, how it is processed, where it is stored, and what rights you have over it. **Because Finite collects health-related information, we have taken specific steps to ensure this data never leaves your device.**

If you have questions or concerns, contact us at: **cankatsarac@gmail.com**

---

## 1. DATA WE COLLECT AND WHY

### 1.1 Data You Provide During Onboarding

To generate your personalized estimate, you provide the following information:

| Data | Purpose | Sensitivity |
|------|---------|-------------|
| **Date of birth** | Calculate actuarial life expectancy | Personal |
| **Country of residence** | Apply country-specific actuarial tables | Personal |
| **Biological sex** | Apply sex-specific actuarial tables | Personal (special category under GDPR) |
| **Smoking frequency** | Adjust life expectancy estimate | Health-related |
| **Alcohol consumption** | Adjust life expectancy estimate | Health-related |
| **Exercise frequency** | Adjust life expectancy estimate | Health-related |
| **Medical conditions** | Adjust life expectancy estimate | Health-related (special category under GDPR) |

### 1.2 Data You Create While Using the App

| Data | Purpose |
|------|---------|
| **Daily reflections** (rating 1–5 and optional note) | Personal journaling |
| **Letters** you write to loved ones | Time-capsule feature |
| **Family member profiles** (name, date of birth, biological sex) | Family countdown feature |
| **App preferences and settings** | Personalization |
| **Premium subscription status** | Feature gating |
| **Onboarding completion status** | App flow management |

### 1.3 Data We Do NOT Collect

- We do not collect your name or email address
- We do not collect precise GPS location
- We do not collect biometric data
- We do not collect photos or media
- We do not use analytics SDKs or advertising SDKs
- We do not run crash-reporting tools that transmit your data to third-party servers

---

## 2. HOW YOUR DATA IS STORED

**All data described in Section 1.1 and 1.2 is stored exclusively on your device using encrypted local storage (AsyncStorage). It is never transmitted to our servers, never uploaded to the cloud, and never synchronized across devices.**

This architecture means:
- **No account is required** to use Finite
- **No data breach on our servers** can expose your health information
- **We cannot access your data** even if legally compelled, because we do not hold it
- **Uninstalling the app permanently deletes all your data**

The only exception is subscription status, which is processed by RevenueCat (see Section 4).

---

## 3. LEGAL BASIS FOR PROCESSING (GDPR)

If you are located in the European Economic Area (EEA), United Kingdom, or Switzerland, we process your data under the following legal bases:

| Data Category | Legal Basis |
|---------------|-------------|
| Health and lifestyle data | **Explicit consent** (Article 9(2)(a) GDPR) — you voluntarily input this data to receive the estimation service |
| Ordinary personal data (birthday, country) | **Legitimate interest / performance of a contract** — necessary to provide the core service you requested |
| Premium subscription data | **Performance of a contract** — processing necessary to provide the service you purchased |

Because all data remains on your device, Article 9 processing of special category data (health data, biological sex) occurs without our involvement as a data controller in the traditional sense. You act as the sole data subject and sole processor of your own health information.

---

## 4. THIRD PARTIES

### 4.1 RevenueCat (Payment Processing)

Finite uses **RevenueCat** to manage in-app subscriptions and purchases. When you purchase a premium subscription, RevenueCat processes:

- Transaction identifiers
- Subscription status and entitlement records
- Platform identifiers (Apple App Store / Google Play Store)
- Device identifiers associated with your subscription

RevenueCat does **not** receive any of your health data, date of birth, reflections, letters, or family data.

RevenueCat's Privacy Policy: [https://www.revenuecat.com/privacy](https://www.revenuecat.com/privacy)

### 4.2 Apple App Store / Google Play Store

Your in-app purchases are processed by Apple or Google. Their privacy policies govern their processing:

- Apple Privacy Policy: [https://www.apple.com/legal/privacy/](https://www.apple.com/legal/privacy/)
- Google Privacy Policy: [https://policies.google.com/privacy](https://policies.google.com/privacy)

### 4.3 No Other Third Parties

We do not use:
- Advertising networks
- Analytics platforms (Firebase, Mixpanel, Amplitude, etc.)
- Social login providers
- Cloud storage providers
- Crash reporting services that transmit data externally

---

## 5. CHILDREN'S PRIVACY

Finite is not directed at children under 13 years of age. We do not knowingly collect personal information from children under 13. The app enforces a minimum age of 13 during onboarding. If you are a parent or guardian and believe your child under 13 has used the app and provided personal information, please contact us at cankatsarac@gmail.com. Since all data is local to the device, you can permanently delete it by uninstalling the app.

For users in the EEA, the minimum age is 16 unless parental consent has been obtained.

---

## 6. YOUR RIGHTS

### 6.1 Rights for All Users

- **Access:** You can view all data you provided within the app at any time through the Settings screen.
- **Deletion:** You can delete all your data by uninstalling the app, or by using the data deletion option in Settings. Because data is stored locally, deletion is immediate and permanent.
- **Correction:** You can update your profile data at any time through the Settings screen.
- **Portability:** Because all data is stored locally on your device, you already have full possession of your data.

### 6.2 Additional Rights for EEA/UK Residents (GDPR/UK GDPR)

You have the right to:

- **Withdraw consent** at any time for health data processing (by deleting your data or uninstalling the app)
- **Lodge a complaint** with your local supervisory authority (e.g., ICO in the UK, CNIL in France, BfDI in Germany, AEPD in Spain)
- **Object to processing** — since all processing is local, you exercise this right by removing the data from your device

### 6.3 Rights for California Residents (CCPA / CPRA)

California residents have the right to:

- **Know** what personal information is collected — see Section 1
- **Delete** personal information — uninstall the app or use Settings > Delete My Data
- **Opt out of the sale of personal information** — we do not sell personal information
- **Non-discrimination** — we will not discriminate against you for exercising your privacy rights

To exercise CCPA rights, contact: cankatsarac@gmail.com

---

## 7. HEALTH DATA — SPECIAL NOTICE

Finite collects health-related information (medical conditions, lifestyle factors, biological sex) for the sole purpose of generating an actuarial estimate. This information:

- **Is never transmitted off your device**
- **Is not used to train AI or machine learning models**
- **Is not shared with health insurance providers, employers, or any third party**
- **Does not constitute a medical record**
- **Cannot be used for discriminatory purposes because we do not possess it**

The app's calculation is a statistical estimate based on publicly available actuarial tables. It is not a medical diagnosis, prognosis, or health assessment. See the Terms of Service for a full medical disclaimer.

---

## 8. DATA SECURITY

Although all data remains on your device and out of our reach, we take the following steps to promote data security:

- All local storage uses platform-level encrypted storage (iOS Keychain / Android Keystore where applicable via AsyncStorage)
- No unencrypted network transmission of personal data occurs
- Our app does not request unnecessary system permissions
- We follow secure coding practices and keep dependencies updated

The security of your device and its lock screen is your responsibility. We recommend enabling device-level encryption and a strong passcode.

---

## 9. DATA RETENTION

Because all data is stored locally on your device, you control retention entirely:

- **Active use:** Data persists until you delete it or uninstall the app
- **App uninstall:** All data is permanently and immediately deleted
- **Settings > Delete My Data:** Clears all locally stored data without uninstalling

We do not retain any copies of your data on our servers.

**RevenueCat subscription records** are retained for as long as necessary to provide subscription services and comply with Apple/Google billing requirements.

---

## 10. INTERNATIONAL DATA TRANSFERS

Because data does not leave your device, there are no international transfers of your personal health or profile data.

RevenueCat may transfer subscription transaction data internationally. This is governed by RevenueCat's privacy policy and their compliance with applicable data transfer mechanisms (including EU Standard Contractual Clauses where applicable).

---

## 11. CHANGES TO THIS POLICY

We may update this Privacy Policy from time to time. Material changes will be communicated via an in-app notice on the app's next launch after the change. The "Last Updated" date at the top will reflect the most recent revision.

Continued use of Finite after a policy update constitutes acceptance of the updated policy. If you do not accept material changes, you should discontinue use and uninstall the app, which will delete all your data.

---

## 12. CONTACT US

For any privacy-related questions, requests, or concerns:

**Email:** cankatsarac@gmail.com
**Developer:** Cankat Saraç

We will respond to all verified requests within 30 days.

---

*This Privacy Policy applies to the Finite mobile application available on the Apple App Store and Google Play Store.*
