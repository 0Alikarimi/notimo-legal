# Privacy Policy — Notimo

**Last updated:** April 25, 2026
**App:** Notimo (Piano Learning App for iOS)
**Developer:** Ali Karimi
**Contact:** notimoapp@gmail.com

---

## TL;DR (Plain English)

Notimo is a piano learning app. We do not run our own servers. We do not
sell, share, or send your data to anyone. We do not use any tracking,
analytics, or advertising SDKs. Everything you do in the app stays on your
device or in your private iCloud account, which only you can read.

The only data we ever "see" is the opaque user identifier Apple gives us
when you sign in with Apple — and that lives in the iOS Keychain on your
own device. We never read it, send it anywhere, or pair it with anything.

---

## 1. Who we are

Notimo is developed by Ali Karimi as an independent indie iOS app. There is
no company, no investors, no marketing team, and crucially **no backend
server we own**. The app talks to exactly two things:

1. **Your device's local storage** (UserDefaults / Keychain / app sandbox)
2. **Your own private iCloud account** (Apple servers, your Apple ID)

That's it. There is no Notimo cloud, no Notimo analytics, no third-party
data brokers.

---

## 2. What data we collect

We list every category Apple's privacy framework recognizes, even when the
data never leaves your device. Honesty over brevity.

### 2.1 Sign in with Apple — Apple User Identifier

When you tap "Sign in with Apple", Apple gives the app an **opaque user
identifier**. This is a long string of random characters that uniquely
identifies you to *this app only*. It is NOT your Apple ID, NOT your email,
NOT your name. It cannot be reversed back to your real Apple ID by us or
anyone else.

- **Where it lives:** iOS Keychain on your device. Apple's secure storage.
- **What it's used for:** to know "this is the same user who signed in
  before" and to attach your iCloud sync data to your account.
- **Never sent to:** any third party. Ever.

### 2.2 Email and name — only if Apple sends them

The very first time you sign in with Apple, Apple may give the app your
email address and full name — but only if you allow it. You can choose:

- **"Hide My Email"** → Apple gives us a relay address that forwards to
  you. We can't see your real email.
- **Don't share name/email** → we get nothing.

If Apple sends an email or name, we store it locally on your device
(UserDefaults) only to display it in the Account section of Settings.
We never email you. We never have a mailing list. We never share it.

### 2.3 Your learning progress (XP, streak, achievements, settings)

Your daily streak, XP, completed lessons, settings (language, theme,
practice goal, metronome sound, etc.), and identified weak notes are
stored:

- **Locally** on your device in UserDefaults.
- **In your private iCloud account** via Apple's iCloud Key-Value Store
  and CloudKit, so the same progress shows up on all your devices using
  the same Apple ID.

This data is encrypted in transit and at rest by Apple. **We have zero
access to it.** Only you, signed into your Apple ID, can read it.

### 2.4 Imported songs and SoundFonts

If you import MusicXML/.mxl files or SoundFont (.sf2) files into Notimo,
they live in the app's sandbox on your device. Filenames may sync to your
iCloud if iCloud Drive is enabled — same as any iOS app. We do not read
these files for any purpose other than playing/displaying them in the app.

### 2.5 Microphone (optional)

Notimo can detect notes you play on an acoustic piano using the
microphone. The audio is processed in real-time and **never recorded,
stored, or sent anywhere**. Once a note is detected, the audio sample is
discarded. You must explicitly opt in via Settings → "Mic Detection".

### 2.6 What we do NOT collect

- ❌ No name, address, phone number (beyond what Apple optionally sends)
- ❌ No location data
- ❌ No advertising identifiers (IDFA)
- ❌ No browsing/usage history outside the app
- ❌ No device fingerprinting
- ❌ No crash reports sent anywhere (Xcode-style, only Apple sees them)
- ❌ No third-party SDKs (no Firebase, Mixpanel, Amplitude, Adjust,
  Branch, Facebook SDK, Google Analytics, etc.)
- ❌ No payment info — we use Apple's standard StoreKit, Apple handles
  all purchase data; we only see "user has Pro: yes/no" locally

---

## 3. Tracking

**We do not track you.** Not within the app, not across apps, not across
the internet. The app's privacy manifest declares `NSPrivacyTracking =
false`, and there are zero tracking domains in the binary.

---

## 4. Third parties

We use exactly two Apple-provided services:

| Service | What for | Apple's policy |
|---|---|---|
| **Sign in with Apple** | User authentication | [apple.com/legal](https://www.apple.com/legal/privacy/data/en/sign-in-with-apple/) |
| **iCloud (KV-Store + CloudKit)** | Sync your progress between your devices | [apple.com/legal/privacy/icloud](https://www.apple.com/legal/privacy/data/en/icloud/) |

Both services are operated by Apple Inc. and governed by Apple's privacy
policies. Notimo never sees the data Apple stores for you.

We do **not** use any non-Apple third-party services.

---

## 5. Children

Notimo is suitable for all ages, but Sign in with Apple has a minimum age
set by Apple (typically 13 in most regions). Children below that should
have a parent's Family Sharing setup. We do not knowingly collect data
from children under 13 — we don't really collect data from anyone — and
the app works fully without sign-in for users who don't want any cloud
sync.

---

## 6. Your rights

You can:

- **See your data:** open the app → Settings → Account. Your Apple
  identifier is in the iOS Keychain (visible via Apple's standard
  developer tools).
- **Stop sync:** disable iCloud for Notimo in iOS Settings → [Your Name]
  → iCloud → Apps Using iCloud.
- **Sign out:** Settings → Account → Sign Out (in-app).
- **Delete your account:** Settings → Account → Delete Account. This
  immediately removes:
  - Your Apple user identifier from the device's Keychain
  - Your locally cached progress
  - Your iCloud Key-Value Store data for Notimo
- **Fully revoke Sign in with Apple:** because we run no servers, we
  cannot revoke your Apple authorization on Apple's side. To do that
  yourself: iOS Settings → [Your Name] → Sign in with Apple → Notimo
  → "Stop using Apple ID". The app shows you this hint after deletion.

---

## 7. Data retention

- **On your device:** until you sign out, delete the account in-app, or
  delete the app.
- **In your iCloud:** controlled by Apple's iCloud retention rules and
  your own Apple settings. When you delete your Notimo account in-app, we
  attempt to delete the iCloud Key-Value entries we wrote. CloudKit
  records (currently empty — we don't write any structured CloudKit data
  in the current version) would also be removed.

---

## 8. Security

- Apple user identifier stored in iOS Keychain with
  `kSecAttrAccessibleAfterFirstUnlock` — the same protection class used
  by all major iOS apps for sensitive credentials.
- Data in iCloud is encrypted in transit (TLS) and at rest by Apple.
- The app uses anti-debug guards in production builds.
- We do not store any passwords or credit card data — Apple handles all
  authentication and payment.

---

## 9. International users

Because there is no Notimo server, your data does not leave your device or
your own Apple iCloud region. Apple stores iCloud data in your region per
their iCloud Terms.

---

## 10. Changes to this policy

If we ever change what data the app collects (e.g., add a feature that
needs new permissions), we'll update this page and bump the "Last updated"
date. For material changes (e.g., introducing any kind of analytics or
backend), the app will show a clear in-app notice and ask for fresh
consent.

---

## 11. Contact

Questions about privacy? Email **notimoapp@gmail.com**.

---

*Notimo is an independent indie project. No backend servers. No tracking.
No data sales. No surprises.*
