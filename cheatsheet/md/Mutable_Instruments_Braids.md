# Mutable Instruments — Braids

- [Manual PDF](../../manuals/Manual - Mutable Instruments Braids Documentation.pdf)

---

```markdown
[**Mutable Instruments Braids v1.8 Manual PDF**](https://mutable-instruments.net/modules/braids/manual/)

# Mutable Instruments Braids 1.8 — Cheat Sheet

A compact reference for **Mutable Instruments Braids** digital macro-oscillator. Braids offers 45+ oscillator models with CV and manual controls for versatile synthesis.

---

## Panel Overview

| Label  | Name                    | Function                                                                 |
|--------|-------------------------|--------------------------------------------------------------------------|
| A      | LED Display & Encoder   | Shows model/settings. Rotate: Select model/option. Press: Enter/confirm. |
| B      | FINE                    | Fine frequency/coarse tune.                                              |
| C      | COARSE                  | Coarse frequency tuning.                                                 |
| D      | FM Attenuverter         | FM input amount (- to + polarity).                                       |
| E      | TIMBRE                  | Model-specific main timbre param (varies by model).                      |
| F      | Timbre Attenuverter     | CV depth/polarity for TIMBRE input.                                      |
| G      | COLOR                   | Model-specific secondary param (varies by model).                        |

---

## Jack Reference

| Jack    | Function                                   | CV Range      |
|---------|--------------------------------------------|---------------|
| **TRIG**   | Trigger/reset for some models, excites percussive models, or triggers internal AD envelope | 0–5V (gate/trig) |
| **V/OCT**  | Classic 1V/oct pitch CV input            | 0–8V typical  |
| **FM**     | Frequency modulation input               | ±5V           |
| **TIMBRE** | CV input for timbre param                | 0V = min knob, +5V = max  |
| **COLOR**  | CV input for color param                 | 0V = min knob, +5V = max  |
| **OUT**    | Audio output (model dependent amplitude) | N/A (audio signal) |

---

## Synthesis Model Selection

- Rotate Encoder (A) to select model.
- Press Encoder to enter settings/options.

Common models:  
- **CSAW** (Yamaha CS80 saw), notch via Timbre/Color
- **/\/|-_-_** (morph: triangle→saw→square→pulse)
- **FM, FBFM, WTFM** (2-op phase modulation, feedback, wild)
- **PLUK, BOWD, BLOW, FLUTE** (physical. Models = need TRIG or GATE)
- **WTBL, WMAP, WLIN, WTx4** (Wavetable/two-dim. wave scan)
- **DRUM, KICK, SNAR, CYMB, BELL, etc** (808 & physical drum models)
- **NOIS, TWNQ, CLKN** (Noise, twin peaks, random sample/hold)

---

## Key Controls (Summary)

**Frequency Controls:**  
- B: FINE — fine tune  
- C: COARSE — coarse tune

**Synthesis Parameters:**  
- E: TIMBRE — model-specific (e.g., morph, index, cutoff, etc.)  
- F: Timbre Attenuverter — CV depth/polarity for TIMBRE  
- G: COLOR — model-specific (e.g., symmetry, feedback, etc.)

**FM Control:**  
- D: FM Attenuverter — mod depth/polarity for FM input (±)

**Model/Option Selection:**  
- A: Encoder  
  - Rotate: browse  
  - Click: enter, select, confirm  
  - “WAVE” menu item: returns to model select

---

## Voltage-Controlled Inputs

- **V/OCT** — Pitch (1V/oct standard, 0V is C0; transposable, quantizable)
- **FM** — Frequency modulation (attenuverter D sets depth/polarity; ±5V typical)
- **TIMBRE, COLOR** — CV (0V–+5V for full sweep; offset by panel knob positions)

## Outputs

- **OUT** — Main audio output; signal level is model-dependent

---

## Menu Options (access via encoder press)

- **META**: Model selection via FM CV (for sequencing through models)
- **BITS, RATE**: Output bit-depth/sample rate
- **TSRC**: Select internal/external trigger/gate
- **TDLY**: Input trigger delay (for tracking fast CV/gate changes)
- **ATT, DEC**: Internal AD envelope settings (if used)
- **FM, TIM, COL, VCA**: Envelope routing amounts (to each param/amp)
- **RANG**: Tuning range (EXT, FREE, XTND, 440)
- **OCTV**: Octave shift
- **QNTZ, ROOT**: Pitch quantizer scale/root
- **FLAT, DRFT, SIGN**: Emulate analog tuning drift/imperfections
- **BRIG**: Screen brightness
- **CAL**: Calibration (see next section)

---

## Calibration

1. Unplug FM input. Patch **V/OCT** input from a calibrated CV source.
2. Set FINE/COARSE to 12 o’clock.
3. Enter **CAL.** in menu, hold encoder 1s.  
    - Display: **>C2**. Send 1V, confirm.
    - Display: **>C4**. Send 3V, confirm.
4. Done.

**TIP:** Use alternate interval for shifting COARSE knob calibration range.

---

## Firmware Update

- Audio file to FM input, power-on holding encoder, follow on-screen prompts (_RDY, @SYN, @CRC).

---

## Extras

- **ADC Debug Page:** Visualize incoming CV levels/polarities.
- **Scrolling Text:** Fun message display and editor.

---

**Reference Links**

- [Official Mutable Instruments Braids Manual](https://mutable-instruments.net/modules/braids/manual/)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
```
This cheat sheet contains all key operational info for fast reference, with jack voltages, button/knob summaries, and quick steps for synthesis/model changes, calibration, and firmware. For deep menu details refer to the full PDF above.