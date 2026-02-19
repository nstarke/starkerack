# Intellijel — Metropolix

- [Manual PDF](../../manuals/metropolix_manual_v1.4_2022.04.04.pdf)

---

[Metropolix Manual PDF](https://manual.intellijel.com/Metropolix_Manual_1.4.pdf)

# Intellijel Metropolix — Eurorack Sequencer Cheat Sheet

> Highly performance-oriented **8-stage, dual-track pitch/gate/clock MOD sequencer** with deep hands-on and CV control.

---

## Quick Reference Table

| Section   | UI Element                       | Functionality / Details                                                                   |
|-----------|----------------------------------|------------------------------------------------------------------------------------------|
| **Jacks** | **TRACK 1 PITCH OUT** (D)       | 1V/Oct pitch (default: TRK 1). Swappable. 0–+5V typical.                                 |
|           | **TRACK 1 GATE OUT** (E)        | Gate output (0V = off, +5V = on). Swappable.                                             |
|           | **TRACK 2 PITCH OUT** (F)       | 1V/Oct pitch (default: TRK 2), swapped as above.                                         |
|           | **TRACK 2 GATE OUT** (G)        | Gate (0/+5V), swappable as above.                                                        |
|           | **CLOCK OUT** (C)                | Clock out, division settable, 0V low, +5V trigger.                                       |
|           | **A OUT / B OUT** (A/B)          | User-assignable: CV, MOD, gates, velocity, clock, trigger, etc. -5V to +5V range.        |
|           | **CLOCK IN** (H)                 | External clock, expects trigger/gate. +1.5V min, typically 0/+5V (range -5V to +5V OK).  |
|           | **RESET IN** (I)                 | Resets sequence (trig), reassignable as RUN input. +1.5V = trig/gate (0–+5V typical).    |
|           | **X / Y / Z IN** (X, Y, Z)       | AUX CV inputs, assignable. Accepts -5V to +5V (full parameter range).                    |
|           | **I2C** (back)                   | Gx/Qx expander support.                                                                  |
| **Sliders/Toggles** | **PITCH SLIDERS**           | 8 per stage; default pitch per stage, 1–4 octaves, root/scale quantizing.                 |
|           | **PULSE COUNT**                  | 8 toggles, 1–8 pulses per stage.                                                         |
|           | **GATE TYPE**                    | 8 switches: Hold, Multi, Single, Rest.                                                   |
| **Knobs** | **CTRL 1 & 2**                   | Assignable to pitch, gate, division, root, scale, velocity, etc. -5V to +5V out when set.| 
|           | **AUX Attenuverters**            | X, Y, Z inputs manual scaling/polarity.                                                  |
| **Buttons** | **RUN**                          | Start/stop sequence.                                                                     |
|           | **RESET**                        | Manual reset (to "first" stage, resets accumulators).                                    |
|           | **LOOPY**                        | Loopy mode (momentary/latch subloops, manual/key mode).                                 |
|           | **SETUP/BPM/SCALE**              | Global configuration, tempo, quantizer/scale/root.                                       |
|           | **ORDER/LEN/DIV/SWING/SLIDE/GATE** | Per-track: playback direction/order, length, clock div, swing (trk 1&2), slide, gate time.|
|           | **EDIT/SLIDE/SKIP/PITCH/GATE/RATCH/PROB/ACCUM/CV** | Per-stage, per-track/lane editing (or per MOD lane).                                   |
|           | **ALT**                          | Access alternate button/slider functions (preset save/load, output, mod assign, etc).    |
|           | **TRACK SELECT** (TRK 1/TRK 2/MOD) | Select which "track" or mod lane is active for editing.                                 |
|           | **Screen Encoder**               | Menu navigation, value adjustment, press for confirm/toggle/parameter select.            |
|           | **AUX X/Y/Z Buttons**            | Input routing, also randomization shortcuts.                                             |

---

## Inputs Summary

| Jack          | Label         | Use               | Range (V)    |
|---------------|---------------|-------------------|--------------|
| CLOCK IN      | H             | Advances seq      | -5 to +5     |
| RESET IN      | I             | Resets seq        | -5 to +5     |
| X AUX IN      | X             | CV/Trig mod       | -5 to +5     |
| Y AUX IN      | Y             | CV/Trig mod       | -5 to +5     |
| Z AUX IN      | Z             | CV/Trig mod       | -5 to +5     |

---

## Outputs Summary

| Jack              | Label   | Use                        | Out Range (V) |
|-------------------|---------|----------------------------|---------------|
| TRACK 1 PITCH OUT | D       | 1V/Oct, swappable          | 0 to +5 (typ) |
| TRACK 1 GATE OUT  | E       | Gate, swappable            | 0/+5          |
| TRACK 2 PITCH OUT | F       | 1V/Oct, swappable          | 0 to +5 (typ) |
| TRACK 2 GATE OUT  | G       | Gate, swappable            | 0/+5          |
| CLOCK OUT         | C       | Divided clock              | 0/+5 trig     |
| A OUT             | A       | User assignable (CV, MOD, etc) | -5 to +5 |
| B OUT             | B       | User assignable            | -5 to +5      |

---

## Panel Controls At-a-Glance

### Sliders & Toggles (Top)
- **PITCH SLIDERS:** Set root pitch for each stage (1–8). Quantize using SCALE. 1–4 octave range.
- **PULSE COUNT:** (Switches below each slider) 1–8 pulses per stage – affects rhythmic length.
- **GATE TYPE:** (Switches below Pulse Count) Choose:  
    - HOLD = sustain gate through all pulses
    - MULTI = gate per pulse
    - SINGLE = one gate per stage
    - REST = no gate

### Center Section
- **Screen + Encoder:** Deep editing, assign destinations, menu navigation.
- **TRACK BUTTONS:** TRK 1, TRK 2, MOD (8 MOD lanes); track/parameter selection.
- **EXIT:** Go back / Home screen / Sync panel.
- **TRANSPORT:**  
    - **RUN:** Play/Stop (or Pause in config)
    - **RESET:** Reset sequence/stage/accum.
    - **LOOPY:** Enter Loopy subloop/manual play mode.
- **GLOBAL SETTINGS:**  
    - **SETUP:** System/global settings.
    - **BPM:** Set/see tempo, tap with button, mod with CV/ctrl/mod.
    - **SCALE:** Quantizer scale/root, user scales, chord locks.

### TRACK SETTINGS:
- **ORDER:** Sequence direction/order (linear, random, shuffle, pendulum, etc).
- **LEN:** Number of stages/total pulses/offset (polyrhythm/phase patterns).
- **DIV:** Clock divider (for track & mod lanes).
- **SWING:** Groove; not present on MOD lanes.
- **SLIDE TIME:** Portamento for slid stages; analog/tempo/acid.  
- **(TRACK) GATE:** Gate time/scale per track (with per-stage override via STAGE GATE).

### STAGE EDIT (EDIT + Button)
- **SLIDE / SKIP / PITCH / GATE / RATCH / PROB / ACCUM / CV:**
    - Per-stage per-track editing for each above function (see table below for summary).

### ALT Functions
- **LOAD (ALT+1):** Load preset/bank.
- **SAVE (ALT+2):** Save preset/bank (confirm overwrites).
- **OUT A, OUT B (ALT+3/4):** Assign output function/track (A or B jack).
- **CLK (ALT+5):** Configure clock out division/offset.
- **MX (ALT+6):** Expander output routing.
- **LIM (ALT+7):** Accumulator (ACCUM) transposition limit/polarities/modes.
- **TYPE (ALT+8):** Set CV Lane output type (Voltage / Gate Toggle).

---

## MOD Lanes

- **8 lanes**, parallel to main sequencer.
- Each has: order (playback), length (stages/pulses), div (clock), and parameter destination (internal param, or OUT A/B)
- Each lane: 8 stage voltages (or gates if routed to gate-type param), ±5V output range for OUT jacks.

---

## Core Per-Stage Parameters (All CV-automatable via AUX/MOD)

| EDIT Mode | Function                                   | Range / Details           |
|-----------|--------------------------------------------|---------------------------|
| SLIDE     | Slide (portamento enabled/disabled)        | per stage                 |
| SKIP      | Stage skipped or not                       | binary                    |
| PITCH     | Override note/scale (or inherit slider)    | C0–C5 (quantized/locked)  |
| GATE      | Per-stage override length or rest/hold     | --/rest/1–100%            |
| RATCH     | Subdivisions per-pulse/ratchet             | 1–8                       |
| PROB      | Probability gate triggers (stage or pulse) | 0–100%                    |
| ACCUM     | Per-stage accumulate amount/trigger        | ±1–7 scale deg, stage/pulse/ratch trigger modes  |
| CV        | Per-stage control voltage (or gate if type set) | –5V to +5V             |

---

## Cheat Sheet: Essential Moves

**Run/Stop:**  
- Press RUN.  
**Reset:**  
- Press RESET to restart sequence from Offset.
**Set BPM:**  
- Press BPM, turn encoder.  
- Long-press BPM for fine.  
- Tap BPM button for tempo tap.
**Change Scale:**  
- Press SCALE, encoder chooses scale/root.
**Load/Save Preset:**  
- ALT+1: Load, ALT+2: Save (bank select with encoder, choose slot 1-8 with stage buttons).
**Per-Track Parameter Edits:**  
- Select TRK 1/2/MOD, press corresponding ORDER/LEN/etc.
**Per-Stage Edits:**  
- Select track (TRK 1/2), EDIT + parameter (SLIDE etc), then press stage button 1–8 to edit.
**Assign Output Functions:**  
- ALT+3/A or ALT+4/B for OUT A/B, select parameter output (CV, MOD max ±5V).
**AUX Inputs:**  
- Patch CV -5V to +5V. Press X/Y/Z button to assign param, set attenuverter for range/polarity.

**Loopy Mode:**  
- Press LOOPY. Hold stage button(s) to loop single or range.  
- Latch: Release/unlatch via LOOPY. Stage buttons become a "manual keyboard" in stop mode.

---

## CV & MIDI Integration

- All assignable modulation: AUX inputs, MOD lanes, CTRL knobs, MIDI in/out (USB micro port; see manual on SysEx and channel/CC assign).
- Inputs accept -5V to +5V for full range mapping. Outputs provide up to ±5V (A/B jack assignments, MOD) or standard 1V/Oct (+0-5V typ) for pitch.

---

## Tips

- **Muting:** Hold LOOPY, then TRK 1/2/MOD or MOD lane to mute/unmute.
- **Copy/Paste:** Hold source (track/stage), press target (see manual for details).
- **Randomization:** ALT + AUX X = full random, ALT + AUX Y = morph, ALT + AUX Z = undo (Active in editing screen).
- **Panel Sync:** Long-press EXIT — clear overrides, use front panel positions.

---

## Useful Ranges & Specs

| Control        | Voltage Range            | Notes    |
|----------------|-------------------------|----------|
| All CV INs     | -5V to +5V              | Full param |
| A/B/MOD CV OUT | -5V to +5V              | User/mapped |
| Pitch OUT      | 0V to +5V (typ)         | 1V/octave, adjustable |
| Gate Outputs   | 0V (low), +5V (high)    | Triggers/gates |
| MIDI           | USB micro-B (rear panel) | Use Intellijel extender if needed |

---

**See full manual for details and advanced configuration:**  
[Metropolix Manual PDF](https://manual.intellijel.com/Metropolix_Manual_1.4.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)