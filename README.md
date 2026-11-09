# Privacy Policy

**Video Edit**
**Version Date: November 9, 2026**
**Effective Date: November 9, 2026**

---

## Introduction

Welcome to Video Edit (hereinafter referred to as "the App"). This App is developed and provided by the developer (hereinafter referred to as "we" or "us"). We understand the importance of your personal information and are committed to protecting your privacy.

This Privacy Policy explains how we collect, use, store, and protect your personal information. **Please read this policy carefully and make sure you fully understand its contents before using the App.**

---

## 1. Information We Collect

### 1.1 Information You Provide

We do not require account registration or login. We do not actively collect your name, phone number, email address, or other personally identifiable information.

### 1.2 Data Generated During App Usage

When you use the App, the following data is stored **locally on your device**:

| Data Type | Description | Storage Location |
|-----------|-------------|-----------------|
| Video file cache | Copies of source videos selected via the system picker | App private directory (`files/picked/`) |
| Export temporary files | Intermediate files generated during video processing | App private directory (`files/works/`) |
| Thumbnails | Cover images extracted from videos | App private directory (`files/covers/`) |
| Project records | Metadata of editing projects (title, duration, resolution, status, etc.) | Local database (`works.db`) |
| Settings & preferences | Default export configuration (resolution, frame rate, bitrate, etc.) | Local preference storage (DataStore) |

### 1.3 Network-Related Data

The App has network access capability (INTERNET permission). When using network-dependent features, the following data may be transmitted:

- **Device information**: Device model, operating system version, App version, language settings — used for compatibility, troubleshooting, and analytics
- **Usage logs**: Crash logs, error reports, feature usage frequency, session duration — used for improving App stability and user experience
- **Advertising identifier (AAID)**: Android Advertising ID — used by advertising partners to serve relevant ads and measure ad performance
- **Feature data**: Data required by cloud-based features (if applicable) — processed in accordance with the specific feature's terms

### 1.4 Data Collected for Advertising

The App displays in-app advertisements through third-party advertising services. To deliver and measure ads, the following data may be shared with advertising partners:

- Android Advertising ID (AAID)
- Device model and operating system version
- App usage data (e.g., screen views, session duration)
- IP address (may be collected by ad networks for fraud prevention)

Advertising partners may use this data to serve personalized ads based on your interests. You can opt out of personalized advertising by resetting your advertising ID or limiting ad tracking in your device settings (Settings > Ads > Opt out of personalized ads).

### 1.5 Data Collected for Analytics

The App uses third-party analytics services to understand how users interact with the App. The following data may be collected for analytics purposes:

- App usage events (e.g., feature usage frequency, screen views, session duration)
- Device information (model, OS version, screen resolution)
- Crash and performance data
- Approximate geographic region (derived from IP address, not precise location)

Analytics data is collected in aggregate form and is used solely to improve the App's functionality, performance, and user experience. We do not combine analytics data with personally identifiable information.

---

## 2. Permissions We Use

The App requests only the minimum necessary permissions:

| Permission | Purpose |
|-----------|---------|
| **Internet Access** (INTERNET) | Network communication for cloud features, crash reporting, and service improvement |
| **Foreground Service** (FOREGROUND_SERVICE) | Keep the export service running in the background during video processing |
| **Foreground Service Type - Data Sync** (FOREGROUND_SERVICE_DATA_SYNC) | Declare the foreground service business type for Android system compliance |
| **Foreground Service Type - Media Processing** (FOREGROUND_SERVICE_MEDIA_PROCESSING) | Declare the foreground service business type for Android 15+ compliance |
| **Wake Lock** (WAKE_LOCK) | Keep the CPU awake during video export to prevent interruption |
| **Notifications** (POST_NOTIFICATIONS, Android 13+) | Display export progress and completion notifications |
| **Ad Services** (ACCESS_ADSERVICES_AD_ID, Android 13+) | Access advertising identifier for personalized ad delivery |

**The App does NOT request the following permissions:**
- Camera permission
- Microphone / audio recording permission
- Precise or approximate location permission
- Contacts permission
- SMS / phone call permission
- Read external storage permission (uses the system file picker instead)

---

## 3. How We Access Video Files

