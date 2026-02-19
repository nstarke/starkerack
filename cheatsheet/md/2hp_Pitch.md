# 2hp — Pitch

- [Manual PDF](../../manuals/2hp_Pitch.pdf)

---

[2hp Pitch Manual PDF](https://twohp.com/manuals/pitch.pdf)

---

# 2hp Pitch – Cheat Sheet

## Overview
**2hp Pitch** is a compact Time Domain Pitch Shifter module for Eurorack with built-in Wow & Flutter modulation. It allows shifting of pitch (±2 octaves), modulation of pitch "instability," and wet/dry mixing. Ideal for creative audio processing, lo-fi effects, and harmonization.

---

## Inputs, Outputs & Parameter Summary

| Name                | Type      | Voltage Range  | Description                                                         |
|---------------------|-----------|---------------|---------------------------------------------------------------------|
| **Audio Input**     | IN        | 10Vpp         | Main audio signal input (patch audio here to be pitch shifted).      |
| **Audio Output**    | OUT       | -             | Main processed audio signal output.                                  |
| **W&F CV Input**    | CV IN     | +5V           | Voltage control for Wow & Flutter depth (modulates instability).     |
| **Mix CV Input**    | CV IN     | +5V           | Voltage control for dry/wet blend.                                   |
| **1V/OCT Input**    | CV IN     | +5V           | Standard 1V/oct pitch input; extends pitch shift control externally. |

---

## Knob / Control Summary

| Name           | Position         | Function                                                                            |
|----------------|-----------------|-------------------------------------------------------------------------------------|
| **W&F Knob**   | Fully CCW → CW  | Controls wow & flutter random modulation depth. CCW = none, CW = maximum.           |
| **Mix Knob**   | Fully CCW → CW  | Mixes between dry (CCW) and wet (CW) signal. Any blend allowed in-between.          |
| **Pitch Knob** | CCW, Noon, CW   | Shifts pitch -2 octaves (CCW) to +2 octaves (CW). Noon = no transposition.          |

---

## Performance Tips

- **Combine VCO**: Create harmonies from a single oscillator by pitch shifting and mixing both.
- **Layer with Loop**: Add tape-style warble to loopers or harmonize sampled material.
- **Use with Play**: Send in drum loops/samples, pitch shift for unexpected timbral changes.
- **Lo-fi Combo with Freez**: Combine Freez and Pitch for ultra-lo-fi, modulate both for unique artifacts.

---

## Voltage Reference

- **W&F CV Input:** 0–+5V
- **Mix CV Input:** 0–+5V
- **1V/Oct Input:** 0–+5V (tracks one octave further than the knob range in either direction)
- **Audio Input:** ±5V (10Vpp typical Eurorack synth audio levels)

---

## Installation Notes

- Align red stripe of power cable with white marker on PCB.
- Module width: 2HP. Depth: 45mm.
- Power: +12V 78mA, -12V 9mA

---

## What is Wow & Flutter?

- **Wow & Flutter** is a modulation effect simulating pitch instability due to tape/turntable irregularities, lending warmth or 'lo-fi' character.

---

**More info:** [twohp.com/modules/pitch](https://twohp.com/modules/pitch)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)