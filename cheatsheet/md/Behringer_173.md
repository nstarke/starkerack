# Behringer — 173

- [Manual PDF](../../manuals/QSG_BE_0720-AAL_173 QUAD GATE-MULTIPLES_WW.pdf)

---

[Behringer SYSTEM 100 Series 173 QUAD GATE/MULTIPLES Manual (PDF)](https://mediadl.musictribe.com/media/PLM/data/docs/P0E5L/173_QUAD_GATEMULTIPLES_QSG_WW.pdf)

---

# Behringer 173 QUAD GATE/MULTIPLES Quick Reference Cheatsheet

---

## Overview

The **Behringer 173 QUAD GATE/MULTIPLES** is a utility Eurorack module combining four gate process channels and six sets of passive 4-way multiples. It’s a simple, but powerful, way to route and manage gate/trigger signals and distribute audio/CV across your modular.

---

## Front Panel Controls & Connections

**No Knobs, Buttons, Sliders, or Toggles — This module is patch-programmable only.**
  
---

### 1. **GATE Section (top 4 rows)**
Four individual gate processors, labeled CH1–CH4.

- **GATE IN** (3.5mm jack, left of each section)  
  - **Type**: Input (accepts gate or trigger)  
  - **Input Impedance**: 160kΩ, unbalanced  
  - **Voltage Range**: Up to +17 dBu (~12V p-p, handle at least ±10V typical modular signals)
- **GATE CV** (3.5mm jack, middle of each section)  
  - **Type**: Control Voltage input  
  - **Impedance**: >50kΩ, unbalanced  
  - **Non-Inverting (active high):** gate opens with CV > +3V  
  - **Inverting (active low):** gate opens with CV < +1.5V  
  - **Voltage Range**: Up to 10V p-p
- **GATE OUT** (3.5mm jack, right of each section)  
  - **Type**: Output (passes gate if input and CV are high/truthy)  
  - **Output Impedance**: 1kΩ, unbalanced  
  - **Voltage Range**: Up to +17 dBu  
  - **Frequency Response**: DC to 20 kHz  
  - **Output Noise**: < -90 dBu

---

### 2. **MULTIPLES Section (bottom 6 rows)**
Six sets of four interconnected jacks per row (A, B, C, D).

- **MULTIPLES A/B/C/D** (total 24x 3.5mm jacks)  
  - **Type:** Passive parallel connections  
  - **How to use:**  
    - Patch an input into A, and the signal appears at B, C, D  
    - You can also patch into B, C, or D — they are all parallel  
  - **Signal Types:** Passes both audio and CV without clipping  
  - **Unbuffered (Passive):** No active circuitry  
  - **No voltage drop unless you split to many loads**  

---

## Voltage and Patch Notes

- **Works with logic, gates, triggers, audio, and CV signals.**
- **Voltage thresholds:**  
  - **CV Gate:** > +3V triggers gate (non-inverting), < +1.5V triggers (inverting)
  - **Max Input/Output:** ~±10V (stated as +17 dBu)
- **Power draw:** 40mA (+12V), 40mA (-12V)

---

## Typical Usage Patterns

- **Gate Channel:**
  1. Patch a gate or trigger signal to **GATE IN**
  2. Patch a control voltage to **GATE CV** to enable/disable passing the gate
  3. Use **GATE OUT** to route the conditioned gate to other modules

- **Multiples:**
  - Patch any signal (CV or audio) into 'A' (or any jack in the row), and break out to up to 3 other places

---

## Reference Summary (All Jacks)

| Label        | Type           | Function                                                | Voltage Range      |
|--------------|----------------|--------------------------------------------------------|--------------------|
| GATE IN      | Input          | Gate/trigger input                                     | ±10V typical       |
| GATE OUT     | Output         | Gate/logic output                                      | ±10V typical       |
| GATE CV      | Input          | Control of gate pass-through (internal logic)           | 0–10V (thresholds: +3V or +1.5V) |
| MULTIPLES A-D| Input/Output   | Passive mults for CV and audio (any jack is input/output)| Modular levels (±10V) |

---

### No knobs, buttons, switches or sliders.

---

For specifics, refer to the [official manual PDF](https://mediadl.musictribe.com/media/PLM/data/docs/P0E5L/173_QUAD_GATEMULTIPLES_QSG_WW.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)