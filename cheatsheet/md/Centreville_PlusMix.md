# Centreville — PlusMix

- [Manual PDF](../../manuals/PlusMix _ centrevillage.pdf)

---

[PlusMix Manual PDF](https://centrevillage.net/products/PlusMix.html)

---

# PlusMix Eurorack Module Cheat Sheet

**Type:** Utility Mixer (Unity / Precision CV Mixer) with Gate-Controlled Switching  
**Width:** 2 HP  
**Depth:** 35 mm  
**Current Draw:** +12V 20mA / -12V 20mA / +5V 0mA  
**Price:** 9,900 JPY

---

## Panel Reference

### Inputs  
- **PLS1** (Input)  
  - Accepts: Audio or CV  
  - Range: Typical Eurorack level (±5V / ±10V)  
- **PLS2** (Input)  
  - Accepts: Audio or CV  
  - Range: Typical Eurorack level (±5V / ±10V)  
- **BASE** (Input)  
  - Accepts: Audio or CV  
  - Always mixed  
  - Range: Typical Eurorack level  
- **SW1** (Gate Input)  
  - Accepts: Gate/Trig signals  
  - HIGH = ≥ 5V, LOW = 0V  
  - Normalized to 5V when unpatched  
- **SW2** (Gate Input)  
  - Accepts: Gate/Trig signals  
  - HIGH = ≥ 5V, LOW = 0V  
  - Normalized to SW1 when unpatched  

### Outputs  
- **MIX** (Output)  
  - Unity-mixed sum of enabled inputs  
  - Range: Follows input levels (expect unity gain, max ±10V)  

### Controls  
- **SW1PL** (Toggle Switch)  
  - Sets gate polarity for PLS1  
  - **H** (High): PLS1 mixed when SW1 gate is HIGH (≥5V)  
  - **L** (Low): PLS1 mixed when SW1 gate is LOW (0V)  
- **SW2PL** (Toggle Switch)  
  - Sets gate polarity for PLS2  
  - **H** (High): PLS2 mixed when SW2 gate is HIGH (≥5V)  
  - **L** (Low): PLS2 mixed when SW2 gate is LOW (0V)  

---

## Usage Overview

- **BASE** input is always mixed/summed to the output.
- **PLS1** is mixed if:
  - SW1 gate is HIGH (≥5V) **and** SW1PL is in **H**
  - SW1 gate is LOW (0V) **and** SW1PL is in **L**
- **PLS2** is mixed under the same rules using SW2/SW2PL.
- **Manual Mute:** With no gates patched to SW1/SW2, the SW1PL/SW2PL switches work as manual mute toggles.
- **Normalization:**
  - SW1 normalled to 5V → PLS1 can be toggled manually if nothing patched.
  - SW2 normalled to SW1 → Both can be manually toggled or linked.

---

## Application Tips

- **Pitch CV Mixing:** High-precision summing means it's safe for pitch CV without drift.
- **Gate-Controlled Mutes:** Use gate/CV sequencers for dynamic signal routing.
- **Audio Utility:** Seamless for unity-gain audio muting and mixing.
- **Live Performance:** Quick manual mutes via panel switches if no gate signals are inserted.

---

## Quick Reference

| Jack/Control | Description                                      | Voltage Range             |
|--------------|--------------------------------------------------|---------------------------|
| PLS1         | Audio/CV Input 1 (gate-controlled mix)           | ±5V / ±10V                |
| PLS2         | Audio/CV Input 2 (gate-controlled mix)           | ±5V / ±10V                |
| BASE         | Audio/CV Input (always mixed)                    | ±5V / ±10V                |
| SW1          | Gate input for PLS1                              | 0V (LOW), 5V+ (HIGH)      |
| SW2          | Gate input for PLS2                              | 0V (LOW), 5V+ (HIGH)      |
| SW1PL        | Toggle: Mix PLS1 on HIGH (H) or LOW (L) gate     | (Polarity Selector)       |
| SW2PL        | Toggle: Mix PLS2 on HIGH (H) or LOW (L) gate     | (Polarity Selector)       |
| MIX          | Unity gain mix output                            | Follows input levels      |

---

## Links

- [Manual PDF & Product Page](https://centrevillage.net/products/PlusMix.html)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)