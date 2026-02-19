# Buchla and Tiptop Audio — 281t Quad Function Generator

- [Manual PDF](../../manuals/Buchla_&_Tiptop_Audio_281t.pdf)

---

[Manual PDF - Buchla Tiptop 281t Quad Function Generator](https://tiptopaudio.com/manuals/281t_manual.pdf)

---

# Buchla Tiptop Audio 281t Quad Function Generator (Eurorack)  
**Cheat Sheet - Quick Reference**

---

## **Core Overview**
- **4 function generators** (A, B, C, D), arranged in two linkable pairs (A+B, C+D).
- Modes per generator: **Transient, Sustained, Cyclic**.
- Can generate AD, ASR, or looping envelopes, or be paired for complex shapes or quadrature operation.

---

## **Inputs / Outputs**

| Function        | Jack Type  | Location         | Voltage Range & Notes                                                        |
|-----------------|------------|------------------|------------------------------------------------------------------------------|
| **IN**          | Input      | Per generator    | Gate or trigger; any voltage above ≈2V is treated as high.                   |
| **CYCLE JACK**  | Input      | Per generator    | Trigger or gate to enable cycling via external signal.                       |
| **CV ATTACK**   | Input      | Per generator    | Unipolar; 0–10V CV controls attack segment rate.                             |
| **CV DECAY**    | Input      | Per generator    | Unipolar; 0–10V CV controls decay segment rate.                              |
| **OUT**         | Output     | Per generator    | Envelope output; 0 to +10V range.                                            |
| **END OUT (Pulse)** | Output      | Per generator    | Triggers at end of decay; 10V logic pulse.                                    |

---

## **Controls**

| Control        | Type             | Per-Gen? | Description                                                           |
|----------------|------------------|----------|-----------------------------------------------------------------------|
| **Attack**     | Knob             | Yes      | Sets rise time (0.001–10s).                                           |
| **Decay**      | Knob             | Yes      | Sets fall time (0.001–10s).                                           |
| **Mode**       | Toggle Switch    | Yes      | Sets mode:<br>**Transient** (trig = AR), **Sustained** (gate = ASR),<br>**Cyclic** (looping AD).|
| **Trigger**    | Push Button      | Yes      | Manually fires the function generator.                                |
| **Cycle Input**| Jack             | Yes      | Accepts external gate/trigger to enable cycling.                      |

### **Global/Paired Controls**
| Control        | Type             | Location  | Description                                                      |
|----------------|------------------|-----------|------------------------------------------------------------------|
| **Quadrature Switch** | Toggle          | Between each pair (A+B, C+D)      | Pair generators; envelope of B (or D) is 90° out of phase to A (or C). |

---

## **Operation Summary**
- **Transient:** Envelope rises on any valid pulse (trigger), falls immediately after reaching 10V.
- **Sustained:** Envelope rises and holds at 10V while input is high (gate); falls when input goes low.
- **Cyclic:** Envelope self-cycles (LFO or looping envelope) as long as cycle is enabled (via switch or jack).
- **Quad (Quadrature) Mode:** Link pairs (A+B or C+D); B (or D) starts its cycle at peak of A (or C).

---

## **Voltage Ranges**
- **Envelope OUT:** 0V (min) to +10V (max)
- **CV Inputs (Attack/Decay):**  0–10V
- **Pulse Outputs:** 10V logic pulse

---

## **Physical Specs**
- **Width:** 28HP
- **Depth:** 32mm
- **Power:** +12V 160mA / -12V 55mA

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)