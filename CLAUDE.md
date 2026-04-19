# Claude Context — Ravinder Gill

## Who I Am
- **Name:** Ravinder Gill (9.18.76)
- **Family:** Wife Sukhi (12.17.1976), Sons Arjun "Dave" (3.14.2006) & Vikram "Vik" (5.12.2001) Kurtis (4.13.1995) Kurtis lives in London and was born to Ravinder high school sweet heart.
- **Work:** Paving / road construction — Superintendent, drives a spreader truck, chip sealing, slurry work. Off season Nov–Mar.
- **Devices:** Samsung Galaxy Z Fold 3 SM-F966U1 (Android 16) + Mac Mini (Apple T2, running Ubuntu t2-noble kernel 6.19.11)
- **Storage:** Google Drive 5TB, Google Photos, Samsung Gallery
- **Subscriptions:** ChatGPT Plus ($20/mo), Claude Code $20, Gemini included with Google One

## How We Work Together
- End of every chat: push updated CLAUDE.md to this GitHub repo (https://github.com/Jatt5abi/claude-context)
- Same repo cloned on Mac (`~/claude-context`) — always in sync
- When session gets long and Claude starts making mistakes: update CLAUDE.md, push, start fresh chat
- When Ravinder says anything like "ok i gotta go", "talk to you later", "goodbye", "later", "peace", "have a coffee", "play with X" — stop, update CLAUDE.md with session notes, push to GitHub, then confirm
- GitHub CLI (`gh`) authenticated as **Jatt5abi** on Android

---

## Session Notes (2026-04-19)

### scrcpy — Phone Mirror to Linux (WORKING)
- Samsung Z Fold 3 mirrors to Mac Mini via scrcpy 3.3.1
- Snap version broken (gpu-2404 slot issue) — use binary from `~/scrcpy-linux-x86_64-v3.3.1/`
- **Wired (USB):** `~/scrcpy-linux-x86_64-v3.3.1/scrcpy -d`
- **Wireless:** connect via `adb connect IP:PORT` first, then `~/scrcpy-linux-x86_64-v3.3.1/scrcpy --tcpip=IP:PORT`
- Wireless port changes every time you leave/re-enter Wireless Debugging on phone
- USB File Transfer (MTP) mode required for wired adb
- Mouse scroll wheel = swipe up/down in TikTok — works great
- Clipboard sync phone→Mac works; Mac→phone needs `--clipboard-autosync` flag

### File Transfer Phone ↔ Mac
- **LocalSend** installed (snap) — works but not seamless, requires IP/PIN on same WiFi
- Google Drive 5TB is fallback

### Office Room Setup (IN PROGRESS)
- Downstairs room (was parents' room) being converted to print lab / Mac office
- Currently has: sit/stand TikTok 80 desk, 2 monitors (Vik's), Mac Mini, standing mirror, chest of drawers, comfy chair
- Bed needs to go to trash (brother's old bed)
- Plan: printer + Mac in one room, build it out slowly
- Considering: 49" curved ultrawide from AliExpress (~$117, verify specs before ordering), 2× Pioneer passive bookshelf speakers
- Amp ordered: **Facmogu F900S** 160W Bluetooth 5.0 amp, 80W×2, comes with 12V PSU — $28 — plug speakers in, pair Mac via BT
- Chair coaster idea: build wood base with casters to raise + roll the comfy chair 😄

### Future Ideas
- **Punjabi 3D prints** — Khanda, Ik Onkar, Punjabi script nameplates for trucker dashboards. Currently only cheap plastic imports from India. Could sell on Etsy + Facebook Punjabi trucker groups. $20-30 per piece.
- Day trading — learn over summer, paper trade first. Need $25K minimum (PDT rule), $50-100K to replace income. Off season starts Nov 2026.

---

## Active Projects

### 3D Printing — Gridfinity Espresso Drawer (IN PROGRESS)
- Printer: **Bambu P1S**
- Drawer: 431.8 × 320.7mm, 82.6mm opening height
- Baseplate: **10×7.5 42mm Gridfinity** — split into 4 plates

**Baseplate status (2026-04-19):**
- Plate 1: PRINTED but magnets misaligned due to over-careful placement at layer resume — may reprint, check if bins still snap first
- Plate 2: DONE — clean, no pause, magnets glued after ✅
- Plate 3: DONE ✅
- Plate 4: PRINTING (~57 min remaining as of session end)
- Filament: Eryone PETG Jet Black

**Key lessons:**
- NO pause for magnets — cold layer line visible + plate shifts on resume. Glue 6×2mm magnets after with super glue.
- Normal placement method: angle plate in, push to end guide, let it sit. Don't fidget with corners.
- Eryone filament: strip cardboard hub, bare spool fits inside Bambu spool shell — no respooling needed. AMS reads fine.

**Bins status:**
- Slim brush tray: DESIGNED in OpenSCAD (`~/Documents/`), PRINTING NOW in matte black PETG (~57 min). Print 2×. Mirror along X axis in Bambu to fix magnet hole orientation.
- Spoon tray: NOT designed — wait to see brush tray result first
- Basket/puck screen ladder holder: DOWNLOADED `~/Downloads/espresso_round_extracted/` — NOT printed
- Portafilter bin: DEPRIORITIZED
- Scale, dosing ring, leveler, WDT, tamp, sweetener: use **ToolTrace** (https://www.tooltrace.ai/) — lay flat, photo, generates custom Gridfinity STL

**Final drawer item list (Bianca V3 only):**
1. 18-24g basket (spare)
2. Blind basket
3. Acaia Lunar scale
4. 2 puck screens
5. Sweetener box (dollar tree wooden box)
6. Spouted portafilter (deprioritized)
7. Dosing ring
8. Leveler tool (lay flat)
9. Flick WDT tool (lay flat)
10. Timemore spring-loaded tamp (lay flat)

**MakerWorld bins:**
- Baskets + puck screens: penguinprints — https://makerworld.com/en/models/718533
- Portafilter (round): https://makerworld.com/en/models/718546 (2×2, 83.5mm)

---

### Photos — DONE (2026-04-17)
- 3,608 photos organized into date folders (2020-09 through 2026-04)
- Location: `/sdcard/Android/media/com.organized.photos/`
- **TODO:** Confirm Google Photos backup → hit "Free up space" → reclaims ~29GB

---

### China 25th Anniversary Video — COMPLETE (2026-04-17)

| File | Duration | Size |
|------|----------|------|
| `25th_Anniversary_FINAL_v2.mp4` | 11m 14s | 734MB |
| `25th_Anniversary_v2_WITH_CREDITS.mp4` | 12m 29s | 744MB |
| `China_25th_Anniversary_Photos.mp4` | 7m 43s | 62MB |

All files at: `/home/ravi/Desktop/China/edit/`
**TODO:** Upload `China_25th_Anniversary_Photos.mp4` to YouTube for family in India

---

## Mac Mini Linux Notes

### scrcpy Binary Location
- Working binary: `~/scrcpy-linux-x86_64-v3.3.1/scrcpy`
- Snap version broken — don't use `/snap/bin/scrcpy`

### Bluetooth Fix (2026-04-18)
- BCM UART Bluetooth was failing — fixed with `sudo apt install apple-firmware-script` then `sudo get-apple-firmware` (option 3) + full reboot

---

## Preferences
- Terse responses — no fluff, witty, fun but brutally honest. No glazing
- Emojis are fine
- No trailing summaries ("here's what I did")
- Long sessions go sideways — reset early, push to GitHub, start fresh chat
