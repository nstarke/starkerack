# xaoc Devices — Sopot

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Manual PDF](manual.pdf)

# Kaona Fractaos Cheat Sheet

## What it is
**Fractaos** is a **4-voice polyphonic, multitimbral fractal oscillator** for Eurorack.  
Each voice contains:
- **2 oscillators**: driver + follower
- **1 ADSR envelope**
- **1 resonant fractal filter**

It supports:
- **Polyphonic MIDI**
- **4x CV/Gate voice input**
- **Drone mode**
- **Multitimbral mode** with different presets per voice

---

## Quick Start
### Basic patch
1. Patch **Out L / Out R** to your mixer/audio interface.
2. Send notes via:
   - **TRS Type-B MIDI**, or
   - **1V/oct + Trig** per voice
3. Set:
   - **Fractal Type** = main sound source
   - **Primitive Type** = modulation shape
   - **Morph** = blend/interaction between the two
   - **Texture** = resonant/fractal filter character
   - **Spread** = detune
4. Use **Loop / Trig / Morph(FM) / Spread / Chaos** switches to choose what the primitive modulates.
5. Short-press encoder for **ADSR**, long-press for **Save/Load/Setup/Multi**.

---

## Core Sound Concept
Fractaos is not a wavetable or sample oscillator. It generates **fractal curves in real time**.

### Main ingredients
- **Driver fractal** = main oscillator shape
- **Primitive fractal** = secondary fractal that modulates the main one
- **Morph** = complex blend between main and primitive behavior
- **Spread** = detune relationship
- **Texture** = fractal filter/resonance/formant extraction
- **Speed / Amount** = internal primitive-derived modulation source

---

## Performance Tips
### Great starter settings
- **Clean tonal patch**
  - Geometric fractal for both main + primitive
  - Low to medium **Chaos**
  - Medium **Depth**
  - Low **Texture**
  - Small **Spread**

- **Animated pad/drone**
  - Main fractal = one of the **Texture** types
  - Slow **Speed**
  - Medium/high **Amount**
  - More **Texture**
  - Use **Drone mode**

- **Metallic / FM-like**
  - Enable **Morph(FM)** only
  - Set **Loop OFF, Trig OFF, Spread OFF, Chaos OFF**
  - Use **Amount** around/above center

- **Percussion**
  - Main fractal = **Kick/Tom/Snare/HiHat/Cymbal**
  - Trigger with gate/MIDI notes
  - Use **Depth** for decay/tail
  - Use **Chaos** for hit variation

---

## Controls Reference

## Knobs / Potentiometers
### Fractal section
- **Fractal Type**
  - Selects main fractal
  - Accesses all main algorithms:
    - **14 geometric**
    - **6 textures**
    - **5 drum models**  
  - Main fractal only can use textures/drums

- **Primitive Type**
  - Selects secondary modulation fractal
  - **Geometric fractals only**
  - No texture or drum primitives

- **Chaos**
  - Chaos amount for main fractal
  - Quantized in steps depending on fractal

- **Primitive Chaos**
  - Chaos for primitive fractal

- **Depth**
  - Recursion/detail density of main fractal
  - Changes in steps
  - **Not CV modulatable**

- **Primitive Depth**
  - Recursion/detail density of primitive

### Interaction / modulation
- **Morph**
  - Blend and interaction between driver and follower
  - Not just a simple crossfade

- **Spread**
  - **Normal mode:** detune between driver and follower
  - **Drone mode:** oscillator spacing / chord selection

- **Texture**
  - Controls fractal filter behavior, resonance, formants, micro-detuning, filter intensity

- **Speed**
  - Primitive-derived LFO speed
  - Range: **0.001 Hz to 12 Hz**
  - Exponential response

- **Amount**
  - Primitive/LFO modulation amount
  - Also affects texture intensity
  - In simplified FM mode:
    - **0–50%** = internal feedback
    - **50% center** = neutral
    - **50–100%** = primitive modulates main frequency

### Pitch/output
- **Pitch**
  - Global pitch transpose
  - About **±2 octaves**

- **Out L**
  - Left output level

- **Out R**
  - Right output level

---

