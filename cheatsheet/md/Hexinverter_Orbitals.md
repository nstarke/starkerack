# Hexinverter — Orbitals

- [Manual PDF](../../manuals/hexinverter-orbitals.pdf)

---

[Hexinverter Orbitals User Manual PDF (v1.04)](https://hexinverter.net/wp-content/uploads/2020/06/Orbitals-User-Manual-v1.04.pdf)

---
# HEXINVERTER ORBITALS CHEAT SHEET

**42HP Dual Bipolar Voltage Controlled Step Sequencer**

## Quick Start

- **Power requirements:** +90mA, -20mA @ 12V (Do not adjust jumpers when powered!)
- **Modes:** Two independent 8 step sequencers or a single 16 step sequencer.
- **CV Output Modes:**
  - Bipolar: `-2.5V to +2.5V` (5V jumper), `-5V to +5V` (10V jumper)
  - Unipolar: `0V to +5V` (5V jumper), `0V to +10V` (10V jumper)
- **Clock:** Internal (adjustable up to ~100Hz) or external (1V logic level, up to 1kHz)
- **Build note:** Very shallow/skiff friendly; ideal for performance setups.

---

## Front Panel Controls & Jacks

### Top Panel: Sequencer Rows (A/B)
- **RATE Knob (A & B):** Adjusts internal clock speed for each sequencer.
- **CV Knobs (per step):** Adjusts output voltage for each step.
- **GATE Switches + LEDs (per step):** Toggles gate ON/OFF for each step & shows active step.
- **RUN Switch (A & B):** Turns sequencer ON/OFF and activates gate output.

### Right Side Outputs
- **CV OUT (A & B):** Control voltage for sequences. (Voltage ranges as above.)
- **GATE OUT (A & B):** Gate output for each sequence step (max 10V).
- **CLK OUT (A & B):** Outputs internal clock (0–5V) for use elsewhere.

### Lower Panel: System/Modulation
- **GATE Knob (A & B):** Adjust duration of step gates (short/long, ties possible if set long).
- **LENGTH Knob (A & B):** Sequence length (Sets length 1–8 for A & B; if A > 8: module enters 16-step mode).
- **MODE Knob (A & B):** Step modes:
    1. FW (Forward)
    2. REV (Reverse)
    3. PND (Pendulum)
    4. RND (Random)
    5. CV (Unclocked voltage addressed)
    6. CLK (Clocked voltage addressed)
- **RUN Input:** Active high logic input (>1V). Enables sequencer.
- **CLK IN:** External clock input (1V logic threshold; up to ~1kHz).
- **RST/CV IN:** Used for:
    - Regular modes: Logic HIGH resets to step 0.
    - CV/CLK modes: 0–5V selects which step is active.
- **REVERSE Input:** Logic HIGH forces sequencer to run backwards.
- **RESET Button:** Resets both sequencers for sync.
- **TRANS A Input:** Adds external CV (e.g. keyboard) to Sequencer A for transposing sequences.
- **SLAVE B>A Switch:** Syncs B’s transport to A.
- **BIPOLAR Switch:** Toggles bipolar/unipolar voltage output.

---

## Inputs/Outputs Reference Table

| Jack Name     | Function                                  | Voltage Range              |
| ------------- | ----------------------------------------- | ------------------------- |
| CV OUT (A/B)  | Sequencer control voltage output          | -2.5V to +2.5V / -5V to +5V (bipolar); 0–5V / 0–10V (unipolar, jumper selectable) |
| GATE OUT (A/B)| Sequencer gate output                     | 0V (off), up to 10V (on, jumper selectable) |
| CLK OUT       | Internal clock output                     | 0–5V                      |
| CLK IN        | External clock input                      | 1V logic (HIGH = >1V), up to 1kHz |
| RUN IN        | Sequencer ON/OFF (active high logic)      | >1V = ON                  |
| RST/CV IN     | Reset (logic >1V) or Step Select (0–5V)   | Reset: >1V, CV: 0–5V      |
| REVERSE IN    | Run backwards (active high logic)         | >1V = Reverse             |
| TRANS A IN    | Add CV to Sequencer A output (transpose)  | -                         |

---

## Voltage-Selectable Jumpers

_Set jumpers on the back to select CV/Gate output range:_

| Bipolar? | 5V Jumper        | 10V Jumper     |
| -------- | ---------------- | -------------- |
| On       | -2.5 to +2.5V    | -5 to +5V      |
| Off      | 0 to +5V         | 0 to +10V      |

**NEVER adjust jumpers with module powered!**

---

## Operating Tips

- **Sequence Length:** Set A’s LENGTH >8 to enter 16-step mode (A + B combined).
- **Voltage Modes (MODE knob):**
  - In CV/CLK modes, supply 0–5V at RST/CV IN to select active step directly.
  - In other modes, RST/CV IN acts as a reset input.
- **Syncing Sequencers:** Use SLAVE B>A switch to synchronize B with A (e.g. for 16-step mode or complex patterns).
- **Transposing Patterns:** Use TRANS A for real-time keyboard-driven transpositions.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)