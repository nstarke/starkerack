# Mutable Instruments — Ripples

- [Manual PDF](../../manuals/Manual - Mutable Instruments Documentation.pdf)

---

[**Ripples 2020 Manual PDF**](https://mutable-instruments.net/modules/ripples/manual.pdf)  
*(Note: Replace with the actual PDF link if available; Mutable Instruments usually hosts manuals here.)*

---

# Mutable Instruments Ripples 2020 — Cheat Sheet

## **OVERVIEW**
- **Type:** Eurorack analog multimode VCF (Voltage Controlled Filter)
- **Modes:** High-pass, Band-pass, Low-pass
- **Features:** Switchable 2-pole/4-pole for BP/LP, voltage-controlled resonance, soft-limiting, built-in VCA on LP out

---

## **FRONT PANEL CONTROLS**

**A. Cutoff Frequency (knob)**
- Range: 20 Hz → 20 kHz

**B. Filter Slope (toggle switch)**
- 2-pole (12dB/oct; down)
- 4-pole (24dB/oct; up)
- *Affects BP and LP outputs only*

**C. Resonance (knob)**
- Self-oscillation: ~75% and up

**D. Input 1 Level (knob)**
- Gain: 0 → 5 (soft clip = overdrive at high setting)

**E. FM Attenuverter (knob)**
- Adjusts amount & polarity of cutoff modulation via FM CV input

---

## **INPUTS & OUTPUTS SUMMARY**

| Jack          | Function                      | Voltage Range         | Notes                                          |
|:-------------:|:----------------------------:|:---------------------:|:-----------------------------------------------|
| In 1          | Audio input 1                | Modular level         | Soft-clipping circuit for overdrive            |
| In 2          | Audio input 2                | Modular level         | Clean input, vintage tone                      |
| FM (CV)       | Cutoff CV (FM) input         | ±5V typical           | Mod amount set by E; responds to attenuverter  |
| V/OCT         | 1V/oct cutoff tracking       | 0–5V (typical)        | Keyboard/sequencer pitch CV in                 |
| RES (CV)      | Resonance voltage control    | 0–5V                  | Exponential response                           |
| LP GAIN (CV)  | VCA for LP output            | 0V = mute;<br>5V = 1x   | >5V compresses; 7V normalized if unpatched     |
| **HP OUT**    | High-pass output             | Modular audio         | Slope varies w/ resonance                      |
| **BP OUT**    | Band-pass output             | Modular audio         | 2-/4-pole selectable                           |
| **LP OUT**    | Low-pass output              | Modular audio         | 2-/4-pole selectable, final output has VCA     |

---

## **USAGE TIPS**
- **Mix both audio inputs** for more complex filtering (Input 1 for overdrive, Input 2 for clean).
- **Select filter slope** with the B switch (only BP/LP).
- **Voltage-control resonance** via Res CV for animated textures & pinging.
- **Self-oscillation:** Use as a sine oscillator if resonance is up.
- **VCA on LP out:** Use LP Gain CV for dynamic level modulation or remove cable to use default 7V (fully open).
- **1V/Oct tracking:** Use V/OCT input if you want filter cutoff tracked by sequencer/keyboard (calibrate as needed).

---

## **CALIBRATION SUMMARY**
1. FREQ ~10 o'clock, RES max, no input or FM CV.
2. Connect keyboard/sequencer to V/OCT.
3. Listen to LP out, adjust on-board trimmer for proper octave tracking (~4 octaves).

---

## **Power Requirements**
- +12V: 35mA; -12V: 35mA  
- Connect bus cable with -12V (red stripe) matching markings.

---

### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)