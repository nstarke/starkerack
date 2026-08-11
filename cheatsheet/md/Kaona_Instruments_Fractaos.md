# Kaona Instruments — Fractaos

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Manual PDF](manual.pdf)

# Kaona Fractaos — Cheat Sheet

## What it is
- **4-voice polyphonic, multitimbral fractal oscillator**
- **8 real-time oscillators** arranged as **4 driver/follower pairs**
- **1 ADSR + 1 resonant fractal filter per voice**
- Play via:
  - **MIDI**
  - **4x 1V/oct CV inputs**
  - **4x Trig inputs**
- Modes:
  - **LIVE**
  - **LOAD preset**
  - **Drone**
  - **MULTI** (different preset / MIDI channel per voice)

---

## Quick start
1. **Patch audio**
   - Use **Out L** and **Out R**.
2. **Play notes**
   - Via **TRS Type-B MIDI**, or
   - Patch **1V/oct** and **Trig** to one or more voices.
3. **Set core tone**
   - **Fractal Type** = main sound source
   - **Primitive Type** = modulation fractal
   - **Chaos / Primitive Chaos**
   - **Depth / Primitive Depth**
4. **Shape timbre**
   - **Morph** blends/warps driver vs follower
   - **Spread** sets detune
   - **Texture** adds resonant/fractal filtering and organic motion
5. **Animate**
   - **Speed** = primitive/LFO speed
   - **Amount** = modulation depth / FM behavior in FM mode
   - Use switches: **Loop / Trig / Morph(FM) / Spread / Chaos**
6. **Set loudness**
   - **Out L** and **Out R** knobs
7. **Envelope**
   - Short press encoder from main screen for **ADSR**
8. **Presets**
   - Long press encoder for **SAVE/LOAD/SETTING/MULTI**

---

## Signal / synthesis concept
- **Driver fractal** = main oscillator curve
- **Primitive fractal** = modulation fractal
- **Morph** is not just a balance; the primitive also modulates the main fractal
- **Texture** acts like a **resonant fractal filter / formant extractor**
- **Spread**:
  - normal mode: detune between driver and follower
  - Drone mode: full 8-oscillator spacing / chord selection

---

## Main controls

### Knobs / potentiometers
| Control | Function |
|---|---|
| **Fractal Type** | Selects main fractal. Accesses geometric + texture + drum algorithms available to main oscillator. |
| **Primitive Type** | Selects modulation fractal. Geometric fractals only. |
| **Chaos** | Chaos amount for main fractal. Quantized by fractal type. |
| **Primitive Chaos** | Chaos amount for primitive fractal. |
| **Depth** | Main fractal recursion/detail depth. Stepped; **not CV modulatable**. |
| **Primitive Depth** | Primitive recursion/detail depth. |
| **Morph** | Blend / transformation between driver and follower behavior. |
| **Spread** | Normal mode: detune driver vs follower. Drone mode: unison/spread/chords. |
| **Texture** | Fractal filter resonance, formants, micro-detune, filter intensity. |
| **Speed** | Primitive-derived LFO speed, about **0.001 Hz to 12 Hz**. |
| **Amount** | LFO depth; also texture intensity; in FM mode becomes bipolar FM/feedback control. |
| **Pitch** | Global continuous transpose, about **±2 octaves**. |
| **Out L** | Left output level. |
| **Out R** | Right output level. |

---

## Switches / buttons / navigation

### Modulation switches
| Control | Function |
|---|---|
| **Loop** | LFO free-run / loop enable. |
| **Trig** | Retriggers primitive/LFO from note events. |
| **Morph (FM)** | Enables Morph modulation; also used to enter simplified FM mode. |
| **Spread** | LFO modulates Spread/detune. |
| **Chaos** | LFO modulates main Chaos. |

### Other buttons
| Control | Function |
|---|---|
| **Drone** | Toggles Drone mode; LED indicates status. |
| **PREV** | Menu navigation; from main screen jumps to **LOAD**. |
| **NEXT** | Menu navigation; from main screen jumps to **MULTI**. |
| **Encoder turn** | Scroll/select values, presets, parameters. |
| **Encoder short press** | From main screen: ADSR. In menus: advance/select. |
| **Encoder long press** | Enter/exit preset/menu system from main screen. |

---

## Important switch combinations

### Simplified FM mode
Set:
- **Loop OFF**
- **Trig OFF**
- **Morph ON**
- **Spread OFF**
- **Chaos OFF**

