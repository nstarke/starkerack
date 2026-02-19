# Pittsburgh Modular — Double Helix Oscillator

- [Manual PDF](../../manuals/Lifeforms Double Helix Oscillator - Pittsburgh Modular Synthesizers.pdf)

---

**[Lifeforms Double Helix Oscillator (Pittsburgh Modular) – Manual PDF](#)**  
*(No direct PDF link provided in your images; replace with actual link if available.)*

---

# Lifeforms Double Helix Oscillator — Cheat Sheet

**Type**: Dual Analog Oscillator & Complex Modulator  
**Size**: 28hp  
**Depth**: 37mm  
**Power**: +12V 223mA / -12V 205mA (no +5V needed, reverse polarity protected)

---

## Quick Start

1. **Primary oscillator outputs**: Sine/Saw/Blade/Sub/Pulse.
2. **Secondary oscillator outputs**: Sine/Saw/Square.
3. **Mix any wave(s) (using In 1 and In 2) into the contour section** for wavefolding and LPG (Low Pass Gate) processing.
4. **Use ‘Impulse’ input** to “strike” the LPG for percussive sounds.
5. **Mix and modulate sources with the dual voltage controlled routers** for complex, flexible CV patching and live performance.
6. **Get modulation from** integrated LFO (sine/square/random) and analog noise.

---

## Inputs & Outputs Reference

### Audio Inputs
| Jack         | Section     | Function                       |
|:-------------|:------------|:-------------------------------|
| In 1         | Contour     | Audio in (mix with In 2). Normalled to primary osc sine. |
| In 2         | Contour     | Audio in (mix with In 1).      |

### Audio Outputs
| Jack          | Section      | Function                      |
|:--------------|:-------------|:------------------------------|
| Sine Out      | Primary      | Sine wave out (±5V)           |
| Saw Out       | Primary/Sec  | Saw wave out (±5V)            |
| Blade Out     | Primary      | Blade wave out (±5V)          |
| Sub Out       | Primary      | Sub square out (±5V)           |
| Pulse Out     | Primary      | Pulse wave out (±5V)           |
| Square Out    | Sec/Mod      | Sec osc output / LFO output   |
| Output        | Contour      | Final contour section out (±5V) |

### Pitch Control
| Jack         | Section         | Function                        | Voltage Range |
|:-------------|:----------------|:--------------------------------|:-------------|
| V/O In       | Primary/Sec osc | 1V/oct pitch CV input           | 0V → +10V/(-1V)* |

### Modulation Inputs (CV)
| Jack                 | Section                | Function / Source             | CV Range  |
|:---------------------|:-----------------------|:------------------------------|:---------|
| FM CV In             | Primary/Sec Osc        | FM amount                     | ±5V*     |
| Blade/Pulse CV In    | Primary Osc            | Waveshape mod                 | ±5V*     |
| Timbre CV In         | Contour                | Wavefolder mod                | ±5V*     |
| Dynamics CV In       | Contour                | LPG mod                       | ±5V*     |
| Impulse In           | Contour                | LPG “strike” (Gate/Trig)      | >2V trig |
| VCR A/B CV In        | Router                 | Level CV for mod channels     | 0–+5V    |

(*Ranges are ±5V typical for Eurorack, but manual does not specify extremes—start safe.)

### Modulation Outputs
| Jack         | Section        | Function                       | Level     |
|:-------------|:---------------|:-------------------------------|:----------|
| Sine/Square/Random Out | Modulation | LFO waveforms (CV)             | ±5V*      |
| Noise Out    | Modulation     | Analog noise                    | ±5V*      |
| VCR Out      | Router         | Mod source A/B or mix           | ±5V*      |

---

## Controls Reference

### Oscillators
- **Frequency Knob (each osc)** — LFO → Audio range sweep (typically 0.01–20kHz)
- **Fine Tune Knob (each osc)**
- **Blade/Pulse CV Knob** — Attenuates Blade/Pulse CV
- **FM CV Knob** — Attenuates FM CV

### Contour Section
- **Timbre Knob** — Wavefolder gain (fold “depth”)
- **Timbre CV Knob** — Attenuates timbre CV input
- **Dynamics Knob** — LPG level (left = closed, right = open)
- **Dynamics CV Knob** — Attenuates dynamics CV input
- **Dynamics Response Knob** — Sets LPG “strike” decay (~LPG envelope time)

### Modulation
- **Frequency Knob** — LFO rate

### Voltage Controlled Routers (Matrix)
- **In A/B Jacks** — Assignable mod sources (A: normalled to sec osc sine, B: normalled to LFO sine)
- **VCR A/B Level Knobs** — Attenuate mod signals through router
- **FM1/FM2/Blade-Pulse/Timbre/Dynamics Source Switches (per mod destination)** — Route A/B/off to that CV in (mixes with its dedicated CV jack)
- **VCR Output Source Switch** — Selects A/B/off for VCR Out
- **VCR Output Jack** — Output of A or B mod signal
- **VCR A/B CV Inputs** — CV for VCR A/B mod signal level

---

## PDF Manual  
*(Replace with actual PDF link if needed; for now, see images above.)*

---

## Additional Notes

- **Impulse Input** makes LPG sound highly dynamic and organic (great for Buchla-like “pinging”).
- **Routing switches** allow switching modulation sources live without repatching.
- **All CV inputs expected to operate in ±5V range** (safe bet for all modulation).
- **All outs and normal audio ins are typically ±5V; adjust downstream gain as needed.**
- **Experiment with cross-patching modulation (Osc2 as LFO, noise as mod, etc.) for complex organic movement!**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)