# Nervous Squirrel — Zeno's Paradox

- [Manual PDF](../../manuals/Nervous Squirrel - Zeno's Paradox.pdf)

---

[Zeno's Paradox Manual (PDF)](https://nervoussquirrel.com/zenos_paradox.html)

---

# Zeno's Paradox Eurorack Module — Cheat Sheet

A unique, ultra-high division clock divider and audio mangler.

---

## **Quick Start**

1. **Patch a clock or audio source** into `CLOCK IN` (>1V pulses work, max input ≈ 18kHz).
2. **Patch from any OUTPUT** to send a divided clock (or audio) elsewhere in your system.
3. **Use RESET** to sync/zero all divisions.
4. **Manual Reset Button**: Click to reset/hold all outputs.

---

## **Inputs, Outputs, and Controls Reference**

### **Inputs**
- **CLOCK IN**  
  - Type: CV or Audio  
  - Voltage: Any signal with >1V threshold  
  - Range: Up to ≈18kHz  
  - Accepts: Audio, pulse wave, white noise, gates, clocks

- **RESET IN**  
  - Type: Gate/trigger  
  - Action: Resets divider chain on rising edge

### **Manual Controls**
- **MANUAL RESET BUTTON**
  - Action: Push to (re)start/halt counters (hold to hold outputs low)

### **Outputs**
- **30 Output Jacks**
  - Arrangement: Each output is half the frequency of the previous (binary ripple counter)
  - Output Level: 7V square pulse  
  - Divisions: /2, /4, /8, ... down to /1,073,741,824 (a billion)
  - Each output LED indicates activity

---

## **Usage Tips**

- **Basic Clock Divider:** Great for events at rare intervals (last LED flashes every 34 years at 1Hz!)
- **Sub-Oscillator:** Feed in any repeating audio (produces 1V/octave descending square subharmonics)
- **Audio Mangler:** White noise gives a "filtered noise" cascade; drums sound crunchy/lo-fi divided.
- **Extreme Timing:** Chain multiple modules for astronomical divisions (reset inputs let you sync up).

---

## **Technical Specs**
- **Width:** 14HP  
- **Depth:** 35mm  
- **Current:** +12V 225mA (all LEDs on); –12V 16mA  
- **Output Voltage:** 7V  
- **Panel:** 2mm aluminum

---

> Full manual and purchase info: [https://nervoussquirrel.com/zenos_paradox.html](https://nervoussquirrel.com/zenos_paradox.html)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)