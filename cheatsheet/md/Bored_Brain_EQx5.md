# Bored Brain — EQx5

- [Manual PDF](../../manuals/EQx5-UserGuide_1.0.pdf)

---

[📄 eqx5 Manual PDF](https://boredbrainmusic.com/wp-content/uploads/eqx5_UserGuide.pdf)

---

# eqx5 (boredbrain) - Cheat Sheet

## Quick Overview

**eqx5** is a 5-band voltage-controlled equalizer (Eurorack format), providing CV control and manual adjustment over each band and overall output level. Ideal for dynamic spectral shaping, filter sweeps, coloring, and stereo or feedback applications.

---

## Controls Reference

### Sliders: Frequency Band GAIN (per band: BASS, LOW-MID, MID, HI-MID, TREBLE)
- **Range:** -10 dB to +10 dB (center is flat)
- **Function:** Adjusts boost/cut for each band.

### Sliders: CV Amount (per band: blue slider)
- **Range:** -10 dB to +10 dB control via external CV.
- **Function:** Sets sensitivity of CV input.
- **Sum:** Manual slider + CV+slider.

### SLIDER: LEVEL
- **Range:** -∞ (full down/off) to +6 dB (full up)
- **Function:** Output volume.

---

## Inputs & Outputs

### Audio
- **IN L / IN R:**  
   - **Type:** Mono (left) or Stereo (both)
   - **Impedance:** 100k ohms

- **OUT L / OUT R:**  
   - **Type:** Stereo output  
   - **Level:** Eurorack standard

### CV Inputs (per band)
- **CV1 (BASS), CV2 (LOW-MID), CV3 (MID), CV4 (HI-MID), CV5 (TREBLE)**
  - **Voltage Range:** -5V to +5V = -10dB to +10dB boost/cut  
  - **Recommended Range:** ±5V (higher voltages will be clipped internally)  
  - **Function:** Modulates band gain, scaled by blue CV slider.

---

## Internal Signal Path

- **All bands** are fully parametric and analog, offering up to ±10dB cut/boost.
- **Bands:**  
    1. **BASS** (75Hz, 1.2 Q)  
    2. **LOW-MID** (350Hz, 1 Q)  
    3. **MID** (1100Hz, 1 Q)  
    4. **HI-MID** (3500Hz, 1 Q)  
    5. **TREBLE** (9000Hz, 1 Q)

- **CV IN** modulates band in addition to the manual slider.

---

## Usage Basics

1. **Patch audio** into IN L (mono) or IN L+R (stereo).
2. **Adjust each frequency band** using the main sliders.
3. **Patch modulation (LFOs, Envelopes, etc.)** into any CV IN jack to control boost/cut for that band.
4. **Set CV amount** with blue CV slider: zero = no CV, up/down matches manual slider scale.
5. **Set output level** with LEVEL slider.
6. **Patch OUT L/R** to next module or main output.

---

## Voltage Reference Table

| Input/Output         | Range           | Purpose          |
|----------------------|-----------------|------------------|
| IN L / R             | Audio (modular) | Signal input     |
| OUT L / R            | Audio (modular) | Equalized output |
| CV1–CV5 (per band)   | -5V to +5V      | Band boost/cut   |

---

## Notes

- **No other controls:** This module uses only sliders.
- **Stereo/dual mono:** Can use with mono or stereo, or process two mono signals in parallel (no cross-talk).
- **CV Summing:** CV is added to manual; use both for maximum effect.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)