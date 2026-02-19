# Schlappi Engineering — Angle Grinder

- [Manual PDF](../../manuals/angle_grinder_manual_20181022.pdf)

---

[**PDF Manual**](https://schlappiengineering.com/anglegrinder/AngleGrinderManual.pdf)

---

# Schipp Engineering ANGLE GRINDER Cheat Sheet

A powerful eurorack quad oscillator / filter / waveshaper.

---

## **Quickstart Modes**

| **Mode**  | **How To** |
|-----------|-------------------|
| **Quad Oscillator (SPIN)** | GRIND→SPIN full CCW, DAMPING full CCW, Input unpatched, set sliders/GRIND to taste |
| **Waveshaping (GRIND)** | Patch signal to IN, monitor GRIND OUT, blend with sliders/GRIND CV, try SPIN oscillating or as LFO |
| **State Variable Filter** | Patch signal to IN, turn up GRIND→SPIN (CW), DAMPING to taste, SPIN outputs become LP/BP/HP/Inv BP |

---

## **Inputs & Outputs**

### **Inputs**
| Jack      | Function | Voltage Range |
|-----------|--------------------------|--------------|
| **IN**           | Audio/CV input to GRIND section | Typical Eurorack audio/CV levels |
| **INJECT**      | Direct input to SPIN core (bypasses GRIND), header-selectable AC/DC coupling | Audio/CV, AC default, spikes for soft sync in AC mode |
| **V/OCT**       | Exponential 1V/oct for SPIN pitch | 0-5V (tracks 4+ octaves) |
| **FM1**         | FM input for SPIN (linear/exponential selectable by rear jumper) | ? |
| **FM2**         | Additional exponential FM input for SPIN | ? |
| **GRIND CV 1-4**  | CV over GRIND VCA per stage (added to corresponding slider) | 0–5V unipolar |

### **Outputs**
| Jack     | Function | Voltage Range|
|----------|-----|----|
| **GRIND OUT**        | Output of GRIND waveshaping/mixing section | Up to ±11V (22Vpp, not limited) |
| **SPIN (0°, 90°, 180°, 270°)** | Sine outputs/quadrature when oscillating, filter responses when filtering | ±2.5V (5Vpp) for sines, up to ±11V when filtering |
| **SPIN LP, BP, HP, Inv BP** | Same four jacks, but named for filter responses when not oscillating | ±11V (22Vpp, not limited) |

---

## **Controls**

### **Knobs**
| Name            | Function                 |
|-----------------|-------------------------|
| **SPIN**        | Coarse tuning (frequency)|
| **FINE**        | Fine tuning (frequency)  |
| **DAMPING**     | Counteracts SPIN oscillation for filter mode |
| **GRIND→SPIN**  | Feedback from GRIND output to SPIN section (controls filter drive / disables osc) |
| **GRIND IN**    | Mix amount of internal (or external) signal to GRIND processing |

### **Sliders**
| Name            | Function               |
|-----------------|-----------------------|
| **GRIND SLIDERS (1–4)** | VCAs for each comparator phase; blends corresponding SPIN output into GRIND. Summed with associated GRIND CV input (0–5V) |

### **Other Switches/Headers**
| Name         | Function             | Location               |
|--------------|----------------------|------------------------|
| **RANGE**    | Oscillator range: LOW (0.3–600Hz) / HIGH (10Hz–20kHz+) | Panel toggle          |
| **FM1 EXP/LIN** | Selects FM1 mode (jumper on module rear)    | Rear header          |
| **INJECT AC/DC** | Selects AC or DC coupling for INJECT input | Rear header (AC default) |

---

## **Operating Notes**

- **SPIN** outputs phase-aligned sines when oscillating, or SVF responses when acting as filter.
- **GRIND** outputs highly variable, complex, or distorted waveforms--morphable by sliders/CV and input/CV mixing.
- **GRIND→SPIN** CW: Strong nonlinear feedback, disables self-oscillation, module acts as a filter.
- **Inject jack** can hard-reset oscillator for sync (AC mode for spikes).
- **1V/oct tracking** is good for 4+ octaves at V/OCT. Ensure FM1 is zeroed if unpatched for precise tracking (FM1 is normalled to GRIND OUT).
- Max output from some outputs can reach ±11V (22Vpp)--ensure downstream circuitry tolerates this.

---

## **Patch Ideas**

- **Quad LFO**: LOW range, patch four SPIN outs to CV destinations for quad panning or modulation.
- **Supersaw**: Feed triangle into IN, GRIND OUT gives thick, animated wave.
- **Metallic Drones**: Patch audio rate to IN, use as filter/waveshaper at high DAMPING and GRIND→SPIN.
- **Stereo FX**: Pan/mix 0°/180° or 90°/270° outputs for spatial effects.
- **Soft Sync**: Use INJECT (AC) with another oscillator to soft-sync Angle Grinder.

---

## **Power & Specs**

- **18HP**
- +12V 81mA / -12V 78mA

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**