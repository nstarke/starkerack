# IO Labs — Flux Sequencer

- [Manual PDF](../../manuals/IO Labs - Flux Sequencer - 107 User Manual.pdf)

---

[**Flux Open Beta V1.07 User Manual (PDF)**](https://iolabs.co.uk/flux/Open_Beta_Flux_v1_07_Manual.pdf)

---

# FLUX Eurorack Sequencer Cheat Sheet

A quick-reference guide for using the IOLabs FLUX Temporal Modulation Synthesis® Eurorack module.

---
## Overview

**FLUX**: A four-channel, 16-step rhythm and CV sequencer featuring novel "Temporal Modulation Synthesis" (TMS) for advanced polyrhythm and timing, per-step parameter locking, internal modulation, and full MIDI and CV support.

### Power Consumption
- **+12V:** 160mA
- **-12V:** 50mA
- **5V:** Not used

---

## Connections

### Outputs (0–8V for CV outs)
| Jack | Function                                | Range/Notes                          |
|------|-----------------------------------------|--------------------------------------|
|  1   | CH1 Main Rhythm Out (gate/trigger)      | 0–5V or 0–8V (typical trigger/gate)  |
|  2   | CH1 Aux 1 Rhythm Out                    | 0–5V or 0–8V                         |
|  3   | CH1 Aux 2 Rhythm Out                    | 0–5V or 0–8V                         |
|  4   | CH1 CV Out                              | 0–8V                                 |
|  5   | CH2 Main Rhythm Out                     |                                      |
|  6   | CH2 Aux 1 Rhythm Out                    |                                      |
|  7   | CH2 Aux 2 Rhythm Out                    |                                      |
|  8   | CH2 CV Out                              | 0–8V                                 |
|  9   | CH3 Main Rhythm Out                     |                                      |
| 10   | CH3 Aux 1 Rhythm Out                    |                                      |
| 11   | CH3 Aux 2 Rhythm Out                    |                                      |
| 12   | CH3 CV Out                              | 0–8V                                 |
| 13   | CH4 Main Rhythm Out                     |                                      |
| 14   | CH4 Aux 1 Rhythm Out                    |                                      |
| 15   | CH4 Aux 2 Rhythm Out                    |                                      |
| 16   | CH4 CV Out                              | 0–8V                                 |

### Inputs
| Jack | Function                                | Range/Notes                                  |
|------|-----------------------------------------|----------------------------------------------|
| 17   | External Clock                         | 0–8V logic-level pulses                      |
| 18   | Reset                                  | 0–8V trigger/gate                            |
| 19   | Start/Stop                             | 0–8V logic                                  |
| 20   | Mute All Rhythm Outs                   | 0–8V logic                                  |
| 21   | CV In A                                | 0–8V                                        |
| 22   | CV In B                                | 0–8V                                        |
| 23   | CV In C                                | 0–8V                                        |
| 24   | CV In D                                | 0–8V                                        |

---

## Panel Elements

### Pots & Encoders

| No. | Name               | Function                                      | Notes                        |
|-----|--------------------|-----------------------------------------------|------------------------------|
| 25  | Macro Pot 1        | Manual modulation source                      | Assignable to parameters     |
| 26  | Macro Pot 2        |                                              |                              |
| 27  | Macro Pot 3        |                                              |                              |
| 28  | Macro Pot 4        |                                              |                              |
| 29  | Navigation Encoder | Selects parameters/pages (push = channel -)   |                              |
| 30  | Param Encoder      | Changes parameter value (push = channel +)    |                              |

### Buttons

| No. | Button                | Function                                                                                       |
|-----|-----------------------|------------------------------------------------------------------------------------------------|
| 31  | Coarse Nav/Param (*)  | Coarse (xN) navigation or parameter change                                                     |
| 32  | Edit All (ALL)        | Edit all steps at once                                                                         |
| 33  | Micro SD              | Micro SD menu (load/save/rename presets)                                                       |
| 34  | Step Select <<        | Previous step                                                                                  |
| 35  | Step Select >>        | Next step                                                                                      |
| 36  | Step On/Off           | Toggle step on/off                                                                             |
| 37  | MOD                   | Enter modulation pages (Evolve LFO, Macro Pots, CV Inputs)                                     |
| 38  | Start/Stop            | Start or Stop sequencer                                                                       |

---

## Quick Parameter Guide

### Rhythm Parameters (Per Step, Channel)
- **PROB:** Probability % (step or per-trigger)
- **LOOP:** Sequence loop range (start > end)
- **MOD:** Select modulation bus (Yellow/Grey/Purple)
- **GATE:** Gate length (% of step/trigger time)
- **DENS:** Trigger density (# per step)
- **CURV:** Temporal curve type
- **VAL:** Temporal curve value (log/lin/exp)
- **DIFF:** Curve division parameter
- **COMP:** Compression/expansion of triggers
- **PHAS:** Phase shift (in degrees)
- **LENG:** Step length (in 16ths)
- **HUMA:** Humanize (1–127, subtle/extreme)
- **MASK:** Logical mute mask (e.g. 1in2, 2in3)
- **MSK>:** Mask shift (starting trigger)
- **AUX1/AUX2:** Select auxiliary output mode (see below)

### CV Output Parameters (Per Step, Channel)
- **CVSEL:** LFO, Envelope, Voltage, Random
- **S+H:** Sample & Hold (per step/trigger)
- **MINV/MAXV:** Min/Max CV output (0–8V)
- **ATK/REL:** Attack/Release (Envelope modes, ms?)
- **CURV:** Attack/Release curve shape
- **FREQ:** LFO frequency (Hz or divisions)
- **SYNC:** LFO/envelope retrigger mode (step/trig)
- **QUAN:** # of quantization nodes per V/oct (1–24)
- **QUAN NODES:** Enable/disable individual quant steps

---

## Aux Output Modes (Per Step, Per Out)
- **OFF:** No out
- **ON:** High while running
- **START/SOS/1st/Last:** Trig at start-of-sequence/step/first/last
- **DEL1–8:** Delayed main rhythm out, 1–8 steps/gates
- **TL1–16:** Clock divider by N
- **&, !&, \|\|, !\|\|, x\|\| (AND/OR logic):** Real-time logic on main/AUX outs
- **CV>1–7V / CV<1–7V:** Out high if CV above/below threshold
- **PPQ 1–48:** Clock generator, pulses-per-quarter
- **/1–16:** Master divider

---

## Modulation Buses
- **Yellow, Grey, Purple:** Assignable per step for selective modulation routing (manual pots, CV, evolve-LFO modulation)

---

## Workflow—Basic Steps

1. **Install & Power**: Mount, use correct ribbon orientation (red stripe = -12V).  
2. **Select Channel/Step**: Use encoders (push left = previous, right = next channel; >>/<< for steps).
3. **Set Parameters**: On main UI, use left encoder to select, right to change.
4. **Edit All Steps**: Press ALL, edit applies to all steps.
5. **Setup Modulation**: Press MOD for modulation pages (Evolve LFOs, Macro Pots, CV Ins). Assign depths/destinations.
6. **Sequence/Loop**: Adjust LOOP/step count, per-step densities, and TMS (CURV/VAL) for unique grooves.
7. **Aux Logic Outs**: Assign per-step utility clocks, logic/gates, delay, dividers.
8. **CV Outs**: Set mode and range for envelopes, LFOs, or stepped voltages—use quantization for pitch output.
9. **Presets**: Press Micro SD to Save/Load. Name up to 8 characters.  
10. **Start/Stop**: Use button or external input/MIDI (configure clock mode in CONFIG).

### MIDI
- Full clock, note & control support (see iolabs.co.uk/downloads for MIDI guide)
  
---

## Display

- IPS. Mount flat for best viewing.
- Blinking * = coarse mode; ALL = all-steps editing.

---

## Tips & Pitfalls

- **No Triggers?** Check PHAS, COMP, DENS, MASK, and MOD bus assignment.
- **Dropped Triggers:** Lower DENS if slave devices can't keep up.
- **External Sync:** Prefer EXTS clock mode for best DAW/clock integration.
- **CV Outs:** 0–8V range, quantize as needed.
- **Preset Auto-load:** Last loaded/saved preset loads on next power-up.

---

## Reference Links

- [**Official Manual PDF**](https://iolabs.co.uk/flux/Open_Beta_Flux_v1_07_Manual.pdf)
- [**Support/Downloads**](https://iolabs.co.uk/downloads)
- [**Contact**](mailto:flux@iolabs.co.uk)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
