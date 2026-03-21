# Fancyyyyy — K-Accumulator Digital Complex Oscillator

- [Manual PDF](../../manuals/K_ACCUMULATOR_Quickstart_v1.02.pdf)

---

[Manual PDF](https://fancysynthesis.net)

# K-ACCUMULATOR Cheat Sheet

## What it is
A **complex digital oscillator voice** built around:
- **Main OSC** with stereo **sine/cosine outputs**
- **Mod oscillator** for PM / harmonic relationships
- **UFG** = function generator / oscillator / modulation source
- **Δ–∑** = stepped/smoothed pattern generator
- **Root** pitch system tying sections together

Best mindset: start from **Centre** (pure sine/cosine), then add **Shift / Depth / Shape / Stretch / Damped-Pulsar** one at a time.

---

## Fast Start
### Centre state
To get back to a clean reference sound:
- Center **all attenuverters**
- **Damped/Pulsar** fully CCW
- **Stretch** fully CCW
- **Shift / Depth / Shape** fully CCW

This always gives **pure sine + cosine** at the main outputs.

### First moves
1. Patch **Sine out** and **Cosine out** to L/R mixer inputs.
2. Use **Freq.** to set oscillator pitch.
3. Raise **Shift** for blended harmonic frequency shifting.
4. Raise **Depth** for self-feedback phase-mod distortion.
5. Raise **Shape** for harmonic wavefolding.
6. Turn **Mod Detune** to animate the folder.
7. Add **Stretch** to shift generated harmonics while keeping the fundamental fixed.
8. Raise a waveshaper CV attenuverter to let **UFG** or **Δ–∑** modulate it.
9. Raise **Damped/Pulsar** for sync + AM from the UFG.
10. Use **1V/TZ** attenuverter to bring in **Δ–∑** pitch motion.

---

## Core Concepts

### Root system
The **Root** section sets the tuning reference for:
- OSC
- UFG
- Mod oscillator

You can quantize Root to:
- **12-TET**
- **Just Intonation**

### Morph system
The **Morph encoder** moves through a matrix of waveshaping topologies, not separate engines.

**Good beginner route:** stay on the **left-hand path**:
- **FMNT → FBPM → 2OP → XPM → Asym**
This path keeps control meanings more consistent.

### OSC control meanings in most modes
- **Shift** = harmonic frequency shifting
- **Depth** = phase modulation / PM amount
- **Shape** = wavefolding

---

## Best Practical Patches

### 1. Pure stereo oscillator
- Go to **Centre**
- Patch **Sine** + **Cosine**
- Tune with **Freq.**
- Optional: route **Root** to OSC for quantized pitch

### 2. Animated harmonic tone
- Start at Centre
- Raise **Shift**
- Raise **Shape**
- Turn **Mod Detune**
- Add a little **Stretch**

### 3. West-coast-ish complex tone
- Morph to **2OP** or **XPM**
- Raise **Depth**
- Set Mod **Order** near center or higher
- Use **Harmonic** for ratio
- Fine-tune with **Detune**

### 4. Percussive / pulsar voice
- Raise **Damped/Pulsar**
- Set **UFG Time** to sub-audio
- Trigger UFG
- Shape UFG with **Skew** and **Shape**
- Patch OSC outputs to LPG/VCA/filter as desired

### 5. Quantized melodic sequence
- Route **Root** to OSC
- Enable **Scale**
- Use **Δ–∑** into OSC via normalled modulation or external patching
- Use **Chance / Length / Smooth** to evolve sequence
- Turn on **Q.Trig** for threshold-triggered UFG behavior

### 6. External audio tracking
- Patch external waveform into **Ext. Sync/Track**
- Set button to **Track**
- K-ACCUMULATOR follows pitch and outputs shaped sine/cosine
- Works well for square waves, weird but recognizable with voice/material

---

## Morph Modes Reference

### Poles
- **FMNT (green)**: formant-like AM + PM
- **Asym (yellow)**: asymmetric PM/AM, granular pulse-train-like spectra

### Left-hand path
- **FBPM (green)**: self-feedback PM, sine-to-saw style distortion
- **2OP (yellow)**: Mod oscillator PMs OSC
- **XPM (red)**: cross-phase modulation feedback

### Right-hand path
- **FBPM2 (green)**: chaotic self-feedback / subharmonic latching
- **2OP2 (yellow)**: separated self-mod vs Mod PM
- **XPM2 (red)**: fully separated XPM controls

### Color meaning
- **Green** = self-feedback PM only
- **Yellow** = Mod oscillator PM added
- **Red** = cross-feedback between oscillators

---

# Controls Reference

## 1. Root Section

### Knobs / Buttons
- **Root knob**
  - Sets root frequency
  - Mode selected by **CRS/FIN/OCT** button
- **CRS/FIN/OCT button**
  - Cycles:
    - coarse
    - fine
    - octave
  - Soft-pickup behavior
- **Scale knob**
  - Selects one of 21 scales in current tuning system
- **TET/JI button**
  - Toggles **12-TET / Just Intonation**
- **Root Send button**
  - Routes Root to:
    - OSC only
    - OSC + UFG
    - UFG only
    - neither

### Jack
- **1V input**
  - 1V/Oct calibrated input for Root pitch
  - **Voltage range: not stated in quick-start manual**

---

## 2. OSC Section

### Outputs
- **Main Sine output**
  - Waveshaped sine output
  - Intended as stereo pair with cosine
  - **Output voltage range: not stated in quick-start manual**
- **Main Cosine output**
  - Waveshaped cosine output
  - **Output voltage range: not stated in quick-start manual**

### Knobs / Buttons
- **Freq.**
  - Main oscillator frequency
- **Q.Trig button**
  - Sends trigger to UFG when oscillator crosses quantizer thresholds
  - Requires Root tracking + scale
- **Stretch**
  - Harmonic stretching / harmonic-only shifting
- **Damped/Pulsar**
  - Amount of damped sync + AM from UFG or external source
- **Ext. Sync/Track button**
  - Cycles:
    - Sync
    - Track
    - Off
- **Shift**
  - Waveshaping control
- **Depth**
  - Waveshaping control
- **Shape**
  - Waveshaping control
- **Morph encoder**
  - Selects morph position
  - Press = coarse/fine
  - Double-press = snap to nearest position

### Jacks
- **Ext. Sync/Track input**
  - External sync source or pitch tracking source
  - **Voltage/audio range: not stated**
- **TZPM input**
  - External AC-coupled through-zero phase modulation
  - **Voltage range: not stated**
- **1V/TZ input**
  - Auto-detecting pitch CV / through-zero FM input
  - Stepped/slower CV treated as DC-coupled 1V/Oct
  - Audio-rate treated as AC-coupled TZFM
  - **Voltage range: not stated**
- **Shift CV input**
  - CV for Shift
  - Normalled from UFG or Δ–∑
  - **Voltage range: not stated**
- **Depth CV input**
  - CV for Depth
  - Normalled from UFG or Δ–∑
  - **Voltage range: not stated**
- **Shape CV input**
  - CV for Shape
  - Normalled from UFG or Δ–∑
  - **Voltage range: not stated**
- **Morph CV input**
  - CV for morph position
  - **Voltage range: not stated**
- **Damped/Pulsar CV input**
  - CV over damped sync/pulsar amount
  - **Voltage range: not stated**

### Attenuverters / mini-controls
- **1V/TZ attenuverter**
- **Shift attenuverter**
- **Depth attenuverter**
- **Shape attenuverter**
- **Morph CV attenuverter**
- These have:
  - midpoint deadzone
  - exponential response
- Bottom-row source select buttons:
  - LED lit = **Δ–∑** normalled
  - LED unlit = **UFG** normalled
  - cable inserted overrides normalization

---

## 3. Mod Section

### Knobs / Buttons
- **Harmonic**
  - Sets Mod oscillator ratio/offset relative to tracked source
- **Order**
  - Sets Harmonic behavior:
    - min = free pitch offset
    - center = blended harmonics above, free below
    - CW = odd-harmonic emphasis
    - CCW = even-harmonic emphasis
    - max = quantized to current scale / integer ratios
- **Detune**
  - Detunes Mod from tracked frequency
  - Also animates main harmonic folder behavior
- **OSC/UFG button**
  - Selects Mod tracking source:
    - OSC
    - UFG
    - none lit = Root

### Jack
- **HMX/TZ CV input**
  - CV for Harmonic / TZ-related behavior
  - Tracks 1V/Oct in free-pitch mode at full attenuverter
  - **Voltage range: not stated**

### Attenuverter
- **HMX/TZ attenuverter**

### Outputs
- **No dedicated Mod audio output shown in quick-start**

---

## 4. UFG Section

### Outputs
- **Function output**
  - Anti-aliased function waveform
  - **Output voltage range: not stated**
- **Gate output**
  - Gate/pulse output, pulse width set by Skew
  - **Output voltage range: not stated**

### Knobs / Switches / Buttons
- **Loop/Trig 3-position switch**
  - Up = toggle looping
  - Middle = single-shot triggered externally
  - Down = momentary manual trigger
- **Time**
  - UFG rate/frequency
- **Skew**
  - Rise/fall asymmetry and gate pulse width
- **Shape**
  - Morphs linear / sine / exponential / raised cosine
- **Type button**
  - 4 trigger response modes:
    - hard sync with subharmonic locking
    - sync reversal
    - sustain + hard sync
    - sustain + sync reversal

### Jacks
- **Time CV input**
  - 1V/Oct tracking
  - Unpatched: random walk available through attenuverter
  - **Voltage range: not stated**
- **Skew CV input**
  - Unpatched: Δ–∑ normalled here
  - **Voltage range: not stated**
- **1V input**
  - 1V/Oct input for UFG frequency
  - **Voltage range: not stated**
- **TZFM input**
  - AC-coupled through-zero FM
  - **Voltage range: not stated**
- **Trig input**
  - External trigger/gate input across full frequency range
  - **Voltage range: not stated**

### Attenuverters
- **Time CV attenuverter**
- **Skew CV attenuverter**

---

## 5. Δ–∑ Section

### Output
- **Δ–∑ output**
  - Stepped or smoothed pattern CV
  - Good for pitch, PM, TZFM, or modulation
  - **Output voltage range: not stated**

### Knobs / Switch
- **Chance**
  - Probability of new values entering sequence
  - min = locked loop
  - max = fully renewed
- **Length**
  - Zooms pattern length from 2–16 steps
  - center deadzone = 8 steps
- **Smooth**
  - Glide/filter amount
- **Pattern switch**
  - Right = enter new value at current step
  - Left = restore previous value
  - Hold right = overwrite pattern
  - Hold left = double-length pattern

### Jack
- **Clock input**
  - External clock breaks UFG normalization
  - **Voltage range: not stated**

---

# Jack Summary

## Outputs
| Section | Jack | Function | Voltage Range |
|---|---|---|---|
| OSC | Sine Out | Main waveshaped sine | Not stated |
| OSC | Cosine Out | Main waveshaped cosine | Not stated |
| UFG | Function Out | Anti-aliased function waveform | Not stated |
| UFG | Gate Out | Gate/pulse output | Not stated |
| Δ–∑ | Δ–∑ Out | Stepped/smoothed pattern CV | Not stated |

## Inputs
| Section | Jack | Function | Voltage Range |
|---|---|---|---|
| Root | 1V In | Root pitch CV, 1V/Oct calibrated | Not stated |
| OSC | Ext. Sync/Track In | External sync or pitch tracking | Not stated |
| OSC | TZPM In | AC-coupled through-zero PM | Not stated |
| OSC | 1V/TZ In | Pitch CV or TZFM, auto-detected | Not stated |
| OSC | Damped/Pulsar CV In | CV over damped sync / pulsar amount | Not stated |
| OSC | Shift CV In | Shift modulation | Not stated |
| OSC | Depth CV In | Depth modulation | Not stated |
| OSC | Shape CV In | Shape modulation | Not stated |
| OSC | Morph CV In | Morph modulation | Not stated |
| Mod | HMX/TZ In | Harmonic modulation / 1V tracking in free mode | Not stated |
| UFG | Time CV In | Rate CV / 1V tracking | Not stated |
| UFG | Skew CV In | Skew modulation | Not stated |
| UFG | 1V In | UFG pitch CV | Not stated |
| UFG | TZFM In | AC-coupled through-zero FM | Not stated |
| UFG | Trig In | Trigger/gate input | Not stated |
| Δ–∑ | Clock In | External clock | Not stated |

---

# Control Summary

## Knobs
- Root
- Scale
- Freq.
- Stretch
- Damped/Pulsar
- Shift
- Depth
- Shape
- Morph
- Harmonic
- Order
- Detune
- Time
- Skew
- UFG Shape
- Chance
- Length
- Smooth

## Attenuverters / mini-pots
- Root 1V attenuverter
- OSC 1V/TZ attenuverter
- Shift attenuverter
- Depth attenuverter
- Shape attenuverter
- Morph CV attenuverter
- Mod HMX/TZ attenuverter
- UFG Time CV attenuverter
- UFG Skew CV attenuverter

## Buttons / push functions
- CRS/FIN/OCT
- TET/JI
- Root Send
- Q.Trig
- Ext. Sync/Track
- Morph encoder press
- Morph encoder double-press
- OSC/UFG (Mod source)
- UFG Type

## Switches / toggles
- UFG Loop/Trig 3-position switch
- Δ–∑ Pattern momentary switch

---

# Important Behaviors / Gotchas
- **Centre** is your reset point. Learn it.
- Many OSC CV inputs are **internally normalled** to **UFG or Δ–∑**.
- OSC bottom-row source buttons:
  - **LED lit = Δ–∑**
  - **LED off = UFG**
- **1V/TZ input auto-detects** slow CV vs audio-rate input.
- **Stretch only works when waveshaping is active.**
- **Detune** affects both Mod pitch relationship and folder animation feel.
- **Q.Trig** only works meaningfully when quantized Root tracking is active.
- **Δ–∑** edits are **non-destructive** at minimum Chance.

---

# Missing Technical Data
The quick-start manual does **not specify actual voltage ranges** for CV inputs or outputs. It only explicitly states:
- some inputs are **1V/Oct calibrated**
- some are **AC-coupled**
- some are **through-zero**
- some are **normalled internally**

For exact voltage ranges, a full technical manual would be needed.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)