Behavior:
- **Amount 0–50%**: internal feedback on main fractal
- **Center**: neutral
- **Amount 50–100%**: primitive modulates main frequency = fractal FM

Notes:
- FM **does not work on Texture main fractals**
- FM **has no effect on Drum curves**
- FM intensity is limited at high pitch for sound quality

---

## Screens / workflow

### Main screen
- Visual display of active curves
- All panel controls active in **LIVE**

### ADSR
- Short press encoder from main screen
- Shared settings across all 4 voice envelopes

### SAVE / LOAD / SETTING / MULTI
- Long press encoder from main screen

### LOAD shortcut
- Press **PREV** from main screen

### MULTI shortcut
- Press **NEXT** from main screen

---

## Envelope
Each voice has its own ADSR, but all 4 share the same parameter settings.

### ADSR ranges
| Parameter | Range / behavior |
|---|---|
| **Attack** | **1 ms to 8 s** |
| **Decay** | up to **8 s** |
| **Sustain** | held level |
| **Release** | up to **12 s** |
| **Curve** | linear / exponential / logarithmic |

Notes:
- If **Sustain = 0**, **Release still works**
- In **Drone mode**, ADSR is effectively not note-triggered; sound is continuously held

### Internal fractal envelope
Per oscillator:
- **Amount** = intensity
- **Speed** = rate
- **Texture** = amount sent to fractal filter

---

## Fractal categories

### 1) Geometric fractals
Use as:
- **Main fractal**
- **Primitive fractal**

Examples:
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

Best for:
- tonal, structured, harmonic or experimental oscillator tones

### 2) Texture fractals
Use as:
- **Main fractal only**

Types:
- Cloud
- Storm
- Aliasing
- String
- Ensemble
- Cluster

Best for:
- noisy pads, atmospheres, drones, wide textures

Notes:
- shown in **red** on screen
- less defined pitch
- higher CPU load possible

### 3) Drum fractals
Use as:
- **Main fractal only**

Types:
- Kick
- Tom
- Snare
- HiHat
- Cymbal

Notes:
- real-time percussion models, not samples
- **Depth** mainly affects tail/duration
- **Chaos** affects variation/roughness/explosiveness
- **MIDI pitch still affects sound**
- **FM has no effect**
- **Morph** can blend drum attack with geometric primitive behavior

---

## Drone mode
Press **Drone** button.

### What changes
- All **8 oscillators** sound continuously
- No note required
- Oscillators are treated more independently
- Panel remains live

### Spread behavior in Drone mode
| Spread zone | Behavior |
|---|---|
| **0–0.02** | Unison |
| **0.02–0.50** | Linear spread from unison up to **+1 octave** across the 8 oscillators |
| **0.50–1.00** | Scans through **13 predefined chords / microtunings** |

### Drone chord list
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

### Outside Drone mode
- **Spread** = driver/follower detune only, up to **+1 octave** on follower

---

## Presets

### Auto-saved in EEPROM
- MIDI settings
- ADSR settings
- MULTI configuration

### SD card presets
- Stored as **.frk** files on rear SD card
- Include:
  - 11 main potentiometer values
  - 5 switch states
  - 5 envelope parameters

### Saving
1. Long press encoder
2. On **SAVE** screen, name preset with encoder
3. Use **NEXT/PREV** for characters
4. When **confirm** appears, press encoder to save

### Loading
- In **LOAD**, encoder scrolls presets
- Selected preset is **applied immediately**
- While in LOAD, **physical knobs/CVs do not control sound**
- Use on-screen arrows to match panel to preset
- Long press encoder to return to LIVE once matched

### LIVE option in preset list
- Restores actual manual/panel state from before LOAD mode

---

## MULTI mode
Assign different presets to different voices.

### What it does
- 4 voices can each:
  - load a different preset, or
  - stay in **LIVE**
- Each voice can respond to a different MIDI channel

### Access
- Short click from **LOAD** screen, or
- **NEXT** from main screen

### In MULTI
- **Preset voices** use their assigned presets
- **LIVE voices** still respond directly to panel controls

### Spread in MULTI
- **Non-Drone**: Spread knob affects **LIVE voices only**; preset voices keep saved Spread
- **Drone**: global Spread affects **all 8 oscillators**, including preset voices

### Exit behavior
- MULTI remains active until:
  - all preset voices are set back to **LIVE**, or
  - channel assignment effectively collapses back to non-MULTI use

---

