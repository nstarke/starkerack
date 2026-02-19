# 2hp — EG

- [Manual PDF](../../manuals/EG_Manual-7ja4.pdf)

---

[EG Envelope Generator Manual PDF (Images above)](#)

---

# EG 2hp Envelope Generator — Cheat Sheet

## Overview

- **Type:** 2-stage envelope generator (Attack/Decay)
- **Envelope shapes:** Switchable linear/exponential
- **CV control:** Attack/Decay
- **Output:** 0–10V envelope
- **Built-in attenuator (AMP)**
- **Super compact (2hp), 3ms–11min per stage**

---

## Panel Control Reference

| Function             | Type                  | Description                                                                 | Voltage Range               |
|----------------------|-----------------------|-----------------------------------------------------------------------------|-----------------------------|
| **TRIG**             | Input jack            | Trigger or gate to fire envelope                                            | Threshold: 2.5V             |
| **ATTACK CV**        | Input jack            | CV input for Attack time                                                    | 0V – 5V                     |
| **ATTACK**           | Knob                  | Manual control for Attack time (min left, max right)                        |                             |
| **DECAY CV**         | Input jack            | CV input for Decay time                                                     | 0V – 5V                     |
| **DECAY**            | Knob                  | Manual control for Decay time (min left, max right)                         |                             |
| **RESPONSE TOGGLE**  | Switch (2-way)        | Select envelope shape: Up = Linear, Down = Exponential                      |                             |
| **AMP**              | Knob                  | Output envelope level; attenuates from 0V (left) to 10V (right)             | Output: 0V – 10V            |
| **ENVELOPE LED**     | LED                   | Visualizes output envelope                                                  |                             |
| **OUT**              | Output jack           | Final envelope output (attack & decay controlled by above)                  | 0V – 10V                    |

---

## Basic Operation

1. **Patch TRIG input** to receive gates/triggers (>2.5V) from sequencer, keyboard, clock, etc.
2. **Set ATTACK and DECAY** with knobs—their full range is 3ms to 11 minutes (per stage!).
3. **Add CV to ATTACK/DECAY CV inputs** for voltage control (0V–5V typical).
4. **Toggle RESPONSE** for desired shape:  
   - **Up = Linear**
   - **Down = Exponential**
5. **Set AMP** for attenuation (0V to 10V envelope output).
6. **Patch OUT** to next destination, like VCA, filter, or other modulation destination.

---

## Technical Specs

- **Width:** 2hp
- **Depth:** 45mm
- **Power:** +12V: 26mA, -12V: 7mA

---

**Quick Reference (Jacks & Controls)**
```
IN:  
 - TRIG (2.5V threshold)  
 - ATTACK CV (0–5V)  
 - DECAY CV (0–5V)  
OUT:
 - OUT (0–10V envelope)

Controls:
 - ATTACK (range: 3ms–11min)
 - DECAY (range: 3ms–11min)
 - RESPONSE TOGGLE (linear/expo)
 - AMP (attenuator for OUT, 0–10V)
 - ENVELOPE LED (visual feedback)
```

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)