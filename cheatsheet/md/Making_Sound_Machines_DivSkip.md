# Making Sound Machines — DivSkip

- [Manual PDF](../../manuals/SKORPION_Manual.pdf)

---

[Manual PDF](https://wmdevices.com/cdn/shop/files/Skorpion_Manual_Rev1.00.pdf)

# WMD Skorpion Cheat Sheet

## What it is
**Skorpion** is a stereo analog **wavefolder / waveform animator** built around a **vector core**:
- Your **IN** signal is compared against **8 thresholds**
- Each threshold crossing can reverse the core’s direction
- **SLOPE** sets how fast the core moves
- **TARGET** sets what voltage the core moves toward
- **SHAPE** adds feedback-based contouring
- **OUTPUT** crossfades from dry → wet → stereo widened wet

It can behave like:
- a classic-ish wavefolder
- a highly asymmetrical folding/distortion source
- a CV/audio-rate animation engine
- a modulation source generator via its many aux outputs

---

## Quick start
1. Patch **audio to IN**
2. Patch **OUT L** and **OUT R** to mixer/output
3. Set:
   - **OUTPUT** around noon to full wet
   - **TARGET** to **5V** or **CLIP**
   - **SYNC** to **SOFT** or **HARD** for stable behavior
   - **EQUALIZE THLDs** ON for simpler/classic folding
4. Raise **FOLD**
5. Adjust **SLOPE**
6. Add **SHIFT** for asymmetry
7. Add **SHAPE** and choose a **SHAPE source** for more complex timbres

If it gets too weird/silent while modulating:
- turn on **DRY IF NO THLDs**

---

## Core sound controls

### FOLD
Amplifies the input against the threshold stack; more fold activity.

### SLOPE
Sets the vector core slew rate. Higher = more harmonic content, brighter/faster motion.

### 1V/OCT
Tracks **SLOPE** so timbre stays more consistent across pitch.

### SHIFT
Offsets the input against thresholds for asymmetry.
- Noon = ~0V shift
- Slow modulation here can create frequency-shift-like effects

### TARGET
Sets where the vector core tries to go:
- **5V**: static destination, squarer sounds
- **CLIP**: uses input waveform (or external CLIP jack) as destination overlay
- **SLIDERs**: uses 8 target sliders as a sequenced destination voltage

### SHAPE
Modulates SLOPE using a selected feedback/control source.
- Noon = no feedback
- **SYM** switch on: shaping is symmetrical for + / – portions of the waveform

### OUTPUT
Crossfader:
- lower half: **DRY ↔ WET**
- upper half: **WET ↔ WIDE**
- **WIDE** brings in stereo delay/mid-side widening

---

## Most important switches / toggles

### EQUALIZE THLDs switch
Forces equal threshold spacing; sounds more like a classic wavefolder.
- **ON**: equalized always on; jack ignored
- **XOR**: equalized on unless jack is high
- **JACK**: equalized off unless jack is high

LED on = thresholds equalized.

### DRY IF NO THLDs
If no thresholds are active, forces dry signal through the core.
Helpful when heavy modulation causes folding to disappear.

### SYNC
Resets vector core at **IN zero crossings**:
- **SOFT**: ramps toward 0V at current slope
- **X**: off
- **HARD**: fast reset to 0V

### OUTPUT switch
- **DC**: direct signal, no filtering
- **FILTERS**: low end (<240Hz) stays centered; highs get delayed/side processed

### TARGET ORDER
How slider targets are selected:
- **SEQ**: by number of active thresholds
- **TIED**: by most recently crossed threshold

### HALT IF TARG=0
If a target slider is at 0, that segment can stop moving, producing square/held sections.

### TRGT MOD mode
- **SYM**: full-wave rectified modulation, symmetrical
- **ASYM**: straight modulation, asymmetrical

---

## Sliders and spring toggle

### Slider contexts
The 8 sliders serve 3 roles:

#### 1) THLDs mode (default)
Sets the **8 threshold voltages** where folds occur.

#### 2) TRGTs mode (hold spring toggle left)
Sets the **8 target voltages** for the target sequencer.

#### 3) MACRO SETUP (hold spring toggle right for ~1 second)
Configures internal modulation.

---

## Macro system
Skorpion has an internal **macro envelope** controlling internal LFO/envelope modulation.

### Spring toggle behavior
- **Tap right**: enable/disable Macro Envelope
- **Hold right**: enter Macro Setup while held
- **Hold left**: edit TRGT sliders

### Macro Env LED
- **Red**: gate on
- **Blue**: envelope level

### Macro Setup sliders
1. **Macro Env Attack**: 50ms–600s  
2. **Macro Env Release**: 500ms–600s  
3. **THLD LFO Amount**
4. **THLD LFO Rate**: 0.0016Hz–6Hz
5. **FOLD normal modulation**
6. **SLOPE normal modulation**
7. **SHIFT normal modulation**
8. **SHAPE normal modulation**

For sliders 5–8:
- quick **top→bottom** gesture = **LFO mode**
- quick **bottom→top** gesture = **ENV mode**

Behavior:
- **LFO**: 0.0016Hz–6Hz, unipolar, amplitude controlled by Macro Env
- **ENV**: 50ms–600s, gated by Macro Env gate, amplitude not scaled by Macro Env
- Routed internally to the corresponding CV normal input

Notes:
- LFOs reset on each Macro gate-on
- Envelopes attack without resetting on retrigger
- LFO disabled at slider bottom; envelopes cannot be disabled

---

## Practical usage tips

### For classic wavefolder territory
- **EQUALIZE THLDs = ON**
- **TARGET = 5V**
- **SHAPE near noon**
- **SYNC = SOFT or HARD**
- Bring up **FOLD**, then tune brightness with **SLOPE**

### For asymmetrical / vocal / unstable folds
- Modulate **SHIFT**
- Use **TARGET = CLIP**
- Feed external signal into **CLIP**
- Add **SHAPE** from **OUT**, **DIFF**, or **DIR**

### For sequenced/talking timbres
- Set **TARGET** toward **SLIDERs**
- Edit **TRGTs**
- Switch **TARGET ORDER** between **SEQ** and **TIED**
- Try **HALT IF TARG=0**

### For stereo width
- Turn **OUTPUT** past noon into **WIDE**
- Use **FILTERS** mode to keep bass centered
- Tap the **DELAY** output as an extra modulation/audio source

### For self-patching
Good aux outputs to patch back in:
- **DIFF → SHAPE CV** for spiky timbres
- **COUNT → TARGET / SHIFT / SHAPE**
- **±G(DIR) → SHIFT**
- **TRGTs out → anything**
- **ABS(IN) → modulation destination**
- **DELAY → SHAPE** with output in wide region

---

## Controls reference

### Knobs
- **FOLD** — amount of folding
- **SLOPE** — vector core rate
- **SHIFT** — input offset/asymmetry
- **SHAPE** — slope feedback amount
- **OUTPUT** — dry/wet/wide blend
- **TARGET** — destination selection between 5V / CLIP / SLIDERs

### Attenuverters / associated CV controls
- **FOLD CV attenuverter**
- **SLOPE CV attenuverter**
- **SHIFT CV attenuverter**
- **SHAPE CV attenuverter**
- **OUTPUT CV attenuverter**

### Rotary / mini switches
- **EQUALIZE THLDs**: ON / XOR / JACK
- **TARGET ORDER**: SEQ / TIED
- **SHAPE source**: IN / OUT / DELAY / COUNT / DIFF / TRGTs / DAC / DIR
- **SHAPE symmetry**: SYM / asym
- **TRGT MOD**: SYM / ASYM
- **HALT IF TARG=0**
- **SYNC**: SOFT / X / HARD
- **OUTPUT**: DC / FILTERS

### Sliders
- **8 THLD sliders** in default mode
- **8 TRGT sliders** when holding spring toggle left
- **Macro setup sliders** when holding spring toggle right

### Spring toggle
- center: thresholds
- hold left: targets
- tap right: macro env on/off
- hold right: macro setup

---

## Jack reference

## Inputs
> Manual states **IN nominal range is ±5V**. Other CV/gate inputs are supported; explicit ranges are only given where stated in the manual. When not explicitly specified, patch typical Eurorack CV/audio.  
> Input impedances: **IN 100kΩ**, **1V/OCT 3MΩ**, **TRGT MOD 20kΩ**, all other CV/gate inputs **220kΩ**.

| Jack | Type | Range / notes |
|---|---|---|
| **IN** | Audio/CV input | **±5V nominal** |
| **CLIP** | Audio/CV input | Range not specified; overrides normal from IN for clip/target overlay |
| **1V/OCT** | CV input | Range not specified |
| **FOLD** | CV input | Range not specified; affects fold amount |
| **SLOPE** | CV input | Range not specified |
| **SHIFT** | CV input | Range not specified |
| **SHAPE** | CV input | Range not specified |
| **TARGET** | CV input | Range not specified |
| **OUTPUT** | CV input | Range not specified; controls dry/wet/wide |
| **TRGT MOD** | CV/audio input | Range not specified; directly modulates TARGET pot output |
| **THLDs/** | CV input | Range not specified; weighted modulation of all thresholds |
| **THLD1** | CV input | Range not specified; direct modulation of threshold 1 |
| **TRGTs** | CV input | Range not specified; modulates all targets together |
| **EQ THLDs** | Gate/CV input | High signal enables/disables equalization depending on switch mode |
| **MACRO ENV** | Gate input | Range not specified; gates macro envelope |
| **HALT** | Gate/CV input | Range not specified; stops vector core motion; audio-rate capable |

---

## Outputs
> Output impedance: **1kΩ**

| Jack | Type | Voltage range / notes |
|---|---|---|
| **OUT L** | Audio output | Range not specified |
| **OUT R** | Audio output | Range not specified |
| **ABS(IN)** | CV/audio output | Full-wave rectified IN; range not specified |
| **G(IN>0)** | Gate output | **0V / +5V** |
| **TRGTs** | CV/audio output | Target sequencer output; range not specified |
| **DIFF** | CV/audio output | Difference between target and vector core; range not specified |
| **±G(DIR)** | Bipolar gate output | **-5V / +5V** |
| **COUNT/** | Staircase CV output | **0V to 4V**, +0.5V per active threshold |
| **DAC** | Weighted staircase CV output | **0V to 4V** full scale |
| **DELAY** | Audio/CV output | Delayed waveform from WIDE section; range not specified |

---

## Output section behavior
### OUTPUT knob
- **Below 12 o’clock**: dry→wet blend
- **Above 12 o’clock**: wet→widened stereo

### DELAY output behavior
Only active when OUTPUT is in the wide region:
- below 12 o’clock: no delay out
- 12:00 to 12:30: fades in
- to ~3:00: delay time increases
- beyond ~3:00: delay time plus slow modulation depth/rate increase

Delay specs:
- fade-in region: **80µs to 1.8ms**
- up to modulation onset: **8.2ms**
- max: **14.4ms ±3ms** at ~2Hz modulation

---

## Threshold/CV behavior summary
### THLDs/
Weighted across all 8 thresholds:
- THLD1 gets CV ÷ 2^7
- THLD2 gets CV ÷ 2^6
- ...
- THLD8 gets CV ÷ 1

### COUNT vs DAC
- **COUNT/**: simple staircase, each active threshold adds **0.5V**
- **DAC**: binary-weighted version of threshold activity, **0–4V**

DAC bit weights:
- THLD1 = 1/256 full scale
- THLD2 = 1/128
- THLD3 = 1/64
- THLD4 = 1/32
- THLD5 = 1/16
- THLD6 = 1/8
- THLD7 = 1/4
- THLD8 = 1/2

---

## Helpful reminders
- If slider LEDs don’t respond as expected, check **EQUALIZE THLDs**
- **SHIFT at noon** is recommended when using **HALT**
- **MACRO ENV** is always **OFF on power-up**
- Settings auto-save after **1 minute** of inactivity
- Audio path is **analog except delay**
- **All CVs support audio-rate modulation** for threshold-related processing

---

## Specs
- **Width:** 20HP
- **Depth:** 38mm
- **Power:** +200mA / -160mA
- **Mid/Side crossover:** 240Hz
- **Max slew rate:** 0.4V/µs
- **Internal LFOs:** 0.0016Hz–6Hz
- **Envelope times:** 50ms–600s

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)