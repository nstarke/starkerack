# Recovery Effects — Bad Comrade

- [Manual PDF](../../manuals/Bad_Comrade_V3_Eurorack_module_manual_Recovery_Effects.pdf)

---

[Bad Comrade V3 Manual (PDF)](https://recoveryeffects.com/products/bad-comrade-v3)

---

# Bad Comrade V3 – Quick Reference Cheat Sheet

**Manufacturer:** Recovery Effects  
**Type:** Glitch / Delay / Distortion Eurorack Module  
**Size:** 4HP, 30mm deep  
**Power Draw:** 20mA  
**URL:** [recoveryeffects.com](https://recoveryeffects.com)

---

## Overview

- **Specialty:** Chaotic delay, freeze, distortion, and glitch FX
- **Unique Features:** Freeze/slice function, voltage control (CV) for MIX and TIME
- **Best Practices:** Power up the module with **GLITCH** and **TIME** knobs turned fully clockwise (wide open).

---

## Controls

| Name     | Type   | Description                                                |
|----------|--------|------------------------------------------------------------|
| MIX      | Knob   | Blend between clean and effected signal (CVable)           |
| GLITCH   | Knob   | Sets noise/clipping threshold (counter-clockwise = higher threshold, more cut/clipping) |
| TIME     | Knob   | Sets delay time (CVable)                                   |
| FREEZE   | Button | Momentary; slices/loops signal at delay time interval      |

---

## Jacks

| Name     | Type | Description                                                        | Voltage Range           |
|----------|------|--------------------------------------------------------------------|------------------------|
| IN       | Input| Audio input                                                        | Modular level audio    |
| OUT      | Output| Audio output (mix of clean/effect as per MIX)                     | Modular level audio    |
| CV MIX   | CV In | External CV for mixing/blending wet/dry signal (overrides MIX knob when patched) | 0–5V                  |
| CV TIME  | CV In | External CV for controlling delay time (overrides TIME knob when patched)         | 0–5V                  |

---

## Basic Operation

1. **Signal Input/Output:**  
   - Patch your signal into **IN** and use **OUT** for the processed audio.
2. **Mix Control:**  
   - Adjust **MIX** knob or patch CV for blending clean and affected signals.
3. **Clipping/Threshold:**  
   - Turn **GLITCH** knob to left for more gating and harsh glitching.
4. **Delay Time:**  
   - Adjust **TIME** for shorter/longer delay. Use CV for modulation/fluctuation.
5. **Freezing:**  
   - Hold **FREEZE** to lock/resample the signal at delay time rate (makes stutter/slice FX).
6. **CV Modulation:**  
   - Patch LFO, envelope, or sequencer to CV MIX and/or CV TIME for dynamic FX.

---

### **Power Up Safety**
- Ensure **GLITCH** and **TIME** knobs are fully clockwise before applying power.

---

## Warranty & Support
- Register within 30 days of delivery for a 1-year limited warranty.
- Support: hello@recoveryeffects.com

---

**Generated With Eurorack Processor:**  
[https://github.com/nstarke/eurorack-processor](https://github.com/nstarke/eurorack-processor)