## MIDI / settings
Access from **SETTING** screen.

### Polyphonic mode
- All voices on one MIDI channel
- Notes distributed across 4 voices

### Multitimbral mode
- One MIDI channel per voice
- Needed for full separate-preset multitimbral use

### MIDI channel conflicts
- If two voices share the same channel in MULTI, conflict is detected
- Affected voices may be locked in **LIVE** and shown in **red**

### MIDI velocity
- Can be **YES/NO**
- Default: **YES**

### MIDI aftertouch
- Supported if controller sends it
- Affects timbral/internal motion rather than pitch directly

---

# Jack reference

## Audio outputs
| Jack | Type | Voltage range | Function |
|---|---|---:|---|
| **Out L** | Audio out | Not specified in manual | Left stereo output |
| **Out R** | Audio out | Not specified in manual | Right stereo output |

## MIDI
| Jack | Type | Voltage range | Function |
|---|---|---:|---|
| **TRS Type-B MIDI In** | MIDI input | Digital MIDI standard | MIDI note/control input |

## Global CV inputs with attenuators
These 8 CV inputs each have a dedicated attenuator.

| CV Input | Voltage range | Function |
|---|---:|---|
| **Texture CV** | **-5 V to +5 V** | Modulates Texture |
| **Pitch CV** | **-5 V to +5 V** | Modulates global Pitch |
| **Spread CV** | **-5 V to +5 V** | Modulates Spread |
| **Morph CV** | **-5 V to +5 V** | Modulates Morph |
| **Speed CV** | **0 to +5 V** | Modulates Speed |
| **Amount CV** | **0 to +5 V** | Modulates Amount |
| **F-Chaos CV** | **0 to +5 V** | Modulates main Chaos |
| **P-Chaos CV** | **0 to +5 V** | Modulates Primitive Chaos |

## Per-voice pitch CV inputs
| Jack | Voltage range | Function |
|---|---:|---|
| **1V/oct Voice 1** | Standard **1 V/oct**; exact accepted voltage range not specified | Pitch CV for voice 1 |
| **1V/oct Voice 2** | Standard **1 V/oct**; exact accepted voltage range not specified | Pitch CV for voice 2 |
| **1V/oct Voice 3** | Standard **1 V/oct**; exact accepted voltage range not specified | Pitch CV for voice 3 |
| **1V/oct Voice 4** | Standard **1 V/oct**; exact accepted voltage range not specified | Pitch CV for voice 4 |

## Per-voice trigger inputs
| Jack | Voltage range | Function |
|---|---:|---|
| **Trig 1** | Not specified in manual | Trigger/gate for voice 1 |
| **Trig 2** | Not specified in manual | Trigger/gate for voice 2 |
| **Trig 3** | Not specified in manual | Trigger/gate for voice 3 |
| **Trig 4** | Not specified in manual | Trigger/gate for voice 4 |

---

# Control reference

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

## Switches / buttons
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
- Rotary encoder
- TFT color screen
- Rear SD card
- Rear micro-USB

---

## Practical patch ideas

### 1. Poly fractal pad
- Main fractal: **Mandelbrot** or **Koch**
- Primitive: **Rössler** or **Julia**
- Slow **Speed**
- Medium **Amount**
- Moderate **Morph**
- Higher **Texture**
- Long ADSR

### 2. Metallic FM tones
- Use **geometric** main fractal
- Enter **simplified FM mode**
- Sweep **Amount** above center
- Try **Dragon**, **Rule30**, **Hilbert**, **Mandelbrot**

### 3. Fractal percussion
- Main fractal: **Kick / Snare / HiHat**
- Lower **Depth** for tighter hits
- Increase **Chaos** for more aggression
- Add a geometric primitive and use **Morph** for tonal tail

### 4. Drone chord machine
- Enable **Drone**
- Turn **Spread** past 0.5 for chord sets
- Use **Texture** fractals for wide atmospheres
- Slowly modulate **Texture**, **Morph**, or **Chaos**

---

## Gotchas
- **Depth** and **Primitive Depth** are stepped and **not CV controllable**
- **Texture** and **Drum** fractals cannot be used as **Primitive**
- In **LOAD**, knobs/CVs are temporarily inactive until returning to LIVE
- In **MULTI**, panel controls affect **LIVE voices**, not preset voices, except some global behaviors like Drone Spread
- **FM**:
  - unavailable on **Texture** main fractals
  - ineffective on **Drum** curves

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)