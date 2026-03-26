---
layout: default
title: Support — WinStbEmu
---

## Getting Started

1. **Install** WinStbEmu from the [Microsoft Store](https://apps.microsoft.com/detail/9PHJ61Z1D326)
2. **Add a portal** — Click the "+" button and enter your Stalker Portal / Ministra URL
3. **Configure** — Select a device profile (MAG250, MAG256, etc.) and enter your MAC address if required
4. **Connect** — Double-click the portal to launch

## Frequently Asked Questions

### What is WinStbEmu?

WinStbEmu is a native Windows MAG set-top box emulator for Stalker Portal / Ministra IPTV middleware. It lets you access your authorized IPTV portal subscriptions from your Windows PC.

### Do I need an IPTV subscription?

Yes. WinStbEmu does not provide any IPTV content. You must have an active subscription to a Stalker Portal or Ministra-based IPTV service.

### Which device profiles are supported?

MAG250, MAG256, MAG270, MAG322, MAG420, MAG520, MAG522, and custom profiles.

### What video formats are supported?

HLS (HTTP Live Streaming) and MPEG-TS via the built-in LibVLC player.

### The portal won't load or shows a blank screen

- Verify your portal URL is correct and accessible from a web browser
- Check that your MAC address matches what your provider expects
- Try a different device profile (some portals require specific MAG models)
- Ensure your internet connection is stable

### Video plays but there's no sound

- Check the volume control in the app overlay
- Verify your system audio output is set correctly
- Try toggling the audio track in playback controls

### The app crashes when loading a portal

- Update to the latest version from the Microsoft Store
- If the issue persists, check the log file at `%LOCALAPPDATA%\WinStbEmu\debug.log`

## System Requirements

- Windows 10 version 2004 (build 19041) or later
- x64 processor (ARM64 via emulation)
- Internet connection
- Active Stalker Portal / Ministra IPTV subscription

## Reporting Issues

If you encounter a bug or need help, please [open an issue](https://github.com/ViSquaredApps/WinStbEmu/issues) with:

1. A description of the problem
2. Steps to reproduce
3. Your Windows version (Settings → System → About)
4. The log file from `%LOCALAPPDATA%\WinStbEmu\debug.log` (remove any sensitive URLs/credentials)

## Privacy

See our [Privacy Policy](privacy).

## Contact

- **Email**: [winstbemu@outlook.com](mailto:winstbemu@outlook.com)
- **Issues & Support**: [GitHub Issues](https://github.com/ViSquaredApps/WinStbEmu/issues)
- **Publisher**: ViSquared

---

© 2026 ViSquared. All rights reserved.
