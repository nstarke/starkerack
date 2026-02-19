# Black Noise — Cosmos

- [Manual PDF](../../manuals/BLACK-NOISE_COSMOS_User-Manual_V1.pdf)

---

[**View COSMOS by Black Noise — Official User Manual (PDF)**](https://blacknoisemodular.com/wp-content/uploads/2024/03/COSMOS_USER_MANUAL_V1.0.pdf)  
*(Link from Black Noise Modular — ensure version and link match latest official document)*

---

# COSMOS Eurorack Module Cheat Sheet

**Quick Reference for Patch, Logic, & Signal Processing**

---

## **Inputs (Jacks & Touch Pads)**

| Input  | Type              | Description                                                                                                                                   | Voltage Range      |
|--------|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|--------------------|
| X IN   | 3.5mm jack        | Main analog input (accepts CV, audio, gate, trigger, uni- or bipolar signals)                                                                 | -10V to +10V       |
| Y IN   | 3.5mm jack        | Secondary analog input (as above)                                                                                                             | -10V to +10V       |
| X Pad  | Capacitive Touch  | Normalled to X In if jack is unpatched. Touch-controlled (performance) analog voltage.                                                         | ~0V to +5V*        |
| Y Pad  | Capacitive Touch  | Normalled to Y In if jack is unpatched.                                                                                                       | ~0V to +5V*        |

> *Touch pad voltage dependent on skin contact and pressure.

---

## **Outputs (all 3.5mm jacks)**

| Output                | Type             | Description                                                                                                                                            | Voltage Range        |
|-----------------------|------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------|
| Analog Outs           | Analog           | 1:1 buffered X, 1:1 buffered Y, Inverted X, Inverted Y, (X+Y)/2, (X-Y)/2, Inverted (X+Y)/2, Inverted (X-Y)/2                                           | -10V to +10V         |
| MIN                   | Analog           | Minimum of X and Y (AND function for logic/gates)                                                                                                      | -10V to +10V         |
| MAX                   | Analog           | Maximum of X and Y (OR function for logic/gates)                                                                                                       | -10V to +10V         |
| INV MIN, INV MAX      | Analog           | Min/Max with opposite phase                                                                                                                            | -10V to +10V         |
| TZ CLIPPER, INV TZ    | Analog           | Through-zero clipper (unique wave/ring mod/XOR effect), and its inverse                                                                               | -10V to +10V         |
| Logic Gates (Gate)    | Digital Gate     | AND, OR, XOR, NOR, NAND, XNOR — logic gates output HIGH when analog outs above 0V (mirrored/not on lower hemisphere)                                   | 0V (LOW), +10V (HIGH)|
| NOT Gates (Gate)      | Digital Gate     | NOT logic of each gate (lower hemisphere)                                                                                                              | 0V (LOW), +10V (HIGH)|
| Trigger Outs          | Digital Trigger  | Fires on rising edge (main hemisphere) or falling edge (lower hemisphere) when gate crosses 0V                                                        | 10ms trigger         |

---

## **Controls**

| Control Location          | Type        | Function                                                                                                   | Notes                        |
|--------------------------|-------------|------------------------------------------------------------------------------------------------------------|------------------------------|
| Rear (PCB trimmers)      | Trimmers    | Calibration of thresholds for gate conversion (adjust if needed; usually set at factory)                    | Only adjust if malfunctioning|
| Touch Pads (Front)       | Touch       | Generates voltage when touched; replaces jack input when unpatched                                         | Performance CV control       |
| No knobs, buttons, or sliders on panel*  |

\*All core CV and gate manipulation occurs via patching, normalization, and external CV/utility modules.

---

## **Patching Quick Reference**

**Combine PEG, logic, and analog**
- **Standard Analog Combo:**  
  - (X+Y)/2, (X-Y)/2, MIN, MAX
- **Digital Logic Outputs:**  
  - Gates for AND, OR, XOR, NOR, NAND, XNOR
  - Triggers (rising and falling edge) both hemispheres
  - NOT versions always mirrored on the lower row

**Special Functions:**
- **Clipping/Ringmod:** TZ Clipper outs for unique analog XOR, ring mod, analog comparators
- **Envelope/Rectifier:** Patch both X and Y with signal/inverted, use MIN, MAX for half/full wave rectification
- **VCA/VC Clipper:** Patch signal and modulation envelope to X/Y, use TZ outputs for clamping/distortion
- **Oscillator:** Self-patch XNOR gate back to input (with/followed by slew/LPF for frequency control)
- **Logic/CV/Gate Manipulation:** Use MAX/MIN for window comparators, clock doubling, random rhythmic Gates with external S&H/noise

---

## **Typical Voltage Ranges**

| Signal Type     | Patchable Range             |
|-----------------|----------------------------|
| CV/Audio In/Out | Bipolar (±10V typical)     |
| Gates/Triggers  | 0V (LOW), 10V (HIGH)       |
| Pads            | 0V to ~+5V (touch)         |

---

## **Other Notes**
- **No menus, switches, or modes:** Everything is patch-dependent!
- **Install with provided ribbon cable only** (special orientation, 10→16 pin).
- **Module Depth:** 30mm
- **Width:** 14 HP
- **Current draw:** +12V: 65mA / -12V: 65mA

---

## **Usage Examples**
- **Half/Full Wave Rectifier, Comparator, Window Comparator, Envelope Follower**
- **VCA, Ring Mod, Oscillator, Clock Multiplier, Random Gate Sequencer**
- **AND/OR/NOT/XOR/NAND/XNOR gates for advanced trigger/logic patching**
- **Wave Shaping, Harmonic Enhancement, Phase-Locked Loops**

Review the [manual PDF](https://blacknoisemodular.com/wp-content/uploads/2024/03/COSMOS_USER_MANUAL_V1.0.pdf) for detailed patch diagrams and example setups.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)