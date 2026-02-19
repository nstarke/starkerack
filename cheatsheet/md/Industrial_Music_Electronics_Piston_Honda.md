# Industrial Music Electronics — Piston Honda

- [Manual PDF](../../manuals/phmk3manual11.pdf)

---

[**Official Piston Honda MkIII Manual PDF**](http://www.industrialmusicelectronics.com/products/21)

# Industrial Music Electronics – Piston Honda MKIII Cheat Sheet  
_Firmware v1.1 • Dual Wavetable Oscillator with Morphing & Nonlinear Waveshaping_

---

## PANEL OVERVIEW

- **Osc A/B:** Independent or linked digital wavetable oscillators, each w/ extensive CV controls.
- **Preset/Manager:** Instantly recall/store 8 global snapshots; morph/cycle between presets.

---

## JACK & CONTROL REFERENCE

| JACK/CONTROL      | TYPE                  | VOLTAGE RANGE              | FUNCTION                                                   |
|-------------------|----------------------|----------------------------|------------------------------------------------------------|
| **CV (XYZ axis)** | Input (attn'd)       | ±8V                        | Morphs X/Y/Z axis of wavetable "cube" (8×8×8 = 512 waves)  |
| **1V/Oct**        | Input                 | 0–8V recommended           | Exponential V/O pitch; follows standard 1V/oct scaling     |
| **CV (General)**  | Input (attn'verter)  | ±8V (±10V max)             | Modulates pitch/frequency (good for vibrato, mod wheel)    |
| **FM/Ext In**     | Input                 | AC, up to 10Vpp            | Audio-rate TZFM OR waveshaper input (via MODE button)      |
| **Sync**          | Input                 | 0–5V                      | Resets oscillator cycle (hard sync)                        |
| **Mix Output**    | Output                | Audio                      | Mix of both Oscillators                                    |
| **Osc Outputs**   | Output                | Audio                      | Individual out for Osc A/B                                 |
| **Preset CV**     | Input (attn)          | ±8V                        | Preset morph/cycle/trigger/random (configurable behavior)  |
| **MicroSD**       | Slot                  | n/a                        | Load custom wavetables (see below)                         |

---

## CONTROL ELEMENTS

| CONTROL           | TYPE          | FUNCTION                                                                              |
|-------------------|---------------|--------------------------------------------------------------------------------------|
| **Freq (Large knob) / Fine (Small knob)** | Pot          | Coarse/fine tuning; Assignable/reversed in global settings                           |
| **XYZ Sliders**   | Slider         | Manual position on X, Y, Z axis of wavetable cube                                    |
| **XYZ Attn'verters** | Pot         | CV polarity/amount for each axis; share CV input between both oscillators            |
| **MODE button**   | Button         | Toggles between oscillator/Ext In processing                                        |
| **SELECT button** | Button         | Focuses OSC for slider/CV assignment and tuning display                              |
| **LINK button**   | Button         | Links Osc B tuning to Osc A (B becomes a follower w/ optional offset/vibrato etc.)   |
| **PRESET button** | Button         | Engage preset/recall mode, edit, or enter preset-morph mode                          |
| **Encoder**       | Knob+Button    | Menu navigation; quick shortcuts for unison/octave; edits presets when pressed       |

---

## KEY OPERATION MODES

### Oscillator Mode
- Each OSC may run independently or B can LINK to A for unison/hard sync/supersaw.
- All tuning and morphing assignable by manual controls & CV.

### External In Mode
- Engage by pressing **MODE**.
- FM/Ext In jack becomes a signal processor (shapes input through selected wavetable).
- Large freq knob = input gain.

### Preset Manager
- Store/recall/morph all settings (8 slots):
    - **Press PRESET**: Scroll/load with encoder or CV input.
    - **Press PRESET again**: Enter MORPH (CV = smooth morph).
    - **Save**: Must use menu command to store permanently.

**Preset CV Input Modes (Global Config):**
- **CV+Offset:** Manual scan & morph via CV + knob for offset.
- **CV+Atten:** CV + knob is attenuator.
- **Trig+Offset:** CV input = trigger to step through presets; knob scans manual.
- **Trig Random:** Each trigger randomizes patch.

---

## SHORTCUTS

- **Unison (Add detuned sub-osc):** Hold Encoder, press SELECT for Oscillator
- **Octave Shift:** Hold SELECT, turn Encoder.

---

## Wavetable Editing/Loading

- Wavetables: 8 files (1.wav–8.wav), each = 64 waves × 256 samples.
- Use free [WaveEdit](https://synthtech.com/waveedit/) or similar.
- MicroSD card (FAT): Only correct format/naming will load.

---

## VOLTAGE REFERENCE SUMMARY

- **CV inputs (XYZ, Main):** ±8V (±10V ok); musical range ~±5V
- **1V/Oct:** 0–8V (C0 at 0V)
- **FM/Ext:** AC (±5V–10V peak); audio-rate signals only
- **Sync:** 0–5V
- **Preset CV:** ±8V

---

## MENU ACCESS

| MENU                   | ACCESS         | FUNCTION         |
|------------------------|---------------|------------------|
| **OSC A/B:**           | Enc+MODE      | Unison, Octave, Morph, Tone |
| **Global:**            | Enc+LINK      | Link, knob assign, load waves, reboot |
| **Preset:**            | Enc+PRESET    | Save, randomize, initialize, reload   |

---

## FACTORY/UTILITY

- **Firmware:** Update via Pickit3 (see website)
- **Calibration:** 1V/Oct tested at 1V & 7V, set trimmer on module rear.
- **Factory Reset:** Power on w/ PRESET button held, no cables inserted.

---

## QUICK PATCH IDEAS

- **Detuned "supersaw":** LINK B to A, dial fine tune for chorus.
- **Stereo/table morphing:** Separate outs, morph/sequence the X/Y/Z axes.
- **Waveshaper/processor:** MODE to Ext In, feed OSC B output to A input for complex waveforms.

---

**[Module Website, Waves, Firmware, Docs](http://www.industrialmusicelectronics.com/products/21)**  
**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**

---