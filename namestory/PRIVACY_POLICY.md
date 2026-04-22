# NAMESTORY APP PRIVACY POLICY

**Effective Date:** April 22, 2026
**Last Updated:** April 22, 2026

## Introduction

Welcome to NameStory ("we," "our," or "us"). We respect your privacy and are committed to protecting your personal information. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you use the NameStory mobile application and related services (the "App").

NameStory is a name-discovery tool. You type a name and the App returns demographic insights (age, gender, likely nationalities), meaning, and cultural context. The App is built for curious users, expecting parents, writers, and anyone researching names. Most of what you do inside the App is stored locally on your device and never leaves it.

## 1. INFORMATION WE COLLECT

### 1.1 Information You Provide Directly

When you create an account (optional), we collect:

- Email address (if you use email sign-up or sign-in)
- Display name (optional, if you set one)
- Authentication credentials from Google Sign-In or Apple Sign-In (we receive a unique identifier, your name, and your email from the provider — never your password)

You are not required to create an account. The App works fully in anonymous mode with no identifying information attached.

### 1.2 Content You Submit

The names you type into the App are sent to third-party statistical APIs (see Section 3.2) to produce demographic predictions. We do not store the names you type on our servers. They transit through the third-party APIs and the result is returned to your device.

### 1.3 Usage Information

We may automatically collect:

- App version, device type, operating system version
- Language and region settings
- Crash diagnostics and error reports (via Expo, if crash reporting is enabled)
- Anonymous analytics events such as screen views and feature usage (only if you consent on first launch)

We do not collect IP addresses beyond what the App's hosting providers log for security purposes.

### 1.4 Location Information

We do not collect precise location data. We do not request location permissions. The App may infer a broad region from your device's language setting to localize content, but no GPS or IP-based geolocation is performed by us.

### 1.5 Information Stored Locally on Your Device

By default, the following data is stored only on your device and never sent to our servers:

- Your search history (names you have looked up and their results)
- Your favorites
- Your language preference
- Your first-run completion flag

If you choose to sign in with Google, Apple, or email, this data can optionally be synchronized to Firebase Firestore so it follows you across devices. Sign-in is always optional.

## 2. HOW WE USE YOUR INFORMATION

We use the collected information to:

- Provide the core name-discovery functionality
- Return statistical predictions from third-party APIs
- Enrich results with Wikipedia context in your language
- Let you maintain a personal history and favorites across devices, if you sign in
- Diagnose and fix crashes and performance issues
- Detect and prevent fraud and abuse
- Comply with legal obligations
- Communicate with you about important App changes, security notices, or support inquiries

We do not use your information to build advertising profiles, train machine learning models, or sell to data brokers.

## 3. INFORMATION SHARING AND DISCLOSURE

### 3.1 We Do Not Sell Your Data

We do not sell, rent, or trade your personal information to third parties for marketing purposes. Ever.

### 3.2 Third-Party APIs That Process Name Queries

When you type a name into the App, that name is sent to one or more of the following public statistical APIs to produce predictions. These are the only outbound requests that carry a name:

- **Agify** (agify.io) — returns predicted age
- **Genderize** (genderize.io) — returns predicted gender
- **Nationalize** (nationalize.io) — returns predicted nationalities
- **Wikipedia** (wikipedia.org via the REST API) — returns the encyclopedia entry for the name
- **REST Countries** (restcountries.com) — returns detail for the top predicted country (capital, population, region, languages, localized country name)

These APIs receive the plain text of the name you type. They may log it along with your IP address for their own rate-limiting, caching, and analytics purposes. We do not control their retention or use of that data. If you search a name you consider sensitive — for example, your own full legal name or a minor's name — please be aware that it will transit through these services.

No other fields from your device (history, favorites, authentication identifiers) are sent to these APIs.

### 3.3 Service Providers We Use

We share limited data with the following trusted service providers strictly to operate the App:

- **Firebase Authentication (Google LLC)** — stores the authentication record tied to your Google, Apple, email, or anonymous account
- **Firebase Firestore (Google LLC)** — optional cloud storage for your history and favorites, only if you sign in and choose to sync
- **Expo (650 Industries, Inc.)** — app build hosting, over-the-air updates, and optional crash diagnostics
- **Apple, Inc.** — App Store distribution, Sign in with Apple, optional TestFlight diagnostics
- **Google LLC** — Google Play distribution, Google Sign-In

These providers are contractually obligated to protect your information and process it only on our instructions, in line with the provider's own privacy policies.

### 3.4 Legal Requirements

We may disclose your information if required by law, legal process, or government request, or when we believe in good faith that disclosure is necessary to:

- Protect our rights, property, and safety
- Protect the rights, property, and safety of our users or the public
- Prevent illegal activities
- Investigate suspected fraud or violations of our Terms of Service

### 3.5 Business Transfers

If NameStory is involved in a merger, acquisition, asset sale, or similar transaction, your information may be transferred to the successor entity. We will notify you through the App and update this Privacy Policy before any transfer takes effect.

