# MEMORY.md — Active Projects & Session Notes

## 3D Printing — Gridfinity Espresso Drawer (IN PROGRESS)

### Drawer & Baseplate
- Drawer: 431.8 × 320.7mm (17" × 12⅝"), 82.6mm opening height
- Baseplate: **Gridflock** system — `~/Downloads/gridfinity-gridflock-baseplate-250x250-320x431-08e58.stl`
- Grid: **7×10 cells** at 42mm = 294mm × 420mm usable area
- Strip gap (right side): **23mm measured with calipers** — do NOT recalculate
- Baseplate status: ALL PLATES DONE ✅, magnets in ✅
- Filament: Eryone PETG Jet Black | Magnets: 6×2mm press-fit

### Strip Bin — CONFIRMED WORKING (2026-04-20)
- Foot profile: **single continuous taper** (Gemini geometry) — NOT the two-step kennetek profile
- `body_w = 21.5mm` (23mm cell - 0.5mm clearance, 0.25mm per side)
- `floor_w = 15.2mm` (body_w - 6.3mm)
- `foot_h = 5.0mm`, `lip_h = 0.8mm` with 0.2mm bottom bevel
- Magnet holes: 7.0mm dia × 2.4mm deep — glue in (6×2mm magnets)
- Files: `~/Documents/slim_tray_26x42_test.scad` (confirmed fit) | `~/Documents/strip_brush_tray_5cell.scad` (15mm walls) | `~/Documents/strip_brush_tray_5cell_10mm.scad` (10mm walls, 1.5mm overhang)

### Bins Status (2026-04-20)
- ✅ Basket holder (ladder style) — printed
- ✅ Strip brush tray 15mm — printed
- ✅ Dosing ring bin 2×2×3 — printed
- ✅ Distributor bin 2×2×3 (71mm outer / 61mm inner / 12mm deep) — printed
- ✅ 3×1 spoon trough — printed
- ✅ 3×1 coffee spoon trough — printed
- ⬜ Strip brush tray 10mm — designed, not yet printed
- ⬜ Leveler bin (same as distributor, 58mm hole)
- ⬜ Scale bin (Acaia Lunar — flat, angled)
- ⬜ WDT tool bin — daily use, via bin generator
- ⬜ Water atomizer bin — 1.25" dia, lay sideways half-sunk, 3u high
- ⬜ Extra spoon trough — spoon sideways, 5mm tall, 1.75" wide, half sunk
- ⬜ Sweetener box bin
- ⬜ Spoon bin with dividers (37mm slots, removable)

### Drawer Item List (Bianca V3)
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

### Tools Used
- Custom bins: **Gridfinity Layout Tool** (https://gridfinitylayouttool.com)
- Custom strip bins: **OpenSCAD** (`~/Documents/`)
- Basket holder: MakerWorld download

---

## Mac Mini Monitor Stem Mount (PRINTING 2026-04-21)
- File: `~/Documents/mac_mini_mount.scad`
- One-piece PETG print — collar clamps vertical monitor arm stem (35mm dia), box holds Mac Mini inside
- Print material: **gloss PETG test print** (matte black is final if gloss looks bad)
- Mac Mini: 7.75" × 7.75" × 1.5" = 196.85 × 196.85 × 38.1mm
- Box interior: 200×198×47mm — 1.57mm per side width clearance
- `box_w = 224`, `box_d = 188` — fits P1S 256×256mm plate
- Collar: M4 clamp bolts at BACK, split gap opens rearward
- Port cutouts: left + right of collar for cable access
- Bottom vent hole: 171.5mm dia centered on floor (Mac Mini intake)
- Side finger holes: 25mm dia, both sides, ~0.5" behind vent circle — power button access
- Front retaining lip REMOVED (was sticking out awkwardly)
- Top surface: solid shelf, Steelers logo TBD via Bambu texture painting
- Status: **PRINTING NOW** — gyroid 15% infill

---

## Office Room Setup (IN PROGRESS)
- Downstairs room converting to print lab / Mac office
- Has: sit/stand TikTok 80 desk, 2 monitors (Vik's), Mac Mini, comfy chair
- Bed needs to go to trash
- Considering: 49" curved ultrawide from AliExpress (~$117)
- Amp: Facmogu F900S installed, working

---

## Future Ideas
- **Punjabi 3D prints** — Khanda, Ik Onkar, nameplates for trucker dashboards. Etsy + Facebook Punjabi trucker groups. $20-30/piece
- **Day trading** — learn over summer, paper trade first. Need $25K min (PDT rule). Off season Nov 2026.
- **Mac Mini case** — Mini Pro 5.1 Plus (G5 tower style) designed for M4. Intel 2018 is 197×197mm — needs redesign or different model. Mac Pro Enclosure (MakerWorld 791767) confirmed fits M1/M2 = same as Intel 2018.

---

## Completed Projects
- **Photos** (2026-04-17): 3,608 photos organized on phone `/sdcard/Android/media/com.organized.photos/` — TODO: confirm Google Photos backup + free up ~29GB
- **China 25th Anniversary Video** (2026-04-17): Files at `~/Desktop/China/edit/` — TODO: upload `China_25th_Anniversary_Photos.mp4` to YouTube for family in India