The App uses the **Android System File Picker** (Storage Access Framework) to access video files you select. This means:

- After you actively select a video file, the system grants the App temporary access to that file
- The App copies the selected file to its private directory for processing
- After processing, the exported video is saved to the device gallery (`DCIM/videoedit/` directory)
- You can delete all temporary files in the private directory at any time using the "Clear Cache" feature within the App

---

## 4. Data Storage and Security

### 4.1 Retention Period

- **Video cache files**: Retained in the App's private directory until you manually clear the cache or uninstall the App
- **Export temporary files**: Deleted immediately after export is complete
- **Project records and settings**: Retained until you uninstall the App

### 4.2 Security Measures

- All data is stored in the sandbox directory assigned by the Android system to each application, which is not directly accessible by other applications
- Video processing is performed entirely on-device using the Android media framework (MediaCodec / MediaMuxer) and OpenGL
- We implement industry-standard security practices to protect data transmitted over the network

### 4.3 Backup

The App has Android's backup feature enabled (`allowBackup=true`). This means your App data (including project records and settings) **may** be backed up via Google Drive. This backup is managed by Google's backup service and is subject to Google's Privacy Policy.

---

## 5. Third-Party Services

The App integrates the following categories of third-party services:

### 5.1 Core Libraries (Local Only)

The following open-source libraries run locally on your device and do not independently collect data:

- **Android Jetpack (AndroidX)** — UI framework, lifecycle management, local database, and navigation
- **JetBrains Kotlin Standard Library** — Language runtime support

### 5.2 Advertising Services

The App displays advertisements through third-party advertising networks. These services may collect the data described in Section 1.4. Common advertising providers include:

- **Google AdMob / Ad Manager** — Serves banner, interstitial, and rewarded ads
- **Other advertising partners** — May vary based on your region and device

Advertising partners use cookies or similar technologies to deliver relevant ads. You can manage your ad preferences or opt out of personalized advertising through your device settings or the ad network's opt-out mechanisms.

### 5.3 Analytics Services

The App uses analytics services to understand usage patterns and improve performance. These services may collect the data described in Section 1.5. Common analytics providers include:

- **Firebase Analytics (Google)** — Collects anonymized usage events and crash reports
- **Other analytics partners** — May be integrated for specific feature analysis

Analytics data is processed in accordance with each provider's privacy policy and applicable data protection regulations.

---

## 6. Protection of Minors

The App is a video editing tool. We do not knowingly collect personal information from minors. If you are a guardian of a minor and believe that the minor has provided personal information through the App, please contact us, and we will take appropriate action.

---

## 7. Your Rights

Under applicable laws and regulations, you have the following rights:

- **Right to Access**: You can view all project records created within the App at any time
- **Right to Deletion**: You can delete temporary files via the "Clear Cache" feature, or delete all local data by uninstalling the App
- **Right to Withdraw Consent**: You can stop using the App and uninstall it at any time
- **Right to Opt Out of Network Data Transmission**: You can disable network access for the App in your device settings if you prefer to use only local features
- **Right to Opt Out of Personalized Advertising**: You can reset your advertising ID or limit ad tracking in your device settings (Settings > Ads > Opt out of personalized ads). This does not stop ads from being displayed, but they will be less relevant to your interests
- **Right to Access Analytics Data**: You can request a copy of the analytics data collected about your usage by contacting us at the email address provided in Section 9

---

## 8. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. When changes are made, we will update the version date and effective date at the top of this page. We recommend that you review this policy periodically to stay informed about how we protect your information.

---

## 9. Contact Us

If you have any questions, comments, or suggestions regarding this Privacy Policy, please contact us at:

- **Developer**: ymwm
- **Email**: [noww6446@gmail.com]

---

## 10. Governing Law and Dispute Resolution

The formation, validity, interpretation, and dispute resolution of this Privacy Policy shall be governed by the laws of the People's Republic of China (excluding laws of the Hong Kong, Macau, and Taiwan regions). Any disputes arising from this policy shall be resolved through friendly negotiation first; if negotiation fails, either party may file a lawsuit with the competent court at the developer's location.

---

*This Privacy Policy is effective as of November 9, 2026.*
