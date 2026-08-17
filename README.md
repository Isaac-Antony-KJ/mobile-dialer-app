<div align="center">

# 📞 Queue Dialer

**A lightweight, installable call-sheet for streamlined outbound calling — sales, surveys, customer support, GOTV, you name it.**

[![Made with HTML5](https://img.shields.io/badge/HTML5-1F7A4D?style=for-the-badge&logo=html5&logoColor=white)](#)
[![Made with JavaScript](https://img.shields.io/badge/JavaScript-1F7A4D?style=for-the-badge&logo=javascript&logoColor=white)](#)
[![PWA Ready](https://img.shields.io/badge/PWA-Installable-1F7A4D?style=for-the-badge&logo=pwa&logoColor=white)](#)
[![License](https://img.shields.io/badge/License-MIT-1F7A4D?style=for-the-badge)](#-license)

*No backend. No sign-up. No data leaving your device.*

</div>

---

## ✨ What it does

Upload a contact list, work through it one call at a time, and log what happened — all in a single HTML file you can host anywhere or drop on your home screen.

| | |
|---|---|
| 📁 **Spreadsheet import** | Drop in an `.xlsx`, `.xls`, or `.csv` file — Column A for **Name**, Column B for **Phone**. Header rows and duplicate numbers are detected and skipped automatically. |
| 🔍 **Searchable selection** | Filter the imported list and select exactly who goes into today's queue. Selections persist through search — nothing silently un-checks itself. |
| 🟩 **The Board** | A color-coded strip showing every contact's status at a glance — pending, answered, no answer, voicemail, or call back. Tap any pending tile to jump straight to it. |
| ☎️ **One-tap dial** | Big call button opens your device's native dialer via `tel:` links. Redial available if a call drops. |
| 🏷️ **Outcome logging** | Every call gets tagged — **Answered / No Answer / Voicemail / Call Back** — instead of a flat "done" checkbox, so your report is actually useful afterward. |
| ✍️ **Manual add** | Add one-off numbers to the queue on the fly, with duplicate and format checks. |
| ⏱️ **Session timer & progress** | Live elapsed time and an X-of-Y counter while you work. |
| 📊 **Session report** | Auto-grouped by outcome with an answer-rate stat. Copy to clipboard, send to WhatsApp, or download as `.txt`. |
| 🌓 **Light / dark theme** | Follows your system setting by default, with a manual override that sticks. |
| 🔒 **Local-only** | Every bit of parsing and queue management happens in your browser. Nothing is uploaded anywhere. |

> **Not yet included:** a native contact-picker integration (e.g. Android's Contact Picker API) — right now, contacts come in via spreadsheet or manual entry. Open an issue or ask if you'd like this added.

---

## 🚀 Getting started

1. Host `queue-dialer.html` anywhere static — GitHub Pages, Netlify, or just open the file locally.
2. On **Android + Chrome**, open the page, tap the **⋮** menu → **Add to Home screen** / **Install app** for a full-screen, app-like experience.
3. Import your list:
   - **Upload a sheet** — drag a file onto the drop zone, or tap to browse, *or*
   - **Skip straight to the queue** and add numbers manually.
4. Search and select who you want to call, then **Create queue**.
5. Work the queue: **Call now** → log the outcome (**Answered / No Answer / Voicemail / Call back**) → the app auto-advances to the next pending contact.
6. When you're done, tap **Pause or end session** to pull up your report — copy it, send it to WhatsApp, or download it as a text file.

---

## 🎨 Theme

The interface uses a small "operator console" palette — mono type for numbers, and colors borrowed from real telephone semantics (green = call, red = end).

| Token | Light | Dark |
|---|---|---|
| Background | `#EDEFEA` | `#101208` |
| Card | `#FFFFFF` | `#191C13` |
| Text | `#171A14` | `#EEF0E6` |
| Answered (green) | `#1F7A4D` | `#45B37B` |
| No answer (red) | `#B23A22` | `#E36A4C` |
| Voicemail (blue) | `#2B5D8B` | `#6FA3D8` |
| Call back (amber) | `#A9761F` | `#DCAB55` |

All colors live as CSS custom properties at the top of the file — change them once, and every component updates.

---

## 🛠️ Built with

- **HTML5 · CSS3 · Vanilla JavaScript** — no build step, no framework
- **[SheetJS (xlsx)](https://sheetjs.com/)** — client-side spreadsheet parsing
- **`tel:` links** — native dialer handoff on mobile browsers

---

## 🔒 Privacy

All parsing and queue management happen locally in your browser. There is no backend, no analytics, and no data transmitted anywhere — the only network calls the app makes are the CDN scripts/fonts it loads and, if you tap it, WhatsApp's share link.

---

## 📄 License

Open-source under the MIT License — free for personal and commercial use.
