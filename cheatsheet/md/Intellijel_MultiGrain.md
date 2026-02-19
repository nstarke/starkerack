# Intellijel — MultiGrain

- [Manual PDF](../../manuals/multigrain_manual_v1.2_2025.09.02.pdf)

---

[**Intellijel Multigrain v1.2 Manual (PDF Previewed)**](#)  
*(Replace with actual link to PDF if available online)*

---

# Intellijel Multigrain v1.2 Cheat Sheet

**Live Stereo Morphing Granular Sampler**

---

## Inputs & Outputs (Jack Reference)

| Jack         | Type      | Voltage Range      | Description                                              |
|--------------|-----------|--------------------|----------------------------------------------------------|
| IN L         | Input     | Audio              | Left audio input                                         |
| IN R         | Input     | Audio              | Right audio input                                        |
| OUT L        | Output    | Audio              | Left audio output                                        |
| OUT R        | Output    | Audio              | Right audio output                                       |
| NEXT         | Input     | >2V trigger        | Advances to next Sound; can be set as RESET for SCAN     |
| GATE         | Input     | >2V gate           | Triggers current Sound                                   |
| SELECT       | Input     | -10V to +10V (±10V, rectified) | Selects which Sound to play                       |
| X            | Input     | -10V to +10V (±10V)           | Assignable CV modulation input                          |
| Y            | Input     | -10V to +10V (±10V)           | Assignable CV modulation input                          |
| Z            | Input     | -10V to +10V (±10V)           | Assignable CV modulation input                          |
| MORPH        | Input     | -10V to +10V (±10V)           | CV input for MORPH fader                                |
| SYNC         | Input     | >2V clock/pulse    | Syncs grain rate/position for Sounds/Live input          |
| A            | Output    | -5V to +5V (±5V)   | Assignable CV output (options per Alt Panel)             |
| B            | Output    | -5V to +5V (±5V)   | Assignable CV output (options per Alt Panel)             |
| SD Card      |           | N/A (microSD slot) | microSD for samples, projects, presets (≤32GB, FAT-32)   |

---

## Panel Controls Overview

### Knobs (with LEDs)
- **START**: Grain starting position in sample/buffer
- **WRAP**: Scan area range window
- **SCAN**: Speed/direction to scan sample area
- **SHAPE**: Grain window shape (7 types, discrete)
- **BLUR**: Reverb amount
- **LEVEL**: Grain output volume
- **RATE**: Grain trigger rate (0–130.8 Hz, or clocked/linked)
- **SIZE**: Grain length (20ms–4s)
- **PITCH**: Pitch shift (-2 to +2 octaves, CV up to ±3)
- **TONE**: 2-pole LPF (CCW) — HPF (CW)

### Fader
- **MORPH**: Scene A ↔ Scene B interpolation (CV, w/ attenuverter*)

### Buttons
- **◎SAMPLE**: Record/assign sample, resample, freeze (read mode-dependent)
- **RATE–SIZE (Link)**: Ties RATE and SIZE behavior 
- **SIZE–PITCH (Link)**: Ties SIZE and PITCH behavior 
- **REVERSE**: Grain playback direction (or ping-pong, hold to enable)
- **SCENE A / SCENE B**: Select/use/edit either scene per Sound
- **ALT / EXIT**: Hold/tap for Alt/settings/exit page
- **CLEAR**: Clear/reset modulation, scenes, sounds, memory etc
- **RAND / X / Y / Z**: Assignable mod pages, per-parameter attenuversion for random/external CV
- **THRU**: Input monitoring/bypass to output (and Blur, with latch/lock options)
- **LATCH**: Sustain sound, toggle latching
- **SOUND 1–8**: Trigger/select 8 Sounds (manual or CV control)

### Other Functions / Hidden Shortcuts
- **Combo Holds:** Hold + press for many actions (see shortcuts below)
- **Long Presses:** Enter ping-pong, quick save/load, etc.

\* **MORPH ATT** (not panel-labeled): Attenuverter for Morph CV

---

## Voltage/Control Summary

| Function           | Source         | Range                | Usage                          |
|--------------------|---------------|----------------------|--------------------------------|
| X/Y/Z Inputs       | CV in         | ±10V                 | Mod-assigned to (almost) any parameter, incl. Reverse  |
| Morph Input        | CV in         | ±10V (±5V sweeps)    | Fader position modulated      |
| Gate/Next Input    | Gate/Trig     | >2V                  | Trigger Sound or advance/scan/reset|
| Select Input       | CV in         | ±10V (rectified)     | Sound selection via CV (0V–5V mapped 1–8) |
| Sync Input         | Trig/Clock    | >2V                  | Syncs grain rate or Live Sound positions |
| A/B Outputs        | CV out        | ±5V                  | Envelope, S&H, random, morph, grain triggers, etc. (assignable)|

---

## Core Workflows

### Loading & Assigning Sounds
- **Load sample:** ALT > /PROJECT, /WAVS, /RECS > assign to SOUND (preview by pressing/latching)
- **Record sample:** Press ◎SAMPLE to record; press ◎SAMPLE again to stop; assign to SOUND or save  
- **Live Sound:** Hold SOUND, press ◎SAMPLE (button turns magenta/pink)

### Playing Sounds/Grains
- **Trigger:** Press/hold SOUND 1–8 (or gate)
- **Latch:** Enable latch, press SOUND (continues sound)
- **Morph:** Move MORPH fader between A↔B for morphing

### Editing Parameters
- **Adjust Knobs:** Direct control over granular/sample params  
- **Assign Mods:** On RAND/X/Y/Z mod page, turn knob for attenuversion  
- **Copy/Randomize:** Hold/press relevant controls (e.g. Hold SCENE A, press SCENE B to copy)

### Scenes & Morphing
- **Edit Scene:** Select Scene A / B, adjust parameters
- **Morph:** Crossfade using fader (CV controllable)
- **Copy Scene:** Hold SCENE, press the other to paste  
- **Randomize Scene:** Hold RAND, press SCENE

### Sampling & Trimming
- **Live/Looping:** Loop: Hold SOUND + press ◎SAMPLE. Freeze w/ ◎SAMPLE. Save to SD by long-press.
- **Trim:** After capture, long-press ◎SAMPLE for advanced trimming/editing.

---

## Reference: Quick Shortcuts

| Action                             | Combo                                                        |
|-------------------------------------|--------------------------------------------------------------|
| Clear Sound                        | Hold CLEAR, press SOUND (once=settings; twice=delete sample) |
| Latch sound, keep latched, edit     | Enable LATCH, press SOUND, adjust params                     |
| Copy Sound                         | Hold SOUND, press destination SOUND                          |
| Morph All Scenes/Sounds            | Hold LATCH, or Scene, or both, then move knob                |
| Assign modulation                  | Hold RAND/X/Y/Z (mod page), turn knob                        
| Modulate Param Across Sounds       | Hold LATCH + param on mod page                               |
| Enable Live Sound                  | Hold SOUND, press ◎SAMPLE                                    |
| Randomize Scene/Sound/X/Y/Z        | Hold RAND, press SCENE/SOUND/X/Y/Z                           |
| Enable THRU/Bypass/Lock            | Press/hold LATCH + THRU; hold to lock                        |
| Enter System Settings Page         | ALT + long-press PROJECT (~4s)                               |
| Reboot Module                      | Hold LATCH + CLEAR (~4s)                                     |
| Quick Open Quantizer               | Long press QUANT                                             |
| Quick Save/Load Preset             | Long press SAVE or LOAD                                      |

(For a full shortcut table, see manual page 53–54)

---

## Assignable CV Output Modes (A/B Outs)
- Morph fader (GREEN)
- Grain trigger pulse (AMBER)
- Grain envelope (BLUE)
- Input envelope follower (MAGENTA)
- Output envelope follower (RED)
- Random S&H per grain (WHITE)
- Grain pitch (CYAN, v1.2+)

---

## Sample/Format Requirements
- WAV, 48 kHz, 16 bit, Stereo, ≤32 seconds  
- microSD, FAT-32, ≤32GB recommended

---

## Other Tips

- **Projects/Presets:** 48 Projects (6x8); 48 Presets per Project
- **Samples:** /PROJECT (per-project: 128), /WAVS (global: 128), /RECS (global: 1024)
- **Firmware Upgrades:** USB-C, hold boot and follow Intellijel Updater

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)
