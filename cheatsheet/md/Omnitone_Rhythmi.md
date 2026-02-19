# Omnitone — Rhythmi

- [Manual PDF](../../manuals/Rhythmi_Information_Package.pdf)

---

**[Rhythmi Manual PDF - Download Link](#)**  
*(Replace with the actual URL if available, as it was not provided in your upload.)*

---

# Rhythmi Eurorack Drum Sequencer — Cheat Sheet

### Quickstart
- **Power up, patch outputs to your drum voices.**
- **Dial in your groove using 'Density' and 'Synco' for each part.**
- **Explore new rhythmic variations by adjusting 'Evolve'.**
- **Shape fills and drive with 'Energy.'**
- **Set loop length, swing, and clock division/multiplication as needed.**

---

## Section Reference

### Input/Output Jacks

| Jack         | Type       | Function                                                                   | Voltage Range          |
|--------------|------------|----------------------------------------------------------------------------|------------------------|
| In           | Input      | External clock input                                                       | Standard clock level   |
| Reset        | Input      | Resets pattern to start                                                    | Gate/trigger           |
| Out          | Output     | Master clock output (follows int/ext clock, division, and swing)           | 0–5V trigger/gate      |
| KICK         | Output     | Kick drum trigger                                                          | 0–5V pulse             |
| SNARE        | Output     | Snare drum trigger                                                         | 0–5V pulse             |
| TOM          | Output     | Tom drum trigger                                                           | 0–5V pulse             |
| TOM CV       | Output     | Tom pitch - 1v/oct quantized minor pentatonic                              | 0–5V (1V/octave)       |
| CRASH        | Output     | Crash drum trigger                                                         | 0–5V pulse             |
| HI-HAT       | Output     | Combined Closed/Open hat: gate = open, short trigger = closed              | 0–5V trigger/gate      |

> *No explicit CV inputs other than for 'Evolve' randomization (see below).*

---

### Knobs, Buttons, and Sliders

| Control          | Type      | Section      | Description                                                                                       |
|------------------|-----------|--------------|---------------------------------------------------------------------------------------------------|
| Encoder (Main)   | Knob/Push | Global       | Loop length (press for base pattern change), evolve (turn), press evolve for variation randomize   |
| Speed Encoder    | Knob      | Clock        | Internal clock speed; Divider/multiplier if external clock in                                      |
| CHH / OHH        | Knob      | Customize    | Adjust density/syncopation for closed/open hi-hat                                                  |
| Synco            | Knobs     | Customize    | Set syncopated:non-syncopated ratio for each piece                                                 |
| Density          | Knobs     | Customize    | Total number of hits for each piece                                                                |
| Tom Amount       | Knob      | Customize    | How many pitches for tom                                                                           |
| Length           | Encoder   | Global       | Loop length in pulses (2–32)                                                                       |
| Energy           | Knob      | Global       | Macro: increases kick/snare/tom density & syncopation; enables crash/fill at top end               |
| Evolve           | Encoder   | Global       | Morph between rhythmic variations; randomize via push/CV                                           |
| Swing            | Knob      | Global       | Moves every 2nd pulse between 50–90% offset (0 = no swing)                                         |
| Progress LEDs    | Lights    | Global       | Pattern progress; color shows base pattern                                                         |
| Vertical LEDs    | Lights    | Clock/Global | Show clock speed, division, energy/cursor/red = fill/crash fired, animations                       |

---

### CV Control & Special Operations

- **Evolve CV randomization:**  
  - Hold 'Speed Encoder' + press 'Evolve Encoder' (LEDs green).  
  - CV above 75% = pattern randomizes (vertical LEDs animate).  
  - Repeat combo (LEDs red) to disable.  
- **State Save:** Pausing clock saves all key state to internal memory.

---

## Rhythmic Logic

- Density + Synco = “Root Rhythm” (when Evolve/Energy at min).
- Evolve = morph between root and randomized preset variations (smooth, persistent).
- Swing = moves every 2nd clock hit to create shuffle/groove.
- Energy at max = adds crash+kick at loop head, crash output can be used as a global reset/trigger.

---

## Tips

- **HI-HAT OUT:** Patch to VCA envelope for length control—gate = open, trigger = closed.
- **Base Patterns:** Long-press main encoder to swap feel (color in LEDs).
- **Tom Pitch:** TOM CV out is 1V/oct, minor pentatonic, range set by 'Tom Amount.'
- **Fills:** Energy up = more fills/variation at loop end.

---

## Reference Links

- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
