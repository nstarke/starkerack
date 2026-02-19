# Omnitone — Rosci

- [Manual PDF](../../manuals/Rosci-Manual.pdf)

---

[**Download the Rosci User Manual (PDF)**](attachment link here)

---

# Rosci Eurorack Module Cheat Sheet (Rev 3)

## Overview
**Rosci** is a voltage-controlled digital oscillator module for Eurorack. It excels at generating customizable waveforms through point manipulation, harmonic enhancement, formant compression, and detuning. Can operate as a VCO (audio rate) or LFO (slow modulation).

---

## Controls & Features

### **Panel Controls**
- **Generate Button**  
  - Generates a new waveform.
  - Used in tuning procedure (see below).

- **Knobs** (can be voltage controlled by CV inputs)
  - **Complexity:** Number of waveform points (2–20).
  - **Roundness:** Interpolation between points.
  - **Harmonics:** Adds up to 6 harmonics.
  - **Formants:** Compress waveform/mimics vowel sounds.
  - **Detune:** Detunes up to a perfect fifth.
  - **Coarse & Fine Tune:** Master pitch tuning.

### **Jumpers (Rear)**
- **VCO/LFO Mode Select:** Move jumper to switch between VCO (20Hz–20kHz) and LFO (0.016Hz–20Hz).

---

## Inputs & Outputs

| Label       | Type    | Description                | Voltage Range        |
|-------------|---------|---------------------------|---------------------|
| V/OCT       | Input   | 1V/oct pitch input        | 0V to +10V*         |
| Complexity  | Input   | CV control, waveform pts  | -10V to +10V        |
| Roundness   | Input   | CV control, interpolation | -10V to +10V        |
| Harmonics   | Input   | CV control, harmonics     | -10V to +10V        |
| Formants    | Input   | CV control, formant amt   | -10V to +10V        |
| Detune      | Input   | CV control, detune amt    | -10V to +10V        |
| OUT         | Output  | Main waveform out         | [Typical Eurorack]  |

\* V/OCT: Typical tolerance ±3 cents.

- All CV inputs are mixed with knob positions. 
- Full sweep of a parameter: 10V.
- Inputs saturate beyond ±10V.

---

## Operation Guide

### **Basic Use**
1. **Patch Output:** Use the OUT jack for audio or modulation signal.
2. **Pitch:** Patch V/OCT for pitch tracking. Use 0V–10V; prefer 2V–8V for best tuning.
3. **Shape:** Shape sound with Complexity, Roundness, Harmonics, Formants, Detune (knobs or CV).
4. **Trigger:** Press Generate to create new waveform.

### **Mode Switch (LFO/VCO)**
1. **Power Off** your system.
2. **Move rear jumper** to “LFO” pins for LFO mode (0.016–20Hz) or “VCO” pins for VCO mode (20Hz–20kHz).
3. **Power On** to use.

### **Tuning Procedure**
1. Set Coarse/Fine tune to minimum.
2. Hold Generate on power up → lights flash red.
3. Send V/OCT 2V (not 0V/10V), press Generate.
4. Lights flash green. Send 2V higher, press Generate.
5. Lights turn multi-color; module exits tuning.

---

## Safety Notes
- Always power off your case when installing or moving Rosci.
- Red stripe on power cable to -12V.

---

## Contact & Support
- [Omnitone.ca](https://omnitone.ca/)
- info@omnitone.ca  
- Instagram: @Omnitone_music

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)