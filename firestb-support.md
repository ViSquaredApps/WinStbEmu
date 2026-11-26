---
layout: default
title: Support — FireStb
permalink: /firestb-support.html
---

## Support — FireStb

FireStb is ViSquared's TV-only app for Android-based Amazon Fire TV / Fire OS devices. It is not the Windows app, a phone app, or a Vega OS app.

**No channels or provider subscription are included.** Only connect to portals, playlists, and content you are authorized to access. For Windows help, use the separate [WinStbEmu support page]({{ '/support.html' | relative_url }}).

## Getting Started

1. Open FireStb on your compatible Fire TV device. Use the remote's directional controls and OK/Select to navigate.
2. On **Portals**, choose **Try demo** to explore sample content without a provider account or purchase.
3. To use your own service, choose **Add** and enter the provider details it supplies. Do not guess a MAC address or device identity if your provider binds access to a particular device.
4. Select the saved provider to connect. Use **Remote help** in Settings for the app's remote-control guide.

## Trial, Unlock, and Restore

The intended Amazon Appstore offer is a **free download**, a **14-day local trial**, and a **one-time permanent app unlock**, planned at **USD $5.99**. Amazon's displayed checkout price and currency apply. The app unlock is not a recurring app subscription and does not pay for any IPTV provider.

The demo remains available without a purchase. Non-demo playback requires an active trial or an app entitlement.

If you previously purchased the app unlock, use **Restore** while signed into the same Amazon account. This asks Amazon for ownership; do not repurchase simply because an ownership check failed.

For a purchase or restore problem, check your internet connection and Amazon account, then contact us with the app version, Fire TV model, and the error shown. **Do not post Amazon account information or raw receipt identifiers publicly.** Amazon handles billing, refunds, and store-account questions through its own support.

## Troubleshooting

### The demo works, but my provider does not connect

- Check the address and credentials directly with your provider.
- Confirm the subscription is active and supports the provider type configured in the app.
- For a Stalker/MAG portal, check the MAC address, device profile, and any provider-required device identity.
- If the provider says the account is locked to another device, ask it to reset or confirm that binding. The developer cannot change a provider's account or subscription.

### Playback fails, buffers, or stops

- Check the Fire TV's connection and try another channel or item from the same provider.
- Check whether your provider limits simultaneous connections or has unavailable content.
- In **Settings**, try switching **Hardware decoding** between **Auto** and **Off** for a device-specific decoding issue.
- Record whether **Try demo** works and the exact non-sensitive error shown; that helps distinguish app/device issues from provider issues.

### How do I control playback?

Use the TV remote and the on-screen playback controls. **Settings → Remote help** explains the app's remote actions. Seeking and catch-up availability depend on the media and provider.

### Can I disable diagnostics?

Yes. In **Settings**, set **Anonymous telemetry** to **Off**. **Detailed portal diagnostics** is a separate opt-in for sharing plain-text portal identity; leave it off unless you want to share that information for troubleshooting.

See the [FireStb privacy policy]({{ '/firestb-privacy.html' | relative_url }}) for the distinction between app telemetry, provider requests, Amazon purchases, and support messages.

### Does clearing app data cancel my purchase?

No. It removes local app settings, viewing state, and trial/license information, not Amazon's purchase record or your provider account. After reinstalling or clearing app data, use **Restore** with the purchasing Amazon account to request ownership again.

## Contact Support

Email **[winstbemu@outlook.com](mailto:winstbemu@outlook.com)** with:

- FireStb version, Fire TV model, and Fire OS version.
- What you expected, what happened, and steps to reproduce.
- Whether the demo works and whether the issue affects all content or just one provider/item.
- A non-sensitive screenshot or the error text, if helpful.

Never send passwords, PINs, authentication tokens, or full stream URLs. Review screenshots and logs before sharing them; provider and account details may be visible.

You can also open a non-sensitive issue at [GitHub Issues](https://github.com/ViSquaredApps/WinStbEmu/issues), beginning the title with **FireStb** so it is not confused with a Windows report. **Issues and attachments there are public.** Redact provider addresses, MAC/device IDs, credentials, purchase/account identifiers, and any other private details.

FireStb does not have the Windows app's in-app support-report workflow; do not follow Windows-only instructions for exporting a diagnostic bundle or locating `%LOCALAPPDATA%` logs.

**Publisher:** ViSquared  
**Privacy:** [FireStb privacy policy]({{ '/firestb-privacy.html' | relative_url }})

---

© 2026 ViSquared. All rights reserved.
