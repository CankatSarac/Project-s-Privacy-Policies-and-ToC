# Project Legal Documents

Central home for the privacy policies and terms of service of apps
built by **Cankat Saraç**. Each subfolder is one app. Each app has its
own `PRIVACY_POLICY.md` and `TERMS_OF_SERVICE.md`.

## Apps

### Pledge

Personal habit-tracking and goal-keeping app.

- [Privacy Policy](./pledge/PRIVACY_POLICY.md)
- [Terms of Service](./pledge/TERMS_OF_SERVICE.md)

### NameStory

Name-discovery app that returns demographic predictions, meaning, and cultural context for any first name.

- [Privacy Policy](./namestory/PRIVACY_POLICY.md)
- [Terms of Service](./namestory/TERMS_OF_SERVICE.md)

### Socrates Pocket

Reflective self-inquiry app that asks Socratic questions — never gives answers. No accounts, local-only storage, AI-generated questions.

- [Privacy Policy](./socrates-pocket/PRIVACY_POLICY.md)
- [Terms of Service](./socrates-pocket/TERMS_OF_SERVICE.md)

## How these are hosted

These documents are served as a public static site via GitHub Pages
(or an equivalent host). App Store Connect and Google Play Console
require publicly reachable URLs in every store listing, and the live
URLs for each app are set in that app's store submission.

Typical URL pattern once GitHub Pages is enabled on this repo:

```
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/namestory/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/namestory/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/pledge/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/pledge/TERMS_OF_SERVICE
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/socrates-pocket/PRIVACY_POLICY
https://<github-user>.github.io/Project-s-Privacy-Policies-and-ToC/socrates-pocket/TERMS_OF_SERVICE
```

To enable GitHub Pages on this repo:

1. Push this repo to GitHub if not already pushed.
2. On GitHub, go to the repo → **Settings** → **Pages**.
3. Set **Source** to **Deploy from a branch**.
4. Pick **main** (or your default branch) and **/ (root)** folder.
5. Save. Within a minute or two the URLs above resolve.

## Adding a new app

1. Create a new subfolder named after the app, lowercase and hyphenated (e.g. `myapp/`).
2. Drop in `PRIVACY_POLICY.md` and `TERMS_OF_SERVICE.md`, mirroring the
   structure of the existing `pledge/` or `namestory/` folders.
3. Update this README with a link to the new app's documents.
4. Commit and push.

## Maintenance

Every legal document in this repository includes an **Effective Date**
and **Last Updated** line at the top. Bump both of them whenever a
document is edited, and notify affected app users through in-app
messaging or email on their next app launch.

Review each document at least once a year regardless of whether
anything has changed.
