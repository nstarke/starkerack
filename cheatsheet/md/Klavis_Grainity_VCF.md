# Klavis — Grainity VCF

- [Manual PDF](../../manuals/Klavis_-_Grainity_User_Manual.pdf)

---

[Download the Klavis Grainity User Manual PDF](https://www.klavis.com/manuals/Grainity_UserManual_A.pdf)  
*(Official source, verify up-to-date version at Klavis.com)*

---

# Klavis Grainity Granular VCF — Cheat Sheet

## Overview
- **Dual VCF**: Analog, digitally-controlled **Granular VCF** + standard **Multimode VCF**; patch separately or combine.
- **Mix Output** provides blend of both filter sections, voltage-controllable with phase-invert.
- **Shared controls** for frequency (cutoff) and resonance (Q).
- **Granular section**: Pattern/"Structure" control, cycle Division, Phase/Track, Detect input for driving filter cycle by triggers or external oscillators.
- **Firmware updates** via audio file to Struct jack.

---

## Front Panel Controls

| Ctrl Name         | Type       | Description                                                                           |
|-------------------|------------|---------------------------------------------------------------------------------------|
| **F (Freq)**      | Slider     | Master cutoff freq for both filters                                                   |
| **Q**             | Slider     | Master resonance for both filters (self-oscillates)                                   |
| **FM**            | Knob       | Bipolar attenuator for FM CV, center = 0, R = +, L = -                                |
| **FM (jack)**     | Input      | Cutoff CV, ±5V                                                                        |
| **V/Oct (jack)**  | Input      | 1V/oct tracking input, ±5V                                                            |
| **Q (jack)**      | Input      | CV for resonance, 0–+5V                                                               |
| **Q (knob)**      | Knob       | Unipolar attenuator for Q jack                                                        |
| **Mix (knob)**    | Knob       | Blend multimode (left) ↔ granular (right) for Mix output; also CV-able                |
| **Mix (jack)**    | Input      | Mix amount CV; summed ±5V with knob                                                   |
| **Type**          | Button     | Tap: select Multimode filter type (see below); Long press: toggle phase invert        |
| **Type LEDs**     | LED        | Shows active filter type; flashes if phase invert is active                           |
| **inv**           | Button     | Long press: toggles Mix phase inversion                                               |

### Granular Section Only

| Ctrl Name         | Type       | Description                                                                           |
|-------------------|------------|---------------------------------------------------------------------------------------|
| **Struct (encoder)**| Knob/Button| Select structure (pattern); hold+turn = fast scroll                                   |
| **Struct (jack)** | Input      | ±5V summed to Structure for voltage/random sweeping                                   |
| **Div (knob)**    | Knob       | Adjust cycle Division, increases step length in Structure                             |
| **Div (jack)**    | Input      | ±5V summed to Div knob                                                                |
| **Φ/Frq (knob)**  | Knob       | Phase delay (Track OFF), or Transpose amount (Track ON)                               |
| **Φ/Frq (jack)**  | Input      | ±5V Phase or Track amount CV                                                          |
| **Track (button)**| Button     | Track ON: Φ/Frq = Transpose (musically quantized); OFF = Φ/Frq = Phase                |
| **Track LED**     | LED        | Lit = Track mode ON                                                                   |
| **Detect (jack)** | Input      | Triggers/Audio to clock granular section (replaces auto-zero-crossing)                |
| **Display (3-digit)**| Numeric   | 1st+2nd: Structure, 3rd: Division                                                    |

### Outputs

| Ctrl Name         | Type       | Description                                                                           |
|-------------------|------------|---------------------------------------------------------------------------------------|
| **M.VCF (jack)**  | Output     | Multimode VCF output                                                                 |
| **G.VCF (jack)**  | Output     | Granular VCF output                                                                  |
| **Mix (jack)**    | Output     | Blend of M.VCF & G.VCF (set by Mix knob/CV, phase invert possible)                   |

---

## Multimode Filter Types (M.VCF)

| Filter | LED    | Description                 |
|--------|--------|----------------------------|
| LP2    | 1      | 12dB/oct low pass          |
| LP4    | 2      | 24dB/oct low pass          |
| HP     | 3      | 24dB/oct high pass         |
| BP     | 4      | 12dB/oct bandpass          |
| BR     | 5      | 12dB/oct band reject       |
| IN     | 6      | Input only (bypass)        |

---

## Voltage Ranges & Signal Levels

| Jack           | Range              | Notes                                       |
|----------------|--------------------|---------------------------------------------|
| Audio Input    | ±5V pp             | DC coupled                                  |
| Detect Input   | ≥300mV, AC coupled | Audio or trigger/gate input                 |
| CV Inputs      | ±5V                | All CVs (Struct, Div, Φ/Frq, Mix)           |
| Q Input        | 0 to +5V           | For resonance                               |
| Outputs        | ±5V pp             | Unity gain, open filter, no resonance        |

---

## Usage Tips
- **Input audio**: Use simple/complex VCO, chords, additive, sync, or even drums/mixed music.
- **Detect input**: Feed separate VCO, LFO, trigger, or rhythm to clock granular structure for special effects (e.g. quantized filtering/chops).
- **Structure**: Cycles through filter-phase patterns (2–8 step/user random); longer for more subharmonics.
- **Division**: Repeat each pattern step; for harmonics/rhythms, or slows down cycles.
- **Phase/Track**: Phase = flanging/chorus effects. Track = musical detuning/harmonic ratios.
- **Firmware Update**: Audio file to Struct jack, hold Track+Type while powering.

---

## Quick-Start Patch Recipe

1. Patch VCO to **Input**, output to system from **Mix** out.
2. Use **Type** to select multimode filter flavor.
3. Try **Structure/Div/Track/Φ** for subharmonics, harmonics or rhythm.
4. Use **Detect** with VCO/gate for rhythmic or externally driven patterns.
5. Fade/blend between granular/"classic" filter with **Mix** knob or CV.

---

## Reference Table: Jacks & Controls

| Name         | Type   | Function / Range for CV/Audio                               |
|--------------|--------|-------------------------------------------------------------|
| **Input**    | In     | Main audio, ±5V pp                                          |
| **Detect**   | In     | Audio or trigs, >300mV AC                                   |
| **V/Oct**    | In     | 1V/octave, ±5V                                              |
| **FM**       | In     | Frequency mod, ±5V                                          |
| **Q**        | In     | Resonance mod, 0–+5V                                        |
| **Struct**   | In     | Structure selection, ±5V                                    |
| **Div**      | In     | Division selection, ±5V                                     |
| **Mix**      | In     | Mix balance CV, ±5V                                         |
| **Φ/Frq**    | In     | Phase/track CV, ±5V                                         |
| **M.VCF**    | Out    | Multimode out, ±5V pp                                       |
| **G.VCF**    | Out    | Granular out, ±5V pp                                        |
| **Mix**      | Out    | Both sections mixed/blend, ±5V pp                           |

---  

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)