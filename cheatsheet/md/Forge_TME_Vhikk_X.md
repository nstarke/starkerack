# Forge TME — Vhikk X

- [Manual PDF](../../manuals/vhikk x.pdf)

---

```markdown
[Official VHIKK X Manual PDF](https://forge-tme.com/vhikk-x/)

# VHIKK X Eurorack Module Cheat Sheet

---

## **Quickstart Overview**

- **VHIKK X** is a multi-algorithm stereo sound source and processor for experimental synthesis.
- Offers 36 algorithms across 4 banks (firmware v003+), combining generation and FX (drones, textures, SFX).
- Designed as a stand-alone sound island with ergonomy and deep internal randomisation capabilities.
- Key controls: two central encoders, two buttons, fixed-function knobs, toggle switches, 11 patch points.
- Input/output is fully stereo with true stereo sound architecture.

---

## **Panel Controls & Interface Reference**

### **Knobs & Encoders**

- **Parameter Knobs:** WARP, SPAN, MIX, FEED, MORPH, FIELD, TIME, FORM — assign to physical & algorithmic parameters.
- **2 Central Encoders:**
  - **Parameter pairs:** BASIS/TIME or SEED/SCAN
  - **MODE button** toggles encoder focus between pairs
  - **Lower button**: 
    - In BASIS/TIME mode → volume (VOL) control ([left=Input, right=Output])
    - In SEED/SCAN mode → switch BANK (firmware v003+)
- **LEDs:** Above encoders & I/O indicate parameter values, bank, level, and clip state.

### **Toggle Switches**

- 2 switches select algorithm — each combo is an algorithm (9 per bank, 4 banks = 36 algos).

### **Buttons**

- **Top (MODE):** Change encoder targets (BASIS/TIME or SEED/SCAN)
- **Bottom:**
  - In BASIS/TIME mode: Engage VOL mode for encoder volume control
  - In SEED/SCAN mode: Bank select (firmware v003+)
- **Both together:** Randomise SEED & SCAN (firmware v003+)

---

## **Input/Output Jack Reference**

### **Audio**

- **Stereo Inputs (L, R)** (bottom left):
  - **Normalled**: Either input can be used for mono signals.
  - **Impedance:** 30kΩ
  - **Clipping:** 20Vpp
  - **Gain:** -∞ to +30dB
- **Stereo Outputs (L, R)** (bottom right):
  - **Normalled**: R output gives mono sum if only R patched.
  - **Impedance:** 1kΩ
  - **Max output:** 18Vpp, with output volume knob/global encoder control.
- **LED bars:** Signal level metering (white = left, red = right).

### **CV Inputs & VCA Routing (bottom center)**

| Label   | Controls           | Input Voltage | Jack Functionality                                 |
|---------|--------------------|--------------|----------------------------------------------------|
| VCA     | Internal stereo VCA| -10V to +10V | +5V = open; >+5V overdrives. Normalled to all CVs. |
| MORPH   | Morph param/route  | -10V to +10V | Normalled to BASIS, FIELD, TIME, FORM when patched.|
| BASIS   | Algorithm param    | -10V to +10V | V/Oct tracking (cal.), mapped to encoder/knob      |
| FIELD   | Algorithm param    | -10V to +10V | -                                                  |
| TIME    | Algorithm param    | -10V to +10V | -                                                  |
| FORM    | Algorithm param    | -10V to +10V | -                                                  |

- **All CV inputs**: 200kΩ impedance, 20Vpp max, 5V swing = full range, per-algorithm mapping.
- **Attenuverter**: Each CV jack (except VCA) is paired with an attenuverter for manual range scaling.

#### **CV Normalling Logic**
- If **VCA CV is patched only:** Normalled to all others.
- If **MORPH CV patched:** Overrides normal, routes to others.
- If none patched: Small offset normalled, lets attenuverters act as fine-tune.

#### **Missing CV**
- **SEED:** No CV, only manual/random control.

---

## **State Saving**

- **Parameters saved after ≈30s unchanged.**
- **SEED, SCAN**: Saved per-algorithm.
- **VOL**: Saved globally.
- **BASIS, TIME**: Saved globally or per-algo (hold MODE on boot for global, bottom button for per-algo).

### **Change Save Mode (fw v003+)**
- Hold top button 5s (both LOGOs blink) to enter mode
- Top = global, Bottom = per-algo, Both = save/exit

---

## **Calibration (fw v003+)**

- Hold **bottom button 5s**: BASIS cv calibration mode
- Follow LED/encoder prompts with 1V & 3V inputs to calibrate (see full manual for procedure)
- Hold **top button 5s** for reference saw wave output (system calibration)
- Hold **bottom button 5s** to reset calibration
- **Press both** to save and exit

---

## **Specs & Power**

- **24HP, 15mm deep**
- **Power Draw:** +12V 100mA / -12V 10mA
- **Audio:** 96kHz, 24-bit I/O, stereo
- **Reverse Polarity Protected**
- **USB-C (side):** Firmware updates only (USB Mass Storage); not for power.

---

## **Warranty / Contact**

- **2-year warranty** (manufacture defects; not misuse)
- Contact: [contact@forge-tme.com](mailto:contact@forge-tme.com)
- Distribution: Signal Sounds (Int'l), list of global retailers in manual.

---

**For detailed algorithm reference, calibration steps, and advanced info, visit the [official manual](https://forge-tme.com/vhikk-x/).**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
```
