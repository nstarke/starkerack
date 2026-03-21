# WMD — Skorpion

- [Manual PDF](../../manuals/SKORPION_Manual.pdf)

---

[Manual PDF](https://wmdevices.com/products/skorpion)

# WMD Skorpion — Cheat Sheet

## What it is
A **stereo wavefolder / waveform processor** built around a “vector core.”  
Instead of simply clipping/amplifying, Skorpion analyzes the **IN** signal against **8 threshold comparators** and reverses the vector core direction when thresholds are crossed. Result: highly controllable, animated folding with sequencing, feedback shaping, stereo widening, and lots of self-patching options.

---

## Fast Start
1. Patch audio to **IN**
2. Patch **OUT L** and/or **OUT R** to your mixer
3. Set:
   - **OUTPUT** around noon or below for mostly wet mono-ish folding
   - **FOLD** to taste
   - **SLOPE** up for brighter/more harmonics
   - **SHIFT** at noon for symmetry
   - **TARGET** to **5V** for hard/square-ish folding, or toward **CLIP** / **SLIDERS** for more complex behavior
4. Move the **8 sliders** in default mode to set fold thresholds
5. Experiment with:
   - **SHAPE** + shape source switch
   - **SYNC**
   - **EQUALIZE THLDs**
   - **TARGET ORDER**
   - **OUTPUT FILTERS/DC**

---

# Core Controls

## Knobs

### FOLD
Amount of wavefolding; effectively amplifies the input against the threshold stack.  
- CV controllable via **FOLD CV jack** + attenuverter

### SLOPE
Rate of change of the vector core. Higher = faster movement = more harmonic content.  
- CV controllable via **SLOPE CV jack** + attenuverter
- **1V/OCT** also affects slope for pitch-consistent timbre

### SHIFT
Offsets the input signal against the comparators for asymmetry.  
- Noon = ~0V shift
- Slow modulation can create frequency-shift-like motion
- CV controllable via **SHIFT CV jack** + attenuverter

### SHAPE
Modulates the slope using selected feedback/modulation source.  
- Noon = no feedback
- CV controllable via **SHAPE CV jack** + attenuverter

### TARGET
Sets vector core destination voltage:
- **5V**: static 5V, more square-like
- **CLIP**: target follows clip/input waveform
- **SLIDERS**: uses 8 target slider voltages as sequenced destinations
- CV controllable via **TARGET CV jack**

### OUTPUT
Crossfade/width control:
- Lower half: **DRY ↔ WET**
- Upper half: **WET ↔ WIDE**
- CV controllable via **OUTPUT CV jack** + attenuverter

---

## Switches / Toggles

### EQUALIZE THLDs (3-position)
Forces equal threshold spacing, making it behave more like a classic wavefolder. LED on = equalized.
- **ON**: always equalized; jack ignored
- **XOR (middle)**: equalized unless jack is high
- **JACK**: off unless jack is high

### DRY IF NO THLDs
If no thresholds are active, output becomes dry/following input. Useful when heavily modulating FOLD so you still get signal.

### SYNC (3-position)
Resets vector core at **IN** zero crossings.
- **SOFT**: ramps toward 0V at current slope
- **X**: off
- **HARD**: fast reset to 0V

### OUTPUT SWITCH
- **DC**: direct signal, no output filtering
- **FILTERS**: low end (<240Hz) centered; highs (>240Hz) delayed / widened by mid-side network

### TARGET ORDER
How slider targets are selected:
- **SEQ**: by count of active thresholds
- **TIED**: by most recently crossed threshold

### SHAPE SYM switch
For the SHAPE circuit:
- **SYM**: symmetric modulation for positive/negative waveform halves
- otherwise asymmetrical behavior

### TRGT MOD SYM / ASYM
For **TRGT MOD** input:
- **SYM**: full-wave rectified; symmetric effect
- **ASYM**: passes direct; asymmetric effect

### HALT IF TARG=0
If a target slider is at 0, this can halt motion during that segment for square/pause-like segments. Normals to HALT behavior.

### Spring Toggle
Multi-function center-off momentary switch next to sliders:
- **Center**: threshold editing
- **Hold left**: edit **TRGTs**
- **Hold right**: after ~1 sec enters **MACRO SETUP**
- **Tap right**: toggles Macro Envelope on/off

---

# Sliders

## Default mode: THLDs
The 8 sliders set the **8 threshold voltages** where folds occur.  
LED brightness shows threshold voltage.

## Hold left: TRGTs
The 8 sliders set the **8 target voltages** used when TARGET points toward **SLIDERS** and/or SHAPE source uses **TRGTs**.

## Hold right: MACRO SETUP
With spring toggle held right, sliders control:

1. **Macro Env Attack** — 50ms to 600s  
2. **Macro Env Release** — 500ms to 600s  
3. **THLD LFO Amount**  
4. **THLD LFO Rate** — 0.0016Hz to 6Hz  
5. **FOLD normal modulation**  
6. **SLOPE normal modulation**  
7. **SHIFT normal modulation**  
8. **SHAPE normal modulation**

For sliders 5–8:
- quick **top→bottom** gesture = **LFO mode**
- quick **bottom→top** gesture = **ENV mode**

Modes:
- **LFO**: 0.0016Hz to 6Hz, unipolar, amplitude controlled by Macro Envelope
- **ENV**: 50ms to 600s envelope, gated by Macro Env gate

---

# Shape Sources
The SHAPE source rotary switch selects what modulates the slope:

- **IN** — direct input
- **OUT** — output feedback; log/exp-like behavior
- **DELAY** — delayed signal from width circuit
- **COUNT** — staircase count of active thresholds
- **DIFF** — target minus current vector position; harsh/spiky
- **TRGTs** — use target sequencer per-segment
- **DAC** — weighted version of threshold count, subtler than COUNT
- **DIR** — ±5V direction signal

---

# Input Jacks Reference

> From manual specs:
> - **IN nominal range:** ±5V
> - **1V/OCT impedance:** 3MΩ
> - **TRGT MOD impedance:** 20kΩ
> - **All other CV/Gate inputs:** 220kΩ
> - Audio/CV inputs support audio-rate modulation unless noted

## Audio / Main CV Inputs

### IN
Main audio input.  
- **Nominal range:** **±5V**
- **Impedance:** 100kΩ

### 1V/OCT
Controls slope for note-consistent timbre across pitches.  
- **Voltage range:** not explicitly stated; standard 1V/oct CV expected

### FOLD CV
CV for Fold amount via attenuverter.  
- **Voltage range:** not explicitly stated

### SLOPE CV
CV for Slope amount via attenuverter.  
- **Voltage range:** not explicitly stated

### SHIFT CV
CV for Shift amount via attenuverter.  
- **Voltage range:** not explicitly stated

### SHAPE CV
CV for Shape amount via attenuverter.  
- **Voltage range:** not explicitly stated

### TARGET CV
CV for Target control.  
- **Voltage range:** not explicitly stated

### OUTPUT CV
CV for Dry/Wet/Wide output control.  
- **Voltage range:** not explicitly stated

---

## Threshold / Target / Logic Inputs

### THLDs/
Weighted global threshold CV input affecting all thresholds:
- THLD1 gets CV ÷ 128
- THLD2 gets CV ÷ 64
- THLD3 gets CV ÷ 32
- THLD4 gets CV ÷ 16
- THLD5 gets CV ÷ 8
- THLD6 gets CV ÷ 4
- THLD7 gets CV ÷ 2
- THLD8 gets CV ÷ 1
- **Voltage range:** not explicitly stated

### THLD1
Direct CV input for first threshold.  
- **Voltage range:** not explicitly stated

### EQ THLDs
Controls threshold equalization depending on switch setting.  
- High gate enables/disables equalization depending on switch mode
- **Voltage range:** not explicitly stated; treat as gate/CV input

### TRGTs
Global CV input that modulates all targets simultaneously.  
- **Voltage range:** not explicitly stated

### TRGT MOD
Directly influences TARGET output; can be symmetrical or asymmetrical.  
- **Voltage range:** not explicitly stated
- **Impedance:** 20kΩ

### CLIP
Overrides the normal clip source (normally IN).  
Use another signal to define clipping/overlay target behavior.  
- **Voltage range:** not explicitly stated

### HALT
Stops vector core movement and holds current voltage. Audio-rate modulatable.  
- **Voltage range:** not explicitly stated

### MACRO ENV
Gate input for Macro Envelope.  
- **Voltage range:** not explicitly stated; gate expected

---

# Output Jacks Reference

> All outputs: **1kΩ impedance**

### OUT L
Main left audio output.  
- **Voltage range:** not explicitly stated

### OUT R
Main right audio output.  
- **Voltage range:** not explicitly stated

### DELAY
Delayed waveform from the WIDE processing section.
- No output if OUTPUT is below noon
- Fades in from ~12:00 to 12:30
- Delay increases to ~3:00, then adds slower modulation up to full CW
- Delay time spec:
  - **80µs to 1.8ms** during fade-in region
  - **8.2ms** by around 2:15
  - **max 14.4ms ±3ms** at 2Hz modulation rate
- **Voltage range:** not explicitly stated

### ABS(IN)
Full-wave rectified version of IN.  
- For modulation or patch utility
- **Voltage range:** derived from IN; not explicitly stated

### G(IN>0)
Gate derived from input polarity:
- **0V** when IN < 0V
- **+5V** when IN > 0V

### TRGTs OUT
Direct output of the target sequencer.  
Useful as modulation source or 8-step wavetable-like oscillator control.  
- **Voltage range:** not explicitly stated

### DIFF
Difference between target voltage and current vector-core voltage.  
Always slopes toward 0V; high harmonic content.  
- **Voltage range:** not explicitly stated

### ±G(DIR)
Bipolar direction gate:
- **+5V** when vector core rises
- **-5V** when vector core falls

### COUNT/
Staircase output based on number of active thresholds:
- **0V to 4V**
- each active threshold adds **0.5V**

### DAC
Weighted version of threshold count:
- **Full scale:** **0V to 4V**
- THLD1 = 1/256 FS
- THLD2 = 1/128 FS
- THLD3 = 1/64 FS
- THLD4 = 1/32 FS
- THLD5 = 1/16 FS
- THLD6 = 1/8 FS
- THLD7 = 1/4 FS
- THLD8 = 1/2 FS

---

# LEDs / Indicators

### Threshold Slider LEDs
Show current slider value in the active context:
- THLDs
- TRGTs
- Macro setup values/modulation state

### EQUALIZE THLDs LED
On when thresholds are equalized.

### MACRO ENV LED
- **Red**: Macro gate is on
- **Blue**: Macro envelope level fading in/out

---

# Important Voltage / Timing Specs

## Explicit ranges from manual
- **IN nominal range:** **±5V**
- **G(IN>0):** **0V / +5V**
- **±G(DIR):** **-5V / +5V**
- **COUNT/:** **0–4V**
- **DAC:** **0–4V**
- **LFO rates:** **0.0016Hz to 6Hz**
- **Envelope times:** **50ms to 600s**
- **Macro env release:** **500ms to 600s**
- **Mid-side crossover:** **240Hz**
- **Max slew rate:** **0.4V/µs**
- **Delay:** **80µs to 14.4ms max** depending on OUTPUT position

## Not explicitly specified in the manual
The manual does **not** give exact voltage ranges for these CV inputs/outputs:
- FOLD CV
- SLOPE CV
- SHIFT CV
- SHAPE CV
- TARGET CV
- OUTPUT CV
- THLDs/
- THLD1
- EQ THLDs
- TRGTs input
- TRGT MOD
- CLIP
- HALT
- MACRO ENV
- OUT L / OUT R
- TRGTs OUT
- DIFF
- DELAY output amplitude

---

# Practical Patch Tips

## 1. Classic-ish wavefolder
- Enable **EQUALIZE THLDs**
- Set **TARGET** near **5V**
- Use modest **FOLD**
- Keep **SHIFT** near noon
- **SYNC** off or soft

## 2. Animated stereo timbre
- Set **OUTPUT** above noon toward **WIDE**
- Use **FILTERS** mode
- Patch **DELAY** somewhere else too
- Modulate **SHIFT** or **SHAPE**

## 3. Sequenced folding
- Hold left and set **TRGT sliders**
- Put **TARGET** toward **SLIDERS**
- Flip **TARGET ORDER** between **SEQ** and **TIED**
- Result: each threshold crossing picks a different destination voltage

## 4. Aggressive / broken digital-ish tones
- SHAPE source = **DIFF** or **OUT**
- Increase **SLOPE**
- Try **HARD SYNC**
- Use **HALT IF TARG=0**
- Patch **±G(DIR)**, **COUNT/**, or **DAC** back into CV inputs

## 5. Stable pitched use
- Feed pitch to **1V/OCT**
- Keep **SHIFT** centered
- Use **SYNC** if needed for more repeatable resets
- Use **TARGET = 5V** for more consistent/firm folded shapes

## 6. “Always audible” setup
- Turn on **DRY IF NO THLDs**
- Good when modulating **FOLD** deeply and folds may disappear

---

# Workflow Notes

- **Default slider mode** = thresholds
- **Hold left** = edit targets
- **Hold right** = macro setup
- Settings save after **1 minute of inactivity**
- **Macro Env** is always **OFF on power-up**

---

# One-Page Mental Model
- **IN** is analyzed by 8 thresholds
- Each threshold crossing flips vector-core direction
- **FOLD** = how hard input hits thresholds
- **SLOPE** = brightness / speed / harmonic density
- **SHIFT** = asymmetry
- **TARGET** = where the vector wants to go
- **SHAPE** = bends slope using feedback/modulation source
- **OUTPUT** = dry/wet/wide stereo treatment
- Sliders are either:
  - thresholds,
  - target sequencer,
  - or macro modulation setup

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)