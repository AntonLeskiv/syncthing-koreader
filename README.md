# Syncthing plugin for KOReader (`syncthing-koreader`)

Fork of [koreader-syncthing](https://github.com/jasonchoimtt/koreader-syncthing) with **Binary Auto-Update** and improved VPN/Firewall support.

This plugin runs a native [Syncthing](https://syncthing.net) instance directly on e-readers running [KOReader](https://github.com/koreader/koreader) (Kindle, Kobo, etc.), allowing seamless peer-to-peer file synchronization between your e-reader and your computer/NAS/phone.

---

## What's New in this Fork?

- 🔄 **Binary Auto-Update**: Checks the official Syncthing GitHub releases and updates the `syncthing` executable directly from the KOReader menu with 1 click.
- ⚡ **Auto-check on Startup**: Option to automatically notify you when a new Syncthing version is released.
- 🔒 **Full VPN & WireGuard Support**: Fixed Kindle firewall rules so Syncthing can sync over WireGuard tunnels (`wg0`) as well as local Wi-Fi (`wlan0`).
- 📱 **Multi-Architecture**: Supports 32-bit ARM (`armv7l`), 64-bit ARM (`aarch64`), and x86/x86_64 devices.

---

## Features

- Manage Syncthing directly from the KOReader network menu.
- Start/stop daemon on demand or automatically with KOReader.
- Web GUI password configuration and QR code display for easy pairing.
- Status and pending device/folder inspection.
- Auto-update binary to the latest stable release.

---

## Installation

1. Download the latest release or clone this repository.
2. Copy the `syncthing.koplugin` folder to your e-reader:
   ```
   /mnt/us/koreader/plugins/syncthing.koplugin/   (Kindle)
   ```
3. Open KOReader and find **Syncthing** in the top menu (Network/Tools tab).
4. Tap **Check for Binary Update** to ensure you have the latest Syncthing release!

---

## Tested Devices

- Kindle Paperwhite (3, 4, 5 / Bellatrix)
- Kindle Oasis, Voyage, Basic, Scribe
- Kobo (Clara, Libra, Sage, Elipsa)

---

## License

GPL-3.0 License (same as upstream `koreader-syncthing`).