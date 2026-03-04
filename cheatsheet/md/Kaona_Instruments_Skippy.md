# Kaona Instruments — Skippy

- [Manual PDF](../../manuals/Skippy_2-2_ENG.pdf)

---

[Download the Skippy Manual PDF](https://www.kaona.fr/download/skippy_user_manual_EN.pdf)

---

# Kaona Skippy Eurorack Module Cheat Sheet

**Module Overview:**  
Kaona Skippy is a 4-track polyrhythmic sequencer offering both matrix (step-based) and non-matrix (time-based) sequencing. Each track is independent and poly-temporal, allowing creative rhythms and algorithmic step generation.

---

## Interface Reference

**Front Panel Elements:**
- **4 Color Buttons:**  
  - Red (Track 1)
  - Yellow (Track 2)
  - Green (Track 3)
  - Blue (Track 4)  
  Used for selecting tracks for editing.

- **Central Encoder Knob:**
  - Rotate: Navigate/select parameter
  - Press: Select/function entry/exit
  - Long Press: Enter/exit System menu
  - Double Click: (in RESET mode) Sync/unsync all tracks
- **Screen:** Shows selected function and track activity.

- **LED Circles:** Show rhythmic activity for each track, color coded.

---

## Inputs & Outputs

| Jack           | Function                  | Details / Voltage Ranges                                   |
|----------------|--------------------------|------------------------------------------------------------|
| CV OUT 1–4     | Sequencer Gates          | 5V gates, match track color. Duration set by **GATES**     |
| CV CLOCK IN    | Clock/Reset input        | Gate/Trig, min. 3V for RESET. Supports matrix/poly clocks. |
| CV CLOCK OUT   | Internal clock out       | 5V logic, clock/tempo depending on CLK settings.           |

---

### Input Function Modes
- **RESET:** All sequences reset to step 0 on input pulse.
- **POLY:** Follows average external clock, preserves non-metric timing.
- **MATRIX:** Strictly follows external steps (can follow swung/irregular clocks).

---

## Main Functions & Parameters

| Function       | Description/How-To                                      |
|----------------|--------------------------------------------------------|
| **BPM**        | Tempo (10–600 BPM); EXT shown if externally clocked    |
| **STEPS**      | Steps per rotation (1–64); some modes auto-set steps   |
| **BEGIN/END**  | Set arc for pattern; not 0-based; direction-sensitive  |
| **GATES**      | Gate duration; longer gates overlap at high speeds     |
| **PROBA**      | Probability to skip enabled step (0–100%)              |
| **CHAOS**      | Randomize step timings; disables for strict algorithms |
| **WAY**        | Set direction: <, >, <>, pause (-). Pause = time stop  |
| **SWING**      | Shuffle alternate steps; not in all algorithms         |
| **GAUSS**      | Logarithmic step distribution; sign sets curve focus   |
| **EUCLID**     | Bjorklund Euclidean gates; x/y pattern (#/total steps) |
| **TILES**      | Matrix: repeat x on/x off; can break at cycle repeat   |
| **POLYR**      | Alternating tempos (e.g., 4/3); auto-calculates steps  |
| **JAZZY**      | 32-step matrix with pre-defined funk/jazz patterns     |
| **SPIN**       | Rotate left/right for matrix/Euclidean functions       |
| **PAUSE**      | Mute any track (blinks); no param editing while muted  |
| **RESET**      | Return all heads to 0; double tap = “sync”             |

---

## System Functions (Long-Press Encoder)

| Function   | Description                                      |
|------------|--------------------------------------------------|
| **SAVE**   | Store 0–64 presets to SD card. Overwrites slot.  |
| **LOAD**   | Recall preset 0–64 from SD card                  |
| **NEW**    | Initialize fresh state (clear settings)           |
| **CLK IN** | Set clock/reset input mode (see above)           |
| **CLK**    | Clock multiply/divide (poly only, not matrix)    |

---

## LED / Button Behavior

- **Button lit:** Track selected for edit.
- **Button blinking:** Track muted via PAUSE.
- **Screen color:** White = normal/selectable, Violet = parameter editing for selected tracks.

---

## Voltage Reference

- **Gate outputs (CV OUT 1–4):** 0V (off) / 5V (on)
- **Clock input:** 3V minimum trigger/gate
- **Clock output:** 5V logic

---

## Quick Usage Tips
- Select track(s) with color buttons for group/individual editing.
- Use encoder to select and change function/parameter.
- Long-press encoder for save/load/system settings.
- RESET and double-tap for instant recall/re-alignment of all tracks.
- For experimenting, try immobilizing a track with WAY set to "-" (pause).

---

## Technical
- **Width:** 10HP
- **Depth:** 32mm
- **Power:** +5V at 200mA (no current draw on ±12V)
- **SD card:** Internal, for presets only.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)