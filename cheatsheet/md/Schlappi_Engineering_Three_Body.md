# Schlappi Engineering — Three Body

- [Manual PDF](../../manuals/three_body_manual_01302023a.pdf)

---

[**Download the Three Body Manual (PDF)**](https://www.schlappiengineering.com/downloads/schlappi_three_body_manual.pdf)  
*Below is a condensed "cheat sheet" reference for the Schlappi Engineering Three Body oscillator module, including jack/knob/voltage details and an operator's quick-start guide.*

---

# Three Body Cheat Sheet

## Overview
- **Triple digital oscillator** for phase and FM synthesis.
- Flexible normalization between oscillators for complex stereo, drone, and FM patches.
- Switchable mode/state per oscillator for FREE (classic VCO/LFO) or RATIO (FM/phase/carrier).

---

## Jack Reference

| Jack                | Type    | Voltage Range    | Function                       | Notes                                     |
|---------------------|---------|------------------|--------------------------------|-------------------------------------------|
| **V/OCT (per osc)** | In      | -8V to +8V       | Linear pitch, best tracking -5V to +5V | Tracks 1V/oct (+RATIO in ratio mode)      |
| **FM**              | In      | -8V to +8V       | Frequency modulation (Expo/Lin)| Will clip above 16Vpp (bipolar), 8V (uni) |
| **PHASE**           | In      | -8V to +8V       | Phase modulation               | Always active, state independent          |
| **FM/PHASE INDEX**  | In      | 0V to +10V       | Index VCA CV (mod amount)      | Unipolar, will clip below 0V/above 10V    |
| **SYNC**            | In      | ~0.7V threshold  | Hard sync or ratio tracking    | Rising edge triggers sync/tracking        |
| **TRANSPOSE**       | In      | -8V to +8V       | Global pitch offset            | No effect in ratio mode                   |
| **SINE**            | Out     | -5V to +5V       | Sine wave                      | Always available                          |
| **COSINE**          | Out     | -5V to +5V       | Cosine wave (center osc only)  | 90° ahead of sine (nominal, not under PM) |
| **TRIANGLE**        | Out     | -5V to +5V       | Triangle wave                  |                                           |
| **SAW**             | Out     | -5V to +5V       | Saw wave                       |                                           |
| **COSAW**           | Out     | -5V to +5V       | Cosine saw (center osc only)   | 90° ahead of saw                          |
| **SQUARE**          | Out     | -5V to +5V       | Square wave                    |                                           |

_All outputs are bipolar, DC-coupled, ~10V peak-to-peak._
  
---

## Control Summary

### Knobs (per oscillator unless noted)
- **COARSE/MULT** – Coarse pitch / Ratio Multiplier
- **FINE/DIV** – Fine pitch / Ratio Divider
- **FM INDEX** – FM depth (outer oscillators)
- **PHASE CV** – Phase modulation depth (outer oscillators)
- **PHASE INDEX 1/2** – Phase mod index depth (center oscillator, two separate inputs)
- **FM CV** – FM modulation depth (center oscillator)

### Jacks (per oscillator)
- See Jack Reference above

### Switches (per oscillator)
- **FREE** / **RATIO**
  - _FREE_: Classic VCO/LFO mode (expo/linear FM & standard pitch)
  - _RATIO_: Tracks center or external via ratio (FM/phase in ratio domain)
- **LIN** / **EXP** / **PH (PHASE)**
  - FM/Phase mode: Linear, Exponential, or Phase
- **HIGH/MULT** / **LOW/DIV**
  - Range or multiply/divide for ratio/carrier frequency
- (Center has additional phase index controls)

### Mode Summary
| Mode        | Description                                                            |
|-------------|------------------------------------------------------------------------|
| Free Expo   | LFO/VCO with exponential FM                                            |
| Free Lin    | LFO/VCO with linear FM                                                 |
| Ratio Phase | Tracking (FM/PM) with phase mod and CV over mult/div                   |
| Ratio Lin   | Tracking with linear FM and CV over mult/div                           |

### Indicators/LEDs
- Three large LEDs: Show sine output (blue=pos, red=neg, purple=audio rate)
- Four small LEDs: Show index VCA modulation activity

---

## Voltage Ranges (Summary)

- **V/OCT, PHASE, FM inputs:** -8V to +8V accepted; best tracking -5V to +5V
- **INDEX / PHASE INDEX inputs:** 0V to +10V unipolar (envelopes, will clip below/above)
- **SYNC in:** ~0.7V rising edge triggers sync/tracking
- **Outputs:** -5V to +5V typical, up to ~12Vpp on some systems

---

## Basic Patching Tips

- **Default Stereo FM:** Use center oscillator as modulator, outer oscillators as ratios/carriers.
- **Phase Modulation:** Center oscillator can receive phase mod from both outer oscillators, patched or normalized.
- **Cross Modulation:** Patch outer phase or FM ins to opposite outs for wild textures.
- **Ratio Tracking:** Outer oscillators in RATIO track to center osc, creating classic DX-style FM when modulating index/depth.
- **SYNC:** Feed external clock/signal to SYNC for hard sync (FREE) or ratio tracking (RATIO).

---

## Internal Normalization

| Input                        | Normalized From                |
|------------------------------|-------------------------------|
| Center PHASE (1/2)           | Outer oscillators' SINE outs  |
| Outer FM (L/R)               | Center SINE / COSINE out      |
| Outer PHASE (L<->R)          | Opposite SINE out             |
| Outer RATIO SYNC             | Tracks center if nothing patched|

---

## Power Draw

- **+12V:** 95mA
- **-12V:** 50mA
- **Inrush:** 200mA on +12V at power up

---

## Back Panel Header Functions

| Name        | Function                                                        |
|-------------|-----------------------------------------------------------------|
| Expander    | Unused (future)                                                 |
| PLL Mode    | On = Phase lock for external tracking (useful for LFO/oscilloscope) |
| Ext. Filter | Switches noise filtering for OSC1,3 PHASE & OSC2 FM (Low/High)  |
| Sq. Phase   | Remove phase mod from square out for pure/sub recovery          |
| Phase Dir   | Same direction for all outs (preserves phase relationship)      |

---

## Calibration

- All units pre-calibrated; calibrate only if necessary (unlikely).
- Use back-panel buttons, 0V and 4V source, follow manual.

---

## Quick Reference -- Basic Patch Ideas

- **Unmodulated Ratio FM:** Center FREE/HIGH, right RATIO, mult/div to tune harmonics.
- **Classic PM:** Center SINE/COSINE outs, phase index up, cross modulate outers for rich stereo.
- **Dub Bass:** Seq clock into left SYNC in ratio mode, mod input to left RATIO, monitor center out.
- **Rhythmic Creaks:** Center FREE, LOW; outer RATIO or FREE, lots of phase index and cross mod.

---

## More Info

- [Schlappi Engineering - Three Body Page](https://www.schlappiengineering.com/three-body)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
