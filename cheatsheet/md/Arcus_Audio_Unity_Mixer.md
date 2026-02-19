# Arcus Audio — Unity Mixer

- [Manual PDF](../../manuals/Unity Mixer - Arcus Audio.pdf)

---

**[Unity Mixer Manual PDF](https://arcusaudio.com/product/unity_mixer/)**

---

# Unity Mixer (Arcus Audio) – Cheat Sheet

### Overview
- **Type**: Dual 3:1 Unity Gain Mixer (Can act as single 6:1)
- **Size**: 2HP (0.4”)
- **Function**: Sums up to 3 signals per mix (2 mixes), or 6 into 1 if chained
- **Signals**: Audio or CV
- **Indicators**: Bi-color LEDs per output show level & polarity

---

## **Jack Reference**

| **Jack**    | **Type**       | **Description**                     | **Voltage Range**   |
|-------------|----------------|-------------------------------------|---------------------|
| IN 1.1–1.3  | Input          | Inputs to Mixer 1 (DC coupled)      | -∞ to +∞ (limited by power rails, typical for Eurorack ~±10V) |
| OUT 1       | Output         | Output for Mixer 1 with LED         | Follows summed input |
| IN 2.1–2.3  | Input          | Inputs to Mixer 2 (DC coupled)      | -∞ to +∞ (±10V suggested) |
| OUT 2       | Output         | Output for Mixer 2 with LED         | Follows summed input |
> *Note*: To use as 6:1 mixer, patch OUT 1 into an input of mixer 2.

---

## **Controls / Indicators**

| **Control / Indicator** | **Type**     | **Function**                          |
|------------------------|--------------|----------------------------------------|
| OUT 1 LED              | Bi-color LED | Shows level and polarity for OUT 1 (Green = positive, Red = negative voltage) |
| OUT 2 LED              | Bi-color LED | Shows level and polarity for OUT 2 (Green = positive, Red = negative voltage) |

> **No knobs, buttons, switches, or sliders.**  
> All mixing is performed at unity gain (no level controls).

---

## **Installation & Specs**

- **Mounting**: 2HP width, M3 x 6mm screws included, aluminum faceplate
- **Power**: 10" power cable included  
    - +12V: 15 mA  
    - -12V: 15 mA  
    - +5V: 0 mA
- **Input Impedance**: 10 kΩ (DC coupled)

---

## **Typical Usage**

- **Summing audio or CV sources** (e.g. mix 3 VCOs, or sum several LFOs/envelopes into one bus).
- **Dual 3-to-1 Mixer:** Use both sections independently.
- **Single 6-to-1 Mixer:** Chain OUT 1 to an IN of Mixer 2.
- **Polarity/Loudness Indication:** LEDs give instant feedback for troubleshooting or creative applications.

---

## **Quick Patching Guide**
1. **Patch up to 3 sources** to each group of inputs (IN 1.1–1.3 or IN 2.1–2.3).
2. **Take summed output** from OUT 1 or OUT 2.
3. **Chain modes:** To combine all 6 inputs, patch OUT 1 into any input of mixer 2, take OUT 2 as final sum.
4. **Watch the LEDs:** Green = positive voltages dominate, Red = negative.
---

*No normalization or advanced controls – simple utility for clean, compact summing with visual feedback.*

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)