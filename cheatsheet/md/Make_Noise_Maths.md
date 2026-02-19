# Make Noise — Maths

- [Manual PDF](../../manuals/MATHSmanual2013.pdf)

---

[**Official Make Noise Maths Manual (PDF)**](https://makenoisemusic.com/content/manuals/MathsManual2013.pdf)

---

# Make Noise MATHS Cheat Sheet

MATHS is a powerful analog function generator, envelope, LFO, and signal processor for Eurorack modular synthesizers.
This cheat sheet summarizes its jacks and panel controls for quickly patching and integrating into your rack.

---

## Quick Functional Summary

- **CH1 & CH4** = Full-featured Envelope/Function Generators (rise, fall, shape, looping, logic outputs, unity out)
- **CH2 & CH3** = Attenuverter/offset channels (create offsets, scale/invert signals)
- **SUM Bus** = Summing mixer (add, invert, subtract voltages — also provides an inverted output)
- **OR Bus** = "Maximum" CV logic (analog OR)
- **Everything is CV-able!**

---

## Panel Controls & Jacks

### **CHANNELS 1 & 4: Function Generators**

#### **Inputs:**
- **Signal Input:** (+/-10V) Direct coupled; processes external CV/audio (lag, ASR, portamento, etc.)
- **Trigger Input:** (min +2.5V for Gate HIGH) Triggers an envelope regardless of signal input.
- **Rise CV Input:** (Linear, +/-8V) CV over rise time, positive increases, negative decreases.
- **Fall CV Input:** (Linear, +/-8V) CV over fall time, positive increases, negative decreases.
- **Both CV Input:** (Exponential, +/-8V) CV over entire function time; positive = quicker.
- **Cycle Input:** (min +2.5V for HIGH) Gates cycle mode ON/OFF.

#### **Outputs:**
- **Unity Output:** (0–8V, not affected by attenuverter, always active)
- **Variable Output:** (up to +/-10V, affected by attenuverter, normalized to SUM/OR, patched out = removed from bus)
- **End of Rise (EOR, Ch1)/End of Cycle (EOC, Ch4):** (0V/10V) Logic pulse at end of rise/fall.

#### **Knobs:**
- **Rise:** Set rise time (fast ← CCW, slow → CW)
- **Fall:** Set fall time (fast ← CCW, slow → CW)
- **Vari-Response:** Morphs shape (Log <-- Lin --> Expo)
- **Attenuverter:** Sets gain/polarity for Variable Out and bus
- **Cycle Button:** Enables/disables self-cycling (LFO mode)

#### **LEDs:**
- **Cycle LED:** Indicates if cycling/LFO mode is engaged
- **EOR/EOC LED:** Shows logic state of EOR/EOC output
- **Unity LED:** Indicates positive (green) or negative (red) output on unity jack

---

### **CHANNELS 2 & 3: Attenuverter and Offset**

#### **Inputs:**
- **Signal Input:** (+/-10V) Pass in CV or audio; if unplugged, normalled to voltage reference for manual offset.

#### **Outputs:**
- **Variable Output:** (up to +/-10V for Ch2, +/-5V for Ch3) Affected by attenuverter knob, normalized to SUM/OR buses.

#### **Knobs:**
- **Attenuverter:** Controls scale and polarity. With nothing plugged to input, controls the level of the output offset.

---

### **BUS OUTPUTS (Bottom Center of Panel)**

- **SUM:** (+/-10V) Adds all variable outputs per knob settings.
- **INVERTED SUM:** (+/-10V) SUM Output, inverted.
- **OR BUS:** (0–10V) Maximum output of all nonnegative Variable Outputs.
- **Variable Outputs 1–4:** Output of each channel. When patched, removes from SUM/OR.
- **SUM Bus LEDs:** Green (positive voltages), Red (negative).

---

## **Reference Table: Inputs, Outputs & Panel Controls**

| Label                | Type     | Range            | Channel(s) | Notes                                                        |
|----------------------|----------|------------------|------------|--------------------------------------------------------------|
| Signal Input         | Input    | +/-10V           | 1,2,3,4    | Direct-coupled; DC+Audio                                     |
| Trigger Input        | Input    | Gate, +2.5V Thresh| 1,4       | Triggers envelope                                            |
| Cycle Input          | Input    | Gate, +2.5V Thresh| 1,4       | Remote cycle ON/OFF                                          |
| Rise CV Input        | Input    | +/-8V            | 1,4        | Linear; affects rise time                                    |
| Fall CV Input        | Input    | +/-8V            | 1,4        | Linear; affects fall time                                    |
| Both CV Input        | Input    | +/-8V            | 1,4        | Exponential; whole function time                             |
| Variable Output      | Output   | +/-10V (Ch1,2,4), +/-5V (Ch3) | 1-4 | Attenuverter controlled, norm’d to SUM/OR                    |
| Unity Output         | Output   | 0–8V             | 1,4        | Raw channel output, unaffected by attenuverter, always active|
| EOR (End-of-Rise)    | Output   | 0V/10V           | 1          | High when rise ends                                          |
| EOC (End-of-Cycle)   | Output   | 0V/10V           | 4          | High when fall ends                                          |
| SUM                  | Output   | +/-10V           | ALL        | All variable outputs summed                                  |
| INVERTED SUM         | Output   | +/-10V           | ALL        | SUM output inverted                                          |
| OR BUS               | Output   | 0–10V            | ALL        | Max of all (no negative voltages)                            |

---

## **Essential Usage Tips**

- Use **Cycle** for LFO, rhythmic clocks, cycling envelopes.
- **Variable Outs**: Patch for custom-scaled/inverted signals. Unpatched routes signal to busses.
- **Unity Outs:** For pure, unattenuated channel output; always present.
- **EOR/EOC**: For logic, retriggers, rhythmic patching, clock division.
- **Rise/Fall CVs:** Patch dynamic modulation for envelopes/LFOs.
- **CH2/3:** Use as CV audio attenuverters or as manual voltage sources (offset).
- **SUM/INV/OR buses:** Powerful CV mixing/combo tools; experiment!

---

## **Advanced Use**
- **Self-patching:** Use outputs (including Unity, INV, SUM, OR) to modulate MATHS’s own CVs.
- **Patch EOR/EOC between Ch1/Ch4 for ping-pong/envelope chaining/complex shapes.**
- **Feed OR out to destinations needing only positive voltages.**
- **Voltage control shape (Vari-Response) with CV for dynamic morphing.**
- **Up to 25-minutes slow or 1kHz fast functions!**

---

## Links

- [**Official Make Noise Maths Manual (PDF)**](https://makenoisemusic.com/content/manuals/MathsManual2013.pdf)
- [**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)

---