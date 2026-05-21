# NameStory — Account & Data Deletion

**App:** NameStory  
**Developer:** Teampire  
**Contact:** cankatsarac@gmail.com

---

## How to delete your account in the NameStory app

1. Open the **NameStory** app on your device.
2. Tap the **Settings** icon (gear icon, top-right of the main screen).
3. Scroll to the **Account** section.
4. Tap **Delete Account**.
5. Read the confirmation prompt and tap **Delete** to confirm.

Your account and all associated data are deleted immediately.

---

## What gets deleted

When you delete your account, NameStory permanently removes:

| Data | Where stored | Deleted? |
|------|-------------|----------|
| Email address / authentication credentials | Firebase Authentication | ✅ Immediately |
| Saved name history (cross-device sync) | Firebase Firestore | ✅ Immediately |
| Local name history | On-device (AsyncStorage) | ✅ Immediately |
| Language preference | On-device (AsyncStorage) | ✅ Immediately |

After account deletion, the app automatically switches to anonymous mode so you can continue using it without an account.

---

## Partial data deletion (without deleting your account)

You can delete your **search history** at any time without deleting your account:

1. Open the **NameStory** app.
2. Go to **Settings**.
3. In the **Data** section, tap **Clear History**.
4. Confirm the action.

This removes all locally stored name searches. It does not affect your account or authentication credentials.

---

## Can't access the app?

If you are unable to access the app to delete your account, email us at **cankatsarac@gmail.com** with the subject line `Account Deletion Request — NameStory`. Include the email address associated with your account. We will delete your account and all associated data within 30 days.

---

## Data retention after deletion

- **Firebase Auth and Firestore data**: deleted immediately upon account deletion request within the app, or within 30 days for email requests.
- **Aggregated, anonymised analytics**: may be retained in aggregate form with no link to any individual user.
- **Crash reports**: retained for up to 90 days by Expo/EAS for system stability purposes, then automatically purged.

---

*Last updated: May 2026*
