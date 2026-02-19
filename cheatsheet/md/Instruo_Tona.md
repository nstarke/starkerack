# Instruo — Tona

- [Manual PDF](../../manuals/Tona-Manual-A5.pdf)

---

[**Download the Instruō tòna User Manual (PDF)**](sandbox:/mnt/data/tòna%20Oscillator%20User%20Manual.pdf)

---

# Instruō Tòna Cheat Sheet

**Type:** All-analog VCO with classic waveforms + analog wavefolder  
**Form factor:** 12HP Eurorack  
**Power:** +12V: 40mA, -12V: 40mA  
**Depth:** 27mm

---

## I/O Jack Reference

### Outputs
| Label           | Type           | Description                         | Typical Voltage Swing |
|-----------------|----------------|-------------------------------------|----------------------|
| Square          | Output         | Square waveform                     | ±5V                  |
| Sawtooth/Ramp   | Output         | Sawtooth/ramp waveform              | ±5V                  |
| Triangle        | Output         | Triangle waveform                   | ±5V                  |
| Sine            | Output         | Sine waveform                       | ±5V                  |
| Wavefold        | Output         | Folded sine via wavefolder          | ±5V                  |

### Inputs
| Label             | Type            | Description                                              | Voltage Range           | Notes                                 |
|-------------------|-----------------|----------------------------------------------------------|--------------------------|---------------------------------------|
| 1V/Oct            | CV Input        | V/oct pitch tracking                                     | -∞ to +∞                | 1V per octave standard                |
| Linear FM         | CV Input        | Linear FM on pitch                                       | -5V to +5V (typical)    | Bipolar, summed with Coarse/Fine      |
| Sync              | Gate/Trig Input | Hard sync input - resets oscillator on rising edge        | >2.5V triggers          | Use sharp-edged signals (square/ramp) |
| Wavefold CV       | CV Input        | CV control of Wavefolder amount                          | -5V to +5V (typical)    | Bipolar, summed with fader            |

---

## Knobs, Sliders, and Controls

| Control                | Type    | Function                                                                 |
|------------------------|---------|--------------------------------------------------------------------------|
| Coarse                 | Knob    | Sets base oscillator frequency (pitch)                                   |
| Fine                   | Knob    | Fine adjustment of pitch, relative to Coarse                             |
| Linear FM Attenuator   | Knob    | Attenuates depth of Linear FM input                                      |
| Wavefold Fader         | Slider  | Amount of wavefolding (left = pure sine, right = fully folded)           |
| Wavefold CV Attenuator | Knob    | Attenuates depth of Wavefold CV input                                    |

---

## QUICK REFERENCE PATCHING

### Basic Oscillator Out
- **Connect:** Any waveform output to your mixer/audio path.
- **Pitch Control:** 1V/Oct input from sequencer/keyboard.

### Wavefolded Out
- **Connect:** Wavefold output for timbre-rich, West Coast flavor.
- **Tweak:** Wavefold fader/slider for amount; modulate with Wavefold CV for e.g., audio-rate timbre modulation.

### Sync
- **Apply:** Connect another oscillator’s ramp/square to Sync for hard sync tones.

### Linear FM
- **Complex timbres:** Feed another oscillator (audio rate preferred) to Linear FM input, set depth with FM Attenuator.

---

## MODULATION/CV RANGES
- All CV inputs respond to bipolar signals (±5V typical).
- Sync triggers on rising edge >2.5V.
- Waveoutput swing: approximately ±5V.

---

## DESCRIBED PATCH IDEAS

- **East Coast Voice:**  
  Mix square, saw, triangle > filter > VCA; envelope CV sweeps filter/VCA; 1V/Oct input from sequencer/keyboard.
- **FM Voice:**  
  Use sine from a 2nd oscillator to tòna’s Linear FM in for FM timbres.
- **Audio-Rate Wavefold Mod:**  
  Patch any output back to tòna’s own Wavefold CV input to modulate timbre with its own waveform.

---

## PANEL DIAGRAM LEGEND

1. Square Out  
2. Saw/Ramp Out  
3. Triangle Out  
4. Sine Out  
5. Wavefold Out  
6. Coarse knob  
7. Fine knob  
8. 1V/Oct Input  
9. Linear FM Input  
10. Linear FM Atten.  
11. Wavefold Fader  
12. Wavefold CV Input  
13. Wavefold CV Atten.  
14. Sync Input

---

### Notes
- Reverse polarity protected.
- All controls are additive: CV is summed with manual settings.
- For all classic and experimental analog VCO & West Coast patches!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)