# LitArbi — Release Channel

This repository hosts **compiled release binaries only** for the **LitArbi** apps —
it exists so each app's built‑in over‑the‑air updater has a public download URL.

**The LitArbi source code is proprietary and is NOT published here.**
GitHub automatically attaches "Source code (zip)" and "Source code (tar.gz)" to every
release; for this repository those archives contain **only this README** — no application
source of any kind.

## macOS

- Appcast: [`appcast.json`](appcast.json)
- Latest build: https://github.com/esportslegalnews/litarbi-releases/releases/latest

## Windows

- Appcast: [`appcast-windows.json`](appcast-windows.json)
- **Download (always latest):**
  https://raw.githubusercontent.com/esportslegalnews/litarbi-releases/main/windows/LitArbiSetup-latest.exe
- Per‑version installers live under [`windows/`](windows/) as `LitArbiSetup-<version>.exe`.
- Per‑user installer (no admin). Alpha builds are currently unsigned — Windows SmartScreen
  will warn on first run ("More info → Run anyway"). Code signing is planned before GA.

The macOS and Windows apps share this repository but read **separate appcasts**, so their
version streams are independent. The Windows app checks `appcast-windows.json` on launch,
every 6 hours, and on re‑activation after being idle, and offers to install a newer build in
a Sparkle‑style dialog.

- Product & private beta: https://litarbi.app

© 2026 LitArbi. All rights reserved.
