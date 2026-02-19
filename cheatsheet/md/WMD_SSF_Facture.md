# WMD SSF — Facture

- [Manual PDF](../../manuals/manual_black_fracture.pdf)

---

[Download the WMD Fracture Manual (PDF)](https://wmdevices.com/pages/fracture)

---

# WMD FRACTURE - CHEAT SHEET

**Multi-Particle Percussion Synthesizer**

## Quickstart
- TRIG input = Play burst (applause, claps, snare, etc.)
- Use SURFACE knob to select "what's being hit" (23 types).
- Tweak DENSITY to increase/reduce the amount of particles.
- DECAY controls burst length (pair with TAIL for shape).
- PUNCH and FREQ sculpt/filter/tune the burst.
- SPREAD randomizes pitch and panning.
- REVERB for additional space.
- INF: Sustains particle stream until Density is changed.

---

## Controls At-A-Glance

### Knobs
| Name     | Function                                                      | CV Input (Range) |
|----------|---------------------------------------------------------------|------------------|
| DENSITY  | Particle generation rate.                                     | 0–5V             |
| SURFACE  | Selects among 23 particle/sample types.                       | 0–5V             |
| DECAY    | Burst length (with TAIL for shape).                           | 0–5V             |
| FREQ     | Alters burst spectrum/pitch or bandpass filter.               | 0–5V             |
| SPREAD   | Randomizes pitch + panning.                                   | 0–5V             |

### Toggles/Switches
- **TAIL** (3 positions): Selects amplitude/probability/combination for burst shape
    - I: Amplitude envelope
    - II: Amplitude & probability
    - III: Probability only
- **PUNCH** (3 positions): Selects filter/pitch processing
    - I: Bandpass post-engine
    - II: Filter + pitch (FREQ = both)
    - III: Parallel bandpass & pitch (extra punch)
- **INF (Infinite)**: Hold for endless particle stream. Press TRIG or DECAY to "burst" density.

### Other Controls
- **REVERB**: Toggles between Room and Hall reverb types.
- **TRIG**: Fires a burst.
- **ACC**: Accents burst (with high TICK).
- **TICK**: Triggers single particle sample.

---

## Jacks Reference

### Inputs
| Jack   | Function                                     | Impedance | Voltage / Type            |
|--------|----------------------------------------------|-----------|---------------------------|
| TRIG   | Burst trigger input                          | 100kΩ     | Gate, 2V Schmitt Trigger  |
| ACC    | Accent input                                 | 100kΩ     | Gate                      |
| TICK   | Single particle trigger                      | 100kΩ     | Gate, 2V Schmitt Trigger  |
| DENSITY| Controls Density                             | 100kΩ     | 0–5V CV                   |
| SURFACE| Selects Surface/sample type                  | 100kΩ     | 0–5V CV                   |
| DECAY  | Controls Decay                               | 100kΩ     | 0–5V CV                   |
| FREQ   | Controls frequency/filter                    | 100kΩ     | 0–5V CV                   |
| PITCH  | Pitch control (overrides FREQ pitch section) | 100kΩ     | 0–5V CV                   |
| SPREAD | Controls Spread                              | 100kΩ     | 0–5V CV                   |

### Outputs
| Jack   | Function            | Impedance | Voltage         |
|--------|---------------------|-----------|-----------------|
| OUT L  | Left audio/Mono     | 220Ω      | 20Vpp max       |
| OUT R  | Right audio         | 220Ω      | 20Vpp max       |

---

## Essential Notes
- All CV inputs **sum with the corresponding knob**.
- Burst pitch variance & panning: Use SPREAD and/or PITCH input.
- PITCH input disables FREQ’s pitch effect—use for full external control.
- All triggers/gates fire on rising edge above 2V.
- Use OUT L alone for mono operation.
- Max audio output voltage: **20Vpp**.
- Latency: **≤1.0ms**

---

### Example Patch (Claps → Applause)
1. Patch gate from sequencer to TRIG.
2. Patch L+R OUT to two mixer channels.
3. Set SURFACE to center for classic claps. DENSITY low-medium, short DECAY.
4. Crank DENSITY + DECAY + SPREAD for crowd applause. Try INF mode!

---

## Specs
- Size: 8hp, 38mm deep (with cables)
- Power: +61mA / -17mA

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)