# SCAPS Simulations for Mixed Sn–Pb Perovskite Solar Cells

This repository contains the **SCAPS-1D** simulation files and exported I–V datasets that support the manuscript:

**Hybrid sequential processing of mixed Sn–Pb narrow-bandgap perovskite solar cells (2025)**

---

## Repository contents

### `Scaps Files - Compositions/`
Device definition files saved from SCAPS-1D (University of Gent, v3.3.12).  
Open these in SCAPS to view full layer stacks, parameters, and run J–V.

- `Pb0.3Sn0.7I2.scaps` — Sn-rich, lowest bandgap case  
- `Pb0.5Sn0.5I2.scaps` — Equimolar composition  
- `Pb0.7Sn0.3I2.scaps` — Pb-rich, higher bandgap case  
- `Figure 2C - Typical.scaps` — Representative device used for Figure 2C

> Notes: files include optical/electrical parameters as used in the paper (mobilities, NA, Dit, cross-sections, Rs/Rsh, thickness, etc.), illumination set to AM1.5G unless otherwise noted.

---

### `Exported J-Vs/`
Outputs used to generate the figures and to report metrics.

- `Pb0.3Sn0.7I2.xlsx`, `Pb0.5Sn0.5I2.xlsx`, `Pb0.7Sn0.3I2.xlsx`  
  – Numeric I–V points exported for each composition (units in sheet headers).
- `Pb0.3Sn0.7I2.png`, `Pb0.5Sn0.5I2.png`, `Pb0.7Sn0.3I2.png`  
  – Per-device I–V plots.
- `Overlaid.png`  
  – Overlay of the three compositions used in the manuscript.
- `Figure 2-c.png`  
  – Final panel image for Figure 2C.
- `Figure2-c.opju`, `IV-Study.opju`  
  – OriginPro project files containing the plotting/overlay setup used to render the PNGs.

---

## How to use

**Run or inspect simulations in SCAPS**
1. Open **SCAPS-1D v3.3.12** (Windows).
2. Load any file from `Scaps Files - Compositions/` (All Scaps Setting → Load all settings).
3. Run Light/Dark J–V as in the paper; parameter values are embedded in the `.scaps` files.

**Reuse plotted data**
- Use the `.xlsx` files in `Exported J-Vs/` to re-plot I–V curves in your preferred tool.
- The provided `.opju` files reproduce the exact overlay/formatting in OriginPro.

---

## Provenance & assumptions
- SCAPS version: **3.3.12** (University of Gent).  
- Illumination: **AM 1.5G, 100 mW cm⁻²**; temperature 300 K (unless otherwise specified in the `.scaps` file).  
- Device naming: `Pb[a]Sn[b]I2` reflects Pb/Sn ratio; three compositions map to Sn-rich → equimolar → Pb-rich.

---

## License
All files in this repository are released under the **MIT license**.  
You are welcome to reuse with attribution.

---

## Citation
If you use these files, please cite:

**Saygili, Y.; Ventosinos, F.; Dehnavi, M.; Yerci, S.; Sessolo, M.; Bolink, H. Hybrid sequential processing of mixed Sn–Pb narrow-bandgap perovskite solar cells. Dalton Trans. 2026, Advance Article. https://doi.org/10.1039/D5DT02879E**
DOI: https://doi.org/10.1039/D5DT02879E


Arranged by: Mohammad Dehnavi
