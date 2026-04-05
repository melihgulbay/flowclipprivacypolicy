# Privacy Policy for FlowClip

**Last Updated:** April 5, 2026  
**Developer:** Melibyte Apps  
**Package:** com.melibyte.flowclip

---

## Overview

FlowClip ("the app", "we") is a video editing application that prioritizes your privacy while providing powerful creative tools. This policy explains what data we collect, why, and how we protect it.

---

## Data Collection

### What We Collect

#### 1. Account Information (Optional — Only if you sign in)
If you choose to use the **Community Workshop** feature, you may sign in with your Google Account. When you do, we collect:

- ✅ **Display Name & Email**: Used solely to create your private user profile. Your email is never shown to other users.
- ✅ **Username**: A public nickname you choose, visible to other users in the Community Workshop.
- ✅ **User ID (UID)**: A unique identifier assigned by Firebase Authentication, used to associate your data with your account.

> **Important**: Signing in is entirely optional. All core video editing features work without an account. If you never sign in, no personal information is collected.

#### 2. Community Workshop Content (Optional — Only if you publish)
If you publish a custom shader effect to the Community Workshop, the following is stored on our servers:

- ✅ **Shader Code (GLSL)**: The source code of your custom effect.
- ✅ **Effect Metadata**: Name, description, and parameter definitions of your effect.
- ✅ **Author Attribution**: Your chosen username and User ID, so the community knows who created the effect.

> **Gallery Archive**: At the end of each monthly cycle, top shaders may be permanently inducted into the FlowClip Gallery. Inducted shaders (including your shader code, metadata, and username) are transferred to and stored on **Cloudflare R2** cloud object storage, where they remain publicly accessible indefinitely. See §Third-Party Services for details.

#### 3. Analytics & Crash Data (Automatic)
We use **Firebase Services (Google)** to collect the following **anonymous** data:

- ✅ **Crash Data**: If the app crashes, we receive a report with the error code and device state (e.g., "Crash in Video Engine on Samsung Galaxy S23").
- ✅ **Usage Analytics**: How the app is used (e.g., "Screen views," "Session duration," "Buttons clicked"). This helps us understand which features are popular.
- ✅ **Device Integrity**: We check if your device environment is secure to prevent piracy and abuse.
- ✅ **Device Information**: Model, OS version, and broad geographic region (City/Country).

### What We DO NOT Collect

- ❌ Precise Location (GPS)
- ❌ Advertising ID (We do not show ads)
- ❌ **Your Media Files**: Your photos, videos, and audio files **never leave your device**. All editing happens locally.
- ❌ **Your Audio/Speech Data**: AI Auto-Captions are processed entirely on your device using a locally downloaded AI model. No audio is ever sent to any server.
- ❌ Payment or Financial Information
- ❌ Contacts, Call Logs, or Messages

---

## Third-Party Services

We use the following third-party services:

