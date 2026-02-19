# Intellijel — Micro VCF

- [Manual PDF](../../manuals/uvcf_manual_2021.08.15.pdf)

---

[µVCF State Variable Filter Manual PDF](https://intellijel.com/downloads/manuals/uVCF.pdf)

---

# µVCF State Variable Filter — CHEAT SHEET

## MODULE OVERVIEW
- **3 Simultaneous Filter Outputs:**  
  - 2-pole (12 dB/oct) Low Pass (LPF)
  - 2-pole (12 dB/oct) High Pass (HPF)
  - 1-pole Band Pass (BPF)
- **Precise 1V/Oct Tracking** (FM1) — Can act as a sine VCO with self-oscillation  
- **Compact (6hp), low noise, easy FM, ideal for smaller racks**

---

## KNOB & CONTROL REFERENCE

| Label         | Type   | Function |
|---------------|--------|----------|
| **FREQ**      | Knob   | Sets filter cutoff frequency. Modulated by FM1 & FM2 inputs. |
| **Q**         | Knob   | Sets resonance. Max = self-oscillating sine (no input needed for sine VCO). |
| **FM2**       | Knob   | Amount & polarity of FM2 CV input. CW = normal; CCW = inverted; noon = off. |
| **Input Atten** | Knob | Attenuates input signal (IN). CW = no attenuation. |
| **FM1 Atten** | Knob   | Attenuates FM1 CV input. CW = no attenuation (standard 1V/oct). |

---

## JACK-IN & OUT SUMMARY

| Jack Label | Type | Description | Voltage Range |
|------------|------|-------------|--------------|
| **IN [A]**   | Audio In  | Filter audio input  | ±5V typical |
| **FM1 [B]**  | CV In     | Cutoff freq. CV; 1V/Oct if full CW on FM1 Atten | ±8V typical, 1V/oct tracking |
| **LPF [C]**  | Audio Out | 2-pole low pass out | ±5V typical |
| **FM2 [D]**  | CV In     | Second cutoff CV; polarity/amount via FM2 knob | ±8V typical |
| **BPF [E]**  | Audio Out | 1-pole bandpass out | ±5V typical |
| **HPF [F]**  | Audio Out | 2-pole high pass out | ±5V typical |

---

## USAGE FLOW

1. **Patch your source** into IN [A]. Adjust Input Attenuator to desired level.
2. **Patch output**:  
   - LPF [C] = low pass  
   - HPF [F] = high pass  
   - BPF [E] = bandpass  
   Take one (or more) to your VCA or mixer.
3. **Set FREQ** to taste.  
4. **Set Q** for resonance. Full CW = self-oscillation, sine oscillator—no input necessary.
5. **Patch CV for modulation** (optional):
   - FM1 [B]: Typical envelope/LFO/pitch, tracks 1V/oct with FM1 Atten fully CW.
   - FM2 [D]: Additional CV, amount/direction as set by FM2 knob.
6. Use white/pink noise as input to demo filter types.

---

## QUICK REFERENCE (TIP SUMMARY)

- **FM1 fully CW:** True 1V/octave tracking, ideal for playing notes or VCO use.
- **Q fully CW, nothing patched to IN:** Sine-wave oscillator (2Hz–20kHz).
- **LPF, HPF, BPF outputs may all be used simultaneously.**
- **Self-resonance = clean, low-distortion sine wave.**

---

### TECHNICAL

- **Width:** 6hp
- **Power:** +12V @ 25mA, -12V @ 24mA
- **Depth:** 21mm

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)