# gridfinity.md — Espresso Drawer Project

## Drawer Specs
- Size: 431.8 × 320.7mm (17" × 12⅝"), 82.6mm opening height
- Machine: Bianca V3

## Baseplate
- System: **Gridflock**
- STL: `~/Downloads/gridfinity-gridflock-baseplate-250x250-320x431-08e58.stl`
- Grid: 7×10 cells at 42mm = 294mm × 420mm
- Strip gap right side: **23mm measured** (calipers — do not recalculate)
- Status: ALL DONE ✅ — magnets in (6×2mm press-fit)
- Filament: Eryone PETG Jet Black

## Strip Bin Geometry — CONFIRMED (2026-04-20)
Single continuous taper foot — NOT the standard two-step kennetek profile.

```openscad
body_w  = 21.5;   // 23mm cell - 0.25mm clearance per side
body_l  = 41.5;
floor_w = 15.2;   // body_w - 6.3mm (Gemini golden rule)
floor_l = 35.2;   // body_l - 6.3mm
foot_h  = 5.0;
lip_h   = 0.8;    // with 0.2mm bottom bevel to clear magnet pocket rims
mag_r   = 3.5;    // 7mm dia — glue in (6×2mm magnets)
mag_h   = 2.4;
```

Key: `clearance = 0.25mm per side`, `floor_offset = 3.15mm per side`

## Custom OpenSCAD Files
| File | Description |
|------|-------------|
| `~/Documents/slim_tray_26x42_test.scad` | Single-cell test piece — confirmed fit |
| `~/Documents/strip_brush_tray_5cell.scad` | 5-cell brush tray, 15mm walls |
| `~/Documents/strip_brush_tray_5cell_10mm.scad` | 5-cell brush tray, 10mm walls, 1.5mm overhang |

## Bins Status
| Bin | Size | Status |
|-----|------|--------|
| Basket holder (ladder) | 2×2×3 | ✅ Printed |
| Strip brush tray 15mm | 5-cell strip | ✅ Printing |
| Dosing ring (71mm hole) | 2×2×3 | ✅ Printing |
| Distributor (71mm/61mm stepped) | 2×2×3 | ✅ Printing |
| Spoon trough 3×1 | 3×1×3 | ✅ Printing |
| Coffee spoon trough 3×1 | 3×1×3 | ✅ Printing |
| Sweetener box bin | 2×3×8 | ✅ Downloaded |
| Strip brush tray 10mm | 5-cell strip | ⬜ Designed |
| Leveler bin (58mm hole) | 2×2×3 | ⬜ Design — same as distributor |
| Scale bin (Acaia Lunar) | TBD | ⬜ Flat/angled |
| WDT tool bin | TBD | ⬜ |
| Tamp bin | TBD | ⬜ |
| Spoon bin with removable dividers | TBD | ⬜ 37mm slots |

## Drawer Item List (Bianca V3)
1. 18-24g basket (spare)
2. Blind basket
3. Acaia Lunar scale
4. 2 puck screens
5. Sweetener box (Dollar Tree wooden box)
6. Dosing ring (76mm)
7. Distributor / leveler
8. Flick WDT tool
9. Timemore spring-loaded tamp
10. Group head cleaning brushes (strip bin)
11. Espresso spoons

## Downloads Kept
| File | Purpose |
|------|---------|
| `gridfinity-gridflock-baseplate-250x250-320x431-08e58.stl` | Baseplate STL |
| `Mini+Pro+5.1+Plus.3mf` | Mac Mini G5 case (M4 — needs resize for Intel) |
| `3x1 coffee spoon.stl` | Coffee spoon trough |
| `3x1 spoons.stl` | Spoon trough |
| `Dosing+Ring_2x2x3_solid_magnets.stl` | Dosing ring bin |
| `sweetner box 2x3x8.zip` | Sweetener box bin |

## Tools
- Bin generator: https://gridfinitylayouttool.com
- Custom strip bins: OpenSCAD
- Standard unit: 42mm grid, 7mm height
