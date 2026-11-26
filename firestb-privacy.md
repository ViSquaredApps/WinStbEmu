---
layout: default
title: Privacy Policy — FireStb
permalink: /firestb-privacy.html
---

## Privacy Policy — FireStb

**Last updated:** November 26, 2026

FireStb is ViSquared's TV-only application for Android-based Amazon Fire TV / Fire OS devices. It lets you connect to providers and playlists you are authorized to use. FireStb does not supply an IPTV subscription, channels, or provider content.

This policy covers FireStb, not the Windows application WinStbEmu. The [WinStbEmu Windows privacy policy]({{ '/privacy.html' | relative_url }}) is separate.

## Data Stored on Your Device

FireStb keeps the following app data locally:

- **Provider settings and credentials** — configured provider addresses, login details, and any device-emulation identity fields needed by your provider. Provider settings are encrypted at rest using a key held by Android Keystore.
- **Preferences and viewing state** — app and diagnostic preferences, favorites, and watch progress.
- **Trial and license information** — local trial timing, a bounded license cache, and a purchase-fulfillment journal used to avoid acknowledging the same Amazon purchase repeatedly.
- **A telemetry installation identifier** — a locally generated identifier used to correlate diagnostic events when telemetry is enabled. It is not an Amazon account identifier.

Android app backups are disabled for FireStb. Encryption of stored settings does not mean every network connection is encrypted.

## Connections to Your Providers

When you configure and use a provider, FireStb sends the requests needed for authentication, browsing, playback, and supported watch-progress operations. Depending on your provider, these requests can include your provider credentials, device-emulation identity, searches, requested content, and playback position. Media playback connects to stream servers selected by that provider.

Your provider and its stream servers therefore receive the information needed to deliver their service, along with normal connection information such as your IP address. Their own privacy policies apply. Whether these connections use HTTPS depends on the addresses and service supplied by your provider; HTTP traffic is not encrypted.

The built-in **Try demo** option does not require a provider account or an app purchase.

## Diagnostics and Usage Telemetry

FireStb uses **Microsoft Application Insights** for crash, performance, connection, browsing, playback, and entitlement diagnostics. Telemetry is **enabled by default**.

The app sends structural information such as app version and distribution, device manufacturer/model, operating-system version, architecture, language, CPU core count, display resolution, session identifiers, event and failure categories, and timing or duration measurements. Exception diagnostics can include exception type, message, and stack trace.

Telemetry uses a persistent, pseudonymous installation identifier and hashes of configured portal identities for correlation. These identifiers can link activity from the same installation or portal; hashing is not a guarantee of complete anonymity.

Structured diagnostic and usage-event fields are designed to omit provider login credentials, PINs, authentication tokens or cookies, stream URLs, search terms, and viewed titles. Exception objects are forwarded to Application Insights, so their messages and stack traces can contain contextual information about a failure; this is not a guarantee that every exception payload is free of user data. Provider requests described above are separate from telemetry.

### Your Telemetry Choices

- In **Settings**, set **Anonymous telemetry** to **Off** to disable the app's telemetry.
- **Detailed portal diagnostics** is a separate, explicit opt-in, **Off by default**. When enabled alongside telemetry, diagnostic events can also include the configured portal's origin (scheme, host, and port, without a path or query), MAC address, and serial number in plain text.
- Leave **Detailed portal diagnostics** off if you do not want to share those portal identity fields. Turning telemetry off prevents their transmission through telemetry even if the detailed-diagnostics preference is on.

The setting name **Anonymous telemetry** does not mean diagnostic events are uncorrelated; the pseudonymous identifiers described above are still used while it is enabled. Turning it off does not disable provider traffic or Amazon purchase operations, and does not remove diagnostics already received.

## Amazon Purchases

The Amazon edition is designed as a free download with a 14-day local trial and a one-time permanent app unlock. The trial and app unlock do not include a provider subscription.

Amazon handles the store account and payment transaction. FireStb uses the Amazon Appstore SDK to request product information, purchases, and restoration or refresh of ownership. The SDK provides account and receipt identifiers, product identifiers, and purchase or cancellation status used to determine app access and acknowledge fulfillment. FireStb also keeps local license state and a fulfillment journal keyed by a hash of the Amazon account/receipt pair.

These are SDK-reported purchase results; FireStb does not currently use a separate developer-hosted server to verify Amazon receipts. Amazon's own privacy and purchase policies apply. Disabling app telemetry does not disable the SDK communication needed for purchases or restoration.

## Support You Choose to Contact

For FireStb support or privacy questions, email [winstbemu@outlook.com](mailto:winstbemu@outlook.com). We receive the email address, message, and any attachments you choose to send so that we can respond to your request.

You can also report a non-sensitive app issue on [GitHub Issues](https://github.com/ViSquaredApps/WinStbEmu/issues). That issue tracker is **public**. Do not send provider credentials, PINs, authentication tokens, receipt/account identifiers, stream URLs, or unredacted logs there.

FireStb does not use WinStbEmu's Windows in-app support-report bundle or signed public reply channel. Contacting support is separate from the app's telemetry settings; turning telemetry off does not prevent you from sending an email or opening an issue.

## Third-Party Services

- **Your configured providers and their media servers** — authentication, browsing, streaming, and supported watch-progress requests.
- **Microsoft Application Insights** — diagnostic and usage telemetry when enabled. See the [Microsoft Privacy Statement](https://privacy.microsoft.com/privacystatement).
- **Amazon Appstore** — product, account, purchase, and entitlement operations. See [Amazon's Privacy Notice](https://www.amazon.com/gp/help/customer/display.html?nodeId=GX7NJQ4ZB8MHFRNJ).
- **GitHub** — this policy/support website and any public issues you choose to submit. See the [GitHub Privacy Statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement).
- **Email** — messages and attachments you choose to send to the support address.

Each service receives the information needed for its role. This policy does not replace those services' privacy policies.

## Managing Your Data

You can change telemetry preferences in the app and remove configured providers. Clearing FireStb's app data in Fire OS settings removes local settings, saved viewing state, identifiers, and trial/license cache. It does not cancel an Amazon purchase, delete a provider account, or delete information already received by Amazon, a provider, the telemetry service, or support.

After clearing app data or reinstalling, use **Restore** with the Amazon account that made the purchase to request ownership again. For questions about information you have shared with the developer, contact the support email. Do not include passwords or other secrets in the message.

## Changes to This Policy

Updates will be posted on this page with a revised "Last updated" date.

## Contact

**Publisher:** ViSquared  
**Email:** [winstbemu@outlook.com](mailto:winstbemu@outlook.com)  
**Help:** [FireStb support]({{ '/firestb-support.html' | relative_url }})

---

© 2026 ViSquared. All rights reserved.
