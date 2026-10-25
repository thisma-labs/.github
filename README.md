<div align="center">

<img src="https://raw.githubusercontent.com/thisma-labs/.github/main/profile/banner.svg" alt="Thisma Labs" width="100%"/>

<br/>

[![Beside](https://img.shields.io/badge/Beside-v0.1.0-22d3ee?style=flat-square)](https://github.com/thisma-labs/beside/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-10%20|%2011-0078D4?style=flat-square&logo=windows&logoColor=white)](https://github.com/thisma-labs/beside/releases/latest)
[![Android](https://img.shields.io/badge/Android-8.0%2B-3DDC84?style=flat-square&logo=android&logoColor=white)](https://github.com/thisma-labs/beside/releases/latest)
[![TLS](https://img.shields.io/badge/TLS-1.3%20mutual-10b981?style=flat-square)](https://github.com/thisma-labs/beside/blob/main/SECURITY.md)
[![Made in](https://img.shields.io/badge/made%20in-Sri%20Lanka-f59e0b?style=flat-square)](https://github.com/thisma-labs)

</div>

```text
  ▄▄████████████████████▄▄
 ██████████████████████████
           ████         ████           thisma-labs@earth
           ████       ▄████            ─────────────────────────────────
           ████     ▄████▀             Org        Thisma Labs
           ████   ▄████▀▄▄             Origin     Sri Lanka
           ████  ████▀ ▄███            Craft      local-first software
           ██▀ ▄████    ▀███▄          Flagship   Beside  •—◎
           ▀ ▄████▀      ▀███▄         Platforms  Windows 10/11 · Android 8+
           ▄████▀          ████        Transport  mutual TLS 1.3 · pinned keys
         ▄████▀▄██████████▄ ▀███▄      Transfers  LAN only · no cloud relay
       ▄████▀▄██████████████ ▀███▄     Accounts   none
      ▄███▀                   ▀███▄    Tracking   zero
      ████▄▄                    ███    Status     v0.1.0 · shipping
       ▀▀▀▀                      ▀▀
```

## `•—◎` Beside

> **Send it. It's there.**
> Direct file, folder and text sharing between **Windows** and **Android**, over your own Wi-Fi.
> No cloud. No accounts. No tracking.

<div align="center">
<a href="https://github.com/thisma-labs/beside">
<img src="https://github.com/thisma-labs/beside/raw/main/assets/beside-hero.png" alt="Beside: wire-speed local peer sharing" width="85%"/>
</a>
</div>

### How a transfer works

```text
  WINDOWS PC                                              ANDROID PHONE
  ──────────                                              ─────────────
      │  1  discover   _beside._tcp.local.  (or QR / IP)       │
      │ ─────────────────────────────────────────────────────► │
      │  2  handshake  mutual TLS 1.3 · pinned SPKI SHA-256    │
      │ ◄════════════════════════════════════════════════════► │
      │  3  verify     8-digit SAS shown on both screens       │
      │ ◄─────────────────── match? ─────────────────────────► │
      │  4  stream     64 KB buffer · SHA-256 · .part → final  │
      │ ═════════════════════════════════════════════════════► │
      │                                                        │
      └──────────── your Wi-Fi. nothing leaves it. ────────────┘
```

| | |
|:--|:--|
| ⚡ **Wire-speed** | Gigabit-class LAN transfers over Wi-Fi, hotspot or USB tethering |
| 🔐 **Mutual TLS 1.3** | `rustls` + `ring`, with pinned device-key fingerprints |
| 🛡️ **SAS pairing** | 8-digit code derived from the TLS exporter to defeat MITM on public Wi-Fi |
| 🗝️ **Keys at rest** | Windows DPAPI and Android Keystore (AES-256-GCM) |
| 🪶 **Flat memory** | Multi-GB files stream through a bounded 64 KB buffer |
| 📡 **Zero-config** | Automatic local discovery, with QR and manual IP fallback |

### Free vs Pro

| | **Free** | **Pro** · $14.99 lifetime · 3 devices |
|:--|:--:|:--:|
| Outgoing file size | 1 MB | **Unlimited** |
| Files per transfer | 1 | **Unlimited batches** |
| Folders | ✕ | **Full trees, paths preserved** |
| Text and snippets | 40 chars | **Unlimited** |
| Paired devices | 1 | **Unlimited** |
| Auto-accept from paired peers | ✕ | **✓** |
| Background listening | ✕ | **✓** |
| Receiving from anyone | **Unlimited** | **Unlimited** |

### Get it

| | | |
|:--|:--|:--|
| 🪟 **Windows 10 / 11** | Installer or portable ZIP | [**Releases →**](https://github.com/thisma-labs/beside/releases/latest) |
| 🤖 **Android 8.0+** | Signed APK (arm64) | [**Releases →**](https://github.com/thisma-labs/beside/releases/latest) |
| 💎 **Beside Pro** | Lifetime license | [**Gumroad →**](https://thismalabs.gumroad.com/l/beside-pro) · [itch.io](https://thisma-labs.itch.io/beside) |
| 📦 **Mirror** | | [SourceForge →](https://sourceforge.net/projects/beside-app/) |

Every release ships with `SHA256SUMS.txt`, so you can verify what you run.

## How we build

```text
local-first    your devices talk to each other, not to our servers
private         no accounts, no telemetry, nothing to leak
verifiable      signed releases, published checksums, a real security policy
small           a 12 MB installer, flat memory, no background bloat
```

## Say hello

- 🐛 Found a bug? [Open an issue](https://github.com/thisma-labs/beside/issues)
- 🔒 Security report? Read [`SECURITY.md`](https://github.com/thisma-labs/beside/blob/main/SECURITY.md)
- ⭐ Like Beside? A star on [the repo](https://github.com/thisma-labs/beside) helps more than you'd think

<div align="center">

<sub>© 2026 Thisma Labs · Built in Sri Lanka · Beside (`•—◎`) is a trademark of Thisma Labs</sub>

</div>