## 4. DATA SECURITY

We implement industry-standard security measures to protect your information:

- Transport Layer Security (TLS) for all network traffic
- Firebase-managed encryption of data in transit and at rest
- Secure authentication protocols (OAuth 2.0, OpenID Connect) for Google and Apple sign-in
- Minimum data collection — the App works without an account and stores history locally by default
- Regular dependency updates and security patches

However, no method of transmission over the internet or electronic storage is 100% secure. We cannot guarantee absolute security, and you use the App at your own risk.

## 5. DATA RETENTION

We retain your information only as long as needed to provide the service or meet legal obligations.

- **Locally stored data** (history, favorites, preferences) — retained on your device until you delete the App, clear history from Settings, or sign out. We have no way to retrieve it.
- **Firebase Auth account** — retained as long as your account is active. Deleted within 30 days of account deletion.
- **Firestore sync data** — retained as long as your account is active. Deleted immediately upon account deletion.
- **Diagnostic and crash data** — retained up to 90 days, then purged.

You may request deletion of your account and all associated data at any time through Settings > Delete Account, or by emailing us at the address in Section 11.

## 6. YOUR PRIVACY RIGHTS

Depending on your jurisdiction, you may have the following rights:

### 6.1 Rights Under GDPR (European Economic Area, United Kingdom, Switzerland)

- Right to access the personal data we hold about you
- Right to rectification of inaccurate data
- Right to erasure ("right to be forgotten")
- Right to restriction of processing
- Right to data portability
- Right to object to processing
- Right to withdraw consent at any time
- Right to lodge a complaint with a supervisory authority

### 6.2 Rights Under CCPA/CPRA (California)

- Right to know what personal information is collected, used, shared, or sold
- Right to delete personal information
- Right to opt out of the sale or sharing of personal information (we do not sell or share)
- Right to correct inaccurate personal information
- Right to limit use of sensitive personal information
- Right to non-discrimination for exercising your rights

### 6.3 How to Exercise Your Rights

Most rights are exercisable directly within the App:

- **Access and portability:** export your history via Settings > Export Data
- **Correction:** edit your display name and email in Settings > Account
- **Deletion:** use Settings > Delete Account, which removes your Firebase account, Firestore sync data, and signs you back into anonymous mode

For requests that cannot be completed in-app, contact us at the address in Section 11. We will respond within 30 days.

## 7. CHILDREN'S PRIVACY

NameStory is not directed to children under 13 (or the equivalent minimum age in your jurisdiction, such as 16 in the EEA). We do not knowingly collect personal information from children under that age. If we discover that a child has provided personal information, we will delete it promptly.

If you are a parent or guardian and believe your child has provided us with information, please contact us using the details in Section 11.

## 8. INTERNATIONAL DATA TRANSFERS

NameStory operates globally. Your information may be processed and stored in countries other than your own, including the United States where our service providers (Firebase, Expo) are headquartered.

For transfers out of the European Economic Area, we rely on:

- Standard Contractual Clauses approved by the European Commission
- Adequacy decisions where applicable
- Other legally recognized transfer mechanisms

By using the App, you consent to the transfer of your information to countries that may have different data protection laws than your country of residence.

## 9. THIRD-PARTY LINKS AND CONTENT

The App may display content pulled from Wikipedia and link out to Wikipedia articles. Wikipedia is operated by the Wikimedia Foundation and governed by its own privacy policy. We are not responsible for the practices of third-party services linked from the App.

## 10. CHANGES TO THIS PRIVACY POLICY

We may update this Privacy Policy from time to time. The "Last Updated" date at the top will reflect any changes. Material changes will be communicated through:

- An in-app notification on next launch
- An email to the address on your account (if any)
- A notice on our support page

Continued use of the App after changes indicates acceptance of the updated Privacy Policy.

## 11. CONTACT US

If you have questions, concerns, or requests regarding this Privacy Policy or your personal data, contact us at:

**Email:** privacy@namestory.app
**Support:** support@namestory.app
**Mailing address:** _(to be populated with your business address before App Store submission)_

For EU users, you may also contact our EU representative:
_(to be appointed and listed here if you are required to have one under GDPR Article 27)_

## 12. CALIFORNIA SHINE THE LIGHT

California Civil Code Section 1798.83 allows California residents to request information about the categories of personal information shared with third parties for direct marketing purposes. We do not share personal information for direct marketing purposes.

## 13. DO NOT TRACK

Some web browsers transmit "do not track" signals. NameStory is a mobile application and does not respond to DNT signals at the browser level. We do not track your activity across third-party websites.

## 14. CONSENT

By using NameStory, you consent to the collection, use, disclosure, and retention of your information as described in this Privacy Policy.

If you do not agree with any part of this Policy, please do not use the App. You may delete the App at any time. If you have an account, use Settings > Delete Account to also remove your server-side data.

---

**This Privacy Policy is effective as of the date listed above. By using NameStory, you acknowledge that you have read, understood, and agreed to the terms of this Privacy Policy.**
