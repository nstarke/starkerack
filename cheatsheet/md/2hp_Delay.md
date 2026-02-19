# 2hp — Delay

- [Manual PDF](../../manuals/Delay_Manual.pdf)

---

[**Delay 2hp Manual (PDF)**](#) <!-- Replace "#" with actual link if available -->

---

# 2hp Delay Eurorack Module Cheat Sheet

## Overview
Full-featured, CV-controllable delay module.  
- Delay time: ms to ~2 seconds  
- CV over all parameters  
- Feedback: from slapback to infinite repeats  
- Compact 2 HP width

---

## Controls & Jacks

| # | Label    | Type        | Function & Details                                      | Voltage Range      |
|---|----------|-------------|--------------------------------------------------------|--------------------|
| 1 | **IN**   | Jack        | Audio Input (10Vpp)                                    | 10Vpp              |
| 2 | *TIME CV*| CV Input    | CV for Delay Time; summed with knob position           | 0V – 5V            |
| 3 | **TIME** | Knob        | Delay Time (min ↔ max, left ↔ right)                   | --                 |
| 4 | *FDBK CV*| CV Input    | CV for Feedback; summed with knob position             | 0V – 5V            |
| 5 | **FDBK** | Knob        | Feedback (repeats; min ↔ infinite, left ↔ right)       | --                 |
| 6 | *MIX CV* | CV Input    | CV for Dry/Wet Mix; summed with knob position          | 0V – 5V            |
| 7 | **MIX**  | Knob        | Dry/Wet Mix (dry ↔ wet, left ↔ right)                  | 10Vpp (output only)|
| 8 | **OUT**  | Jack        | Audio Output (10Vpp)                                   | 10Vpp              |

---

## Quick-Start

- **Patch audio input** to `IN`  
- **Patch output** from `OUT`  
- Use **TIME** knob (and/or *TIME CV*) to set delay length  
- Use **FDBK** knob (and/or *FDBK CV*) to set number/decay of repeats (fully right = infinite)  
- Use **MIX** knob (and/or *MIX CV*) to blend dry and wet (left = dry, right = wet)  
- All CVs: 0V (min) to +5V (max); summed with corresponding knob

---

## Installation (Summary)
- 2 HP width, 47mm depth (skiff-friendly)
- Power: +12V: 72mA, -12V: 28mA
- Red stripe on ribbon cable = -12V (typically bottom)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)