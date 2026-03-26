---
layout: default
title: Privacy Policy — WinStbEmu
---

## Privacy Policy — WinStbEmu

**Last updated:** March 21, 2026

WinStbEmu ("the App") is a native Windows desktop application that emulates a MAG set-top box for connecting to authorized Stalker Portal / Ministra middleware IPTV services. This privacy policy explains what data the App collects, stores, and transmits.

## Data Stored Locally

The App stores the following data on your device in `%LOCALAPPDATA%\WinStbEmu\`:

- **Portal configurations** — portal name, URL, MAC address, and device profile name
- **Application settings** — log level, capture assets preference, telemetry opt-out preference
- **Debug log** — a rotating log file (`debug.log`) truncated on each app start, containing diagnostic information for troubleshooting

All data is stored locally on your device. The App does not use cloud storage, accounts, or server-side databases.

## Network Communications

The App makes network requests solely to connect to IPTV portals that you configure:

- **Portal discovery** — HTTP requests to the portal URL you provide, to locate the portal endpoint
- **Portal communication** — HTTP requests to the portal's Stalker middleware API for authentication, channel lists, and stream URLs
- **Media streaming** — direct connections to media stream URLs provided by the portal (HLS, MPEG-TS)

The App does not communicate with any server other than the portals you configure.

## Crash Reporting (Optional)

The App includes optional crash reporting via Microsoft Application Insights. When enabled (the default), the following data is sent to Microsoft Azure in the event of an application error:

- Exception type, message, and stack trace
- App version and Windows OS version
- A randomly generated device identifier

**The following data is never sent:**

- Portal URLs, names, or configurations
- MAC addresses
- Authentication tokens or cookies
- Any user-entered content

You can disable crash reporting at any time in **Settings → Crash Reporting**. When disabled, no data is transmitted to any external service.

## Third-Party Services

- **Microsoft Application Insights** — used for optional crash telemetry (see above). Subject to the [Microsoft Privacy Statement](https://privacy.microsoft.com/privacystatement).
- **WebView2** (Microsoft Edge) — used to render portal UI. WebView2 may collect diagnostic data per its own privacy policy. The App configures WebView2 to operate within the application context only.

## Data Sharing

The App does not sell, rent, or share any user data with third parties. No advertising, analytics (beyond optional crash reporting), or tracking is performed.

## Children's Privacy

The App is not directed at children under 13 and does not knowingly collect personal information from children.

## Changes to This Policy

Updates to this privacy policy will be posted at this URL. The "Last updated" date at the top will be revised accordingly.

## Contact

If you have questions about this privacy policy, please email [winstbemu@outlook.com](mailto:winstbemu@outlook.com) or open an issue at [github.com/ViSquaredApps/WinStbEmu](https://github.com/ViSquaredApps/WinStbEmu/issues).

---

© 2026 ViSquared. All rights reserved.
