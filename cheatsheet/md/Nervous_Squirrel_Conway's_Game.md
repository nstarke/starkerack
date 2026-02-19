# Nervous Squirrel — Conway's Game

- [Manual PDF](../../manuals/Nervous Squirrel - Conway's Game.pdf)

---

[Conway's Game Eurorack Module Manual (PDF)](attachment:/ConwaysGameManual.pdf)  
*(Based on images provided above)*

---
# Conway's Game Eurorack Module Cheat Sheet

A pattern generator using Conway’s Game of Life, and a 64-output MIDI-to-trigger/gate converter.


## Inputs & Outputs

### Inputs
- **MIDI IN:**  
  - Accepts standard MIDI (5-pin DIN).  
  - Responds to notes C2 (36) – E7 (100)  
  - Controls which outputs are triggered in MIDI mode.

- **CLOCK IN:**  
  - Accepts gates/triggers or audio-rate signals to set simulation speed.  
  - Internal clock: 10Hz default, external up to ~270Hz (can operate "weird" above this).

- **RESET:**  
  - Button input (likely can be used with external trigger/gate).  
  - Clears current Game of Life loop and all stuck MIDI notes.

### Outputs
- **64 TRIGGER/GATE OUTPUTS (8x8 grid):**  
  - One output per Game of Life cell.  
  - **Voltage:** 8V (trigger/gate)  
  - **Trigger Length:** 20ms (in trigger mode)  
  - Used for sequencing drums, envelopes, or other modules.


## Controls / Switches

- **MIDI/LIFE Toggle:**  
  - Switches between MIDI mode (manual trigger control) and Game of Life automaton mode.

- **TRIGGERS/GATES Toggle:**  
  - Sets all outputs to either:
    - **Trigger Mode:** Fires a 20ms trigger pulse on every event.
    - **Gate Mode:** Output remains HIGH (8V) as long as cell is alive.

- **RESET Button:**  
  - Manually resets simulation/start conditions and clears stuck MIDI notes.


## Usage Summary

- **Game of Life Mode**
  - Select random start (auto or via RESET).
  - Cells evolve per GOL rules, driving 64 output jacks.
  - Simulation resets when cells die out or stabilize.

- **MIDI Mode**
  - Incoming notes C2–E7 each trigger corresponding output.
  - Can trigger all 64 outputs via MIDI.

- **Clock Control**
  - Use internal or external clock (LFO, VCO, audio) for step timing.
  - Very high rates (>270 Hz) may yield experimental behaviors.

- **Output Function**
  - All 64 jacks output TRIG or GATE signals per pattern/mode.
  - Patch directly to drums, envelopes, sequential logic, etc.


## Technical Details

- **Width:** 20HP  
- **Depth:** 43.5mm (behind 2mm panel)  
- **Current Draw:**  
  - +12V: 80mA (GOL mode typical), max 215mA (all LEDs lit via MIDI)  
  - -12V: 0mA  
- **Outputs:** 8V, 20ms (trigger), 64 outputs


---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)