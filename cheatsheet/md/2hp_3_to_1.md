# 2hp — 3 to 1

- [Manual PDF](../../manuals/3_To_1_Manual.pdf)

---

[**Download the 2hp 3:1 Manual (PDF)**](#)  
*(Replace with actual PDF link as needed; the manual pages are in your screenshots.)*

---

# 2hp 3:1 Cheat Sheet

### Overview
- **3:1** is a voltage-controlled gate switch.
- Routes one of three gate/trigger inputs to a single output, or sums multiple gates for **polyrhythms**.
- Has both **selective switching** and **gate summing** (mixing) modes.
- Voltage control over input selection enables creative rhythmic patching.

---

## Panel Reference

| # | Label    | Type          | Function                                                                          | Voltage Range     |
|---|----------|---------------|-----------------------------------------------------------------------------------|-------------------|
| 1 | **IN 1** | Input Jack    | Gate/Trigger Input Channel 1                                                       | Threshold 2.5V    |
| 2 | IN 1 LED | LED           | Indicates IN 1 is selected                                                         | —                 |
| 3 | **IN 2** | Input Jack    | Gate/Trigger Input Channel 2                                                       | Threshold 2.5V    |
| 4 | IN 2 LED | LED           | Indicates IN 2 is selected                                                         | —                 |
| 5 | **IN 3** | Input Jack    | Gate/Trigger Input Channel 3                                                       | Threshold 2.5V    |
| 6 | IN 3 LED | LED           | Indicates IN 3 is selected                                                         | —                 |
| 7 | **MODE** | Toggle Switch | Left: Output selected input; Right: Sum selected inputs (outputs 5ms triggers)     | —                 |
| 8 | **SEL CV**| Input Jack   | CV input for selection (adds to SEL knob)                                          | 0V–5V             |
| 9 | **SEL**  | Knob          | Manually select input (far left=IN 1, far right=IN 3/all if SUM)                   | —                 |
|10 | OUT LED  | LED           | Indicates activity at OUT                                                          | —                 |
|11 | **OUT**  | Output Jack   | Gate/Trigger Output of selected/summed inputs                                      | 0V–5V             |

---

## How To Use

### 1. **Basic Switching Mode**
- Set **MODE** toggle LEFT.
- Use **SEL** knob (and/or **SEL CV** jack) to choose which IN (1/2/3) is routed to **OUT**.
- Output mirrors currently selected **IN**.

### 2. **Gate Summing (Mixing/Polyrhythm) Mode**
- Set **MODE** toggle RIGHT.
- The more you turn **SEL** right, the more inputs are summed at **OUT**:
    - Full left: IN 1 only
    - Full right: IN 1 + IN 2 + IN 3
- **OUT** outputs 5ms triggers whenever active gate(s) are summed (pulse width = 5 ms).

### 3. **CV Control**
- Patch a CV/gate/step sequencer into **SEL CV** for dynamic input switching or summed patterns.
- **SEL CV** range: 0V–5V (adds to manual **SEL** knob position).

---

## Voltage Ranges

- **Inputs (IN 1–3):** Accept gates/triggers, threshold at 2.5V.
- **Output (OUT):** 0V (low) or 5V (high/trigger).
- **CV Input (SEL CV):** 0V–5V; controls selection (summed with **SEL** knob).

---

## Installation

- **Format:** 2HP Eurorack
- **Depth:** 47mm (skiff friendly)
- **Power:** +12V: 32mA; -12V: 3mA
- **Connect power with red stripe facing the front.**

---

## Quick Tips

- **Sequenced switching:** Drive SEL CV with a stepped sequence for evolving patterns.
- **Layered triggers:** In SUM mode, send drums/clock/gates to all three inputs for complex polyrhythms.
- **Fast rhythm combos:** Use SUM mode to combine different clocks into one bursty output.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)