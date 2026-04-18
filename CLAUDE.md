# Claude Context — Ravinder Gill

## Who I Am
- **Name:** Ravinder Gill (9.18.76)
- **Family:** Wife Sukhi (12.17.1976), Sons Arjun "Dave" (3.14.2006) & Vikram "Vik" (5.12.2001) Kurtis (4.13.1995) Kurtis lives in London and was born to Ravinder high school sweet heart.
- **Work:** Paving / road construction — Superintendent, drives a spreader truck, chip sealing, slurry work
- **Devices:** Samsung Android (Termux) + Mac Mini
- **Storage:** Google Drive 5TB, Google Photos, Samsung Gallery
- **Subscriptions:** ChatGPT Plus ($20/mo), Claude Code $20 Gemini included with google 1

## How We Work Together
- End of every chat: push updated CLAUDE.md to this GitHub repo (https://github.com/Jatt5abi/claude-context)
- Same repo cloned on Mac (`git clone https://github.com/Jatt5abi/claude-context.git`) — always in sync
- Open `~/claude-context` as working directory in Claude Code on any device
- When Ravinder says anything like "ok i gotta go", "talk to you later", "goodbye", "later", "peace", "have a coffee", "play with X" — stop, update CLAUDE.md with session notes, push to GitHub, then confirm
- GitHub CLI (`gh`) authenticated as **Jatt5abi** on Android

---

## Session Notes (2026-04-17 — full day)

### Gridfinity Espresso Drawer
- Confirmed standard Gridfinity 42mm grid
- Drawer dimensions: 17" × 12⅝" × 3¼" opening = 431.8 × 320.7 × 82.6mm
- Fits **10×7 standard 42mm Gridfinity baseplate** (420×294mm with small margins)
- Tried GridCoffee (78mm grid system) — skipped, mostly plain trays
- Moka pot accessories removed from drawer (modded basket, dosing ring, tamp for moka)

**Final drawer item list (Bianca V3 only):**
1. 18-24g basket (spare)
2. Blind basket
3. Acaia Lunar scale
4. 2 puck screens
5. Sweetener box (dollar tree wooden box)
6. Spouted portafilter (deprioritized — print last)
7. Dosing ring
8. Leveler tool (lay flat, clears opening easily)
9. Flick WDT tool (lay flat — too tall standing)
10. Timemore spring-loaded tamp (lay flat — too tall standing)

**Bins found on MakerWorld:**
- Baskets + puck screens: penguinprints — https://makerworld.com/en/models/718533
- Portafilter (round): https://makerworld.com/en/models/718546 (2×2, 83.5mm)
- Bezerra portafilter bin in Downloads (3×6, deprioritized)

**Plan for remaining items (tamp, WDT, leveler, dosing ring, scale, sweetener box):**
- Use **ToolTrace** (https://www.tooltrace.ai/) — lay tools flat on paper, take top-down photo, generates custom Gridfinity STL inserts
- Use standard 42mm grid in ToolTrace so bins snap to standard baseplate

**TODO next session:**
- Ravinder to experiment with ToolTrace and report back
- Confirm Google Photos backup completed + free up ~29GB on device
- Once all bins confirmed, print baseplate (10×7) and all bins

---

## Active Projects

### Photos — DONE (2026-04-17)
- 3,608 photos organized into date folders (2020-09 through 2026-04)
- Location: `/sdcard/Android/media/com.organized.photos/` (one folder per month)
- WhatsApp images merged into date folders; DCIM originals deleted
- **This folder is the ONLY local copy — do not delete until Google Photos backup confirmed**

**TODO:**
- Confirm Google Photos backup completed
- Hit "Free up space on device" in Google Photos → reclaims ~29GB

---

### 3D Printing — Gridfinity Espresso Drawer (IN PROGRESS)
- Printer: **Bambu P1S**
- Drawer: 431.8 × 320.7mm, 82.6mm opening height
- Baseplate: **10×7 standard 42mm Gridfinity**
- See item list and bin plan above

---

### China 25th Anniversary Video — COMPLETE (2026-04-17)

**Final output files:**
| File | Duration | Size | Notes |
|------|----------|------|-------|
| `25th_Anniversary_FINAL_v2.mp4` | 11m 14s | 734MB | Film + music, v2 edit |
| `25th_Anniversary_v2_WITH_CREDITS.mp4` | 12m 29s | 744MB | Film + music + end credits |
| `China_25th_Anniversary_Photos.mp4` | 7m 43s | 62MB | All 188 photos, YouTube stills |

All files at: `/home/ravi/Desktop/China/edit/`

**Build scripts:**
- `build_cinematic.py` — main film (32 clips, v2 edit)
- `build_credits_and_stills.py` — end credits + YouTube stills

**v2 edit narrative (32 clips):**
- Opening title
- **HK:** rooftop breakfast (CHINAVID1), TST waterfront (0044), Sukhi walking HK skyline (0045), Ravi in HK (0025)
- **Transit:** lounge (0062), Ravi & Sukhi at terminal (0083), train window crossing (ChinaVid3)
- **Shenzhen:** skyline arrival (ChinaVid4), wave building (0090), couple selfie (0091), Ravinder wonder (0103), Ravinder still (0203)
- **Coffee:** detail shot (0047), Roastery stairs (0197)
- **Ferry centrepiece:** boarding (0140) → mid-river (0143) → Pudong REVEAL (0155) → docking (0156)
- **Bund:** Sukhi stills (0172, 0175), Peace Hotel (0184)
- **Temple:** red lanterns (0232)
- **Night:** Bund walk (0216), Pudong skyline (0210), neon streets (0208)
- **Grandeur:** Shanghai Tower aerial (0237)
- **Art:** digital wall (0247), lotus architecture (0250), neon climax (0252)
- **Home:** Ravinder with son (0273)
- Finale title

**Clips removed from v1:** hotel room towers (0087), hotel window (0115)

**Music:**
- `music2.mp3` (128s intro) + `music.mp3` (looped, 546s) = 674s bed → `music_v2.mp3`
- Build scripts cache clips by beat name (not index) — re-run safe

**TODO:**
- Upload `China_25th_Anniversary_Photos.mp4` to YouTube for family in India

---

## Preferences
- Terse responses — no fluff, witty, fun but brutly honest. No glazing
-  emojis are fine 
- No trailing summaries ("here's what I did")
