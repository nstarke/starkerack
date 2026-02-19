# Erica Synths — Black Multi Mode VCF

- [Manual PDF](../../manuals/black_multimode_vcf_manual_web.pdf)

---

[Erica Synths Black Multimode VCF Manual (PDF)](https://www.ericasynths.lv/shop/eurorack-modules/by-series/black-series/black-multimode-vcf/)

---

# Erica Synths Black Multimode VCF — Cheat Sheet

**Type:** Multimode Analog VCF  
**Modes:** Simultaneous HP, BP, LP outs  
**Core:** AS3320 (custom multimode chip, made in Riga!)  
**Special feature:** Adjustable germanium diode overdrive on input

---

## Controls & Jacks Overview

### Inputs
| Label          | Type | Description                           | Range       |
| -------------- | ---- | ------------------------------------- | ----------- |
| IN             | Audio| Audio input (apply overdrive via knob)| -           |
| CUTOFF CV      | CV   | Modulates cutoff frequency            | ±5V (10Vpp) |
| RESO CV        | CV   | Modulates resonance                   | ±5V (10Vpp) |

### Outputs
| Label    | Type  | Description                             | Range   |
|----------|-------|-----------------------------------------|---------|
| LP OUT   | Audio | Lowpass output                          | 10Vpp   |
| BP OUT   | Audio | Bandpass output                         | 10Vpp   |
| HP OUT   | Audio | Highpass output                         | 10Vpp   |

### Knobs and Controls

- **CUTOFF**: Manual cutoff frequency
- **RESONANCE**: Manual resonance (will self-oscillate at max)
- **IN/DRIVE LVL**: Audio input/drive control  
  - Up to 12:00 = increasing input level  
  - Past 12:00 = adds germanium diode overdrive
- **C-OFF CV**: Attenuverter for cutoff CV input (bi-polar modulation)
- **RESO CV**: Attenuator for resonance CV input

---

## Quick Operation Guide

1. **Patch Audio Source:**  
   Patch your waveform/signal into **IN (Audio Input)**.

2. **Output Selection:**  
   Use **LP OUT**, **BP OUT**, and/or **HP OUT** simultaneously.

3. **Set Input Gain & Overdrive:**  
   Adjust **IN/DRIVE LVL**.  
   - Below 12 o'clock = clean gain  
   - Above 12 o'clock = overdrive coloration (unique germanium diode circuit)

4. **Shape With Filter:**  
   - **CUTOFF** for frequency sweep  
   - **RESONANCE** for resonance/squelch. Fully clockwise will self-oscillate.

5. **Add Modulation:**  
   - Patch CV into **CUTOFF CV** for filter sweeps (±5V for full sweep, attenuate/bipolar with **C-OFF CV**).
   - Patch CV into **RESO CV** to modulate resonance amount (attenuate with **RESO CV** knob).

6. **Experiment:**  
   Use the outputs in parallel for creative patching (e.g., parallel HP/LP, band splitting, etc).

---

### Voltage Ranges
- **CV Inputs:** ±5V (10V peak-to-peak) for full sweep
- **Audio Outputs:** 10V peak-to-peak

---

## Important Specs

- **Width:** 10HP
- **Depth:** 35mm
- **Power:** +12V: 27mA, -12V: 29mA
- **Skiff-friendly construction**

---

**Pro Tips**
- Use the overdrive for aggressive textures.
- Use external or internal modulation (LFO, envelope, sequencer) for dynamic filter sweeps.
- The self-oscillation mode can be used as a sine wave oscillator.

---

For warranty, maintenance, and more, see Erica Synths [official site](https://www.ericasynths.lv/shop/eurorack-modules/by-series/black-series/black-multimode-vcf/).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)