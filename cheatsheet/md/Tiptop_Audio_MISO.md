# Tiptop Audio — MISO

- [Manual PDF](../../manuals/Tiptop_Audio_miso.pdf)

---

[Tiptop Audio MISO Manual (PDF)](http://tiptopaudio.com/manuals/MISO%20Manual.pdf)

---

# Tiptop Audio MISO Eurorack Cheat Sheet

**MISO = Mix, Invert, Scale, Offset**  
Utility module for manipulating and combining up to four signals (audio or CV). Two identical sections (Top: 1+2, Bottom: A+B) plus voltage-controlled crossfader.

---

## Inputs, Outputs & Controls

| **Jack/Control**   | **Section**      | **Function**                                                  | **Voltage Range**       |
|--------------------|------------------|---------------------------------------------------------------|-------------------------|
| `1 IN`             | Top (Channel 1)  | Signal input                                                  | ±10V                    |
| `2 IN`             | Top (Channel 2)  | Signal input                                                  | ±10V                    |
| `A IN`             | Bottom (Channel A)| Signal input                                                 | ±10V                    |
| `B IN`             | Bottom (Channel B)| Signal input                                                 | ±10V                    |
| `OUT 1`            | Top (Channel 1)  | Channel 1 processed output                                    | ±10V                    |
| `OUT 2`            | Top (Channel 2)  | Channel 2 processed output                                    | ±10V                    |
| `OUT A`            | Bottom (Channel A)| Channel A processed output                                   | ±10V                    |
| `OUT B`            | Bottom (Channel B)| Channel B processed output                                   | ±10V                    |
| `1+2 OUT`          | Top              | Mix of Top channels (1+2) after processing                    | ±10V                    |
| `A+B OUT`          | Bottom           | Mix of Bottom channels (A+B) after processing                 | ±10V                    |
| `CV`               | Center           | Crossfade control voltage input                               | ±10V (center = 0V)      |
| `Σ (Sigma)`        | Center           | Final Crossfader mix output                                   | ±10V                    |

**Knobs:**
- **Scale/Invert Knob (each channel):**  
  Adjusts gain and inverts signal (center is unity/no invert, left = inverted, right = positive gain)
- **Offset Knob (each channel):**  
  Adds DC voltage (±10V max) to processed signal
- **Crossfade Knob (center):**  
  Manual control of the crossfader (blends between Top and Bottom sections, or can be modulated by CV)

**Indicators:**
- **LED on Mix Out (1+2 & A+B):**  
  Yellow = positive voltage, Red = negative voltage

---

## Quick Reference Summary

- **Each section has two independent channels:** 1/2 (Top), A/B (Bottom).
- **Each channel offers:**  
  - Input jack (accepts CV or audio)
  - Scale/Invert knob: adjusts gain and polarity
  - Offset knob: adds constant voltage
  - Output jack

- **Mix Out**: Outputs the sum of both channels within the section
- **Crossfader**: Blends between Top and Bottom mixes, modulated by center CV or manual knob
- **Sigma (Σ) Output**: Final crossfader output

---

## Typical Patch Examples

- Offset generator: Leave input unpatched, use Offset knob to manually create CV
- Attenuverter: Use Scale/Invert knob to adjust level and invert, pass signal through channel
- Mixer: Use both inputs in a section, summed at Mix Out
- CV crossfade: Send two different modulations into 1+2 and A+B, crossfade between them (manual or CV)
- Complex LFO shaping: Mix and morph LFO shapes using scale, offset, and crossfader

---

## Power & Specs

- **Size:** 10HP, Depth: 42mm
- **Power:** +12V 55mA / -12V 55mA

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)