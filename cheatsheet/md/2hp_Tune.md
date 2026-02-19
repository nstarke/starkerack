# 2hp — Tune

- [Manual PDF](../../manuals/Tune_Manual_2023.pdf)

---

[2hp Tune Manual PDF](https://twohp.com/manuals/tune.pdf)

---

# 2hp Tune Cheat Sheet

2hp Tune is a voltage quantizer that snaps incoming CV signals to musical scales with selectable root and bias.

---

## **Jacks**

| Jack            | Function                              | Voltage Range     |
|-----------------|---------------------------------------|------------------|
| **Input**       | CV signal to be quantized             | 0V to +5V        |
| **Bias CV In**  | CV to modulate BIAS knob              | 0V to +5V        |
| **Output**      | Quantized V/Oct CV output             | 0V to +5V        |

---

## **Knobs and Controls**

| Control       | Function                                                                                               |
|---------------|--------------------------------------------------------------------------------------------------------|
| **Scale Knob**| Selects which musical scale to quantize to (see LEDs for indication).                                  |
| **Bias Knob** | Adjusts the root note position within the scale (completely left = root, completely right = last note).|

---

## **LEDs**
- Indicate the selected scale:
  - **MAJ** = Major or Major Pentatonic
  - **MIN** = Minor or Minor Pentatonic
  - **HRM** = Harmonic Minor or Egyptian Minor
  - **WHL** = Whole Tone or Octatonic (0,2)
  - **DIM** = Diminished or Octatonic (0,1)
  - **All LEDs ON** = Chromatic

---

## **Scales and LED Indications**

| Scale                     | LED Indication        |
|---------------------------|----------------------|
| Chromatic                 | All LEDs             |
| Major                     | MAJ                  |
| Major Pentatonic          | MAJ,                 |
| Minor                     | MIN                  |
| Minor Pentatonic          | MIN,                 |
| Harmonic Minor            | HRM                  |
| Egyptian Minor            | HRM,                 |
| Whole Tone                | WHL                  |
| Octatonic (0, 2)          | WHL,                 |
| Diminished                | DIM                  |
| Octatonic (0, 1)          | DIM,                 |

---

## **Quick Usage Steps**

1. **Patch** CV source into **Input**.
2. **Patch** quantized output from **Output** to oscillator/VCA/etc.
3. Use **Scale Knob** to pick a scale (LEDs show which).
4. Use **Bias Knob** to select the scale's root note (full left = lowest, full right = scale rotated to highest note as root).
5. Optionally patch modulation into **Bias CV In** for voltage control over root note (0V–5V).

---

## **Other Info**

- **Module Width:** 2HP
- **Power Draw:** +12V 40mA / -12V 3mA
- **Depth:** 45mm

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
