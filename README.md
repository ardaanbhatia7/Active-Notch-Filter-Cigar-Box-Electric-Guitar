# Active Notch Filter for Cigar Box Electric Guitar

A complete analog hardware project that designs, simulates, and demonstrates an **active notch filter** for removing unwanted frequency content in a cigar box electric guitar signal path.

This repository contains the simulation files, PCB/schematic design files, demonstration videos, and the project report used to document the full design/build process.

---

## Project Overview

This project compares passive and active notch filter approaches, then implements an active design suitable for guitar signal conditioning.

### What this project demonstrates
- Analog filter design (passive + active notch topologies).
- LTspice simulation workflow and AC/frequency-response verification.
- Practical op-amp implementation and gain staging for instrument-level signals.
- PCB and schematic implementation in KiCad for manufacturable hardware.
- End-to-end hardware demonstration in a real guitar context.

---

## Repository Contents

- `Ardaan_EE202_FinalProject_Report.pdf`  
  Full final report with design rationale, analysis, calculations, and results.
- `ActiveNotchFilter.asc`  
  LTspice schematic for the active notch filter implementation.
- `PassiveNotchFilter.asc`  
  LTspice schematic for passive notch filter baseline/comparison.
- `1719.kicad_sch`  
  KiCad schematic source for the hardware design.
- `1719.kicad_pcb`  
  KiCad PCB layout source for the hardware implementation.
- `Yash_Ardaan_NotchFilter_Demo.mp4`  
  Video demo focused on notch filter behavior/performance.
- `Yash_Ardaan_Guitar_Demo.mp4`  
  Video demo of the guitar setup and practical output.

---

## Technical Snapshot

From the simulation files in this repo:

- Passive network uses a twin-T style RC arrangement with representative values such as:
  - `R1 = 10k`, `R2 = 10k`, `R3 = 5k`
  - `C1 = 81.2n`, `C2 = 81.2n`, `C3 = 162.4n`
- Active simulation includes op-amp stages and ±9 V supplies.
- Active design includes feedback and buffering stages to improve notch depth/behavior compared to a purely passive implementation.
- Hardware design references an LM324-class op-amp implementation in KiCad.

> The complete derivation, measured/simulated plots, and design decisions are documented in the report PDF.

---

## How to Open / Reproduce

### 1) LTspice simulations
1. Open `PassiveNotchFilter.asc` in LTspice.
2. Run AC analysis and inspect notch behavior.
3. Open `ActiveNotchFilter.asc`.
4. Run AC analysis and compare notch depth/shape and response.

### 2) KiCad hardware files
1. Open `1719.kicad_sch` in KiCad Schematic Editor.
2. Open `1719.kicad_pcb` in KiCad PCB Editor.
3. Review footprint assignment, routing, and board stackup.

### 3) Demonstration videos
- Watch `Yash_Ardaan_NotchFilter_Demo.mp4` and `Yash_Ardaan_Guitar_Demo.mp4` for practical behavior and end-to-end usage.

---

## Resume-Focused Highlights

If you're reviewing this project from my resume, key evidence of engineering work includes:

- Designed and analyzed active/passive analog notch filters for audio-frequency applications.
- Performed simulation-driven validation using LTspice.
- Translated simulated circuits into PCB-realizable schematic/layout workflows in KiCad.
- Produced a formal project report and practical demo videos to communicate technical outcomes.

---
