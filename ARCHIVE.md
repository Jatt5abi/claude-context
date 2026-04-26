# ARCHIVE.md — Long-Term Memory

> Nothing deleted, ever. Claude greps this when you mention old topics.
> Trigger words: project names, tools, people, places — anything specific.

---

## Gridfinity — Espresso Drawer (Lelit Bianca V3) ✅ DONE

### Drawer & Baseplate
- Drawer: 431.8 × 320.7mm (17" × 12⅝"), 82.6mm opening height
- Baseplate: Gridflock system — `~/Downloads/gridfinity-gridflock-baseplate-250x250-320x431-08e58.stl`
- Grid: 7×10 cells at 42mm = 294mm × 420mm usable area
- Strip gap (right side): **23mm measured with calipers** — do NOT recalculate
- Baseplate: ALL PLATES DONE ✅, magnets in ✅
- Filament: Eryone PETG Jet Black | Magnets: 6×2mm press-fit

### Strip Bin Geometry — CONFIRMED WORKING (2026-04-20)
- Foot profile: single continuous taper (Gemini geometry) — NOT two-step kennetek profile
- `body_w = 21.5mm` (23mm cell - 0.5mm clearance, 0.25mm per side)
- `floor_w = 15.2mm` (body_w - 6.3mm)
- `foot_h = 5.0mm`, `lip_h = 0.8mm` with 0.2mm bottom bevel
- Magnet holes: 7.0mm dia × 2.4mm deep — glue in (6×2mm magnets)
- Files: `~/Documents/slim_tray_26x42_test.scad` | `~/Documents/strip_brush_tray_5cell.scad` | `~/Documents/strip_brush_tray_5cell_10mm.scad`

### Bins Printed ✅
- Basket holder (ladder style)
- Strip brush tray 15mm
- Dosing ring bin 2×2×3
- Distributor bin 2×2×3 (71mm outer / 61mm inner / 12mm deep)
- 3×1 spoon trough
- 3×1 coffee spoon trough

### Bins Designed But Not Printed
- Strip brush tray 10mm (1.5mm overhang)
- Leveler bin (same as distributor, 58mm hole)
- Scale bin (Acaia Lunar — flat, angled)
- WDT tool bin
- Water atomizer bin (1.25" dia, sideways half-sunk, 3u high)
- Extra spoon trough (sideways, 5mm tall, 1.75" wide, half sunk)
- Sweetener box bin
- Spoon bin with dividers (37mm slots, removable)

### Drawer Items
1. 18-24g basket (spare)
2. Blind basket
3. Acaia Lunar scale
4. 2 puck screens
5. Sweetener box (Dollar Tree wooden box)
6. Dosing ring (76mm)
7. Distributor / leveler tool (63.5mm)
8. Flick WDT tool
9. Timemore spring-loaded tamp
10. Group head cleaning brushes (strip bin)
11. Espresso spoons

### Tools
- Gridfinity Layout Tool: https://gridfinitylayouttool.com
- Custom bins: OpenSCAD (`~/Documents/`)
- Basket holder: MakerWorld download

### Kitchen Drawer Note
- Likely same drawer dimensions as espresso drawer — measure first but high probability match
- All specs above reusable

---

## Mac Mini Monitor Stem Mount

- File: `~/Documents/mac_mini_mount.scad`
- One-piece PETG — collar clamps monitor arm stem (35mm dia), box holds Mac Mini
- Mac Mini: 7.75" × 7.75" × 1.5" = 196.85 × 196.85 × 38.1mm
- Box interior: 200×198×47mm — 1.57mm per side clearance
- `box_w = 224`, `box_d = 188` — fits P1S 256×256mm plate
- Collar: M4 clamp bolts at BACK, split gap opens rearward
- Port cutouts: left + right of collar
- Bottom vent hole: 171.5mm dia centered (Mac Mini intake)
- Side finger holes: 25mm dia, both sides, ~0.5" behind vent
- Front retaining lip: REMOVED
- Top: solid shelf, Steelers logo TBD via Bambu texture painting
- Print: gyroid 15% infill, gloss PETG test (matte black final)

---

## Mac Mini G5-Style Case

- Mini Pro 5.1 Plus (G5 tower style) designed for M4
- Intel 2018 Mac Mini: 197×197mm — needs redesign or different model
- Mac Pro Enclosure (MakerWorld 791767) confirmed fits M1/M2 = same as Intel 2018

---

## MoneyMate — AI Finance Agent (SCRAPPED 2026-04-26)

- Was: Claude API + Telegram Bot + YNAB, running on Mac Mini
- Bot: @moneymateaibot on Telegram
- Scrapped — deleted `~/moneymate/`
- Vision preserved: proactive agent that texts you when to act on money
- "The personal assistant the wealthy have always had, for regular people"
- If revived: agent-first architecture (it contacts YOU), not chatbot

---

## Pale Horse Driver App PWA

- Live: pale-horse-driver-app.vercel.app
- Stack: Vercel + pdf-lib + Resend
- CDL driver application PWA
- Last worked: v15, Isabel email, I-9 attestation, all sig fixes

---

## Peptide Storage Box (OpenSCAD)

- 4x 3ml vials, pen, syringes
- M screw hinges, hex pattern lid
- Design was pending 2026-04-23 morning

---

## Photos & Videos

- 3,608 photos organized on phone: `/sdcard/Android/media/com.organized.photos/`
- TODO: confirm Google Photos backup + free up ~29GB
- China 25th Anniversary video: `~/Desktop/China/edit/China_25th_Anniversary_Photos.mp4`
- TODO: upload to YouTube for family in India

---

## Heyron / OpenClaw / Discord

- Heyron is a paid AI agent platform ($30/mo) — tokens + infra covered, model router picks AI
- Jeem213 (Discord) built a skill library: https://github.com/jeem213/Heyronskills
- Stuart = the AI agent (capybara theme)
- "Hindsight" = local vector DB for semantic memory search via ngrok
- Concept worth revisiting: vector memory for large archive search
