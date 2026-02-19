# ADDAC Systems — ADDAC-714 Vintage Clipper

- [Manual PDF](../../manuals/ADDAC714_VintageClipper_A_0.pdf)

---

[ADDAC714 Vintage Clipper User's Guide (PDF)](https://www.addacsystem.com/Manuals/ADDAC714_USER_GUIDE.pdf)

# **ADDAC714 Vintage Clipper – Cheat Sheet**

A dual-channel, diode-based soft clipper for Eurorack. Provides "vintage" diode clipping with selectable symmetry and post-clip output gain. Practical as a tone-shaper, saturator, or "brick wall" limiter in your signal path.

---

## **Quick Start**

1. **Input Signal:** Patch audio into IN 1 and/or IN 2 (IN 1 normalled to IN 2 if nothing plugged in).
2. **Engage Effect:** Toggle BYPASS switch UP (active, effect engaged).
3. **Set Gain:** Turn GAIN to set clipping amount (how much signal hits the diodes).
4. **Set Symmetry:** Switch SYMMETRY UP (bipolar, even/odd harmonics) or DOWN (unipolar, odd harmonics only).
5. **Output Level:** Adjust OUTPUT GAIN for desired volume at OUT jack.
6. **Monitor Clipping:** Watch CLIP LED for indication of clipping at output.
7. **Patch Out:** Use OUT 1/2 to patch clipped signal onward.

---

## **Controls & Function Summary**

### **Front Panel Controls:**

| Control         | Type         | Function                                                             |
|-----------------|--------------|----------------------------------------------------------------------|
| BYPASS (CH1/CH2)| Toggle       | UP = Effect Active, DOWN = Bypassed                                  |
| GAIN (CH1/CH2)  | Knob         | Sets threshold/clipping amount; more gain, more clip                 |
| SYMMETRY        | Toggle       | UP = Symmetrical (even & odd harmonics), DOWN = Unsymmetrical (odd only) |
| OUTPUT GAIN     | Knob         | Sets post-clip output volume                                         |
| CLIP LED        | LED          | Indicates output clipping                                            |

---

### **Jacks (per channel):**

| Jack        | Type | Description                                                                             | Voltage Ranges                  |
|-------------|------|-----------------------------------------------------------------------------------------|---------------------------------|
| IN 1 / IN 2 | In   | Audio signal input (Left input normalled to Right if Right not connected)               | Not specified, but audio range  |
| OUT 1 / OUT 2| Out | Audio signal output after clipping, eq, gain                                            | Up to Eurorack standard ±10V*   |

*\*(actual range may depend on input signal, module does not amplify beyond x2 post-clip stage)*

---

### **Signal Flow (per channel):**
1. **Input → Clipper (GAIN & SYMMETRY) → Passive 3.3kHz LPF → Output Op-Amp (x2 gain, OUTPUT GAIN knob) → Output**
2. BYPASS switch reroutes input signal past the clipper to output stage.

---

### **Technical Specs**

- Width: 6HP
- Depth: 4 cm
- Power: 40mA @ +12V / 40mA @ -12V

---

#### **Tips & Usage**
- Use high GAIN for heavier distortion, OUTPUT GAIN to rebalance level.
- Toggle SYMMETRY for timbral variety—odd/even (fuzzier) vs. odd-only (harsher).
- Experiment with various input sources: drums, bass, synth lines.
- Engage BYPASS for easy comparison or channel switching.

---

**No CV control. All controls are manual (no voltage-controlled inputs/outputs).**

---

**Clipping is passive and diode-based for "vintage" soft clip feel, with a characterful lowpass roll-off (3.3kHz, -3dB).**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)