# Tiptop Audio — Z4000

- [Manual PDF](../../manuals/Tiptop_Audio_z4000.pdf)

---

[Z4000 Voltage Controlled Envelope Generator Manual PDF](http://tiptopaudio.com/z4000-ns/)

# Tiptop Audio Z4000 VC-EG Cheat Sheet

**The Z4000 is a four-stage envelope generator (Attack, Decay, Sustain, Release) with unique CV processing features (Attenuverter/Deviater) for shaping, scaling, inverting, mirroring, or offsetting the envelope.**

---

## 🛠 **Panel Controls Summary**

| Name           | Type    | Function                                                                               | Range        |
|----------------|---------|----------------------------------------------------------------------------------------|--------------|
| **A (Attack)** | Knob    | Sets attack time; voltage controllable                                                 | 0ms to minutes (via knob & CV) |
| **D (Decay)**  | Knob    | Sets decay time; voltage controllable                                                  | 0ms to minutes (via knob & CV) |
| **S (Sustain)**| Knob    | Sets sustain level; voltage controllable                                               | 0V (min) to ~8V (max, via knob & CV) |
| **R (Release)**| Knob    | Sets release time; voltage controllable                                                | 0ms to ∞ (fully CW) (via knob & CV) |
| **Attack Curve Switch (ATK)** | Toggle   | Selects attack curve slope (exponential/logarithmic)                          | N/A          |
| **Attenuverter**| Knob   | Scales and inverts envelope output; 12h = 0V, CW = full pos, CCW = full neg            | ± envelope out |
| **Deviater**    | Knob   | Offsets envelope output voltage (+ or - static voltage)                                | ± static V   |
| **Deviater CV Amt** | Knob | Level of external signal mapped by Deviater VC input                                 | N/A          |

---

## 🔌 **Jacks Reference (Inputs & Outputs)**

| Jack Label         | Type   | Function                                                     | Voltage Range      |
|--------------------|--------|--------------------------------------------------------------|--------------------|
| **GATE**           | In     | Gate/trigger input to start envelope                         | +2V min (typical)  |
| **RTRG (Retrigger)**| In    | Pulse retriggers envelope during held gate                   | +2V min (typical)  |
| **A, D, S, R**     | In     | Voltage control for Attack, Decay, Sustain, Release          | 0–5V = 0–100% of parameter; summed w/ knob |
| **DEVIATER VC**    | In     | Modulates Deviater offset                                    | 0–5V for full range|
| **OUT**            | Out    | Main envelope output (processed by Attenuverter and Deviater)| ±8V maximum (scaled/inverted/offset) |

---

## 🚦 **Usage Quick Start**

1. **Basic Envelope**  
   - Plug gate into **GATE**  
   - Set envelope shape:  
     - **Attack=Min, Decay=50%, Sustain=50%, Release=50%**
   - Set **Attenuverter** to full CW (full pos)
   - Set **Deviater** to center (0 offset)
   - Patch **OUT** to desired CV input (VCA, filter, etc.)

2. **Sculpt Envelope**
   - Adjust **A/D/S/R** for shape and timing.
   - **First 50%**: fine tuning, ultra-fast percussive/transient control  
   - **Above 50%**: extends segment times up to minutes *or infinite Sustain*
   - Switch **ATK** (Attack Curve) for subtle slope changes.

3. **Advanced Shaping**
   - **Attenuverter**:  
      - Center = 0V
      - CW = normal
      - CCW = inverted envelope  
      - LED indicates polarity (red = pos, yellow = neg)
   - **Deviater**  
      - CW = +V offset
      - CCW = -V offset  
      - Modulate with **Deviater VC** or external signal for dynamic shifting, mirroring, clipping etc.

4. **Voltage Control**
   - Patch CV sources (sequencer, LFO, other envelopes) into **A/D/S/R** or **Deviater VC** as desired  
   - 0–5V = full range for segment control (CV is summed with knob)

5. **Retrigger**
   - Send pulses to **RTRG** (while GATE is held) to restart Attack for accents, modulation, or rhythmic variations

---

## 🛑 **Protection**

- **Reverse Polarity Power Protection**: Module is fully protected, cannot be damaged by reverse power plug-in.

---

## **Summary Table**

| Function         | Jack/Control     | Voltage/Action       | Note              |
|------------------|-----------------|----------------------|-------------------|
| Envelope Gate    | GATE (In)       | >2V trigger/gate     |                   |
| Retrigger        | RTRG (In)       | >2V pulse retrigger  |                   |
| Attack CV        | A (In)          | 0–5V                 | Summed w/ knob    |
| Decay CV         | D (In)          | 0–5V                 | Summed w/ knob    |
| Sustain CV       | S (In)          | 0–5V                 | Summed w/ knob    |
| Release CV       | R (In)          | 0–5V                 | Summed w/ knob    |
| Deviater Mod     | DEVIATER VC (In)| 0–5V                 | Summed w/ knob    |
| Envelope Output  | OUT (Out)       | -8V to +8V (max)     | Depends on Attenuverter/Deviater settings |
| Attack Curve     | ATK Switch      | Expo/Log selection   | Subtle, long Attack best auditioned |

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)