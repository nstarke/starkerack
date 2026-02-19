# Intellijel — Unity

- [Manual PDF](../../manuals/unity-mixer_manual_2020.04.15.pdf)

---

[**Intellijel Unity Mixer Manual (PDF)**](https://intellijel.com/downloads/manuals/Intellijel_Unity_Mixer_Manual_2020.pdf)  
*(Assuming the manual reflects the attached content)*

---

# Intellijel Unity Mixer Cheat Sheet

**Type:** Dual 3:1 / 6:1 Unity Gain Mixer  
**HP:** 2hp  
**Function:** Mixes audio or CV signals with no attenuation or amplification (unity gain).  
**Current Draw:** 11mA @ +12V; 14mA @ -12V  
**Max Output Voltage:** ±10.5V

---

## Panel Overview

| Jack | Label (from top to bottom) | Function                                              |
|------|---------------------------|-------------------------------------------------------|
| 1    | IN 1                      | Top mixer input 1 (audio or CV, ±10.5V max)           |
| 2    | IN 2                      | Top mixer input 2 (audio or CV, ±10.5V max)           |
| 3    | IN 3                      | Top mixer input 3 (audio or CV, ±10.5V max)           |
| 4    | OUT 4                     | Top mixer output (sum of IN 1, IN 2, IN 3)            |
| 5    | IN 5                      | Bottom mixer input 1 (audio or CV, ±10.5V max)        |
| 6    | IN 6                      | Bottom mixer input 2 (audio or CV, ±10.5V max)        |
| 7    | IN 7                      | Bottom mixer input 3 (audio or CV, ±10.5V max)        |
| 8    | OUT 8                     | Bottom mixer output (sum of IN 5, IN 6, IN 7, and—if OUT 4 is unpatched—also the sum from top mixer, for up to 6:1 mixing) |

> **No knobs, buttons, sliders, or toggles are present on this module.**

---

## Connection Reference

- **Inputs:** Accept either audio or CV within ±10.5V range.
- **Outputs:** Clip at ±10.5V if input sum is higher.

### Dual Mixer Mode
- [1], [2], [3] → summed to [4]
- [5], [6], [7] → summed to [8]
- Use as two independent 3:1 summing mixers.

### 6:1 Mixer Mode
- If [4] is unpatched, both sums ([1]+[2]+[3]+[5]+[6]+[7]) appear at [8].
- Useful for summing up to 6 audio or CV signals to a single output.

---

## Special Features

### Attenuation Jumpers (On Rear PCB)
- Per-mixer -6dB option, set via circuit board jumper.
- Useful for giving extra headroom if using hot signals (e.g. raw VCOs).
- **-6dB attenuates summed output by half.**
- *Access by removing the module from case; see manual page 5 for layout.*

---

## Usage Tips

- Use for merging CV or audio without needing per-channel level control.
- Works well after/with dedicated attenuators (e.g., Intellijel Triatt/Quadratt).
- If lacking mix headroom, set rear jumper to -6dB for either section.

---

## Quick Reference

- **Inputs/Outputs:** Accepts/buffers both audio and CV, ±10.5V max
- **Output headroom:** +10.5V to -10.5V before clip
- **Attenuation:** Optional rear jumper for -6dB per section
- **No local panel controls**

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)