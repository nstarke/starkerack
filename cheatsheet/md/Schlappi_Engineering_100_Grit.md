# Schlappi Engineering — 100 Grit

- [Manual PDF](../../manuals/100_GRIT_MANUAL_20190826.pdf)

---

[Schlappi Engineering 100 Grit Manual (PDF)](https://schlappiengineering.com/100grit-manual.pdf)  
*(Manual also available via Schlappi Engineering website)*

---

# **Schlappi Engineering 100 Grit Cheat Sheet**

## **Module Overview**
- Analog filter-based distortion/VCA with touch points for chaotic interaction.
- Based on a transistor ladder low-pass filter, OTA VCA, and distortion circuit.
- 8 Touch Points for “circuit bending”-like performance.

---

## **Panel Controls & Functions**

### **Knobs**
- **IN 1 / IN 2**: Audio input gain for each input.
- **FREQUENCY (large center knob)**: Filter cutoff frequency.
- **FM 1 / FM 2 (with CV pots under each)**: Control cutoff via external CV.
- **RES**: Filter resonance.
- **RES CV (with CV pot under RES)**: External CV to resonance.
- **GAIN**: Output/VCA gain and distortion amount.
- **GAIN CV (with CV pot under GAIN)**: External CV to gain stage.

### **Switches**
- **Gain x100**: Massive distortion/feedback switch.

---

## **Input, Output, & Touch Point Reference**

### **Audio Inputs**
| Jack        | Voltage Range | Notes                                        |
|-------------|--------------|----------------------------------------------|
| **IN 1**    | ±12V (24Vpp) | Main audio in (mixes to filter).             |
| **IN 2**    | ±12V (24Vpp) | Second audio in (mixes to filter).           |

### **CV Inputs**
| Jack        | Voltage Range | Function                                    | Normalling/CV Action                        |
|-------------|--------------|---------------------------------------------|---------------------------------------------|
| **FM 1**    | ±12V         | Filter cutoff CV (sums w/ FM 2).            | Norm: DIST (distortion output FM).          |
| **FM 2**    | ±12V         | Filter cutoff CV (V/Oct okay for tracking). | -                                           |
| **RES CV**  | ±12V         | Resonance CV.                               | Norm: DIST (audio-rate resonance mod).      |
| **GAIN CV** | ±12V         | VCA gain and distortion depth.              | Norm: POLE 2 (second filter pole out FM).   |

- *Unity gain at 5V for GAIN and RES CV. Higher voltage = more gain.*

### **Audio Outputs**
| Jack  | Voltage Range | Source                                  |
|-------|---------------|-----------------------------------------|
| **OUT**  | up to ±11V  | Post-filter, pre-distortion (VCA/clean). |
| **DIST** | ~±6V        | Distortion circuit output.              |

---

### **Touch Points**
- **Eight brass balls** (shown in touch point map).  
- Each is a direct circuit node for “patching” with fingers, cables, clips, or conductive objects.
- Used for chaotic control and feedback.

#### **Touch Point Functions (Clockwise from top left)**
**Left Set:**
- DIST 2 OUT – Second distortion circuit out (audio).
- GAIN CV – VCA gain CV node.
- DIST 2 AMP PIN – Dist 2 amp core (capactive/feedback).
- RES CV – Resonance CV node.

**Right Set:**
- DIST 1 AMP PIN – Dist 1 amp core.
- FREQ CV – Filter cutoff CV node.
- DIST OUT – Main distortion out.
- GAIN CV – Same as left.

---

## **Headers (Jumpers)**
- **J9: Input to Resonance** – ON by default. Removes “bass drop” at high resonance. Remove for classic, whistling, self-oscillation style resonance.
- **J10: Output Source** – Default right two pins (“VCA” output, OUT is post-VCA). Move to left pins for filter direct output.

---

## **Calibration**
- **RV3: Resonance Amplitude** – Sets self-oscillation threshold.
- **RV4/RV8: Symmetry** – Factory adjusted; do not touch.

---

## **Typical Patch Setups**

### **VCF/VCA**
- Audio In via IN 1, monitor OUT.
- GAIN above 75%: heavy distortion.
- ADD Env to GAIN CV for VCA.
- V/Oct to FM 2 = pitch tracking.

### **Distortion**
- Monitor DIST output.
- GAIN and GAIN CV = distortion level.
- Use RES CV for unique feedback sounds.

### **Noise Box**
- No input; monitor DIST out.
- All knobs ~25-60% up.
- Play touch points for chaotic noise.

---

## **Extra Notes**
- **All CV/audio inputs:** Protected to ±12V (rails).
- **Touch Points:** Safe to bridge/patch, always current-limited.

---

## **Voltage Reference**
- **Nominal input signals:** ±5V (10Vpp), but up to ±12V is fine.
- **OUT:** up to ±11V, rails possible with hot input/gain.
- **DIST:** Up to ~±6V (clipped/limited by circuit).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)