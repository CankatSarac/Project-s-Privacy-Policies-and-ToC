# Wherefy — Privacy Policy

**Last updated:** November 7, 2026

This policy covers Wherefy's Android app, package
`com.cankatsarac.wherefy`, and its dedicated photo-analysis service. Wherefy is
developed by **Cankat Saraç**. Contact: **cankatsarac@gmail.com**.

Wherefy estimates possible places from photographs that you choose to submit.
Its guesses and coordinates can be wrong. Choosing a photo is separate from
asking for an online analysis; photos are submitted when you request analysis.

## Photos, notes and analysis

For an online analysis, Wherefy sends the selected image, any optional note or
location hypothesis, your selected response language, and the chosen AI model
over HTTPS to its analysis service. The service uses Cloudflare to process the
request and forward it to OpenRouter and the selected AI model provider.

The image file may contain personal information, visible text, faces or embedded
metadata. Submit images and notes that you are comfortable sending to these
providers. A returned place is an estimate based on the image, not a report of
your device's current GPS location.

The dedicated analysis service processes photos, prompts and results in memory.
It does not save them in its application database or application logs. This does
not describe every infrastructure record or the independent retention practices
of Cloudflare, OpenRouter or the selected model provider.

OpenRouter routes requests to an available provider for the model selected.
Model availability and providers can change. The providers' rules for retention,
safety review and model training can differ; an analysis is not represented as
having guaranteed zero retention. See [OpenRouter's privacy policy](https://openrouter.ai/privacy)
and its [model-provider terms](https://openrouter.ai/docs/guides/privacy/provider-logging).
Cloudflare's processing is also described in its
[privacy policy](https://www.cloudflare.com/privacypolicy/).

## Guest access and security records

The Android analysis service issues a random guest access token without asking
for your name or email address. The app keeps the token in secure storage on
your device and uses it to authenticate later analysis requests. It is not a
verified personal identity or a subscription entitlement.

To prevent abuse and manage limited service capacity, the application database
keeps:

- A cryptographic hash of the guest token, its creation time and expiry time.
- A keyed hash derived from the network IP address supplied by Cloudflare. The
  network-hash value changes daily; the raw IP address is not saved in this
  application database.
- Random request reservation identifiers, dates and timestamps used to enforce
  request limits.

Token hashes can link the same guest's requests across days during the retention
period. These records do not contain the submitted photo, note, hypothesis,
prompt, analysis result, email address or payment information.

Guest sessions expire after seven days. An hourly cleanup normally removes
expired sessions and request reservations older than seven days, so deletion
can take an additional hour. An interruption to the service or scheduled
cleanup can delay that deletion. Cloudflare may separately process network and
security information under its own terms.

## Information saved on your device

Wherefy stores app preferences, your selected language and theme, local usage
counters, saved photos, notes and previous guesses on your device so you can
revisit them. The discovery album and practice features also use local storage.
The guest access token is stored separately in secure device storage and is
replaced when it expires and you next request access.

The app's clear-history and delete-data controls remove the corresponding local
records and saved photos. They do not delete a copy that you previously shared
to another app, a provider's independently retained data, or the security records
that remain subject to the short retention period above.

## Purchases and subscriptions

Where purchase options are available, Google Play processes Android payments,
renewals, cancellations and refunds. RevenueCat helps the app check subscription
access and restore purchases. This can involve an anonymous app-user identifier,
product and transaction identifiers, purchase history, entitlement status and
technical app or device information needed for the service.

Wherefy does not send the photos, notes or analysis results described above to
RevenueCat as part of this purchase integration, and the developer does not
receive your full card or bank details. The availability of purchase options
does not change the photo-sharing choice described above. See
[Google's privacy policy](https://policies.google.com/privacy) and
[RevenueCat's privacy policy](https://www.revenuecat.com/privacy).

## Your choices and external services

You choose whether to use the camera or system photo picker and which image to
submit. Camera access is requested when you choose to take a photo. You can
remove a selected photo before analysis and control saved local data in Settings.

Opening a candidate location in Google Maps sends that candidate's coordinates
to Google Maps. If you deliberately use a system sharing or copying feature,
the content you choose is handled by the destination app or system service under
its own privacy terms.

Wherefy does not sell your photos or personal information. Privacy enquiries and
requests can be sent to **cankatsarac@gmail.com**, identifying the app as Wherefy.

## Changes

This page will be updated when Wherefy's data handling changes. The date at the
top identifies the latest revision. This policy does not replace another app's
policy or the separate terms of service.
