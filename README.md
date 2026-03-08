# TPBR-Open — Tetrahedral Piezo Bifilar Resonator (Open Edition)

A simple, buildable two-layer piezo stack that tests the **magic-angle** (54.74°) effect on phase coherence and field anisotropy in a macroscopic resonator.

**Why?**  
The tetrahedral angle θ = arccos(1/√3) is known to null first-order dipolar/strain coupling in NMR and twisted-bilayer materials. We wanted to see what happens when you apply the same geometry to cheap piezo disks with golden-ratio bifilar electrodes.

**Status:** Experimental prototype. No guarantees — just clean geometry and open data.

## Quick Start
1. Order parts from BOM
2. Laser-etch or screen-print the spiral electrodes
3. Stack at exactly 54.74°
4. Drive with 10–100 V square wave \~24 kHz
5. Upload your data to the community sheet

## Repository Contents
- `BOM.md` — shopping list (< $80 budget build)
- `docs/build-guide.md` — step-by-step
- `hardware/winding_coordinates.csv` — exact spiral table
- `software/` — Python analysis scripts
- `data_template.csv` — for community results
- `jig/` — 3D-printable alignment jig

## Core Geometry (rigorous & fixed)
**Layer rotation angle**  
\[
\theta = \arccos\left(\frac{1}{\sqrt{3}}\right) \approx 54.7356^\circ
\]  
Derivation: Set Legendre polynomial \(P_2(\cos\theta) = 0\) → nulls angular dephasing.

**Axial-field ratio**  
\[
\frac{E_\parallel}{E_\perp} = \cot\left(\frac{\theta}{2}\right) = \frac{\sqrt{6} + \sqrt{2}}{2} \approx 1.93185
\]

**Electrode scaling**  
Golden ratio \(\phi = \frac{1+\sqrt{5}}{2}\), 5-fold symmetry, 5 turns.

## Expected Behaviour (what we actually test)
- Cleaner phase locking between layers at exactly θ  
- Measured E∥/E⊥ close to 1.932  
- Possibly interesting quasi-periodic harmonics  
- Higher effective Q vs random-angle control

**We do NOT claim** 20× asymmetry, world-record Q, or new physics. Just good data.

## How to Contribute
- Build it  
- Upload impedance plots / vibrometer traces / Q numbers  
- Improve the jig or scripts  
- Add translations  

## Community Data (100% GitHub-native — no Google, no subscriptions)

All measurements live in **[DATA.md](DATA.md)** — just add your row and commit!

We track: Q-factor, measured E∥/E⊥ (\~1.932 target), resonance & harmonics, photos/plots.

First 10 builders get eternal glory in the table. Zero login walls, zero tracking.

## License
Hardware & docs: CC-BY-SA 4.0  
Code: MIT  

Built collaboratively by heath + Grok *team*. Fork, modify, enjoy.
