# Modulaire Maritime — Phosgène Wavetable FM Oscillator

- [Manual PDF](../../manuals/Phosgène _ Modulaire Maritime.pdf)

---

[Manual PDF / source](https://www.modulaire-maritime.com/phosg%C3%A8ne)

# Modulaire Maritime Phosgène — Cheat Sheet

## What it is
**Phosgène** is a **2hp digital wavetable / FM oscillator** with:
- **60 wavetables total**
- **2 banks of 30 waves**
- **Two parallel sound engines / outputs**
  - **Wavetable / waveshaping output**
  - **FM output**
- Shared controls for wave/folding/FM behavior
- **V/Oct tracking over 8 octaves**
- Internal setting memory for:
  - bank
  - wave
  - octave

## Quick start
1. Patch **V/OCT** from your sequencer/keyboard.
2. Take audio from either:
   - **WAVE** for wavetable/waveshaped tones
   - **FM** for darker, tighter FM tones
3. Set **COARSE** to tune.
4. Use **WAVE SEL** CV/input and front-panel selection to choose the waveform.
5. Use **FM MOD CV** to push deeper modulation / timbral movement.
6. Use the **OCTAVE** switch to shift pitch up/down by octaves.
7. Use **OCT DISPLACE** if the wavetable range is too bright/high and you want more usable low-end.

## Sound / behavior notes
- **Waveshaping / folding** is available on the wavetable side.
- **FM uses a 100 Hz frequency base**, producing a more restrained spectrum, good for:
  - tight FM basses
  - dark/deep modulation tones
- **FM and wavetable functions share controls**, but the FM engine has its own output.
- The module has an intentionally **lower-resolution digital character (11-bit)**, so some aliasing / grit is part of the sound.
- **Octave Displace applies only to the wavetable side**, not the FM side.

---

## Controls

### Knobs / panel controls
- **COARSE**
  - Main coarse tuning control.

### Switches / buttons
- **OCTAVE**
  - Octave up/down switching.
  - Changes pitch in **1 octave steps**.

- **BANK 1 / BANK 2**
  - Selects which set of 30 wavetables is active.

- **OCT DISPLACE**
  - Shifts the wavetable octave range lower.
  - Useful to:
    - keep brighter/folded tables in a more usable range
    - reduce excessively high/alias-prone behavior
    - extend low-end on wavetable tones
  - **Does not affect FM output/range**.

---

## Inputs and outputs

> **Important:** The provided manual page does **not specify exact voltage ranges** for the jacks below. Those ranges are therefore **not documented in the source provided**.

### Inputs
- **V/OCT**
  - 1V/oct pitch input
  - Tracks across **8 octaves**
  - **Voltage range:** *not specified in manual*

- **FM MOD CV**
  - CV input for deeper FM / modulation amount behavior
  - Shared modulation interaction with the FM engine
  - **Voltage range:** *not specified in manual*

- **WAVE SEL**
  - CV/input for waveform selection
  - **Voltage range:** *not specified in manual*

### Outputs
- **WAVE**
  - Audio output for the wavetable / waveshaping path
  - **Voltage range:** *not specified in manual*

- **FM**
  - Audio output for the FM path
  - **Voltage range:** *not specified in manual*

---

## Reference summary

### I/O at a glance
| Jack | Type | Function | Voltage range |
|---|---|---|---|
| V/OCT | Input | 1V/oct pitch control | Not specified |
| FM MOD CV | Input | FM/modulation CV input | Not specified |
| WAVE SEL | Input | Wave selection CV/input | Not specified |
| WAVE | Output | Wavetable / waveshaping audio out | Not specified |
| FM | Output | FM audio out | Not specified |

### Controls at a glance
| Control | Type | Function |
|---|---|---|
| COARSE | Knob | Coarse tuning |
| OCTAVE | Switch | Octave up/down in 1-octave steps |
| BANK 1 / BANK 2 | Switch | Select wavetable bank |
| OCT DISPLACE | Switch | Shifts wavetable octave range lower |

---

## Practical patch ideas

### 1. Basic oscillator voice
- **V/OCT** from sequencer
- **WAVE** to filter/VCA
- Use **COARSE** for tuning
- Select bank/wave to taste

### 2. Dark digital bass
- Patch from **FM** output
- Sequence with **V/OCT**
- Use lower octave settings
- Add envelope/VCA after output

### 3. Animated wavetable line
- Send slow CV/LFO to **WAVE SEL**
- Listen from **WAVE**
- Use **OCT DISPLACE** if the upper range gets too brittle

### 4. Parallel dual-tone patch
- Patch **WAVE** and **FM** to separate mixer channels
- Sequence both from same **V/OCT**
- Blend bright wavetable edge with darker FM weight

---

## Memory
Phosgène saves the last used:
- **Bank**
- **Wave**
- **Octave**

These settings are restored on power-up.

## Caveats
- The source page is descriptive rather than a full technical manual.
- **Exact jack voltage ranges, output levels, power draw, and calibration details are not provided** in the supplied manual page.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)