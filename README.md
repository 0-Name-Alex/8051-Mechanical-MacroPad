# ⌨️ 8051 Mechanical Macro Pad

<div align="center">

**A custom mechanical macro keypad engineered around the classic 8051 microcontroller architecture.**  
Designed in KiCad EDA — featuring mechanical switch matrix, diode isolation, and programmable macro functionality.

[![EDA](https://img.shields.io/badge/EDA-KiCad-314CB0?logo=kicad&logoColor=white)](https://www.kicad.org/)
[![MCU](https://img.shields.io/badge/MCU-8051%20Architecture-blueviolet)](#)
[![Hardware](https://img.shields.io/badge/Hardware-Custom%20PCB-388E3C)](#)
[![Status](https://img.shields.io/badge/Status-PCB%20Routing%20(WIP)-orange)](#)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

</div>

---

## 🎯 Project Overview

This project is a dedicated **hardware macro pad** powered by an 8051 microcontroller. Designed for productivity, gaming macros, and shortcut triggering, it provides tactile mechanical switch input with hardware-level debouncing and matrix scanning.

### ✨ Hardware Highlights

- 🔘 **Mechanical Switches**: Footprints compatible with standard Cherry MX / Kailh / Gateron style switches.
- ⚡ **Anti-Ghosting Matrix**: Individual diode isolation for each switch, supporting N-key rollover across macro triggers.
- 🧠 **8051 Core**: Demonstrates hardware implementation and register-level firmware scanning on the classic embedded 8051 architecture.
- 📐 **Compact Form Factor**: Designed for minimal desktop footprint alongside a primary keyboard.

---

## 📊 Development Status

```
[████████████████████] 100%  Schematic Design & Netlist (Done)
[██████████████░░░░░░]  70%  PCB Layout & Trace Routing (In Progress 🔄)
[░░░░░░░░░░░░░░░░░░░░]   0%  Final Fabrication Gerbers & BOM (Upcoming)
[░░░░░░░░░░░░░░░░░░░░]   0%  Firmware Implementation & Keymapping (Upcoming)
```

> ⚠️ **Note:** This project is actively being routed and finalized in KiCad. Final revision Gerbers and assembly photos will be added upon manufacturing!

---

## 📁 Repository Files

| File | Description |
|---|---|
| `MEchanical Macro pad.kicad_pro` | Master KiCad project file |
| `MEchanical Macro pad.kicad_sch` | Full electrical schematic diagram & switch matrix netlist |
| `MEchanical Macro pad.kicad_pcb` | Board layout, copper traces, footprints, and silk screen |

---

## 🛠️ Opening the Project

1. Install [**KiCad EDA**](https://www.kicad.org/) (version 7.0 or later recommended).
2. Clone this repository:
   ```bash
   git clone https://github.com/0-Name-Alex/8051-Mechanical-MacroPad.git
   ```
3. Open `MEchanical Macro pad.kicad_pro` in KiCad to view both the schematic and PCB layout editor.

---

## 📄 License

Open-source hardware project licensed under the MIT License.
