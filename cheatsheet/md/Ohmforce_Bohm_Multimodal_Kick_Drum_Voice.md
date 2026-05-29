# Ohmforce — Bohm Multimodal Kick Drum Voice

- [Manual PDF](../../manuals/Bohm_Eurorack_Manual_Compiled.pdf)

---

[Manual PDF / Source](https://bohm-eurorack-manual.readthedocs.io/en/latest/index.html)

# Bohm Eurorack Cheat Sheet

## What it is
**Bohm** is a **stereo dual-voice Eurorack kick module system** with optional expanders:

- **Bohm** main module: kick synthesis engine
- **Groove** expander: secondary kick / techno rumble / layered percussion
- **Performer** expander: DJ-style effects, ducking, stereo processing

## Size / Installation
- **Bohm:** 18HP
- **Groove:** 10HP
- **Performer:** 8HP

Install with power off, ribbon cable aligned correctly (**red stripe orientation matters**), then secure without overtightening.

---

## Quick Start
1. Install and power up the module.
2. Select a **kick model**.
3. Trigger the sound with **HIT**.
4. Shape the drum using:
   - **VELOCITY**
   - **LENGTH**
   - **SUSTAIN**
   - **ATTACK**
   - **PITCH**
   - **CURVE**
   - **TRS DECAY**
   - **COLOR**
   - **FX**
   - **TRS TONE**
5. Use:
   - **Studio Mode** for immediate sound design
   - **Live Song Mode** for sequenced kick changes
   - **Jam Mode** for improvised performance

---

## Core Sound Controls
These controls change behavior depending on the selected **model**.

- **HIT** — triggers the kick
- **VELOCITY** — controls impact / hit strength
- **LENGTH** — overall hit duration
- **SUSTAIN** — tail/body sustain
- **ATTACK** — transient sharpness
- **PITCH** — base drum pitch  
  - documented range is roughly **C1 to C2**
- **CURVE** — pitch envelope/response shape, inspired by **808/909** kick behavior
- **TRS DECAY** — decay time for transient/resonant section
- **COLOR** — tonal character / timbre shaping
- **FX** — effect amount/character
- **TRS TONE** — tone shaping for transient/resonant section

> Because Bohm uses different internal DSP “models,” the exact meaning and feel of each control can vary by model.

---

## Running Modes
- **Studio Mode**  
  Immediate parameter changes; best for production and patch building.

- **Live Song Mode**  
  Sequenced kick changes; optimized for live performance.

- **Jam Mode**  
  Improvisation-focused mode for spontaneous tweaking.

---

## Expanders

### Groove
Adds:
- secondary kick voice
- techno rumbles
- layered percussion

### Performer
Adds:
- DJ-style effects
- ducking
- stereo processing

---

## Calibration
Use calibration if:
- knobs feel inaccurate
- CV response seems off
- pitch tracking seems wrong

Calibration may include:
- knob sweeps
- CV checks
- optional **3V pitch calibration**
- separate calibration for **Groove** and **Performer**

---

## Firmware Update
Uses the included **microSD card**.

### Update steps
1. Download firmware package
2. Copy contents to the **SD card root**
3. Reinsert the SD card
4. Power on the Eurorack system

- Update time: about **20 seconds**

---

## Storage / Technical Notes
- **microSD / SDHC** supported up to **32GB**
- Must be **FAT32 with MBR**
- Stores:
  - firmware
  - kick models
  - samples
  - user wavetables
  - system settings
  - up to **32 programs**

---

# I/O and Control Reference

## Audio / CV Inputs
**Not explicitly listed in the provided manual extract.**  
The extract mentions calibration of **CV inputs**, so voltage-controlled inputs exist, but **jack names and voltage ranges are not provided** in the attached text.

### Known from the extract
- **CV inputs:** present
- **Pitch calibration:** optional **3V** pitch calibration mentioned

### Voltage ranges
- **CV input ranges:** **not specified in provided manual text**
- **Pitch CV reference:** **3V calibration point** mentioned, but this is **not a full operating range specification**

---

## Audio / CV Outputs
**Not explicitly listed in the provided manual extract.**  
The module is described as **stereo**, so stereo outputs are implied, but exact jack names and output voltage levels are **not provided** in the attached text.

### Voltage ranges
- **Audio output levels:** not specified
- **CV output ranges:** not specified

---

## Knobs / Buttons / Sliders / Toggles
The attached manual text explicitly names these front-panel controls:

- **HIT**
- **VELOCITY**
- **LENGTH**
- **SUSTAIN**
- **ATTACK**
- **PITCH**
- **CURVE**
- **TRS DECAY**
- **COLOR**
- **FX**
- **TRS TONE**

### Control type note
The extract does **not** specify whether each item is a:
- knob
- button
- slider
- toggle

However:
- **HIT** is most likely a trigger/performance control
- the others are likely parameter controls, typically knobs in Eurorack context

Because the source extract does not state panel hardware types explicitly, these should be treated as **named controls, type unspecified**.

---

## Practical Use Tips
- Start in **Studio Mode** to learn how each model responds.
- Treat **PITCH + CURVE** as the main “character” section for classic kick behavior.
- Use **ATTACK** and **TRS TONE** to define click/punch.
- Use **LENGTH**, **SUSTAIN**, and **TRS DECAY** to move from short punchy kicks to long booming tails.
- Use **COLOR** and **FX** last for finishing and performance shaping.
- If your pitch or modulation feels wrong, run **calibration** before troubleshooting the patch.

---

## Missing Details From Provided Extract
The attached text does **not** include a full jack table. Missing specifics include:
- exact input jack names
- exact output jack names
- trigger/gate input specs
- audio output levels
- CV input ranges
- whether controls have dedicated CV attenuators
- exact button/encoder/toggle assignments

If you want, I can also turn this into a **compact performance card** or a **full structured reference table** based strictly on the extracted manual text.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)