# 8051 Mechanical MacroPad — AI Agent Guide

Custom mechanical macro keypad hardware designed in **KiCad EDA 10.0** around the classic **8051** microcontroller (`0-Name-Alex/8051-Mechanical-MacroPad`).

## 1. Design Files (Preserve Exact Filenames)
- [`MEchanical Macro pad.kicad_pro`](MEchanical%20Macro%20pad.kicad_pro): Master KiCad project configuration.
- [`MEchanical Macro pad.kicad_sch`](MEchanical%20Macro%20pad.kicad_sch): Electrical schematic (8051 MCU core, diode-isolated Cherry MX/Kailh/Gateron switch matrix, crystal/reset/ISP headers).
- [`MEchanical Macro pad.kicad_pcb`](MEchanical%20Macro%20pad.kicad_pcb): PCB layout (Routing WIP; ~70% complete).

## 2. Automated Verification & Exports via `kicad-cli`
KiCad 10 CLI is installed at `"C:\Program Files\KiCad\10.0\bin\kicad-cli.exe"`:
- **Electrical Rules Check (ERC)**:
  ```powershell
  & "C:\Program Files\KiCad\10.0\bin\kicad-cli.exe" sch erc "MEchanical Macro pad.kicad_sch" --exit-code-violations
  ```
- **Design Rules Check (DRC)**:
  ```powershell
  & "C:\Program Files\KiCad\10.0\bin\kicad-cli.exe" pcb drc "MEchanical Macro pad.kicad_pcb" --exit-code-violations
  ```
- **Export Gerbers / Drill / BOM** only into an untracked or dedicated output folder—never commit `.kicad_prl`, `.history/`, or `*-backups/` (enforced by `.gitignore`).
