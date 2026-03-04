# Cute Lab — Mom Jeans

- [Manual PDF](../../manuals/mom-jeans-manual-rev1-1.pdf)

---

[**Mom Jeans User Manual PDF**](sandbox:/mnt/data/MomJeans_Manual_Rev_1.1.pdf)

---

# Mom Jeans (CuteLab) Eurorack Module Cheat Sheet

Pulsar synthesis VCO with unique density and grain-width modulation for advanced digital timbres.

---

## **Panel Controls & Reference**

### **Knobs**
| # | Name     | Function                                              | CV Input (Jacks)    | Voltage Range                                 |
|---|----------|-------------------------------------------------------|---------------------|-----------------------------------------------|
| 1 | Pitch    | Sets base oscillator frequency                        | V/Oct (#14)         | 1V/oct standard, accepts ±V (typically -5V/+5V) |
| 3 | Density  | Adjusts pulsaret grain width (main timbre control)    | Density CV (#4)     | ±5V (typical CV range)                        |
| 6 | Cadence  | Rate of internal density modulation                   | Cadence CV (#11)    | ±5V                                           |
| 7 | Torque   | Mod amount from internal modulator                    | Torque CV (#12)     | ±5V                                           |
|10 | Shape    | Pulsaret waveform selection (sinc→triangle→rectangle→saw variants) | Shape CV (#13)      | ±5V                                           |

### **Buttons & Toggles**
- **2: Range button** – Switches Pitch range:  
    - Normal: 220Hz–880Hz  
    - Extended (LED lit): 27.5Hz–3520Hz
- **8: Coupling toggle** – Quantizes internal mod rate (Cadence) to frequency ratios.
- **9: Quantization toggle** – Quantizes Cadence to stepped values related to pitch.

### **Jacks**
| #  | Type     | Name              | Function                                       | Voltage Range       |
|----|----------|-------------------|------------------------------------------------|--------------------|
|  4 | CV In    | Density           | Modulates grain width                          | ±5V                |
| 11 | CV In    | Cadence           | Modulates modulation rate                      | ±5V                |
| 12 | CV In    | Torque            | Modulates modulation amplitude                 | ±5V                |
| 13 | CV In    | Shape             | Modulates the current waveform                 | ±5V                |
| 14 | CV In    | V/Oct             | Exponential pitch control (1V/oct)             | −/+V, 1V/octetave  |
| 15 | Audio In | Linear FM         | Linear FM input (symmetric Hz mod)             | ±5V/line level     |
| 16 | CV In    | FM Index          | Attenuverts Linear FM amplitude                | ±5V                |
| 17 | Audio In | Sync              | Hard syncs oscillator phase/rate               | 0–5V (typical gate/square) |
| 18 | Audio Out| Square            | Classic square wave (bypasses Shape param)     | ±5V (audio)        |
| 19 | Audio Out| Pulsar            | Main output, full pulsar synthesis tone        | ±5V (audio)        |

*#5 is a Cadence rate indicator LED.*

---

## **Signal Flow & Core Functions**

- **Pitch:** Set and control via knob, range button, and V/Oct CV for musical tracking.
- **Density:** Morphs between classic subharmonic and noise textures by stretching/overlapping grains; main sound-shaping parameter.
- **Cadence (rate):** Speed of the cyclic modulation of density (vibrato or audio-rate), CV controlled.
- **Torque (depth):** Depth/amount of cyclic density modulation, CV controlled.
- **Shape:** Smoothly crossfades through seven waveforms per grain, from soft to bright.
- **Coupling/Quantization toggles:** Force tight/stepped relations between modulation rates and pitch for more musical/organ-like timbres.

---

## **Key Usage Tips**

- **Blend Square and Pulsar outputs** for rich bass or hybrid tones.
- **Extreme Density:** Far min and max produce noisy/rhythmic or digital textures.
- **Coupling/Quant ON:** Maintains consistent pitch and creates stepped, "organ"-like transitions between timbres.
- **Standard VCO use:** Use only Pitch, V/Oct, Linear FM, Sync, and Square Out.
- **Pulsar synthesis:** Use Density, Cadence, Torque, and Shape controls—modulate them for evolving digital sounds.

---

## **Manual Patch Inspirations**

- **Super PWM:** Classic but richer pulse mod—from square and density mod.
- **Pocket Monsters:** Wild digital screeches—modulate pitch/cadence.
- **Ghost Vibes:** Fine/fleeting granular shimmer—fast, gentle density mod.
- **Spelunker:** 8-bit, chirpy digital—low pitch + max density mod + saw/stepped shape.
- **Simple Sinc:** Smooth, sine-like—low shape, varied density for gentle harmonics.
- **Captain Crunch:** Bright, bell-like—pair audio-rate density mod with coupling.

---

**Power:** 10-pin ribbon (2x5), +12V: ~80mA; -12V: ~2mA

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)