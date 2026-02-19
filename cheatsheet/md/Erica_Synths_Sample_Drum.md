# Erica Synths — Sample Drum

- [Manual PDF](../../manuals/FINAL_sample_drum_instrukcija_A4.pdf)

---

[**Erica Synths Sample Drum Manual (PDF)**](https://www.ericasynths.lv/media/SampleDrum_Manual_1.04.pdf)

---

# Erica Synths Sample Drum Cheat Sheet

## Overview

Dual-channel, performance-focused sample player. Each channel is independently addressable and features:
- Fast sample playback and triggering
- Live and auto/manual slicing
- Extensive CV assignment
- FX and envelopes per channel
- Sample recording and trimming
- Project memory

---

## Front Panel Controls & Features

| Control/Jack   | Description |
|:--------------:|:------------|
| **A/DATA**     | Main data/selection encoder (push to confirm/select) |
| **B, C, D/BACK, E, F** | Context-sensitive encoders (see menus/functions below). D/BACK: also acts as a back/return button. |
| **TRG1/PLAY**  | Manual Trigger button Ch1 (Performance mode only); preview sample |
| **TRG2/SHIFT** | Manual Trigger button Ch2; also SHIFT for accessing secondary functions; preview waveform/sample info |
| **OLED Screen**| Visual feedback, waveforms, menues, scopes |
| **SD Card Slot | For sample/projects management (microSD, must keep directory structure as specified) |
| **CH1/CH2 Toggle** | Select which channel (for sample loading/editing/assign) |

---

### Input/Output Jack Summary

| I/O            | Function | Voltage Range |
|:--------------:|:---------|:--------------|
| **TRIG 1, 2**  | Trigger Inputs (Ch1 & Ch2 sample playback) |  |
| **CV1, CV2, CV3 (x2)** | 3 Assignable CV per Channel: tune/sample/start/end/loop/slice FX/env, etc.<br>**CV3 on CH2 used for sample recording** | Configurable: <br> -5V to +5V<br> -10V to +10V <br> 0V to +5V <br> 0V to +10V <br> 1V/Oct (no depth setting)|
| **OUT 1, 2**   | Individual Channel Audio Outputs | 10V ptp max (settable via menu) |
| **SD**         | MicroSD slot for samples/projects |
| **Power**      | Standard Eurorack header (65mA @ +12V, 2mA @ -12V) |

---

## Top-Level Workflow

### 1. **Loading Samples**
- Prepare mono 16-bit, 48kHz (or lower) WAVs, store in `SAMPLES` folder on SD card.
- In `LIBRARY` Menu, select samples with A/DATA encoder; push to upload to RAM.
- Preview with TRG1/PLAY (audio), TRG2/SHIFT (waveform/size).

### 2. **Sample Editing (SAMPLE Menu)**
- Access playback start, loop, end; play direction/mode (forward, backward, looping).
- Assign tuning (supports proper 1V/Oct).
- Enter slicing (auto: linear/zero-cross; or manual with ADD/REMOVE slices).
- Slices: up to 32 per sample; playback modes: FWD, BKW, RND, CV, NONE.
- Adjust envelope: attack, hold, decay (time & shape); Short/Mid/Long/Relative scaling.

### 3. **Recording Samples**
- In LIBRARY menu, select RECORD for sample input via CV3 (CH2).
- Set input RANGE, LEVEL, and THRESHOLD.
- 48kHz, 12-bit ADC, 30 sec max.
- Trim edit, slice and save to SD.

### 4. **CV Assignment**
- Assign any CV input on each channel to nearly any parameter (tune, playback mode, start, end, envelope stages/shape, FX params, slice, etc.).
- Set CV input range:
  - -5V/+5V (default, most LFOs)
  - -10V/+10V
  - 0/+5V (for sequenced sources)
  - 0/+10V (envelopes)
  - 1V/Oct (for pitch/slice/sample)
- Assign depth for mod destinations. View incoming signals on scope.

### 5. **FX**
- Delay, Reverb, Lowpass/Highpass, Bitcrush, Fold, Drive (per channel).
- 3 parameters each, CV-assignable.

### 6. **Performance Menu**
- Assign 6 main encoders (A–F) to instantly tweak any assignable parameter per channel.
- Encoders: A/B/C for Ch1, D/E/F for Ch2.

### 7. **Projects & Settings**
- Save all settings (samples, edits, FX, CV, encoder assignments) as Projects (Single: one channel, Double: both).
- Recall instantly for performance. Double loads interrupt playback.
- Update system, adjust output levels, display settings, and trigger delays in SETTINGS.

---

## Quick Reference

### KNOBS/ENCODERS
- **A/DATA:** select, confirm, menu navigate (push to enter).
- **B/C/D/E/F:** context: start/loop/end/slice/fx/env/assign CV parameters, etc.
- **D/BACK:** "return/back" to previous screen.

### BUTTONS
- **TRG1/PLAY:** Manual trig Ch1.
- **TRG2/SHIFT:** Manual trig Ch2 or SHIFT (hold).
- **CH1/CH2 Toggle Switch:** Select channel for edit/load/assign.

### INPUT JACKS
- **CH1:** TRIG1, CV1, CV2, CV3
- **CH2:** TRIG2, CV1, CV2, CV3 (CV3 = REC input)

### OUTPUT JACKS
- **OUT1:** Audio out ch1
- **OUT2:** Audio out ch2

---
## Technical Specs

- **Sample Playback**: ~5 min mono RAM per load
- **Sample Rate**: 48kHz, 16bit (ADC record: 48kHz, 12bit)
- **Pitch**: 1V/Oct accurate (C0–C8 range)
- **Panel**: 14HP, 30mm depth
- **Power**: 65mA @ +12V, 2mA @ -12V

---

# [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
