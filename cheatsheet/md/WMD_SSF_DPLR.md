# WMD SSF — DPLR

- [Manual PDF](../../manuals/DPLRmanual1.3.pdf)

---

[Link to DPLR Manual (PDF)](https://wmdevices.com/products/ssf-dplr)

# DPLR Eurorack Dual/Stereo Delay Cheat Sheet

## Overview
DPLR is a dual/stereo delay module with voltage control, cross-channel feedback (XTALK), and variable low-pass filtering. It offers classic, ping-pong, and experimental delay effects.

---

## **Inputs and Outputs:**

| Jack        | Function                                         | Notes/Voltage Range          |
|-------------|--------------------------------------------------|------------------------------|
| **IN**      | Signal input to the delay                        | Audio level (typical modular)|
| **DLY CV**  | CV input for main DELAY time (A/B)               | 0–5V CV                      |
| **SPRD CV** | CV input for SPREAD (offset delay for B)         | 0–5V CV                      |
| **RGN CV**  | CV input for REGEN (feedback amount)             | 0–5V CV                      |
| **OUT A**   | Main delay output + mixed B XTALK                | Audio out                    |
| **OUT B**   | B delay out, affected by SPREAD/XTALK            | Audio out                    |

---

## **Controls:**

| Control   | Function                                                   |
|-----------|------------------------------------------------------------|
| **D / DELAY AMOUNT** | Sets delay time (40ms – 700ms, manual & CV)    |
| **R / REGEN AMOUNT** | Adjusts feedback for repeats, manual & CV      |
| **S / AMOUNT**       | Sets WET signal (0%–100%; 2x gain at max)      |
| **L1 / DELAY A**     | Delay time for A output (linked to DELAY knob) |
| **L2 / SPREAD (B)**  | Offsets B delay from A, ping-pong/dual delays  |
| **M / MODE SELECT XTALK / FILTER** | Tap to cycle XTALK (cross-feedback) modes, hold for filter slope levels |

---

## **Button/LED Functions:**

| Control      | Function                                                                                                   |
|--------------|------------------------------------------------------------------------------------------------------------|
| **XTALK LEVEL LED**     | Shows XTALK amount (RED: none, BLUE: max)                                                       |
| **FILTER SLOPE LED**    | Shows low pass filtering level (brighter = more filtering)                                     |
| **M / MODE Button**     | Short press: XTALK mode; Hold 1s: Filter slope mode                                            |

---

### **XTALK Modes:**
- **Cycles through 7 settings**: Cross-feedback from A ↔ B increases with higher settings.

### **FILTER Modes:**
- **Cycles through 4 filter slopes**: From minimal ("noisy") to heavy ("smooth, dark").

---

## **Basic Use:**
1. **Patch Input**: Send audio to **IN** jack.
2. **Set Delay**: Rotate **D/DELAY AMOUNT** knob to adjust time; patch CV for modulation.
3. **Spread for Stereo**: Use **L2/SPREAD** knob to offset B channel; CV input for animation.
4. **Adjust Feedback**: **R/REGEN** knob for repeats; patch CV for evolving textures.
5. **Wet/Dry Mix**: **S/AMOUNT** knob combines dry/wet; max = all wet (x2 gain).
6. **Experiment with Modes**: Tap **M** for XTALK; hold for filter.
7. **Output**: Use **OUT A** and/or **OUT B** for mono or stereo effects.

---

> **Tip:** Use XTALK and SPREAD to create dynamic ping-pong delays, stereo widening, or wild feedback networks!

---

## **Reference: Voltage Control**
- **All CV Inputs**: 0–5V for full range modulation.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
