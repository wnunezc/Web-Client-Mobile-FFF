# Web Client FFF

Web Client FFF is an Android 7.0+ native APK that runs a multi-profile WebView client with local profile isolation, compact profile tabs, per-profile automation controls, report ZIP generation, premium licensing, scheduled ads for free users, and mandatory in-app update checks.

This repository branch is the public distribution channel only. It contains no source code, signing keys, local configuration, private logs, screenshots, or secrets.

## Download

[![Download APK](https://img.shields.io/badge/Download-APK-2ea44f?style=for-the-badge&logo=android&logoColor=white)](https://raw.githubusercontent.com/wnunezc/Web-Client-Mobile-FFF/master/releases/web-client-fff-v1.0.0.apk)

Direct file:

- [`releases/web-client-fff-v1.0.0.apk`](https://raw.githubusercontent.com/wnunezc/Web-Client-Mobile-FFF/master/releases/web-client-fff-v1.0.0.apk)

The app checks `version.json` every time it opens. If a newer version is available, the app blocks normal use, downloads and verifies the APK, then opens the Android installer. Android still requires user confirmation for the installation and may require allowing installs from this app as a trusted source.

## Current Version

- Version: `1.0.0`
- Android: `7.0` or newer
- Update metadata: `version.json`

## Capabilities

- Native Android/Kotlin WebView client.
- Up to 3 free profiles opened as compact tabs.
- Premium license support for up to 5 profiles.
- Isolated WebView sessions per supported profile.
- Per-profile Click Event Service and Emergency Heal configuration.
- Background operational support for inactive profiles while the app process remains active.
- Screen-off session keep-alive service with Android foreground notification.
- Local report ZIP generation for support.
- GitHub issue prefill support.
- Scheduled ad container for free users.
- PayPal-based premium purchase flow through Key-Master.
- Mandatory update check on every app launch.

## Permissions

The app blocks its main UI until required Android permissions are available:

- Install unknown apps for Web Client FFF: required so mandatory APK updates can open the Android installer.
- Notifications on newer Android versions: required for the foreground keep-alive notification.

The app does not require Accessibility permission in this release.

## License Plans

Free mode:

- Up to 3 profiles.
- Scheduled ads may be shown.

Basic:

- 2.00 USD.
- 1 year.
- 1 device.
- Up to 5 profiles.
- Ads disabled.

Lifetime:

- 20.00 USD.
- Lifetime license.
- 1 device.
- Up to 5 profiles.
- Ads disabled.

Multi-device:

- 200.00 USD.
- 2 years.
- Up to 50 devices.
- Up to 5 profiles per device.
- Ads disabled.

Using more than 3 profiles may require a high-end phone or emulator because multiple WebViews can consume significant CPU, memory and battery.

## Privacy, Support And License Policy

Premium purchases are processed through PayPal and Key-Master. The APK does not store PayPal secrets, full card data or bank data, and it does not mark payments as paid by itself.

For purchase and support, the app or Key-Master may use purchase email, PayPal identifier when available, purchase ID, license ID, visible device code, device binding, plan, activation state and technical logs.

Support is handled through GitHub Issues first and the helpdesk at:

- https://helpdesk.lh-2.net

Report ZIP files can include device, WebView, logs, technical captures and license status. Do not share private account credentials, PayPal passwords, 2FA codes, full card data or private screenshots.

Premium benefits may be suspended or revoked for refunds, disputes, chargebacks, payment fraud, license abuse, unauthorized redistribution, modified APKs or false support claims. When validation reports that a license is not usable, the app returns to free mode.

## Published Files

Only these files are intended for this public distribution branch:

- `README.md`
- `version.json`
- `releases/web-client-fff-v1.0.0.apk`

No source code, Gradle files, Android project files, keystores, passwords, `local.properties`, logs, captures or private diagnostics should be published here.

## Technical Debt

Public release text is English-only for now. Localized public README and policy pages will be prepared later.
