# Humble Audio — Quad Operator

- [Manual PDF](../../manuals/Quad Operator Manual.pdf)

---

[Manual PDF](https://www.dropbox.com/paper/doc/print/JsIQoU7GbeAboEJku9ZgE?print=true)

# Humble Audio Quad Operator + Algo Expander Cheat Sheet

## What it is
A 4-operator digital linear FM oscillator bank for Eurorack.

- 4 operators, each with:
  - variable waveform: **sine → triangle → square → saw**
  - independent output
  - per-operator gain/VCA behavior
  - modulation sends to any operator, including self
- Can run as:
  - **classic ratio-locked FM voice**
  - **4 independent oscillators** in free mode
  - **quad/LFO modulation source**
- Optional **Algo expander**:
  - save/recall FM matrices
  - crossfade between saved/live algorithms

---

## Quick start
### For classic harmonic FM
1. Set **VCO/LFO** to **VCO**
2. Put all 4 operators in **LOCK**
3. Set all **Detune** knobs to **12 o’clock**
4. Set all **Shape** knobs fully CCW (**sine**)
5. Set all **Mod 1–4** knobs fully CCW
6. Tune with **Coarse** and **Fine**
7. Use each operator’s **Ratio** to choose integer harmonic relationships
8. Turn up modulation sends gradually

### For 4 independent oscillators
1. Put operator(s) in **FREE**
2. In free mode:
   - **Ratio knob** becomes coarse tuning
   - **Ratio CV** becomes **1V/oct** for that operator
3. Patch from individual **Op 1–4 outputs**

### For modulation/LFO use
1. Set **VCO/LFO** to **LFO**
2. Use **Reset** to restart phase
3. Keep operators in **LOCK** if you want phase-related complex modulation

---

## Core concepts

### LOCK vs FREE
**LOCK**
- Operator frequency is an **integer ratio** of master pitch
- Best for harmonic / classic FM sounds
- **Ratio knob** selects approx **x1/11 to x11** in integer steps
- **1V/Oct**, **Coarse**, and **Fine** affect all locked operators

**FREE**
- Each operator becomes its own oscillator
- **Ratio knob** = operator coarse tuning
- **Ratio CV** = **1V/oct** for that operator
- Better for independent voices or inharmonic FM

### Gain behavior
Each operator’s **Gain CV** controls:
- its output level
- how strongly it modulates other operators via its sends

So gain acts like a built-in VCA for both carrier level and modulation depth.

### Mod matrix
Each row is a source:
- Operator 1
- Operator 2
- Operator 3
- Operator 4
- AR FM external input

Each **Mod 1–4** knob sends that source to the destination operator.

Example:
- In Operator 2 row, **Mod 1** = amount Operator 2 modulates Operator 1
- Self-modulation is allowed

---

## Front panel controls

## Master controls
- **Coarse**
  - Master tuning
  - Affects all operators in **LOCK**
  - Exponential response over **8 octaves**
- **Fine**
  - Master fine tune
  - Range: **±6 semitones**
- **VCO/LFO switch**
  - Sets frequency range for master tuning
- **1V/Oct input**
  - Pitch CV for all operators in **LOCK**
- **LF FM input**
  - Low-frequency pitch modulation
  - Best for vibrato, bends, envelopes
  - Range corresponds to **±6 semitones**
- **AR FM input**
  - External audio-rate modulator input
- **Reset input**
  - Resets phase of all operators

---

## Per-operator controls
Each operator has:

- **Lock/Free toggle**
  - LOCK = ratio-locked FM operator
  - FREE = independent oscillator
- **Ratio knob**
  - LOCK: integer ratio relative to master pitch
  - FREE: operator coarse tuning
- **Ratio CV jack**
  - LOCK: modulates ratio parameter
  - FREE: becomes **1V/oct** for that operator
- **Detune knob**
  - Fine tuning
  - Range: **±6 semitones**
- **Shape knob**
  - Crossfades **sine → triangle → square → saw**
- **Shape CV jack**
  - CV over waveshape
- **Gain CV jack**
  - Controls operator level and modulation intensity
  - Normalled high, so operator is active without patching
- **Mod 1–4 knobs**
  - Send this operator as FM to Operators 1–4
- **Op output jack**
  - Individual output for that operator

---

## External modulation section
For the dedicated **AR FM** input:

- **AR FM jack**
  - External audio-rate modulator input
- **AR FM Gain knob**
  - Adjusts external input level
  - Set to avoid clipping
- **Clip LED**
  - Red LED = external input clipping
- **Gain AR FM CV jack**
  - VC over external modulation depth
  - Normalled high
- **Mod 1–4 knobs**
  - Send external AR FM source to Operators 1–4

---

## Algo expander
Adds algorithm save/recall and crossfading of the modulation matrix.

### What gets stored
Only modulation matrix values:
- all **Mod 1–4** knobs for:
  - Operator 1
  - Operator 2
  - Operator 3
  - Operator 4
  - AR FM input row

### Slots
- **A**
- **B**
- **C**
- **Live** = current physical knob positions

### Buttons / controls
- **A / B / C / Live buttons**
  - **Long press A/B/C** until LED blinks twice = save to slot
  - **Short press** = assign slot into crossfade selection
- **Crossfade knob**
  - Morph between left/right selected algorithms
- **Crossfade CV input**
  - CV control of algorithm morph

### Important behavior
- If using only **A/B/C** slots, the physical **Mod** knob positions are ignored
- Double-tap **Live** if you want only current panel settings

---

## Patch tips
### Simple 2-op FM voice
- Op1 = carrier, monitor **Op1 out**
- Op2 = modulator
- Both in **LOCK**
- Op1 ratio = 1
- Op2 ratio = 2 or 3
- Op2 row: raise **Mod 1**
- Keep shapes near sine for cleaner FM

### Feedback FM
- Use self-modulation by turning up an operator’s own destination knob
- Or patch an output externally and return it via **AR FM**

### Layered outputs
- Since each operator has its own output, you can:
  - mix multiple carriers
  - process operators separately
  - use one operator as audible carrier and others as CV/audio modulators

---

## Voltage ranges and signal reference

## Inputs
| Jack | Type | Voltage Range | Normal | Notes |
|---|---|---:|---:|---|
| **Reset** | Gate in | **0V / 5V**, threshold ~**2.5V** | 0V | Phase reset for all operators |
| **1V/Oct** | CV in | **-1V to +5V** | 0V | Master pitch for locked operators |
| **LF FM** | CV in | **-5V to +5V** | 0V | Low-frequency pitch modulation |
| **Ratio 1–4** | CV in | **-5V to +5V** | 0V | Ratio control in lock; **1V/oct** in free |
| **Shape 1–4** | CV in | **-5V to +5V** | 0V | Wave shape modulation |
| **Gain 1–4** | CV in | **0V to +5V** | **+5V** | Controls output level and FM send intensity |
| **Gain AR FM** | CV in | **0V to +5V** | **+5V** | External modulation depth |
| **AR FM** | Audio in | **Trimmable for -5V to +5V or -10V to +10V** | 0V | External audio-rate FM source |
| **Algo Crossfade** | CV in | Not specified in manual | — | CV over algorithm crossfade |

## Outputs
| Jack | Type | Voltage Range | Sample Rate | Notes |
|---|---|---:|---:|---|
| **Op 1–4** | Audio/CV out | **-5V to +5V** | **48 kHz** | Individual operator outputs |

---

## Parameter ranges
| Parameter | Range |
|---|---|
| **Coarse (VCO mode)** | **16.35 Hz (C0) to 2093 Hz (C7)** |
| **Coarse (LFO mode)** | **0.511 Hz (C-5) to 65.41 Hz (C2)** |
| **Fine** | **±6 semitones** |
| **Ratio 1–4 (LOCK)** | **x1/11 to x11** relative to master coarse/fine |
| **Ratio 1–4 (FREE, VCO)** | **16.35 Hz (C0) to 2093 Hz (C7)** |
| **Ratio 1–4 (FREE, LFO)** | **0.511 Hz (C-5) to 65.41 Hz (C2)** |
| **Detune 1–4** | **±6 semitones** |
| **Shape** | Crossfade: **sine / triangle / square / saw** |
| **Gain 1–4** | **0 to 1** multiplier |

---

## CV scaling note
For **Ratio** and **Shape** parameters:
- **5V of CV = full knob travel**
- Bipolar CV can sweep beyond current knob setting in either direction

---

## Calibration
Use if pitch tracking seems off.

### Patch:
- **Op1 → Ratio1**
- **Op2 → Ratio2**
- **Op3 → Ratio3**
- **Op4 → Ratio4** and **1V/Oct** via **unbuffered split**
  - Important: use **Op4** for the split

### Trigger calibration:
1. Flip Operator 1 free/lock once
2. Flip Operator 2 free/lock once
3. Flip Operator 3 free/lock once
4. Flip Operator 4 free/lock once
5. Flip **VCO/LFO** switch **5 times quickly**

Success indication:
- Gain LEDs blink twice

---

## Firmware / physical specs
- Firmware update via **micro USB** on back
- Manual mentions firmware version **1.0.4**
- **Quad Operator**
  - **30 hp**
  - **25 mm deep**
  - **+12V: 140 mA**
  - **-12V: 13 mA**
- **Algo expander**
  - **4 hp**
  - **25 mm deep**
  - **+12V: 5 mA**
  - **-12V: 0 mA**

---

## Best-use summary
- Use **LOCK + sine + no detune** for stable, harmonic FM
- Use **FREE** for separate oscillators or inharmonic textures
- Use **Gain CV** like a modulation VCA
- Use **AR FM** for external operators, feedback, or wild FM
- Use **Reset** in LFO mode for repeatable modulation shapes
- Use **Algo** to store and morph FM routings

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)