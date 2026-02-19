# 4ms — Rotating Clock Divider

- [Manual PDF](../../manuals/RCD-manual-1.2.pdf)

---

[**Rotating Clock Divider Manual PDF**](https://4mscompany.com/p.php?p=151&c=24)

---

# 4ms Rotating Clock Divider (RCD) Cheat Sheet

**PCB v1.2, Firmware v1.1**  
**4HP, 60mA @ +12V/+15V**

---

## Overview

The RCD takes a master clock input and outputs 8 different clock divisions, rotatable by CV. Divisions, mode, and rotation are easily voltage- or jumper-controlled. Optionally, deep configuration is available at the back (jumpers).

---

## Front Panel Controls & Jacks

| Label     | Type    | Function                                      | Voltage Range         |
|-----------|---------|-----------------------------------------------|-----------------------|
| **Clock In**   | Input   | Main clock input, rising edge triggers           | 3.5V – 15V            |
| **CV Rotate**  | Input   | Rotates output divisions per jack               | 0V – +5V              |
| **CV Reset**   | Input   | Syncs/resets count on next rising clock         | 3.5V – 15V (Trig)     |
| **/1 ... /8**  | Output  | Divided clock outputs                         | GATE: 0V/High, 50%duty<br>TRIG: Follows clock pw |
| **LEDs**       | Visual  | Show clock activity/output states              | -                     |
| (No knobs, sliders, or toggles on the front panel) |

---

## Voltage-Controlled Inputs

- **Clock In** — 3.5V–15V, triggers on rising edge  
- **CV Rotate** — 0V to +5V; each ~0.67V step (max-div 8) advances all outs by 1 division  
- **CV Reset** — 3.5V–15V, pulse resets counters on next clock

---

## Outputs

- **8x Divider Outs** _(3.5mm jacks, labeled 1–8, see below for mapping)_
    - **Spread Off, Max Div 8**: 1, 2, ... 8 (_+ Rotate offset R_)
    - **Spread On**: /1, /2, /3, /4, /6, /8, /12, /16 (_rotates with CV_)
    - **GATE Mode**: 0V/High, 50% duty (divided waveform)
    - **TRIG Mode**: Short pulse equals input clock pulse width

---

## Back Panel Jumpers (Options, or use Breakout)

| Label      | Setting         | Action/Description          |
|------------|----------------|----------------------------|
| **Up/Down**| ON: Downbeat    | All outputs fire on 1st beat. <br>OFF: Upbeat (default)   |
| **Trig/Gate** | ON: Gate Mode  | 50/50% gate outs. <br>OFF: Trigger Mode (default)|
| **Max-Div-Range 16** | ON: Max /16 | Sets the highest division |
| **Max-Div-Range 32** | ON: Max /32 | Used with above for /32 or /64 |
| **Spread**   | ON: Spread     | Evenly spreads outputs in max range |
| **Auto-Reset**| ON: Enables (16/32/64/128) | Auto-resets at end of cycle |

- **Max-Div by**:  
  - Both 16 & 32 OFF: Max /64  
  - 16 ON, 32 OFF: Max /16  
  - 16 OFF, 32 ON: Max /32  
  - 16 ON, 32 ON: Max /8

---

## Reference: Output Jack Mapping (Default, Spread OFF, MaxDiv 8)

| CV Rotate Voltage  | <0.67V | 0.67–1.3V | 1.3–1.9V | 1.9–2.5V | ... up to >4.5V |
|--------------------|--------|-----------|----------|----------|-----------------|
| **/1**             | 1      | 2         | 3        | 4        | up to 8         |
| **/2**             | 2      | 3         | 4        | ...      | wraps to /1     |
| ...                | ...    | ...       | ...      | ...      | ...             |
| **/8**             | 8      | 1         | 2        | ...      | wraps to /7     |

---

## Special Modes & Details

- **Spread Mode ON**: Jacks follow intervals: /1, /2, /3, /4, /6, /8, /12, /16  
  _Good for musical/rhythmic divisions._
- **Auto Reset**: Automatically resets the divider count after n clocks (per jumper and Max Div).
- **Bus Clock Input**: Can clock from Eurorack bus (jumper); patched clock overrides bus.
- **5V/12V Power**: Selectable with rear jumper ("EXT"=5V; "INT"=12V, factory default).
- **LED Brightness**: Rear trim pot.

---

## Quickstart / Typical Patch

1. **Patch clock source** into Clock In (5V square or trigger).
2. **Patch Divider outputs** (1–8) to modules/drums/sequencers, etc.
3. **Apply CV to Rotate** input to shift all outputs together.
4. **Patch Reset** with a trigger or out from another divider to resync cycle.

---

## Advanced

- Rear jumpers set gate/trigger, up/down counting, auto-reset, Spread, Max-Div range, bus clock.
- Use the RCD Breakout for easy mode changes.

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)