## Switches / Buttons
### Modulation switches
- **Loop**
  - ON = looping LFO
  - OFF = one-shot if Trig ON, otherwise inactive except special modes

- **Trig**
  - Retriggers primitive/LFO from each note
  - With Loop OFF: one-shot per note
  - With Loop ON: loops while note held

- **Morph (FM)**
  - Enables LFO modulation of Morph
  - Special role in simplified FM mode

- **Spread**
  - Enables LFO modulation of Spread/detune

- **Chaos**
  - Enables LFO modulation of main Chaos

### Mode/navigation
- **Drone**
  - Enables continuous drone mode
  - LED indicates status

- **PREV / NEXT**
  - Menu navigation
  - From main screen:
    - **PREV** = jump to LOAD
    - **NEXT** = jump to MULTI

- **Encoder (turn + push)**
  - Navigate screens and edit values
  - **Short press on main screen** = ADSR
  - **Long press on main screen** = preset/menu screens
  - **Long press** also exits LOAD/MULTI back to main screen

---

## Special Mode: Simplified FM
Use this exact switch combo:
- **Loop OFF**
- **Trig OFF**
- **Morph ON**
- **Spread OFF**
- **Chaos OFF**

Behavior:
- **Amount 0–50%**: self-feedback / sharper tone
- **Center**: neutral
- **Amount 50–100%**: primitive modulates frequency of main fractal

Notes:
- FM does **not** work on **Texture** or **Drum** main fractals
- FM is limited in high register to preserve sound quality

---

## Fractal Types Summary

### Geometric fractals
Usable as **main or primitive**. More tonal/stable.
- Mandelbrot
- Julia
- Cantor
- Sierpinski
- Dragon
- Rule30
- Lorenz
- Hénon
- Rössler
- Logistic
- Collatz
- Hilbert
- Fibonacci
- Koch

### Texture fractals
**Main only**. More noisy/atmospheric/pad-like.
- Cloud
- Storm
- Aliasing
- String
- Ensemble
- Cluster

### Drum fractals
**Main only**. Real-time synthesized percussion models.
- Kick
- Tom
- Snare
- HiHat
- Cymbal

Notes:
- **Morph** can blend drum attacks with a geometric primitive
- **FM has no effect on Drum curves**

---

## ADSR Envelope
Shared settings across all 4 voices, though each voice has its own envelope instance.

### Parameters
- **Attack:** **1 ms to 8 s**
- **Decay:** up to **8 s**
- **Sustain:** held level
- **Release:** up to **12 s**
- **Curve:** linear / exponential / logarithmic

### Access
- **Short press encoder** from main screen

### Important behavior
If **Sustain = 0**, Release still works if the note is released before decay completes.

---

## Drone Mode
Enable with **Drone** button.

### What changes
- Sound is continuous; no normal ADSR triggering
- All **8 oscillators** run simultaneously
- Spread becomes special:
  - controls unison / spread / chords

### Spread behavior in Drone mode
#### Zone 1: **0–0.02**
- Full unison

#### Zone 2: **0.02–0.50**
- Linear spread from unison to **+1 octave**
- Oscillator 0 stays anchored
- Oscillator 7 reaches +1 octave at 0.50

#### Zone 3: **0.50–1.00**
Scans through **13 chord/microtuning sets**:
- Unison cluster
- Maj triad spread
- Min triad spread
- Sus4 / Fifths
- Major 7th
- Minor 7th
- Add 9
- Add 11
- Add 13
- Just intonation
- 7-limit flavor
- 19-TET slice
- BP subset

### In normal mode
- Spread simply detunes follower vs driver, up to **+1 octave**

---

## Presets
### Storage
- Presets are **.frk** files on SD card
- EEPROM auto-saves:
  - MIDI settings
  - ADSR settings
  - MULTI configuration

### SAVE
- Long-press encoder from main screen
- SAVE appears first
- Encoder selects characters
- NEXT moves cursor
- When **confirm** is shown, press encoder to save

### LOAD
- Short click from SAVE screen
- Encoder scrolls presets
- Presets apply immediately for auditioning
- In LOAD mode, **physical knobs/CVs do not control sound**
- Use arrow guidance on screen to match panel to preset
- Long press returns to main/LIVE operation

