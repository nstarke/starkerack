# WMD SSF — Crater

- [Manual PDF](../../manuals/Kick_Manual.pdf)

---

[Crater Manual PDF (image reference)](#)

---

# WMD Crater – Eurorack Cheat Sheet

**Category:** Hybrid Kick Drum Synth Voice  
**Size:** 8hp  
**Audio Output Range:** 20Vpp  
**CV Inputs Impedance:** 100kΩ

---

## Panel Controls

### Knobs
- **PITCH**: Sets kick oscillator pitch (5Hz–100Hz)
- **SATURATION**: Controls boost & saturation *before* clipping; accepts CV ±5V
- **CLICK LEVEL**: Click volume
- **CLICK TIMBRE**: Selects among 14 click samples, each with noise tail
- **DECAY**: Kick oscillator decay time (affects tail; sustains while TRIGGER is high, decays when released)
- **CLICK DECAY**: Click/noise tail decay time
- **SUSTAIN**: Sets sustain level of oscillator (use gates or sequences for basslines)
- **PITCH ENVELOPE – AMOUNT**: Depth of pitch envelope applied to the oscillator
- **PITCH ENVELOPE – DECAY**: Pitch envelope decay

### Toggles / Switches
- **CLIPPING (3-position toggle):**
  - Left: Off (no clipping)
  - Middle: Moderate clipping, fades to clean
  - Right: Max (diode) clipping—hard distortion

---

## Inputs

| Jack         | Type           | Details                                      | Voltage Range / Thresh.         |
|--------------|----------------|----------------------------------------------|-------------------------|
| **TRIGGER**  | Gate In        | Triggers the kick                            | 2V threshold (Schmitt Trigger) |
| **ACCENT**   | Gate In        | Triggers accent (plug in alone for always-accented) | 2V threshold           |
| **1V/OCT**   | CV In (pitch)  | Standard pitch tracking (kick FM / melodies) | 1V/octave               |
| **SATURATION CV** | CV In | Modulates saturation (attenuates signal with negative CV) | ±5V typical            |
| **CLICK LVL CV** | CV In   | Controls click level remotely                 | ±5V typical             |
| **DECAY CV** | CV In (kick)   | Modulates kick decay time                    | ±5V typical             |
| **CLICK DECAY CV** | CV In | Click/noise tail decay modulation             | ±5V typical             |
| **SUSTAIN CV** | CV In        | Modulates sustain level                      | ±5V typical             |
| **PITCH ENV DECAY CV** | CV In | Modulates pitch envelope decay              | ±5V typical             |
| **PITCH ENV AMOUNT CV** | CV In | Modulates pitch envelope amount            | ±5V typical             |

---

## Outputs

| Jack           | Type         | Details                  | Voltage Range         |
|----------------|--------------|--------------------------|----------------------|
| **AUDIO OUT**  | Audio Out    | Main output; kick, click | 20Vpp max, 220Ω      |

---

## Usage Tips

- **LED Display:** Shows visual impact of kick
- **SUSTAIN for Basslines:** Hold triggers/gates for sustained 808-style bass; sequence 1V/oct for melodic kicks
- **Accent Input:** Plug in for louder or modified kicks, or use for always-accented hits
- **CLIPPING Modes:** Middle for moderate, right for max/gabber, left for clean
- **CV Modulation:** Most controls have CV inputs (±5V recommended); respond to external envelopes, LFOs, or sequencers
- **SATURATION Order:** Saturation occurs before clipping; use to shape distortion response
- **CLICK Section:** Adjust decay and timbre for punchy or metallic attacks

---

## Reference Specs

- **Size:** 8hp
- **Depth:** (with cables)
- **CV Inputs:** 100kΩ impedance
- **Gate Inputs:** 100kΩ, 2V threshold (Schmitt Trigger)
- **Audio Output:** 220Ω, 20Vpp max

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)