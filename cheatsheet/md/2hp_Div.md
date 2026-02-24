# 2hp — Div

- [Manual PDF](../../manuals/Div_Manual.pdf)

---

[**Div Module Manual PDF**](sandbox:/mnt/data/Div_Manual.pdf)

---

# 2hp Div Eurorack Module Cheat Sheet

## **Module Overview**
- **2-channel** voltage-controlled clock divider/multiplier
- Multiplies or divides incoming clock by: **1, 2, 3, 4, 5, 6, 7, 8, 16**
- **Individual controls & CV** for each channel
- **Dynamic rhythms** from a single clock input
- **2 HP width** (skiff friendly)

---

## **Front Panel Controls**

| # | Label      | Type | Description | Voltage Range |
|---|------------|------|-------------|--------------|
| 1 | **IN**     | Jack | Clock input (shared for both channels) | Threshold: +2.5V |
| 2 | **RATE 1** | Knob | Division/multiplication selector for CH1:<br>`/16 ... /1 ... x16` | - |
| 3 | **RATE 1 CV** | Jack | CV control of CH1 rate | 0V–5V |
| 4 | **LED 1**  | LED  | Lit when OUT1 emits a pulse | - |
| 5 | **OUT 1**  | Jack | Output clock CH1 | 0V–5V |
| 6 | **RATE 2** | Knob | Division/multiplication selector for CH2:<br>`/16 ... /1 ... x16` | - |
| 7 | **RATE 2 CV** | Jack | CV control of CH2 rate | 0V–5V |
| 8 | **LED 2**  | LED  | Lit when OUT2 emits a pulse | - |
| 9 | **OUT 2**  | Jack | Output clock CH2 | 0V–5V |

### **Division / Multiplication Settings**
- **Knob Left:** `/16` (slowest)
- **Knob Center:** `/1` (original clock)
- **Knob Right:** `x16` (fastest)
- **Intermediate positions:** `/8, /7, /6, /5, /4, /3, /2, x2, x3, x4, x5, x6, x7, x8`

---

## **How To Use**

1. **Patch a clock** signal to **IN** (min level +2.5V).
2. Adjust **RATE 1** and **RATE 2** knobs to select division/multiplier for each channel.
3. Optionally, patch **CVs (0-5V)** to **RATE 1 CV** and/or **RATE 2 CV** for external modulation.
4. Take divided/multiplied clocks from **OUT 1** and **OUT 2**.
5. LEDs indicate when each output pulses.

---

## **Power Specifications**
- **+12V:** 30mA
- **-12V:** 3mA
- **Depth:** 46mm

---

For more advanced utility and dynamic clock manipulation, use with sequencers, logic modules, or modulation sources.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)