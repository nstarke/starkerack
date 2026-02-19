# Instruo — Arbhar

- [Manual PDF](../../manuals/Arbhar-Manual-Firmware-2.0-A5.pdf)

---

**[Instruō Arbhar Granular Audio Processor – User Manual (Firmware 2.0)](https://www.instruomodular.com/wp-content/uploads/2023/01/arbhar_v2_user_manual.pdf)**

---

# Instruō arbhar Granular Audio Processor  
**Quick Reference & Cheat Sheet (Firmware 2.0)**

---

## Basic Usage Overview

- **Record Audio:**  
  Press the **Capture** button to record audio into the selected layer. Each layer holds up to 10s audio.
- **Granular Playback:**  
  Audio is broken into "grains" which can be scattered, reversed, repitched, panned, and layered for textural manipulation.
- **Layers:**  
  6 layers (Alpha, Beta, Gamma, Delta, Epsilon, Zeta), each with a dedicated buffer. Omega mode links all layers for simultaneous access.
- **Granular Modes:**  
  - **Scan Mode:** Use the **Scan** knob to "scrub"/freeze through audio.
  - **Follow Mode:** **Scan** knob controls speed/direction through audio (playback independent from pitch).

---

## Panel Controls Reference

### Knobs

| Name                 | Function                                                                          | CV Input (Range)              |
|----------------------|-----------------------------------------------------------------------------------|-------------------------------|
| Input Level          | Sets input/preamp gain, includes analog saturation                                | No CV                         |
| Output Level         | Sets output level                                                                 | No CV                         |
| Dry/Wet              | Crossfades dry vs granular audio                                                  | Yes (±5V summed, 10V total)   |
| Intensity            | Number/density/rate of grains                                                     | Yes (±5V summed, 10V total)   |
| Grain Window         | Grain envelope (Square ↔ Gaussian ↔ Saw)                                          | Yes (±5V summed, 10V total)   |
| Grain Direction      | Probability (FWD↔REV) playback                                                    | Yes (±5V summed, 10V total)   |
| Length               | Grain duration (~4ms–3s, exp distribution)                                        | Yes (±5V summed, 10V total)   |
| Scan                 | Grain position in buffer                                                          | Yes (±5V summed, 10V total)   |
| Spray                | Range of randomization from scan position                                         | Yes (±5V summed, 10V total)   |
| Pitch                | Grain pitch                                                                       | Yes (1V/Oct; ±5V)             |
| Pitch Deviation      | Random/quantized per-grain pitch deviation (semitones)                            | Yes (±5V summed, 10V total)   |
| Sensitivity (Sense)  | Sensitivity of onset detection OR input 2 level (stereo mode)                     | No CV                         |
| Hold                 | Debounce/Min-record or min time between onsets/gates (5ms–10s)                    | Yes (via Mod CV input)        |
| Dub                  | Sound-on-Sound: Blend level of prior layer value when overdubbing                 | Yes (±5V summed, 10V total)   |
| Layer                | Select the active layer (alpha–zeta/omega)                                        | Yes (±5V summed, 10V total)   |

### Buttons

| Name     | Function                                                                  |
|----------|--------------------------------------------------------------------------|
| Capture  | Start/stop record (mode settable; see capture modes below)               |
| Shift    | Shift for alt/multi functions                                             |
| Strike   | Trigger a grain from Strike Granular Engine / accent / undo / erase etc.  |

### Switches/Indicators

| Name                     | Function                                                     |
|--------------------------|-------------------------------------------------------------|
| Layer Indicators         | Show selected layer; omega = all layers linked              |
| Granular Stream Display  | Shows layer, scan, grain activities, record/play state      |
| Grain Direction/LEDs     | Direction of active grains, indicates mode                  |
| Onset Indicator/LED      | Status of onset detection                                  |

---

## Inputs & Outputs

### Audio I/O

| Jack                | Function                                                                  |
|---------------------|--------------------------------------------------------------------------|
| Input (In)          | Primary audio in (AC coupled); defaults to mic if unpatched              |
| Onset Input         | Audio in for onset detection, also becomes Right channel in Stereo mode   |
| Outputs 1 & 2       | Main outputs (coin toss/mix grains; stereo/mono operation)               |

### Pulse & CV I/O

| Jack               | Function                                                      | CV Range               |
|--------------------|--------------------------------------------------------------|------------------------|
| Capture Pulse In   | Triggers/holds recording (mode selectable: Momentary/Latch/Retrigger) | Trigger/gate |
| Strike Input       | Pulse in, triggers single grain (Strike Engine)               | Trigger/gate           |
| 1V/Oct Input       | Pitch CV                                                      | ±5V (1V/Oct)           |
| Intensity CV       | Controls Intensity knob                                       | ±5V (10V total span)   |
| Length CV          | Controls grain Length                                         | ±5V (10V total span)   |
| Scan CV            | Controls Scan position (or speed in Follow Mode)              | ±5V (10V total span)   |
| Spray CV           | Controls grain Spray                                          | ±5V (10V total span)   |
| Layer CV           | Voltage control over which layer(s) are active                | ±5V (10V total span)   |
| Grain Dir. CV      | Per-grain direction probability                               | ±5V (10V total span)   |
| Grain Window CV    | Envelope shape modulation                                     | ±5V (10V total span)   |
| Pitch Deviation CV | Per-grain pitch deviation (random or quant)                   | ±5V (10V total span)   |
| Dub CV             | Overdub Blend (0=replacement, 50%=mix, 100%=sum)              | ±5V (10V total span)   |
| Dry/Wet CV         | Modulate dry/wet balance                                      | ±5V (10V total span)   |
| Mod CV (Expansion) | Assignable: Hold, Reverb, Delay, Panning (preset.txt settable)| ±5V (10V total span)   |
| Pulse Output       | Trigger/gate based on onset/grain/strike/loop (mode settable) | +5V, 10ms trig/gate    |
| USB Port           | Load/Save audio, update firmware, access scenes/layers/presets| USB flash drive        |

#### Panel Inputs/Outputs Complete List

- **Audio Input (In)**
- **Onset Input (2nd input / right in stereo)**
- **Capture Pulse Input**
- **Strike Input**
- **1V/Oct Input**
- **Intensity CV**
- **Length CV**
- **Scan CV**
- **Spray CV (Expansion)**
- **Layer CV (Expansion)**
- **Grain Window CV (Expansion)**
- **Pitch Deviation CV (Expansion)**
- **Dub CV (Expansion)**
- **Dry/Wet CV (Expansion)**
- **Mod CV (Expansion)**
- **Pulse Output**
- **Audio Output 1/2**

---

## Special Modes & Operations

### Input & Output Modes

- **Mono Input:** Default. Input = mono, Onset = mono onset.
- **Stereo Input:** Input = L, Onset = R, Sensitivity knob = R level.
- **Mono Output:** Output 1 = mono mix; Output 2 is normalled unless patched.
- **Stereo Output:** Patch both outs for stereo; phase switch can change 2nd out polarity.

### Recording Modes

- **Capture Modes:**  
  - *Momentary (default):* Records as long as pulse/Capture button held
  - *Latching:* Start/stop with triggers
  - *Retrigger:* (preset only) Each retrigger restarts record head
- **Accumulative (Optional):** Multiple passes add to one buffer position, rather than reset each time (toggle with Capture+Shift).

### Synthesis Controls

- **Intensity Knob:** More grains (center) = denser, less (extreme) disables engine.
- **Strike Engine:** Fire grains one at a time (for accents, rhythm) via Strike input or button.
- **Length Knob:** Grain duration (~4ms–3s).
- **Scan Knob:** Position in audio buffer (or speed in Follow Mode).
- **Spray Knob:** Adds random offset to scan position (moving/randomness through audio).
- **Pitch/Pitch Dev.:** Main pitch and random or quantized deviation per grain.
- **Grain Window & Direction:** Envelope per grain and probability of forward/reverse playback.

### File System & Scenes

- **USB Flash Drive:** Used for audio, scenes, presets, firmware.  
    - `/arbhar_library/` for layers (36 x 10s files)
    - `/arbhar_scenes/` for full scenes (preset.txt + up to 6 files)
    - `_updater` for firmware
- **Clone, Load, Save:** Use Shift+Capture+Strike to access and navigate menu (layer knob for slot), Shift to audition or confirm.
- **Factory Reset:** Hold Shift+Capture, press Strike 7x rapidly.

---

## CV Expansion & Voltage Ranges

- **ALL CV Inputs:** Bipolar ±5V for full knob travel; summed with knob position.  
  (i.e., -5V = min, 0V = knob only, +5V = max; total range from -5V to +5V = 10V travel).
- **1V/Oct Input:** Proper 1V/oct response, ±5V range.
- **Pulse Output:** +5V triggers/gates (10ms or as set by mode).

---

## Quick Reference: Front Panel (Numbers from Manual)

| # | Name                       | Function                          |
|---|----------------------------|-----------------------------------|
| 1 | Condenser Microphone       | Onboard mic input                 |
| 2 | Input                      | Audio in (AC)                     |
| 3 | Input Level                | Preamplifier / gain               |
| 4 | Input Indicator            | Input presence/level LED          |
| 5 | Dry/Wet                    | Mix knob                          |
| 6 | Output Level               | Output gain                       |
| 7/8 | Outputs 1/2              | Audio outs (mono/stereo modes)    |
| 9 | Capture Button             | Start/stop recording              |
| 10 | Capture Pulse Input       | Pulse/gate record control         |
| 11 | Shift Button              | Alt/multi functions               |
| 12 | Layer                     | Selects layer (alpha–zeta/omega)  |
| 13 | Layer Indicators          | Layer identification              |
| 14 | Granular Stream Display   | Layer/scan/grain/rec/play LED bar |
| 15 | Intensity                 | Granulation density knob          |
| 16 | Intensity CV Input        | Grain density CV                  |
| 17 | Strike Button             | Accent grain/undo/erase           |
| 18 | Strike Input              | Trigger grain                     |
| 19 | Grain Window              | Envelope shape                    |
| 20 | Grain Direction           | FWD/REV probability               |
| 21 | Grain Dir. Indicators     | FWD/REV grain LED                 |
| 22 | Length                    | Grain duration                    |
| 23 | Length CV                 | Duration CV                       |
| 24 | Scan                      | Position (or speed in Follow)     |
| 25 | Scan CV                   | Position CV                       |
| 26 | Spray                     | Random offset                     |
| 27 | Pulse Output              | Grain/onset/loop trigger/gate out |
| 28 | Pitch                     | Grain pitch                       |
| 29 | 1V/Oct                    | Pitch CV (1V/oct)                 |
| 30 | Pitch Deviation           | Random/quant deviation            |
| 31 | Onset Input               | Audio onset detection input        |
| 32 | Onset Indicator           | Onset detection armed LED         |
| 33 | Sensitivity (Sense)       | Onset sens. or input 2 level      |
| 34 | Hold                      | Min. time/gate length/loop time   |
| 35 | Dub                       | Overdub/replacement ratio         |

---

## Additional Tips

- **Shift + [Knob/button]:** Many alternate functions/modes (see manual for combinations).
- **Wavetable Mode:** Turn Length to full CCW—acts as a wavetable oscillator from the audio.
- **Accumulative Recording:** Capture + Shift toggles accumulative mode for overdub collaging.
- **Track & Hold:** Shift (dbl tap+hold), then adjust parameters, they only activate on release.

---

### [**Full Manual PDF (Instruō official)**](https://www.instruomodular.com/wp-content/uploads/2023/01/arbhar_v2_user_manual.pdf)

---
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
