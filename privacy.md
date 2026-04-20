---
layout: default
title: Privacy Policy — WinStbEmu
---

## Privacy Policy — WinStbEmu

**Last updated:** April 20, 2026

WinStbEmu ("the App") is a native Windows desktop application that emulates a MAG set-top box for connecting to authorized Stalker Portal / Ministra middleware IPTV services. This privacy policy explains what data the App collects, stores, and transmits.

## Data Stored Locally

The App stores the following data on your device in `%LOCALAPPDATA%\WinStbEmu\`:

- **Portal configurations** — portal name, URL, MAC address, device profile name, and optional emulation fields
- **Application settings** — log level, capture assets preference, telemetry preferences (crash reporting and usage data sharing)
- **Debug log** — a rotating log file (`debug.log`) containing diagnostic information for troubleshooting (capped at 10 MB)

All data is stored locally on your device. The App does not use cloud storage, accounts, or server-side databases.

## Network Communications

The App makes network requests solely to connect to IPTV portals that you configure:

- **Portal discovery** — HTTP requests to the portal URL you provide, to locate the portal endpoint
- **Portal communication** — HTTP requests to the portal's Stalker middleware API for authentication, channel lists, and stream URLs
- **Media streaming** — direct connections to media stream URLs provided by the portal (HLS, MPEG-TS)

The App does not communicate with any server other than the portals you configure and the optional telemetry service described below.

## Telemetry (Optional)

The App includes optional telemetry via Microsoft Application Insights. Telemetry has two tiers, both of which can be disabled.

### Crash Reporting (Settings → Crash Reporting)

When enabled (the default), the following data is sent to Microsoft Azure:

- Exception type, message, and stack trace
- App version and Windows OS version
- Machine name (as device identifier)
- Device hardware context: CPU name, GPU name, RAM, CPU core count, display resolution, device type (laptop/desktop)
- Hashed identifiers for anonymous correlation:
  - Portal URL origin → `portalHash` (SHA256, truncated, not reversible)
  - MAC address → `user_Id` (SHA256, truncated, not reversible)
  - Serial number → `serialHash` (SHA256, truncated, not reversible)
- Sanitized portal URL (scheme + host + path only — query strings, fragments, and credentials are stripped)
- Usage events: playback start/stop, channel switches, portal connections, fullscreen toggles, settings changes
- Performance metrics: channel switch time, playback duration, portal session duration

You can disable crash reporting at any time in **Settings → Crash Reporting**. When disabled, no telemetry data of any kind is transmitted.

### Share Usage Data (Settings → Share usage data)

This is an additional opt-in setting (disabled by default) that, when enabled, includes plaintext device emulation fields alongside the data described above:

- MAC address (plaintext)
- Serial number (plaintext)
- Device IDs, hardware versions, vendor, STB type, image version, signature, timezone, custom user agent

This data helps diagnose portal connection issues and improve compatibility with different IPTV providers.

**The following data is never sent, regardless of settings:**

- Login credentials (username, password)
- PIN codes
- Authentication tokens or cookies

### Disabling Telemetry

- **Settings → Crash Reporting = Off** disables all telemetry. No data is transmitted to any external service.
- **Settings → Share usage data** is automatically disabled when Crash Reporting is off.

## Third-Party Services

- **Microsoft Application Insights** — used for optional telemetry (see above). Subject to the [Microsoft Privacy Statement](https://privacy.microsoft.com/privacystatement).
- **WebView2** (Microsoft Edge) — used to render portal UI. WebView2 may collect diagnostic data per its own privacy policy. The App configures WebView2 to operate within the application context only.

## Data Sharing

The App does not sell, rent, or share any user data with third parties. Telemetry data is used solely by the developer to diagnose issues and improve the App.

## Children's Privacy

The App is not directed at children under 13 and does not knowingly collect personal information from children.

## Changes to This Policy

Updates to this privacy policy will be posted at this URL. The "Last updated" date at the top will be revised accordingly.

## Contact

If you have questions about this privacy policy, please email [winstbemu@outlook.com](mailto:winstbemu@outlook.com) or open an issue at [github.com/ViSquaredApps/WinStbEmu](https://github.com/ViSquaredApps/WinStbEmu/issues).

---

© 2026 ViSquared. All rights reserved.
