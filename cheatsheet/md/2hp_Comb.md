# 2hp — Comb

- [Manual PDF](../../manuals/Comb_Manual.pdf)

---

[**Download the Comb 2HP Manual (PDF)**](#)  
*(Replace # with your actual manual link, since PDF was not provided in your upload)*

---

# Comb 2HP (Eurorack) — Quick Reference Cheat Sheet

A compact IIR peaking comb filter module with CV-controllable cutoff, resonance, and damp control. Features intense resonant feedback, phaser/thickening, or metallic/chaotic effects.

---

### Inputs, Outputs, and Controls

| Label           | Type    | Description                                                                | Voltage Range |
|:----------------|:--------|:---------------------------------------------------------------------------|:-------------|
| **IN**          | Input   | Audio input. Modular-level signal.                                         | 10 Vpp       |
| **FREQ CV**     | CV In   | Control voltage input for cutoff frequency. Adds to knob position.          | ±5V          |
| **FREQ**        | Knob    | Sets cutoff (inverse to delay). Right = higher, left = lower. At 500Hz, 2ms delay. | -            |
| **RES CV**      | CV In   | Control voltage for resonance. Adds to knob.                               | ±5V          |
| **RES**         | Knob    | Sets feedback amount (resonance/peaks intensity).                          | -            |
| **DAMP CV**     | CV In   | Control voltage for damp(en) (dampening filter in feedback loop). Adds to knob. | ±5V          |
| **DAMP**        | Knob    | Sets feedback path LPF cutoff. Left = max damp (dark); right = no damp (bright). | -            |
| **OUT**         | Output  | Audio output. Modular-level signal.                                        | 10 Vpp       |

---

### Basic Usage Guide

- **Connect your audio signal** to **IN**.
- **Set FREQ** to pick the comb spacing (related to the "tuned" delay time).
    - Higher = brighter, more closely spaced peaks; lower = darker, more spaced.
- **Increase RES** for sharper, more resonant peaks. High enough, can self-oscillate!
- **Adjust DAMP** to filter the feedback path.
    - Left: Heavy filtering, tames metallic overtones (darker).
    - Right: Open/bright resonances, more "ringy."
- **Patch CV to FREQ, RES, or DAMP** for animation. EG: modulate FREQ for moving phaser, RES for feedback sweeps, DAMP for timbral morphing.
- **Extreme RES settings**: white noise in produces string/pluck sounds; signals can get chaotic!

---

#### Voltage Ranges

- All CV inputs: ±5V (adds to knob value)
- Audio IO: 10 Vpp

---

### Sonic Tips

- **Subtle FREQ, low RES**: Gentle thickening, phaser/ensemble feel.
- **Extreme FREQ, max RES**: Self-oscillation, synthetic string/reed sounds.
- **DAMP to left**: Tames the brilliance, good for "lo-fi" or mellow repeats.
- **DAMP to right**: Brighter, metallic results, more feedback.

---

For detailed reference, consult the [full manual (PDF)](#).

---
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)