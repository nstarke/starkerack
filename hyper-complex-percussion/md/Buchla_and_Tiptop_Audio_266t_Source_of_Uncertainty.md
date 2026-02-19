# Buchla and Tiptop Audio — 266t Source of Uncertainty

- [Manual PDF](../../manuals/Buchla_&_Tiptop_Audio_266t.pdf)

---

[**Download the SOURCE OF UNCERTAINTY - MODEL 266t Manual PDF**](https://tiptopaudio.com/manuals/buchla-266t-manual.pdf)

---

## Using the Buchla 266t "Source of Uncertainty" for Dense, Complex Rhythms and Percussion

The **266t Source of Uncertainty** is a treasure trove for rhythmic and percussive complexity. It won't make drum sounds directly, but it will drive drum modules, percussion voices, sample players, or even full synth voices in unpredictable, highly musical ways. Let's break down how to exploit each section to create dense, polyrhythmic, and hyper-complex percussion:

---

### 1. **Noise Source**

**White, Pink, Blue Noise:**
- **Percussive Voice**: Run noise outputs through short envelopes and VCAs for classic hi-hats, snares, and shakers.
    - _Patch idea:_ Pink/white noise → VCA → LPG or filter → Out. Trigger the envelope with different, complex gate sources.
- **Shape Uniquely**: Modulate the filter or envelope with other random voltages from the 266t for organic imperfection.
- **Stereo Layering**: Pan blue/pink/white noise variants left and right for width in percussion layers.

---

### 2. **Fluctuating Random Voltages**

- **Complex Modulation**: Use this as a wobbly, unpredictable CV to modulate percussion parameters (pitch, tone, decay) or effect parameters.
- **Dynamic Polyrhythm**: Patch the output to modulate the clock rate of a sequencer, clock divider, or envelope, causing the entire rhythmic grid to warp and shift.
- **Accent Variation**: Use it to open/close a VCA or LPG controlling noise for organic ghost notes or fluctuating percussive amplitude.

---

### 3. **Sample & Hold**

- **Rhythmic Stepping**: Feed in a steady or swung clock to the pulse input, and a clock-divided or random signal for the CV input.
    - _Self-altering Patterns:_ When CV input is a slow LFO, noise, or another random source, the rhythmically sampled CV creates endlessly shifting patterns.
    - _Ping-Pong Effect:_ Use the “alt” outputs to create bouncing, ping-ponging accents or triggers for percussion.
- **Multi-Layer Polyrhythm**: Take the regular output to one percussion channel and the “alt” to another, deriving interleaved, offset patterns.

---

### 4. **Integrator**

- **Slew for Groove**: Smooth out rapid CV changes to create swung, lagged, or staggered modulation. Applied to pitch, this generates glissandi; to amplitude, funky volume swells.
- **Timing Shape**: Slew-rate modulation can dramatically adjust how quickly random values change, making patterns less robotic or adding humanized feel.

---

### 5. **Quantized Random Voltage**

- **Random Stepped Patterns**: Trigger with odd/even clocks or any rhythm. The stepped voltages can drive percussive pitch, rhythm accents, or even micro-sequencing.
- **Step Control**: Select n+1 or 2^n distributions for more constrained or totally wild pitch/parameter jumps.
- **Multi-Signature Clocks**: Use the quantized output to step sequencers or clock dividers/multipliers set to different time signatures, generating polyrhythms.

---

### 6. **Stored Random Voltage**

- **Distribution Shaping**: Use the right output and its “curve” control to bias rhythms toward busier or sparser moments on the fly. Clock the random pulse from a complex rhythm generator for even more unpredictability.
- **Dual CV Paths**: Send the two outputs to different drum voices, panned left and right—or to VCOs for random percussion timbres.

---

## Advanced Polyrhythmic Techniques

- **Layer Multiple Outputs**: Send pulses and random CVs to several percussion sources with varied clock rates and modulations for dense metric overlays.
- **Clustered Sampling**: Cross-patch random outputs to control the pulse rate, creating feedback for bubbling, fractal patterns.
- **Unpredictable Fills**: Use Integrator outputs for fill CVs, ramping and gliding between values mid-bar for wild, non-repeating fills.

---

### **Quick Patch Inspiration**

- **Poly-Tempo Percussion Grid:**
    - Master clock → clock divider (for main rhythm)
    - Fluctuating random voltage (modulates clock division amount)
    - Quantized random voltage → S&H pulse input (for trigger distribution)
    - Noise (any color) → LPG/VCA, triggered by S&H “alt” output for off-beat or ghost hits
    - Stored random voltage → modulate drum module decay/pitch for every hit

- **Randomized Hi-Hat Machine:**
    - Blue/Pink/White noise → VCA
    - CV from quantized or stored random → VCA level
    - Regular clock → Sample & Hold pulse input
    - Alt Output → triggers different hat samples for ping-pong hats

---

### Tips for Uniqueness & Punch

- _Stack Noise Colors:_ Blend with multed outputs and cross-modulate or pan for rich, layered percussion.
- _Dynamic Parameter Control:_ Assign different random outputs to decay, filter cutoff, pitch—no two hits will be the same.

---

**Maximize unpredictability by combining several random sources; use attenuators and offset modules if needed to fine-tune the chaos!**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)