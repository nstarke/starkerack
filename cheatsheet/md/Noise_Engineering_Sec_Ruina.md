# Noise Engineering — Sec Ruina

- [Manual PDF](../../manuals/Seca Ruina - Noise Engineering Documentation.pdf)

---

[Seca Ruina Manual PDF](https://manuals.noiseengineering.us/sr/)

---

# Seca Ruina Cheat Sheet

**Type:** Multiband distortion/VCA  
**Size:** 6HP Eurorack  
**Depth:** 0.8 inch  
**Power:** 2x5 Eurorack (+12V: 85mA, -12V: 80mA)  
**Voltage Range (CV Inputs):** 0V to 5V

---

## Quick Start

1. **Patch audio to `In`.**
2. **Patch `Sum (Σ) out`** to your mixer for combined distorted output.
3. **Adjust High, Mid, Low knobs** for per-band drive.
4. (Optional) **Patch envelopes/CV to band or ALL CV inputs** for dynamic control or VCA use.
5. **Use individual High/Mid/Low outs** to process bands separately.

---

## Interface Reference

### Inputs

| Jack      | Function                               | Voltage Range   |
|-----------|----------------------------------------|-----------------|
| In        | Audio input                            | Audio signal    |
| High In   | CV for High-band drive                 | 0V to 5V        |
| Mid In    | CV for Mid-band drive                  | 0V to 5V        |
| Low In    | CV for Low-band drive                  | 0V to 5V        |
| All In    | CV for simultaneous drive of all bands | 0V to 5V        |

---

### Outputs

| Jack        | Function                             |
|-------------|--------------------------------------|
| High out    | Processed high-frequency band        |
| Mid out     | Processed mid-frequency band         |
| Low out     | Processed low-frequency band         |
| Sum (Σ) out | Summed output (all 3 bands mixed)    |

---

### Controls

| Control          | Function                                           |
|------------------|----------------------------------------------------|
| High knob        | Sets drive for High frequency band (CV offset)      |
| Mid knob         | Sets drive for Mid frequency band (CV offset)       |
| Low knob         | Sets drive for Low frequency band (CV offset)       |

- **No buttons, sliders, or toggles on this module.**

---

## Patch Examples

- **Patch 1:** Simple waveform to In, Sum out to mixer, play with knobs.
- **Patch 2:** Complex sound (drums/melody) to In, adjust drives for creative distortion.
- **Patch 3:** Oscillator to In, envelope/LFO to All CV for multiband distortion with VCA control.

---

### Power Connection

- Align the ribbon cable so the red stripe is on the -12V side of both the module and power board.
- Double check proper orientation before powering on.

---

> **Warranty:** Manufacturer covers repair/replacement for defects; user damage charged at cost. Contact Noise Engineering for repairs.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)