### LIVE option
- Restores current manual panel state and previous envelope
- Exits preset override

---

## MULTI Mode
Each of 4 voices can load a different preset or remain LIVE.

### Access
- From main screen, **NEXT**
- Or click forward from LOAD

### Behavior
- Each voice can have:
  - its own preset
  - its own MIDI channel
  - its own volume

### Important
- If two voices share the same MIDI channel in MULTI, conflicting voices are forced to **LIVE** and shown in red

### Spread in MULTI
- **Non-Drone:** Spread knob affects **LIVE voices only**; preset voices keep stored Spread
- **Drone:** global Spread controls **all 8 oscillators**, including preset voices

### Exit logic
- MULTI stays active until no preset voices remain
- To fully return to LIVE:
  - set preset voices back to **LIVE**, or
  - make channel assignments collapse back as desired

---

## MIDI / Settings
### Polyphonic mode
- All voices share one MIDI channel
- Default: **MIDI channel 1**

### Multitimbral mode
- Each voice can use its own MIDI channel

### MIDI velocity
- Default = **YES**
- Can be disabled for simple note on/off behavior

### MIDI aftertouch
- Adds internal timbral movement/organic drift
- Not pitch modulation
- Depends heavily on selected fractal/settings

---

# Jack Reference

## Audio Outputs
- **Out L** — stereo left audio output  
  - Voltage range: **not specified in manual**

- **Out R** — stereo right audio output  
  - Voltage range: **not specified in manual**

---

## MIDI
- **TRS Type-B MIDI In**
  - Voltage range: **N/A digital MIDI**

---

## Per-voice pitch/gate inputs
- **4 × 1 V/oct inputs**
  - One per voice
  - Standard pitch CV
  - Voltage range: **not specified in manual**

- **4 × Trig inputs**
  - One per voice
  - Triggers/gates each voice
  - Voltage range: **not specified in manual**

---

## CV Inputs with attenuators
There are **8 CV inputs**, each with its own attenuator.

### Bipolar CV inputs
These accept **-5 V to +5 V**:
- **Texture CV**: **-5 V to +5 V**
- **Pitch CV**: **-5 V to +5 V**
- **Spread CV**: **-5 V to +5 V**
- **Morph CV**: **-5 V to +5 V**

### Unipolar CV inputs
These accept **0 V to +5 V**:
- **Speed CV**: **0 V to +5 V**
- **Amount CV**: **0 V to +5 V**
- **F-Chaos CV**: **0 V to +5 V**
- **P-Chaos CV**: **0 V to +5 V**

---

# Control Summary Table

## Knobs
- Fractal Type
- Primitive Type
- Chaos
- Primitive Chaos
- Depth
- Primitive Depth
- Morph
- Spread
- Texture
- Speed
- Amount
- Pitch
- Out L
- Out R

## Switches / Buttons
- Loop
- Trig
- Morph (FM)
- Spread
- Chaos
- Drone
- PREV
- NEXT
- Encoder push

## Other hardware
- TFT screen
- Rear SD card
- Rear micro-USB for updates

---

## What is and isn’t CV controllable
### CV controllable
- Texture
- Pitch
- Spread
- Morph
- Speed
- Amount
- Fractal Chaos
- Primitive Chaos

### Not CV controllable
- **Depth**
- **Primitive Depth**
- Fractal Type
- Primitive Type
- Output levels
- Most menu functions

---

## Best-use mental model
Think of Fractaos as:
- a **polyphonic dual-oscillator voice engine**
- where both oscillators are **fractal generators**
- and the second fractal acts as a **modulator / animator / FM source / envelope source**
- with **Texture** adding a resonant spectral sculpting layer

---

## Fast workflow
### For poly synth duties
- Use geometric fractals
- Low chaos
- moderate morph
- low spread
- shape via ADSR

### For drones
- Engage Drone
- choose a Texture or harmonic geometric fractal
- turn Spread into chord zone
- slow Speed + medium Amount
- increase Texture carefully

### For experimental/percussive
- Try Rule30, Lorenz, Hénon, Collatz
- or use Drum curves
- modulate Chaos and Morph
- use Trig mode for note-synced movement

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)