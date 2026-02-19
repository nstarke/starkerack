# Bastl Instruments — ABC Mixer

- [Manual PDF](../../manuals/manual-abc-web.pdf)

---

[Download the Bastl Instruments ABC Mixer Manual (PDF)](https://bastl-instruments.com/content/manuals/ABC_manual.pdf)

---

# Bastl Instruments ABC Mixer Cheat Sheet

### Overview
- **ABC** is a compact 6-channel mixer for eurorack, primarily designed for audio mixing, but modifiable for mixing CV.
- It can function as two independent 3-channel mixers or as a single 6-channel mixer, depending on jack usage.

---

## Inputs & Outputs Reference

| Label      | Type        | Function                                                             | Voltage Range         |
|------------|-------------|-----------------------------------------------------------------------|-----------------------|
| **A–F**    | Input       | Six AC-coupled audio inputs (can be modded for DC, see below)        | Audio: ±5V typical    |
| **A+B+C**  | Output      | Mix of inputs A, B, C (if used, output is isolated from D+E+F)       | Audio out             |
| **D+E+F**  | Output      | Mix of inputs D, E, F, **PLUS** A+B+C if the A+B+C out is unused     | Audio out             |

---

## Front Panel Controls

| Control         | Type   | Function                    | Range   |
|-----------------|--------|-----------------------------|---------|
| 6x Gain Knobs   | Knob   | Individual input level A–F  | 0–1     |

*No buttons, sliders, or toggles on front panel.*

---

## Key Usage Tips

- **Dual Mixer Mode:** Use both A+B+C and D+E+F outputs for two separate 3-channel audio mixes.
- **Single Mixer Mode:** Leave A+B+C output *unplugged*; all six inputs mix at D+E+F output.
- **Maximum Gain:** Each channel's gain knob goes from 0 (off) to 1 (unity gain).
- **Stereo Use:** Use normalization jumpers on rear for quick stereo sets—A to D, B to E, C to F.

---

## Customization (Back Panel)

- **Solder Jumpers (6 jumpers):** Configure to bypass input capacitors, changing from AC to DC coupling. This enables CV mixing (mixes DC voltages).
- **Normalization Jumpers (3 jumpers):** A→D, B→E, C→F for stereo/linked setups.

---

## Technical Specs

- **Width:** 5 HP
- **Depth:** 35 mm (skiff friendly)
- **Power:** +12V (<10mA), -12V (~10mA)
- **Protection:** PTC fuse and diode
- **Coupling:** AC (unless modified for DC/CV)

---

## Installation Notes

- **Double check ribbon cable polarity!**
- **Red stripe = -12V rail**
- Only connect/disconnect power with your case powered off.

---

## Links

[Download the Bastl Instruments ABC Mixer Manual (PDF)](https://bastl-instruments.com/content/manuals/ABC_manual.pdf)

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
