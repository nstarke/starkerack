# Shakmat — Time Wizard

- [Manual PDF](../../manuals/TW-User_Manual.pdf)

---

[**Official Manual PDF**](https://www.shakmat.com/wp-content/uploads/2019/01/time_wizard_manual_v1.pdf)

---

# Shakmat Time Wizard – Cheat Sheet

## Overview
- **8 HP** digital clock divider and logic module for Eurorack
- **6 dividers** (A1-A3, B4-B6), each with activity LED and selectable division settings
- **4 three-way switches** for advanced signal routing, multiplicative/divider logic, and resets
- Enables creation of polyrhythms, odd time signature sequences, and complex clocking

---

## Inputs & Outputs Reference

| Label         | Type         | Description                                      | Voltage Range   |
|---------------|--------------|--------------------------------------------------|-----------------|
| CLK (1)       | Input        | Main clock input                                 | 0–5V trigger    |
| RST/IN B (2)  | Input        | Reset input (default) or independent clock for B | 0–5V trigger    |
| A1, A2, A3 (E-G) | Output    | Dividers 1–3 outputs (activity LED)              | 0–5V trigger    |
| B4, B5, B6 (H-J) | Output    | Dividers 4–6 outputs (activity LED)              | 0–5V trigger    |

**Outputs 5 & 6 can optionally output half-period gates** (jumper on back).

---

## Front Panel Controls

| Control           | Function                                                    |
|-------------------|------------------------------------------------------------|
| **A. Multiply A** | Multiplies clock to A1-A3 by ×3 or ×4 (upper = off)        |
| **B. Clock B**    | Selects clock source for B4-B6:<br>&bull; Upper: normal (same as main clock)<br>&bull; Mid: B4 clocks B5/B6 (chained)<br>&bull; Lower: RST/IN B (2) is independent clock for B4-B6 |
| **C. Logic A2**   | Adds logic to A2 output:<br>&bull; Upper: off<br>&bull; Mid: A2 AND B5<br>&bull; Lower: A2 OR A3                         |
| **D. Reset B6**   | B6 resets:<br>&bull; Upper: off<br>&bull; Mid: resets A1-A3<br>&bull; Lower: resets all dividers                         |

---

## Usage Guide

### Basic Operation
1. **Connect your clock (0–5V)** to **CLK IN [1]**.
2. Use **A1-A3** and **B4-B6** outputs for divided clock signals. Division ratios set by potentiometers.
3. Optionally connect **RST/IN B [2]** to externally reset all dividers.

### Advanced Modes (Switches)
- **Multiply A:** Multiplies main clock for A channel (A1-A3) by 3 or 4 for complex decompositions (e.g., triplets, odd divisions).
- **Clock B:** Lets you:
    - Chain divisions (B4→B5→B6)
    - Use a different clock for B4-B6 (independent rhythms/polyrhythms)
- **Logic A2:**
    - Create composite rhythms with A2 & B5 (half periods) or A2 | A3 (sequencing tricks)
- **Reset B6:**
    - Use B6 as a reset signal for A only or both sections for structured patterns.

### Back Panel Jumper
- Activates “half-period gates” (longer gates instead of triggers) for B5 & B6 outputs.

---

## Electrical Specs

| Power           | 20mA @ +12V, 0mA @ -12V, 0mA @ +5V |
|-----------------|------------------------------------|
| Signals         | Inputs & outputs: 0–5V trigger     |
| Depth           | 22 mm                              |

---

## Quick Reference Diagram

```
  /-------------------------------\
  | A1  A2  A3   B4  B5  B6       |
  | |   |   |    |   |   |        |
  | CLK IN       RST/IN B         |
  |                                 
  | [X] Multiply   [X] Clock B     |
  | [X] Logic A2   [X] Reset B6    |
  \-------------------------------/
```

---

## Useful Links

- [**Official Manual PDF**](https://www.shakmat.com/wp-content/uploads/2019/01/time_wizard_manual_v1.pdf)
- [**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)