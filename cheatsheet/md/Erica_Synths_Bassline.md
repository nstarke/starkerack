# Erica Synths — Bassline

- [Manual PDF](../../manuals/BASSLINE_web.pdf)

---

[Erica Synths Bassline Module Manual (PDF)](https://www.ericasynths.lv/en/shop/instruments-47/drum-modules-795/bassline/)

---

# Erica Synths Bassline — Quick Reference Cheat Sheet

## What Is It?
The Erica Synths Bassline is a full analog synth voice in a Eurorack module, best for acid basslines and fat synth parts. It includes a VCO, transistor-based suboscillator, VCF, and envelopes.

---

## Front Panel Controls

**Knobs:**

| Knob        | Function                                                      | Range/Notes            |
| ----------- | ------------------------------------------------------------- | ---------------------- |
| TUNE        | Set VCO initial tune                                          | Manual only            |
| SUBOSC LVL  | Level of transistor-based suboscillator                       | Manual only            |
| DETUNE      | Detune the main oscillator vs. suboscillator                  | Manual only            |
| CUTOFF      | VCF Cutoff frequency                                          | Manual only, CV input  |
| RESONANCE   | VCF Resonance                                                | Feedback, acid tones   |
| F ENV       | Filter envelope amount                                        | Manual only            |
| VCA ENV     | VCA envelope amount                                           | Envelope strength      |
| VCO CV      | Manual offset of VCO pitch                                    | Manual only            |

**Buttons:**

| Button   | Function                                         |
| -------- | ------------------------------------------------ |
| ACCENT   | Triggers the Accent circuit                      |
| SLIDE    | Activates Portamento/Slide                       |
| OUT      | Main audio output                                |
| MAIN OUT | Same as OUT (duplication)                        |

---

## Inputs and Outputs

| Jack        | Type         | Description                                | Voltage Range         |
| ----------- | ------------ | ------------------------------------------ | --------------------- |
| VCO CV      | Input (CV)   | Controls VCO pitch (1V/oct)                | 0V to +10V            |
| GATE        | Input        | Gate/Trigger for envelope and VCA          | 0V = off, 2V+ = on    |
| ACCENT      | Input        | Boosts envelope intensity for punch        | 0V = no accent, 5V+   |
| SLIDE       | Input        | Initiates slide/portamento                 | 0V = off, 5V+ = on    |
| OUT         | Output       | Main audio output                          | -5V to +5V            |
| MAIN OUT    | Output       | Duplicate main output                      | -5V to +5V            |
| VCF ENV     | Input (CV)   | VCF Envelope CV input                      | 0V to +10V            |

---

## Usage Workflow

1. **Pitch control:** Send VCO CV (1V/oct) and use TUNE for fine adjustment.
2. **Suboscillator amount:** Adjust SUBOSC LVL for punch and body.
3. **Detuning:** Adjust DETUNE for richer analog texture.
4. **Gate/Accent/Slide:** Use GATE to trigger notes, ACCENT for punchier envelopes, and SLIDE for acid slides.
5. **VCF shaping:** Use CUTOFF and RESONANCE for filtering, F ENV to control how much envelope affects cutoff, VCF ENV for external modulation.
6. **VCA envelope:** Set how "snappy" or sustained the volume is with VCA ENV.
7. **Patch outputs:** OUT and MAIN OUT both output the final signal.

---

## Voltage Reference

- **VCO CV:** 1V/oct (typically 0–10V)
- **Gate/Accent/Slide:** 0V (off), 2V+/5V+ (on)
- **VCF ENV:** 0–10V

---

## Special Features

- Analog transistor suboscillator with detune
- Full analog OTA-based VCF for classic acid tones
- Accent and Slide for TB-303 style patterns

---

**More info & detailed manual:**  
[Erica Synths Bassline - Official Manual PDF](https://www.ericasynths.lv/en/shop/instruments-47/drum-modules-795/bassline/)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)