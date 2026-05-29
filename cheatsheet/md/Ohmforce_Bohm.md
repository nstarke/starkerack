# Ohmforce — Bohm

- [Manual PDF](../../manuals/Bohm documentation.pdf)

---

[Manual PDF](https://ohmforce.com/wp-content/uploads/2025/03/Bohm-Manual.pdf)

# Ohmforce Bohm Cheat Sheet

## What it is
**Bohm** is a **stereo dual-voice kick system** for Eurorack:
- **Bohm** = main kick voice
- **Groove expander** = secondary kick / rumble / tops voice
- **Performer expander** = stereo input, ducking, performance FX

## Quick start
1. **Trigger `HIT`** to fire the main kick.
2. Pick a **model** with the **FUNCTION** encoder.
3. Shape the kick with:
   - `LENGTH` = decay/duration
   - `SUSTAIN` = body/level
   - `ATTACK` = punch
   - `PITCH` = base pitch
   - `CURVE` = 808-ish CCW → 909-ish CW pitch sweep
   - `TRS DECAY` = click length
   - `TRS TONE` = click brightness
   - `COLOR` = oscillator/timbre behavior
   - `FX` = post-effect amount
4. If installed, clock **Groove** from `CLOCK` for rumble/taps.
5. If installed, use **Performer** to duck/process external stereo audio.

---

# Core workflow

## 1) Select a model
- Turn **FUNCTION** to browse kick models.
- Press **FUNCTION** to enter model variations/menu.
- In **Studio mode**, changes are immediate.

## 2) Main kick behavior
- `HIT` works as **trigger or gate**
  - **Trigger** = normal kick hit
  - **Gate held high** = sustain while gate is high, decay when released
- `PITCH` spans roughly **C1 (32.7 Hz) to C2 (65.4 Hz)**
- `CURVE`
  - **CCW** = faster drop to base pitch, more 808-like
  - **CW** = slower sweep, more 909-like

## 3) Groove expander behavior
- `CLOCK` triggers Groove voice independently of `HIT`
- Best use: feed it a regular clock, often **16th notes**
- `2 / 3 / 4` shape tap/envelope levels after each Bohm hit
- `LENGTH` and `PITCH` are **relative to Bohm**
  - center = same as Bohm
  - left = lower/shorter
  - right = higher/longer
- `COLOR` blends sound generators:
  - repetition
  - kick reverb
  - noise
  - grit + sub
- `TAPS` output can emit Groove envelope, or other selectable envelopes in settings

## 4) Performer expander behavior
- Stereo `IN` is ducked on every `HIT`
- `DUCK` controls how much input ducks
- `VOL` balances Bohm/Groove against the external input
- `ON/OFF` toggles or gates the Performer FX section
- FX can process:
  - `ALL`
  - `KICK`
  - `INPUT`

---

# Best-use tips

## For classic techno kick
- Start with **FM-2X**, **HZ-1**, **VX-T**, or **WT-4**
- Set:
  - medium `LENGTH`
  - medium/high `ATTACK`
  - low-mid `PITCH`
  - `CURVE` slightly CW for 909-ish snap
  - short `TRS DECAY`
  - brighter `TRS TONE`

## For 808-style long kick / bass
- Lower `PITCH`
- Increase `LENGTH`
- `CURVE` more CCW
- Raise `SUSTAIN`
- Try **BASS** FX variation on supported models

## For pitch tracking / basslines
- Set:
  - `PITCH` knob fully CCW
  - `PITCH` attenuverter fully CW
  - system `PITCH CV` mode to proper 1V/oct window: `0..1V`, `1..2V`, or `2..3V`
- Use a **1V/oct** sequencer
- Use enough `LENGTH`, or a gate into `HIT`

## For Groove rumbles
- Patch steady clock into `CLOCK`
- Raise Groove `VOL`
- Use `COLOR` toward repetition/reverb area
- Use `2/3/4` to build movement
- Groove `LENGTH` only affects repetition generator, mainly from about **3 o’clock to full CW**

## For sidechain/performance use
- Patch stereo music into Performer `IN`
- Use `DUCK` for pumping
- Set Performer FX to `DJ FILTER`, `BEAT ROLL`, or `SLIP ROLL`
- Use synced FX switching if you want clean transitions on next `HIT`

---

# Models at a glance

## FM-2X
- 2-operator FM kick
- Great for punchy synthesized kicks
- `ATTACK` strongly affects FM bite
- `TRS TONE` changes modulator waveform character

## HZ-1
- Wavetable kick + transient synth
- Good all-rounder
- `COLOR` adds transient distortion/motion

## OLP4
- 4-operator FM / OPL-style
- Most experimental
- `COLOR` inactive
- `TRS TONE` adds FM feedback/noisiness
- Groove supported in newer firmware

## PM-K1
- Physical-model acoustic bass drum
- Very different control mapping
- Groove **not supported**
- Good for acoustic/organic kick textures

## PX3
- Wavetable + layered object-hit samples
- Harder / more experimental character

## SP-6
- Digital-sounding wavetable + synthesized transient layers

## VX-T
- Wavetable + FM transient synth
- Nice for click/toc/hihat-flavored transients

## WT-4
- Analog-ish wavetable + synthesized transient layers

## XT-88
- User wavetable + user sample model
- Loads from microSD:
  - `wavetables/`
  - `samples/`

---

# Variations / menu essentials

## Bohm common variations
### FX type
- `TUBE`
- `BASS`
- `SOFT`
- `HARD`
- `WAVEFOLD`
- `BITCRUSH` (some models)
- `DECIM` (some models)

### Stereo
- `STEREO` = width 0% to 100%

## Groove variations
### FX type
- `LP`
- `HP`
- `BP`
- `DIST`

### Stereo
- `STEREO` = width 0% to 100%

## Performer variations
- `DUCK TIME` = duck release time
- `DUCK SMTH` = duck curve smoothing
- `DUCK BS` = band-split frequency for more transparent ducking
- FX types:
  - `DJ FILTER`
  - `HP`
  - `LP`
  - `BEAT ROLL`
  - `SLIP ROLL`
- `DJ RESO` = filter resonance
- `CHN` = `ALL`, `KICK`, `INPUT`

---

# Running modes

## Studio mode
- Default on power-up
- Immediate editing
- Best for sound design and browsing models

## Live Song mode
- Programs act as **step sequences of kick snapshots**
- Trigger `FUNCTION` to advance to next step
- New step becomes active on next `HIT`

## Live Jam mode
- Programs act as **banks of kick snapshots**
- Turn **FUNCTION** to choose next kick
- Press **FUNCTION** to cue it
- It becomes active on next `HIT`

## Snapshot basics
- Save a snapshot by holding **HIT** and pressing **FUNCTION**
- Snapshots store:
  - model variations
  - knob positions
- `LOAD`
  - loads variations only
- `LOAD W/ POTS`
  - loads variations + pot positions

---

# System settings worth knowing
- **PITCH CV**: select 1V/oct mapping window (`0..1V`, `1..2V`, `2..3V`)
- **ATTVERT 2**: map `SUSTAIN` attenuverter to `SUSTAIN CV` or `VELOCITY CV`
- **FUNC RAND**: randomize Bohm+Groove or all including Performer
- **PERF FX**: FX switch `INSTANT` or `SYNCED`
- **PERF ON/OFF**: `TRIG` or `GATE`
- **GRV ENV**: `FALL` or `SUSTAIN`
- **TAPS OUT**: `GROOVE`, `I BOHM`, `PERF`, `BOHM`
- **PANNING**: hard-pan Bohm/Groove/Performer left, center, or right
- **POST EQ**: output EQ for Bohm/Groove
- **IN VOL**: attenuate Performer input
- **PERF VOL**: Performer slider controls `B+G` or `BOHM`
- **PERF MAX**: max Performer-controlled output level
- **LOCK MODEL**: prevent accidental model changes in Studio mode
- **BACKUP / RESTORE** via SD card
- **FACTORY RESET**

---

# I/O and control reference

## Global technical CV/audio specs
- **CV input range:** **±5V**  
- **0..5V compatible:** yes
- **Knob/CV resolution:** **16-bit**
- **Audio output:** stereo
- **Sample rate:** **48 kHz**
- **Latency:** **0.33 ms**

---

## Bohm main module

### Jacks
| Jack | Type | Range | Function |
|---|---|---:|---|
| `LENGTH CV` | CV in | **±5V** | Modulates kick duration |
| `ATTACK CV` | CV in | **±5V** | Modulates attack amount |
| `SUSTAIN CV` | CV in | **±5V** | Modulates sustain/volume |
| `HIT` | gate/trigger in | **0..5V compatible** / CV input spec **±5V** | Triggers or sustains the kick |
| `TRS DECAY CV` | CV in | **±5V** | Modulates transient decay |
| `TONE CV` | CV in | **±5V** | Modulates transient tone |
| `FUNCTION CV` | CV in | **±5V** | In Studio: randomize current variations; other contexts depend on mode |
| `VELOCITY CV` | CV in | **±5V** | Modulates kick velocity/level |
| `PITCH CV` | CV in | **±5V** | Pitch modulation; can be configured for 1V/oct over selected 1V window |
| `CURVE CV` | CV in | **±5V** | Modulates pitch curve |
| `COLOR CV` | CV in | **±5V** | Modulates timbre/wavetable behavior |
| `FX CV` | CV in | **±5V** | Modulates FX amount |
| `OUT L/R` | stereo audio out | Eurorack audio | Main stereo output |

### Knobs / controls
| Control | Type | Function |
|---|---|---|
| `LENGTH` | knob | Kick duration |
| `SUSTAIN` | knob | Kick body/level |
| `ATTACK` | knob | Attack/punch |
| `PITCH` | knob | Base kick pitch |
| `CURVE` | knob | Pitch drop shape: 808-like CCW → 909-like CW |
| `TRS DECAY` | knob | Click/transient duration |
| `COLOR` | knob | Timbre / wavetable behavior |
| `FX` | knob | Kick post-effect amount |
| `TRS TONE` | knob | Click brightness |
| `FUNCTION` | push encoder | Model select, menu navigation, variation editing |
| `HIT` | button | Manual trigger; can also be held |
| `microSD slot` | storage | Firmware, models, user wavetables/samples |

### Attenuverters / trims
| Control | Type | Function |
|---|---|---|
| `LENGTH` attenuverter | trim | CV depth/polarity for LENGTH CV |
| `ATTACK` attenuverter | trim | CV depth/polarity for ATTACK CV |
| `SUSTAIN` attenuverter | trim | CV depth/polarity for SUSTAIN CV or VELOCITY CV depending on setting |
| `PITCH` attenuverter | trim | CV depth/polarity for PITCH CV |
| `CURVE` attenuverter | trim | CV depth/polarity for CURVE CV |
| `COLOR` attenuverter | trim | CV depth/polarity for COLOR CV |

---

## Groove expander

### Jacks
| Jack | Type | Range | Function |
|---|---|---:|---|
| `FX CV` | CV in | **±5V** | Modulates Groove FX |
| `CLOCK` | trigger in | **0..5V compatible** / CV input spec **±5V** | Triggers Groove voice/taps |
| `COLOR CV` | CV in | **±5V** | Modulates sound source blend |
| `VOL CV` | CV in | **±5V** | Modulates Groove volume |
| `LENGTH CV` | CV in | **±5V** | Modulates Groove duration (repetition source only where applicable) |
| `PITCH CV` | CV in | **±5V** | Modulates Groove pitch relative to Bohm |
| `TAPS CV` | CV in | **±5V** | Shapes tap envelope |
| `TAPS CV OUT` | CV out | not explicitly stated; Eurorack CV | Outputs selected envelope (`GROOVE`, `I BOHM`, `PERF`, or `BOHM`) |

### Knobs / sliders
| Control | Type | Function |
|---|---|---|
| `2` | knob | 2nd tap/envelope level |
| `3` | knob | 3rd tap/envelope level |
| `4` | knob | 4th tap/envelope level |
| `LENGTH` | knob | Groove length relative to Bohm |
| `PITCH` | knob | Groove pitch relative to Bohm |
| `FX` | knob | Groove post-effect amount |
| `COLOR` | knob | Selects/blends sound generators |
| `VOL` | slider | Groove output level |

### Attenuverters / trims
| Control | Type | Function |
|---|---|---|
| `FX` attenuverter | trim | CV depth/polarity for FX CV |
| `COLOR` attenuverter | trim | CV depth/polarity for COLOR CV |

---

## Performer expander

### Jacks
| Jack | Type | Range | Function |
|---|---|---:|---|
| `DUCK CV` | CV in | **±5V** | Modulates ducking amount |
| `FX CV` | CV in | **±5V** | Modulates Performer FX parameter |
| `ON/OFF CV` | gate/trigger in | **0..5V compatible** / CV input spec **±5V** | Toggles or gates FX depending on system setting |
| `IN L/R` | stereo audio in | Eurorack audio | External stereo input |
| `VOL CV` | CV in | **±5V** | Controls Bohm/Groove or Bohm-only level depending on setting |

### Knobs / buttons / sliders
| Control | Type | Function |
|---|---|---|
| `DUCK` | knob | Amount of ducking on external input |
| `FX` | knob | Performance FX parameter |
| `ON/OFF` | button | Activate/deactivate or gate the FX section |
| `VOL` | slider | Level of Bohm/Groove before mix/effect, depending on settings |

---

# Installation / power / size
## Width
- **Bohm:** 18HP
- **Groove:** 10HP
- **Performer:** 8HP
- **Full set:** 36HP

## Depth
- **Bohm:** 28 mm
- **Groove:** 26 mm
- **Performer:** 26 mm

## Power
- **Bohm:** +12V 130 mA / -12V 10 mA
- **Groove:** +12V 20 mA / -12V 10 mA
- **Performer:** +12V 10 mA / -12V 5 mA
- **+5V:** unused

---

# microSD / firmware / user files
- microSD / SDHC Class 10+
- Up to **32 GB**
- **FAT32 with MBR only**
- Used for:
  - firmware updates
  - model files
  - XT-88 user wavetables and samples
  - backup/restore

## XT-88 user file formats
### Wavetables
- `.wav`
- Serum/Serum 2 compatible, assumed **2048-cycle**
- or **mono 32-bit float**, assumed **1024-cycle**
- max **16 wavetables** or until **1.4 MB** memory full

### Samples
- `.wav`
- mono or stereo
- 16-bit / 24-bit integer or 32-bit float
- **48 kHz**
- max **256 samples** or until **14 MB** memory full

---

# Practical patch recipes

## Simple standalone kick
- Trigger sequencer → `HIT`
- Bohm `OUT` → mixer
- Start with FM-2X
- Tune with `PITCH`, `CURVE`, `LENGTH`, `ATTACK`

## Techno rumble
- Main trigger → `HIT`
- 16th clock → Groove `CLOCK`
- Groove `VOL` up
- Groove `COLOR` toward repetitions/reverb
- Adjust `2/3/4` and Groove `FX`

## Sidechain external synths
- External stereo synth → Performer `IN`
- Kick trigger → `HIT`
- Increase Performer `DUCK`
- Output from Bohm `OUT`

## Envelope utility patch
- Use Groove `TAPS OUT` to modulate another VCA/filter
- In settings, choose source:
  - Groove envelope
  - inverted Bohm envelope
  - Bohm envelope
  - Performer duck envelope

---

# Gotchas
- **Groove does nothing without `CLOCK`**
- **Groove `LENGTH` only affects repetition source**
- **PM-K1 does not support Groove**
- For pitch tracking, ensure sequencer is **1V/oct**
- The module can preload next live snapshot, so ultra-fast step changes may be limited by model load time
- If you add Groove/Performer after purchase, **calibration is recommended**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)