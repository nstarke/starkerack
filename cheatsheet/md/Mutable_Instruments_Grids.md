# Mutable Instruments — Grids

- [Manual PDF](../../manuals/Manual - Mutable Instruments Grids Documentation.pdf)

---

[**Mutable Instruments Grids Manual (PDF)**](https://mutable-instruments.net/modules/grids/manual.pdf)

---

# Mutable Instruments Grids Cheat Sheet

### Overview
Grids is a 3-channel clock-driven trigger generator designed to create and morph rhythmic drum patterns. It interpolates between learned rhythms on a 2D map (X/Y), with adjustable density ("fill") and randomization ("chaos"). 3 outputs are typically for BD (kick), SD (snare), and HH (hi-hat), but can be patched freely.

---

## Panel Controls

| Label | Control Type | Description |
|-------|--------------|-------------|
| **A** | Knob         | Internal clock rate: 40–240 BPM (fully CCW disables internal clock; expects external clock) |
| **B** | Button       | Tap/Reset: Tap twice for tempo, tap once to unlock CLOCK knob. Flashes on beat. |
| **C1**| Knob         | Map X: Selects X-position on rhythm map (CV-controllable 0–5V) |
| **C2**| Knob         | Map Y: Selects Y-position on rhythm map (CV-controllable 0–5V) |
| **D** | Knob         | Chaos: Amount of randomization/ghost notes (CV-controllable 0–5V) |
| **E1**| Knob         | Fill 1 Density (BD): Channel 1 density (CV-controllable 0–5V) |
| **E2**| Knob         | Fill 2 Density (SD): Channel 2 density (CV-controllable 0–5V) |
| **E3**| Knob         | Fill 3 Density (HH): Channel 3 density (CV-controllable 0–5V) |
|       | 3 LEDs       | Indicate clock resolution, tap/reset, swing, euclidean mode, triggers/gates, and output layout (in options mode) |

---

## Input & Output Jack Reference

| Jack    | Type        | Function                                    | Voltage Range           |
|---------|-------------|---------------------------------------------|-------------------------|
| CLOCK   | Input       | External clock input; active if INT clock off (A fully CCW). | 0–+5V (higher OK)      |
| RESET   | Input       | External reset (pattern start)              | 0–+5V (higher OK)      |
| MAP X   | CV Input    | Modulate X position (C1)                    | 0–5V (sum with knob)   |
| MAP Y   | CV Input    | Modulate Y position (C2)                    | 0–5V (sum with knob)   |
| CHAOS   | CV Input    | Modulate Chaos randomness (D)               | 0–5V (sum with knob)   |
| FILL 1  | CV Input    | Modulate Fill 1 density (E1)                | 0–5V (sum with knob)   |
| FILL 2  | CV Input    | Modulate Fill 2 density (E2)                | 0–5V (sum with knob)   |
| FILL 3  | CV Input    | Modulate Fill 3 density (E3)                | 0–5V (sum with knob)   |
| TRIG 1  | Output      | Channel 1 trigger (BD)                      | +5V, 1ms default       |
| TRIG 2  | Output      | Channel 2 trigger (SD)                      | +5V, 1ms default       |
| TRIG 3  | Output      | Channel 3 trigger (HH)                      | +5V, 1ms default       |
| ACC 1   | Output      | Channel 1 accent                            | +5V, 1ms pulse         |
| ACC 2   | Output      | Channel 2 accent                            | +5V, 1ms pulse         |
| ACC 3   | Output      | Channel 3 accent                            | +5V, 1ms pulse         |

**Note:** Under alternate output configuration, ACC outputs can be set to ACC/CLK/RST (see Options below).

---

## Quick Start

1. **Connect outputs:** TRIG 1, 2, 3 to drum modules.
2. **Set clock:** Use internal clock (A knob) or patch external clock to CLOCK input (A fully CCW).
3. **Select rhythm:** Use C1 (Map X) and C2 (Map Y) to pick a rhythm base.
4. **Set density:** Use E1, E2, E3 to control pattern fill for each channel.
5. **Chaos:** Turn D knob for probabilistic ghost notes/variation.
6. **Accent:** Feed ACC outputs to modules for accents.

---

## Options Menu (hold TAP/Reset button for 0.5s, unplug CV inputs!)
- Cycle through settings by turning the specified knob. LEDs indicate mode.

| Function                     | Control   | LEDs On                                        | LEDs Off                             |
|------------------------------|-----------|------------------------------------------------|--------------------------------------|
| **Clock Resolution**         | E1        | 4, 8, 24 ppqn (LEDs show selection)            |                                      |
| **Tap Tempo/Reset Mode**     | E2        | Tap sets TEMPO                                 | Tap resets pattern                   |
| **Swing (internal clock only)**| E3      | CHAOS sets Swing                               | CHAOS is randomization               |
| **Euclidean Mode**           | C1        | Grids pattern generator                        | Euclidean sequencer                  |
| **Trig/Gate Output**         | C2        | Gates (length = clock hi duration)             | 1ms triggers                         |
| **Alt ACC Outputs**          | D         | ACC/CLK/RST                                    | ACC1/2/3 (default accent outs)       |

---

## Power / Installation

- 16HP width, ribbon cable: -12V/+12V (2x5)
- Power: −12V rail = 1mA, +12V rail = 25mA
- **Red stripe** must match board marking ("Red stripe")

---

## Modulation Summary

- **All major params (Map X, Map Y, Chaos, Fill 1/2/3) are CV-controllable (0–5V). Sum with panel setting.**
- **CLOCK/RESET expects typical eurorack 0–5V logic.**
- **Outputs (TRIG, ACC):** +5V logic, 1ms (trigger) or gate (if option set).

---

## [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)