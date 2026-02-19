# Buchla and Tiptop Audio — 266t Source of Uncertainty

- [Manual PDF](../../manuals/Buchla_&_Tiptop_Audio_266t.pdf)

---

[**Download the Manual PDF (Source of Uncertainty - Model 266t)**](https://tiptopaudio.com/manuals/buchla_266t_manual.pdf)

---

# Buchla/TIPTOP Source of Uncertainty 266t – Cheat Sheet

## Overview
The **266t Source of Uncertainty** is a classic random voltage generator with multiple independent sections, ideal for generative and experimental patches. It features several types of noise, fluctuating and quantized random voltages, sample & hold, integrator (slew), and elaborate stepped random voltage generators.

---

## Panel Sections, Jacks & Controls

### **1. Noise Source**
- **Outputs (3)**
  - **Blue Noise:** -3dB/oct, low-frequency biased
  - **Pink Noise:** Flat (equal across frequency)
  - **White Noise:** +3dB/oct, high-frequency biased

### **2. Fluctuating Random Voltages**
- **Inputs**
  - **CV In:** 0–10V, controls rate of fluctuation
- **Outputs**
  - **CV Out:** 0–10V fluctuating random voltage (LED shows rate)
- **Knob**
  - **Rate:** 0.05 Hz (slowest) to 50 Hz (fastest), sets probable voltage change rate

### **3. Sample and Hold**
- **Inputs**
  - **Pulse In:** External clock or trigger (2–10V typical Euro signals)
  - **CV In:** Voltage source to sample (±5V recommended for full range)
- **Outputs**
  - **CV Out:** Sampled/held voltage
  - **Alt:** Alternates sampling to two outputs (ping-pong effect)
- **Notes:** Pulse “Alt” divides incoming clock to alternate outputs

### **4. Integrator (Slew Limiter)**
- **Inputs**
  - **In:** Voltage to smooth (stepped or discrete)
  - **CV In:** 0–10V, controls amount of smoothing
- **Output**
  - **Out:** Slewed/smoothed voltage
- **Knob**
  - **Slew Rate:** 0.01 (none) to 10 (max glide)
- **Trim**
  - **TR1:** (rear trimmer, sets overall smoothing range)

### **5. Quantized Random Voltage**
- **Inputs**
  - **Pulse In:** External clock or trigger
  - **CV In:** 0–10V, controls number of steps
- **Outputs**
  - **n+1 Out:** 5V range, locally scaled (sparser quantization)
  - **2^n Out:** 10V range, evenly distributed
- **Knob**
  - **Steps:** Sets number of voltage steps (1–6)

### **6. Stored Random Voltage**
- **Inputs**
  - **Pulse In:** External clock or trigger
  - **CV In:** 0–10V, controls right output distribution skew
- **Outputs**
  - **Left Out (Linear):** Evenly distributed random 0–10V
  - **Right Out (Skew):** Skewed distribution based on knob/CV
- **Knob**
  - **Distribution Curve:** CCW = low skew, Middle = bell, CW = high skew

---

## Voltage Ranges & General Notes
| Section        | Input Voltage      | Output Voltage  |
|----------------|-------------------|-----------------|
| CV Inputs      | 0–10V typical     |                 |
| Noise Out      |                   | ±5V             |
| Fluctuating    | 0–10V (CV in)     | 0–10V           |
| Sample & Hold  | 2–10V (Trig in)   | ±5V             |
| Integrator     | 0–10V (CV in)     | 0–10V           |
| QRV/SRV Outputs|                   | 0–10V           |

- **Pulses:** Any typical 5V–10V Euro triggers/clocks.
- **CV Inputs:** Respond to unipolar 0–10V (Euro standard).
- **Outputs:** Most outputs are 0–10V, except noise (bipolar).

---

## What Each Section Does
- **Noise:** Raw random voltages, for audio or sample sources.
- **Fluctuating:** Smoothly morphing random voltages.
- **Sample & Hold:** “Freeze frame” sampled value at pulse input.
- **Integrator:** Slew/portamento for incoming steps.
- **Quantized Random:** Stepped random voltages (adjust step count).
- **Stored Random:** Stepped random with variable statistical distribution.

---

### **Physical Specs**
- **Size:** 24 HP
- **Depth:** 25mm
- **Power:** +12V/150mA, -12V/100mA

---

## Useful Patch Ideas
- **Self-generating/random melodies:** S&H/Quantized/Stored sections into pitch or filter cutoff.
- **Generative clocks:** Quantized/Stored into tempo division/multipliers.
- **Automated parameter movement:** Fluctuating random into panning, reverb, etc.
- **Slew beats:** Integrator for smoothed parameter automation.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)