# Sealyte

Sealyte is a lightweight Windows game-library launcher that consolidates your installed games from multiple PC clients into a single personal hub, combining a Steam-powered discovery page with a high-performance Tauri desktop app.

> *Sealyte is an independent community project. It is not affiliated with, endorsed by, or an official product of Valve, Steam, Epic Games, GOG, or Discord.*

---

## Download & Installation

1. **[Download Sealyte.exe](https://github.com/Sealient/Sealyte/releases/download/v0.1.0/Sealyte.exe)**
2. Run the executable to install it instantly for your user account without requiring administrator permissions.
3. Launch Sealyte straight from your desktop shortcut or Start menu.

* **Install Location:** Automatically places itself in your local programs directory (`%LOCALAPPDATA%\Programs\Sealyte`) and cleans up shortcuts cleanly upon uninstallation.
* **Prerequisites:** Sealyte aggregates your existing client installations; keep Steam, Epic Games, GOG Galaxy, or Discord installed for the games you wish to play.
* **SmartScreen Note:** Because the project does not currently utilize a paid commercial code-signing certificate, Windows SmartScreen may display an unknown-publisher warning on first run.

---

## Core Features

* **Unified Game Library:** Automatically scans installed Steam games, Epic Games manifests, and GOG Galaxy entries across drives. Includes support for custom folder scanning and manual executable additions.
* **Complete Control:** Launch supported games, open installation directories, copy paths, hide clutter, manage hidden titles, and select custom cover art effortlessly.
* **Smart Artwork Caching:** Automatically fetches official base-game covers from Steam and SteamGridDB, with manual fallback options for custom PNG, JPG, or WebP cover art.
* **Sealyte Discover:** Browse live public Steam featured categories and search results directly inside the app, with purchases safely opening your default web browser.
* **Steam Profile Integration:** Securely connect via Steam OpenID to view public profile data without ever sharing or storing your password.
* **Discord Rich Presence:** Automatically displays Sealyte status while active and switches to the live game title upon launching a title. Fully customizable or toggleable via settings.
* **Polished Interface:** Choose between clean card or list layouts, customize pointer lighting effects, reduce motion, and toggle low-memory mode. Includes custom window controls and a draggable frameless title bar.

---

## Performance & Low-Memory Mode

Sealyte is engineered for extreme efficiency, running lean on system resources.

* **Low-Memory Mode:** Enabled by default. It limits initial batch rendering, defers artwork loading until visible, and strips non-essential visual effects.
* **WebView2 Runtime:** The user interface runs on Microsoft's native WebView2 architecture. Keep in mind that Windows splits WebView2 processes away from the main executable when inspecting total RAM usage.

---

## Discord Setup

1. Open your desktop Discord app and verify that **User Settings → Activity Privacy → Share your activity status** is enabled.
2. Open Sealyte. It connects to the local Discord client automatically without requiring credentials or tokens.
3. Use Sealyte's **Settings → Discord Rich Presence** to adjust activity text, test connections, or disable presence entirely.

---

## Privacy & Service Notes

* **Steam OpenID:** Reads only publicly available profile data shared by Steam.
* **Public APIs:** The Discover tab queries public Steam store fronts directly without accessing your browser session or store cookies.
* **Local Storage:** All user preferences, game paths, and custom cover settings remain stored locally on your machine.
