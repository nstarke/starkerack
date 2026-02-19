# Zlob — Triple Cap Chaos

- [Manual PDF](../../manuals/Zlob Modular - Triple Cap Chaos.pdf)

---

[Triple Cap Chaos - Zlob Modular Manual PDF](https://zlobmodular.com/product/triplecapchaos/)

---

# Triple Cap Chaos (C³ Chaos) — Cheat Sheet

## Overview
A unique 2hp analog Eurorack module based on chaotic attractor circuits. Functions as a chaos-based noise oscillator, audio mangler, and pseudo ring modulator/harmonics generator. Not V/oct; focus is on chaotic, unpredictable audio-rate behavior.

---

## Panel Controls & Connections

### Knobs:
- **Emanate**
  - **Coarse control** of chaos intensity.
  - CCW = high activity/chaos
  - CW = more stability/oscillation (up to ~250 Hz).
- **Width / CV ATT**
  - **Fine chaos/oscillation control**.
  - When no CV cable plugged into “CV”: Normal operation.
  - When CV present: Acts as **attenuator** for incoming CV.

---

### Jacks:
#### Inputs
- **IN**
  - **AC-coupled audio input** (also accepts CV).
  - Interacts with the internal oscillator for mangling, pseudo ring-mod, harmonics, or bitcrushing.
- **CV**
  - Expects **±5V max**.
  - Modulates chaos spectrum (affected by Width/CV ATT knob when patched).

#### Outputs
- **X**
  - **Windy/noisy, sinusoidal-based chaotic audio**.
  - ~10Vpp, slight DC offset possible depending on knob settings.
- **Y**
  - **Square/aggressive chaotic audio**.
  - ~10Vpp.

---

## Typical Ranges/Quirks
- **Not 1V/oct tracking** and has a *narrow frequency range*.
- All knobs fully CW: ~150–200 Hz; Emanate full CCW & Width full CW: ~250 Hz.
- Extreme input signals can halt oscillation (go silent).
- Outputs are audio-rate ±5V centered, approx. 10V peak-to-peak.
- **X output**: May have some DC offset variation depending on settings.

---

## Quick Operation Reference

| Control      | Function                                               |
|--------------|-------------------------------------------------------|
| Emanate      | Coarse chaos/osc. spectrum (CCW = more chaos)         |
| Width/CV ATT | Fine chaos/osc. control / CV attenuator if patched    |

| Jack | Type  | Use           | Voltage Range        |
|------|-------|---------------|----------------------|
| IN   | Input | Audio/CV      | AC-coupled           |
| CV   | Input | Chaos Mod CV  | ±5V max              |
| X    | Output| Chaotic audio | ~10V pp (centered)   |
| Y    | Output| Aggressive audio | ~10V pp (centered) |

---

## Extra Tips
- Use both outputs simultaneously for stereo or dual-mono chaos.
- Feed audio into "IN" for unique mangling/folding/ring-mod effects.
- Use CV to modulate chaotic character in real-time.
- The double-sided panel allows visual customization (graphics vs. minimal).

---

### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)