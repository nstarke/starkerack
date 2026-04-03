# Humble Audio — Quad Operator Algo Extension

- [Manual PDF](../../manuals/Quad Operator Manual.pdf)

---

[Manual PDF](https://www.dropbox.com/paper/doc/print/JsIQoU7GbeAboEJku9ZgE?print=true)

# Humble Audio Quad Operator Cheat Sheet

## What it is
A **4-operator digital linear FM oscillator/LFO bank** with:
- 4 independently usable operators
- continuously variable waveshape per operator: **sine → triangle → square → saw**
- full **modulation matrix**: each operator can modulate any operator, including itself
- **AR FM external audio-rate mod input** with its own modulation sends
- optional **Algo expander** for saving/crossfading FM routing setups

---

## Quick-start patch
For classic, harmonic FM:
1. Set **VCO/LFO** to **VCO**
2. Put all 4 operators in **LOCK**
3. Set all **Detune** knobs to **12 o’clock**
4. Set all **Shape** knobs fully CCW (**sine**)
5. Turn all **Mod 1–4** knobs fully CCW
6. Patch **1V/Oct** and take audio from one or more **Op outputs**
7. Raise one operator’s **Mod** send into another operator
8. Use the modulating operator’s **Gain CV/level** to animate FM depth

---

## Core concept
Each row = one **operator**.

Each operator has:
- a tuning control (**Ratio** in LOCK, coarse tuning in FREE)
- **Detune**
- **Shape**
- **Gain**
- four **Mod sends** to Operators 1–4

### LOCK vs FREE
**LOCK**
- Operator follows master pitch at an **integer ratio**
- Best for classic harmonic FM
- Ratio knob selects **1/11 to 11x** relative to master tuning, in integer steps

**FREE**
- Operator becomes an independent oscillator/LFO
- Ratio knob becomes the operator’s own coarse tuning
- Ratio CV becomes **1V/oct** for that operator
- Better for independent oscillators / inharmonic FM

---

## Master controls

### Coarse knob
- Master tuning for all operators in **LOCK**
- Exponential response across **8 octaves**
- Range:
  - **VCO mode:** **16.35 Hz (C0) to 2093 Hz (C7)**
  - **LFO mode:** **0.511 Hz (C-5) to 65.41 Hz (C2)**

### Fine knob
- Master fine tune for all locked operators
- Range: **±6 semitones**

### VCO / LFO toggle
- Changes base frequency range of the whole module

### 1V / Oct input
- Master pitch CV for all operators in **LOCK**
- **Voltage range:** **-1V to +5V**
- Normal: **0V**
- Sample rate: **6 kHz**

### LF FM input
- Low-frequency pitch modulation input for all locked operators
- Good for vibrato, bends, pitch envelopes
- **Voltage range:** **-5V to +5V**
- Normal: **0V**
- Sample rate: **6 kHz**

### AR FM input
- External **audio-rate modulation input**
- Lets external audio modulate internal operators
- Especially useful for feedback/complex FM patches
- **Voltage range:** trimmable for **-5V to +5V** or **-10V to +10V**
- Normal: **0V**
- Sample rate: **48 kHz**

### Reset input
- Resets phase of all operators
- Useful in LFO mode / as a modulation source
- Works regardless of lock/free state
- **Gate input:** **0V / 5V**, threshold about **2.5V**
- Normal: **0V**
- Sample rate: **6 kHz**

---

## Per-operator controls

For each operator 1–4:

### Lock/Free toggle
- **LOCK:** ratio-based tuning relative to master pitch
- **FREE:** independent oscillator/LFO

### Ratio knob + Ratio CV
- **LOCK:** integer multiplier of master pitch
  - Range: **x1/11 to x11**
- **FREE:** continuous coarse tune for that operator
  - **VCO mode:** **16.35 Hz to 2093 Hz**
  - **LFO mode:** **0.511 Hz to 65.41 Hz**

**Ratio CV input**
- In **FREE**, acts as **1V/oct** for that operator
- **Voltage range:** **-5V to +5V**
- Normal: **0V**
- Sample rate: **6 kHz**

### Detune knob
- Fine tune per operator
- Range: **±6 semitones**

### Shape knob + Shape CV
- Morphs waveform:
  - **sine → triangle → square → saw**
- Good starting point for clean FM: full CCW = **sine**

**Shape CV input**
- **Voltage range:** **-5V to +5V**
- Normal: **0V**
- Sample rate: **6 kHz**

### Gain CV
- Controls operator level **and** how strongly it modulates destinations
- Think of it like a built-in VCA for both audio output and FM send intensity
- Normalled to **full gain**

**Gain CV input**
- **Voltage range:** **0V to +5V**
- Normal: **+5V**
- Sample rate: **6 kHz**

### Mod 1 / 2 / 3 / 4 knobs
- FM send amounts from this operator to Operators **1–4**
- Includes **self-modulation**
- Effective send level depends on operator **Gain**

---

## External AR FM section
The external AR FM source behaves like another modulator with its own send row.

### AR FM Gain knob
- Sets incoming external modulation level
- Adjust to avoid clipping

### AR FM clipping LED
- Red LED = input clipping/distortion
- Reduce AR FM Gain if it lights

### Gain AR FM CV input
- VCA for external modulation amount
- Normalled to full gain
- **Voltage range:** **0V to +5V**
- Normal: **+5V**
- Sample rate: **6 kHz**

### AR FM Mod 1–4 knobs
- Amount of external audio-rate modulation sent to Operators **1–4**

---

## Algo expander
Adds saved FM-routing “algorithms” and crossfading.

### What it stores
Only the **modulation matrix settings**:
- all **Mod 1–4** knobs for the 4 operators
- **AR FM Mod 1–4** knobs

### Slots
- **A**
- **B**
- **C**
- **Live** = current actual knob positions

### Buttons
- **Long press A/B/C**: save into that slot
- **Short press a slot**: select it into the crossfade pair
- Press two slots to define left/right endpoints
- Double-tap **Live** to use only current knob positions

### Crossfade knob / CV
- Crossfades between selected left/right algorithms
- Manual text does not specify CV voltage range for expander crossfade jack

### Important behavior
- If using only **A/B/C** and not **Live**, the physical Mod knobs on Quad Operator are ignored

---

## Input / output reference

## Inputs

### Master inputs
| Jack | Function | Voltage Range | Normal | Sample Rate |
|---|---|---:|---:|---:|
| Reset | Phase reset trigger/gate for all operators | **0V to 5V** (threshold ~**2.5V**) | 0V | 6 kHz |
| 1V / Oct | Master pitch CV for locked operators | **-1V to +5V** | 0V | 6 kHz |
| LF FM | Global low-frequency FM/pitch modulation | **-5V to +5V** | 0V | 6 kHz |
| AR FM | External audio-rate modulator input | **trimmable -5V to +5V or -10V to +10V** | 0V | 48 kHz |

### Per-operator inputs
| Jack | Function | Voltage Range | Normal | Sample Rate |
|---|---|---:|---:|---:|
| Ratio 1–4 | Ratio CV in LOCK / 1V-oct in FREE | **-5V to +5V** | 0V | 6 kHz |
| Shape 1–4 | Wave shape CV | **-5V to +5V** | 0V | 6 kHz |
| Gain 1–4 | Operator gain / FM index VCA | **0V to +5V** | +5V | 6 kHz |
| Gain AR FM | External mod input gain CV | **0V to +5V** | +5V | 6 kHz |

## Outputs
| Jack | Function | Voltage Range | Sample Rate |
|---|---|---:|---:|
| Op 1 | Operator 1 output | **-5V to +5V** | 48 kHz |
| Op 2 | Operator 2 output | **-5V to +5V** | 48 kHz |
| Op 3 | Operator 3 output | **-5V to +5V** | 48 kHz |
| Op 4 | Operator 4 output | **-5V to +5V** | 48 kHz |

---

## Full control reference

## Knobs
### Master
- **Coarse** — master tuning
- **Fine** — master fine tuning

### Per operator 1–4
- **Ratio**
- **Detune**
- **Shape**
- **Mod 1**
- **Mod 2**
- **Mod 3**
- **Mod 4**

### External AR FM
- **AR FM Gain**
- **AR FM Mod 1**
- **AR FM Mod 2**
- **AR FM Mod 3**
- **AR FM Mod 4**

### Algo expander
- **Crossfade**

## Toggles
- **VCO/LFO**
- **Operator 1 Lock/Free**
- **Operator 2 Lock/Free**
- **Operator 3 Lock/Free**
- **Operator 4 Lock/Free**

## Buttons
- **Algo A**
- **Algo B**
- **Algo C**
- **Algo Live**

---

## Practical patch tips

### For clean/harmonic FM
- Keep operators in **LOCK**
- Use **integer ratios**
- Keep **Detune at noon**
- Start with **sine waves**
- Add modulation slowly

### For animated FM
- Patch envelopes/LFOs to **Gain 1–4**
- This changes both output level and FM depth dynamically

### For independent oscillator bank use
- Put operators in **FREE**
- Use each output separately
- Ratio CV becomes per-operator **pitch CV**

### For gnarlier tones
- Use:
  - non-sine shapes
  - self-modulation
  - FREE mode
  - detuning
  - external **AR FM**
  - feedback-style patches with locked operators

---

## Calibration
If pitch tracking seems off:

### Patch:
- **Op 1 → Ratio 1**
- **Op 2 → Ratio 2**
- **Op 3 → Ratio 3**
- **Op 4 → Ratio 4** and **1V/Oct** via **unbuffered split**

Important:
- Use **Op 4** for the split to 1V/Oct
- Use an **unbuffered** mult/splitter

### Trigger calibration:
1. Flip Operator 1 Lock/Free once
2. Flip Operator 2 Lock/Free once
3. Flip Operator 3 Lock/Free once
4. Flip Operator 4 Lock/Free once
5. Flip **VCO/LFO** switch **5 times quickly**

Success indication:
- Gain indicator LEDs blink **twice**

---

## Specs
### Quad Operator
- **Width:** 30 hp
- **Depth:** 25 mm
- **Power:** +12V **140 mA**, -12V **13 mA**

### Algo expander
- **Width:** 4 hp
- **Depth:** 25 mm
- **Power:** +12V **5 mA**, -12V **0 mA**

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)