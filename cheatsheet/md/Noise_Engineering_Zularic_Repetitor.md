# Noise Engineering — Zularic Repetitor

- [Manual PDF](../../manuals/Zularic Repetitor Manual - Noise Engineering Documentation.pdf)

---

[PDF Manual Link](https://manuals.noiseengineering.us/zr/)

---

# Noise Engineering Zularic Repetitor Cheat Sheet

## **Module Type**
- **Rhythm Generator**
- **8HP Eurorack**

---

## **Power Requirements**
- **+12V:** 50mA
- **-12V:** 5mA
- **Connector:** 2x5 Eurorack ribbon (red stripe = -12V)

---

## **Inputs, Outputs, and Controls**

### **Inputs**
| Jack      | Purpose                      | Voltage Range           |
|-----------|-----------------------------|-------------------------|
| **Beat**  | Clock input (advances time) | Triggers ≈2.5V & up     |
| **Measure** | Measure reset (resyncs parts) | Trigger ≈2.5V & up      |
| **Mother CV** | Select Mother pattern or modulate pattern | ~7V                    |
| **Child 1-3 CV**  | Time offset for each Child relative to Mother | ~7V          |

---

### **Outputs**
| Jack             | Purpose                        | Voltage Range      |
|------------------|-------------------------------|--------------------|
| **Mother Out**   | Main pattern gate output       | Gate ≈6V           |
| **Child 1-3 Out**| Offset pattern gate outputs    | Gate ≈6V           |

---

### **Front-panel Controls**
| Name           | Type        | Description                                                                                     |
|----------------|-------------|-------------------------------------------------------------------------------------------------|
| **Mother**     | Knob + CV   | Selects Mother pattern (acts as attenuator for Mother CV)                                       |
| **Child 1-3**  | Knob + CV   | Controls beat offset from Mother for each "Child" output (acts as attenuator for Child CV ins)  |
| **World**      | Toggle      | Select Old World (Indian/African/Vodou) or New World (Funk, Rock, etc.) pattern bank            |
| **RST**        | Button      | Pauses time advance while held, resets to measure start on release                              |
| **LEDs**       | Indicator   | Show selected mother pattern and world bank                                                     |

---

## **Basic Operation**
1. **Clock:** Patch a clock to **Beat** for operation.
2. **Reset:** Optionally patch a reset/measure pulse to **Measure** for periodic resync.
3. **Patterns:** Select pattern set with **Mother** knob (+ CV modulation).
4. **Offsets:** Use **Child 1-3** knobs (or CV) to shift pattern in time vs Mother output.
5. **Pattern Source:** Toggle **World** for Old/New World rhythms.
6. **Gate Outputs:** Patch Mother and up to three Child outputs to envelopes, drum modules, etc.

---

## **Special Modes**
- **Divider Mode:** Switches to clock-divider (~1, 2, 3 sections, controllable by CV/knob).
- **Random Mode:** Random gate generation, probability set by knob/CV.

---

## **Pattern Reference**
- **Patterns:** 30 included, covering African, Indian, Funk, Rock, Latin, etc.
- **Overview:** Each pattern outputs four rhythm parts; variations via offset.
- **Pattern diagrams:** Refer to manual p. 6-8 for beat maps.

---

## **Patching Tips**
- Start with basic clock to Beat, play with Mother and Child knobs.
- Add slow LFO, random CV, or stepped sequencer to Mother/Child CVs for variation.
- Try using divided clocks or rhythm generators to dynamically shift time offsets.

---

🔗 [Manual PDF](https://manuals.noiseengineering.us/zr/)  
🔗 [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)