### 1. Firebase Authentication (Google Sign-In)
**Purpose**: To allow optional sign-in for the Community Workshop.
- **Data Collected**: Google account name, email address, and a unique user ID.
- **Privacy Policy**: [Google Privacy Policy](https://policies.google.com/privacy)

### 2. Cloud Firestore (Firebase)
**Purpose**: To store user profiles, usernames, and published community shader effects.
- **Data Stored**: Username, User ID, shader code, and effect metadata.
- **Data Visibility**: Your email is stored in a private collection only you can access. Your username and published shaders are publicly visible.
- **Privacy Policy**: [Firebase Privacy Policy](https://firebase.google.com/support/privacy)

### 3. Google Analytics for Firebase
**Purpose**: To understand user behavior and improve app features.
- **Data Collected**: Usage data, device information, session metrics.
- **Privacy Policy**: [Google Privacy Policy](https://policies.google.com/privacy)

### 4. Firebase Crashlytics
**Purpose**: To detect, diagnose, and fix crashes (bugs).
- **Data Collected**: Crash logs, stack traces, device state info (RAM, OS version) at the time of crash.
- **Privacy Policy**: [Firebase Crashlytics Privacy Policy](https://firebase.google.com/support/privacy)

### 5. Google Play Integrity API
**Purpose**: To detect fraudulent devices, unauthorized modification/tampering, and piracy.
- **Data Collected**: Integrity tokens containing device signals.
- **Privacy Policy**: [Google Play Data Safety](https://developer.android.com/google-play/guides/data-safety)

### 6. Cloudflare R2 Object Storage
**Purpose**: To host the permanent FlowClip Gallery archive of inducted community shaders.
- **Data Stored**: Shader code (GLSL), effect metadata, and author username for shaders inducted into the Gallery at the end of a monthly cycle.
- **Visibility**: Gallery content is publicly readable by all FlowClip users.
- **Retention**: Permanent (Gallery shaders are not deleted after induction).
- **Privacy Policy**: [Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/)

### 7. FFmpeg
**Purpose**: Video processing engine.
- **Data Sent**: None (Runs securely on-device).

### 8. Hugging Face (AI Model Download)
**Purpose**: To download on-device AI speech recognition models for the Auto-Caption feature.
- **Data Sent**: None. Only a standard HTTPS download request is made to retrieve the AI model file. Your IP address is visible to Hugging Face's servers during this download.
- **Data Processed Locally**: Your audio is processed entirely on your device using the downloaded model. No audio is ever sent to any server.
- **Privacy Policy**: [Hugging Face Privacy Policy](https://huggingface.co/privacy)

---

## Data Storage & Security

- **Local Media**: Your projects, media files, and exported videos remain on your device at all times.
- **Account Data**: Stored securely in Google's Cloud Firestore with strict access controls. Your private profile (including email) can only be read by you.
- **Community Data**: Published shaders and your public username are visible to all users of the Community Workshop.
- **Gallery Data**: Shaders inducted into the FlowClip Gallery are stored on Cloudflare R2 and are publicly accessible indefinitely. This data is not deleted on request, as it forms a permanent curated archive.
- **Transmission**: All data is transmitted securely via HTTPS encryption.
- **Retention**: Firebase Analytics data is retained according to Google's standard retention policies (typically 2–14 months). Active community data is retained until you delete it or the monthly cycle ends. Gallery-inducted data is retained permanently.

---

## Permissions

FlowClip requests permissions strictly for functionality:

| Permission | Purpose |
|---|---|
| `READ_MEDIA_VIDEO` | To select videos for editing. |
| `READ_MEDIA_AUDIO` | To select music/audio for your project. |
| `READ_MEDIA_IMAGES` | To browse and select photos from your gallery for editing. |
| `READ_MEDIA_VISUAL_USER_SELECTED` | To support Android 13+'s partial media access ("Selected Photos"), allowing you to grant access to only specific photos/videos rather than your entire gallery. |
| `CAMERA` | To record video directly from your device camera for importing into the timeline. All recordings stay on your device. |
| `RECORD_AUDIO` | To record voice/audio directly from your device microphone for importing into the timeline. All recordings stay on your device. |
| `INTERNET` | Required by Firebase (Auth, Firestore, Analytics, Crashlytics), Play Integrity, and Community Workshop. **Your media files are NOT sent over the internet.** |

---

## Your Rights & Control

You have full control over your data:

- **Don't Sign In**: All core editing features work without an account. No personal data is collected.
- **Delete Your Account Data**: You can request deletion of your account and all associated data by contacting us at the email below.
- **Delete Published Shaders**: You can delete your own published shaders at any time during the active monthly cycle from the Profile tab. Note: shaders that have been inducted into the permanent FlowClip Gallery cannot be removed on request, as they form part of the curated public archive.
- **Sign Out**: You can sign out at any time from the Profile tab, which stops all account-related data syncing.
- **Uninstall**: Uninstalling the app stops all data collection. Local data is removed from your device.
- **Android Settings**: You can revoke file permissions at any time.

---

## Children's Privacy

FlowClip does not knowingly contact or collect personal information from children under 13. If you believe we have inadvertently collected such information, please contact us so we can verify and delete it.

---

## Changes to This Policy

We may update this Privacy Policy from time to time. We will notify you of any changes by updating the "Last Updated" date at the top of this page. We encourage you to review this policy periodically.

---

## Contact

For questions about this Privacy Policy or to request data deletion:

- **Developer:** Melibyte Apps
- **Email:** melibyteapps@outlook.com
- **App:** FlowClip

---

## Summary

**FlowClip is a local-first video editor. Your videos never leave your device. If you choose to sign in for the Community Workshop, we store your username and published shader effects securely. We collect anonymous crash reports and usage stats to improve the app. We never sell your data.**
