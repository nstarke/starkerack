# ADDAC Systems — ADDAC-112 Granular Looper

- [Manual PDF](../../manuals/ADDAC112_Granular_E_0.pdf)

---

Certainly! Here’s a concise **cheat sheet** for the **ADDAC112 VC Looper & Granular Processor** Eurorack module, distilled from the manual you provided.  
*(Images attached above for visual reference, but here’s a written summary.)*

---

# ADDAC112 VC Looper & Granular Processor Cheat Sheet

**Manual PDF:**  
[ADDAC112 User's Guide PDF (source: addacsystem.com)](https://media.addacsystem.com/firmwares/ADDAC112_firmware.zip)  
*(Direct link to firmware, see [addacsystem.com](https://addacsystem.com/en/products/modules/addac100-series/addac112) for updated docs.)*

---

## Module Overview

- **Type:** Stereo Looper, Granular Processor, & Real-time Sample Manipulator
- **Sections:** Looper Engine, Granular Engine, Output Mixer
- **Power:** 240mA @ +12V / 70mA @ -12V / 32HP+13HP / 4.5cm deep

---

## Inputs / Outputs (I/O) Summary

### Audio Inputs
| Jack Label        | Description                   | Signal Level          |
|-------------------|------------------------------|-----------------------|
| IN 1 (Mono/L)     | Mono input (synth or line)   | 10Vpp Synth, 2Vpp Line|
| IN 2 (Mono/R)     | Mono (normalled to IN 1 when unpatched) | 10Vpp Synth, 2Vpp Line|
| STEREO LINE IN    | Stereo, line-level input     | 2Vpp Line             |

### Audio Outputs
| Jack Label        | Description                |
|-------------------|---------------------------|
| Left Output       | Master stereo (L)         |
| Right Output      | Master stereo (R)         |
| Mono Output       | Sum of L+R                |
| INS MONO OUT      | Mixed input: all inputs summed to mono |

### CV & Trigger Inputs *(All CV in: ±5V range typical, 0-10V functional, see notes)*
- **All front panel knob parameters** have dedicated CV inputs
    - (Position, Deviation, Length, etc. – see controls list)
- **Trigger Inputs:**  
    - Playback and recording controls (NEW REC, REC, PLAY, STOP, FORWARD/REVERSE)
    - Clock input (in 'Clocked Mode' via STOP jack)

---

## Panel Controls Reference

### Knobs & Sliders (Per section; each has CV in)
- **Input Stage:**
  - INPUT GAIN
- **Looper:**
  - LOOP VOLUME
  - LOOP SELECT
  - LOOP PITCH
  - OVERDUB DECAY
  - REC PROBABILITY
  - REC DELAY (and DELAY DEVIATION)
- **Granular:**
  - GRAINS ACTIVE
  - POSITION
  - POSITION DEVIATION
  - PLAY LENGTH
  - LENGTH DEVIATION
  - GRAIN LOOP DELAY & DEVIATION
  - GRAIN DIRECTION
  - GRAIN PITCH
  - VOLUME MIN / DEVIATION
  - GRAIN PANNING
  - ATTACK / DECAY (grain envelope)
  - GRAINS VOLUME
  - GRAINS FEEDBACK

- **Output Mixer:**
  - DRY VOLUME
  - LOOP VOLUME
  - GRAINS VOLUME

### Buttons (Looper Control)
- **REC NEW** – Start new loop (variable/fixed length)
- **REC** – Overdub current loop
- **PLAY** – Play/stop/retrigger loop
- **STOP** – Stop playback/recording or quantize triggers in 'Clocked' mode
- **CLEAR** – Clear loop (long press: erase from list)
- **MENU Encoder** – Enter/confirm menu navigation

### Toggles & Switches
- **RETRIG/PAUSE:** Playhead triggers from start or toggles pause.
- **SYNC REC/UNSYNC:** Rec head follows or is independent from playhead.
- **REC MODE:** [STOP / LOOP / OVERDUB] - Determines end of rec behavior.
- **FORWARD/REVERSE:** Loop playback direction.
- **REPEAT MODE:** Grain repeat probability vs. number of repeats.
- **SIZE DIVISION:** [FREE/8/16] for granular quantization.
- **Various Menu Options:** (Quantize, Samplerate, Bit Depth, Pitch Tracking, Clocked Mode, etc.)

---

## OLED Screen

- Shows: Looper state, Levels, Quantization, # Grains, Loop selection, Pitch, Panning, Envelope, etc.
- Info & Settings displayed via MENU

---

## SD Card Handling

- Used for storing/loading Banks (presets/loops)
- Up to 99 presets & 99 loops per bank
- Max 30MB per bank
- **Format:** FAT16 recommended
- **File structure:** `/BANK[n]/WAV/*.wav`
- **Save current bank before power down to keep data!**
- Loops as .WAV files, clean headers/no metadata recommended (use MediaHuman or similar if needed)

---

## Voltage Control Reference

| CV Input            | Function           | Range        |
|---------------------|-------------------|--------------|
| All parameter CV In | Modulates panel   | 0-10V*       |
| Trigger In (REC, PLAY, etc.) | Action   | Gate/Trig: >2V|
| CV Out?             | None (except INS MONO OUT - audio, not CV) |
> \* Typical Eurorack 0-10V. Not officially specified in manual, but common for ADDAC.

---

## Operating Steps (Quickstart)

1. **Audio In/Out:** Patch input, set INPUT GAIN until LED indicates healthy level. Patch output.
2. **Create/Load Bank:** MENU > BANK > NEW/LOAD.
3. **Record Loops:**
    - [NEW REC] to record, press [REC]/[PLAY]/[STOP] to finish.
    - Select via [LOOP SELECT] or CV.
4. **Granular Processing:** Engage grains with GRAINS VOLUME, adjust granular controls.
5. **Save:** MENU > BANK > SAVE to SD before switching off.
6. **Navigate Presets/Loops:** Use [PRESET SELECT]/[LOOP SELECT] knobs or CV.

---

## Expert Features

- **Quantized recording/playback & scales (chromatic, major, etc.)**
- **Menu controls:** Sample rate, bit depth, mono/stereo, overdub origin (play/rec/both), pitch range, etc.
- **Granular randomization/deviation via second knob per parameter**
- **Normalize loop volume:** MENU + [REC]
- **Duplicate loop:** MENU + [NEW REC]
- **Resize loop:** MENU + [CLEAR BUFFER]
- **Firmware update:** via rear USB and Chrome browser DFU tool

---

### For more in-depth reference, see the original manual!  
**Manual download:**  
[ADDAC112 User's Guide PDF](https://media.addacsystem.com/firmwares/ADDAC112_firmware.zip)  
[Official ADDAC112 product page (for updates)](https://addacsystem.com/en/products/modules/addac100-series/addac112)

---

*Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)*