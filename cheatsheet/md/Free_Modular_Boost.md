# Free Modular — Boost

- [Manual PDF](../../manuals/boost_manual.pdf)

---

**[Boost Free Modular - Manual PDF](manual-link-placeholder)**

# Boost Free Modular Cheat Sheet

A compact reference for quickly using and patching the Boost Free Modular.

---

## Overview
**Boost** is an all-analog module for amplifying and saturating your signal. It combines up to **26dB gain** with musical diode clipping and a sweepable **Tone** control for shaping distortion harmonics. Use it to drive quiet sources to Eurorack levels, add overdrive/distortion, or shape characterful tones.

---

## Controls

| Control | Type | Range/Notes |
|---------|------|-------------|
| **Drive** | Knob | Adjusts gain and clipping: <br> - CCW = Unity gain (no boost)<br> - CW = +26 dB gain (distortion) |
| **Tone** | Knob | High-frequency content: <br> - Left = Tames harsh harmonics<br> - Center = Neutral<br> - Right = Boosts high-end, harsher sound |

---

## Jacks (Inputs/Outputs)

| Jack     | Type   | Voltage/Impedance       | Description                                      |
|----------|--------|------------------------|--------------------------------------------------|
| **Input**  | Audio In | AC-coupled, >1MΩ     | Accepts Eurorack or line-level audio.             |
| **Output** | Audio Out| Up to ~13Vpp (neutral tone), up to rail-to-rail at max high tone | Outputs boosted/clipped signal. |

**No CV (control voltage) or gate inputs/outputs.**  
*Automate distortion amount by placing a VCA before Boost.*

---

## Operational Tips

- **Distortion Amount**: Reduce signal level before Boost (e.g., with VCA) to decrease drive/distortion.
- **Signal Leveling**: Attenuate output after Boost for "distortion only" without loudness increase.
- **Tone Shaping**: Post-clipping EQ with the Tone control to emphasize or cut high-frequency harmonics.
- **Source Use**: Amplifies mics, line signals, or adds drive to modular sources.

---

## Frequency Response

- **Drive at Max:** Output clipped at ~13Vpp (neutral tone). Tone boost can exceed this, causing further harsh distortion.
- **Tone CCW:** Warmer, reduced highs.
- **Tone CW:** Brighter, increased highs and potential to clip harder.

---

## Reference

**Inputs:**  
- Mono audio (AC-coupled, >1MΩ). Handles microphone/line/Eurorack levels.

**Outputs:**  
- Mono audio. Max ~13Vpp (with neutral tone, can go up to power rails with boosted highs).

**Knobs:**  
- Drive (Gain/Distortion)  
- Tone (HF shaping, pre/post clipping)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

*Note: Manual PDF link is placeholder, provide the original PDF link as needed.*