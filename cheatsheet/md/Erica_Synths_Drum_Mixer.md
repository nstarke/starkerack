# Erica Synths — Drum Mixer

- [Manual PDF](../../manuals/MIXER_instrukcija_xs.pdf)

---

[**Erica Synths Mixer Manual (PDF)**](https://www.ericasynths.lv/shop/eurorack-modules/by-series/drum-series/drum-mixer/)

---

# Erica Synths Drum Mixer Cheat Sheet

**Overview:**  
The Erica Synths Drum Mixer is a 6-channel audio module designed for summing drum voices in a modular system. Key features include channel compression, effect send/return, and dual outputs.

---

## Inputs / Outputs Reference

| Jack       | Function                                              | Notes / Voltage Ranges     |
|------------|------------------------------------------------------|----------------------------|
| `IN1–IN7`  | Audio Inputs (channel 1–7)                           | ±5Vpp max, input signal is muted when potentiometer is fully CCW |
| `AUX OUT`  | Post-fader / post-comp send output for effects loop   | Audio signal out           |
| `AUX IN`   | Effects return input                                 | Audio signal in            |
| `MAIN OUT` | Main summed audio output (post compressor & effects) | Audio signal out           |

---

## Knobs / Controls Reference

| Control      | Type      | Function                                       | Notes                                                         |
|--------------|-----------|------------------------------------------------|---------------------------------------------------------------|
| `IN1–IN7`    | Potentiometer | Controls input level for corresponding input | Sets gain, provides visual feedback via LEDs, up to ±5Vpp     |
| `COMP AMT`   | Potentiometer | Amount of compression applied                 | Adjusts signal compression to taste                           |
| `RELEASE`    | Potentiometer | Compression release time                      | Sets the release time for compressor                          |
| `SWITCHES`   | Toggle switches | Routes each input to Main output and/or Aux Send | Assigns each channel's signal to main or auxiliary outputs |

---

## LEDs

- **Channel LEDs:** Show visual feedback for input signal level (illuminated when signal reaches ±5Vpp).
- **Clip LED:** Indicates when signal level exceeds headroom, risk of distortion.

---

## Signal Routing Tips

- **Channel Assign:** Use switches per input channel to route to Main output, Aux Send, or both.
- **Compression:** Use COMP AMT and RELEASE to dial in dynamic control across summed channels.
- **Effects Loop:** Patch from AUX OUT to external FX, return to AUX IN. Only channels routed to Aux Send are sent to this path.

---

## Tech Specs
- **Mixer Gain:** Adjustable per channel
- **Max Input Level:** 10V peak-to-peak
- **Headroom:** >20Vpp
- **Depth:** 35mm

---

## Quick/Typical Workflow

1. **Patch** drum/audio sources to `IN1–IN7`.
2. **Set channel levels** with each channel's potentiometer.
3. **Assign outputs** for each channel with toggle switches (Main, Aux, or both).
4. **Optionally compress** the mix with COMP AMT and RELEASE.
5. **Apply FX**: Send to external FX via AUX OUT and return processed audio via AUX IN.
6. **Monitor** the main mix from `MAIN OUT`.

---
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
