# Tiptop Audio — HATS808

- [Manual PDF](../../manuals/Tiptop_Audio_HATS808_ns.pdf)

---

[**Tiptop Audio HATS808 Manual (PDF)**](https://tiptopaudio.com/manuals/HATS808.pdf)

---

# Tiptop Audio HATS808 Eurorack Cheat Sheet

## **Quick Start**
1. **Open Hat:**  
   - Patch GATE to **OH GATE IN**  
   - Patch **OH OUT** to mixer/audio  
   - Set **LEVEL** ~50%

2. **Closed Hat:**  
   - Patch GATE to **CH GATE IN**  
   - Patch **CH OUT** to mixer/audio  
   - Set **LEVEL** ~50%

3. **Choke Function:**  
   - Both hats triggered together: CH envelope chokes OH decay (classic 808 behavior).  
   - Disable choke: Move PCB header jumper to alternate position.

---

## **Inputs (Jacks)**

| **Input**        | **Function**                | **Voltage Range** |
|------------------|----------------------------|-------------------|
| CH GATE IN       | Closed hat trigger         | +5V (Gate/Trig)   |
| CH ACCENT IN     | Accent for closed hat      | +5V (Gate/Trig)   |
| OH GATE IN       | Open hat trigger           | +5V (Gate/Trig)   |
| OH ACCENT IN     | Accent for open hat        | +5V (Gate/Trig)   |
| VC-Q             | Resonance (Q) modulation   | 0–5V (CV)         |

---

## **Outputs (Jacks)**

| **Output**       | **Signal**                         |
|------------------|------------------------------------|
| CH OUT           | Closed hat audio                   |
| OH OUT           | Open hat audio                     |
| BandPass OUT     | Band-passed noise source (raw)     |

---

## **Knobs/Controls**

| **Control**   | **Description**                                                  |
|---------------|------------------------------------------------------------------|
| CH LEVEL      | Output level for closed hat (soft to hot/overdriven)             |
| OH LEVEL      | Output level for open hat (soft to hot/overdriven)               |
| ACCENT (CH)   | Accent amount for triggers & gates; also fine level control      |
| ACCENT (OH)   | Accent amount for triggers & gates; also fine level control      |
| DECAY         | Controls OH envelope decay duration                              |
| Q             | Bandpass filter resonance (min = "808", full = oscillation/crush)|
| VC-Q (knob)   | Offset for the incoming VC-Q CV signal                           |

---

## **Key Features & Tips**

- **Output Gain:** LEVEL knobs allow for overdriven, harmonically-rich sound when maxed.
- **Accents:** Add dynamics—use external triggers for pattern accents, or rely on internal normalization for fine-tuning.
- **Choke:** Classic hi-hat interaction for dynamic rhythmic textures; disable with internal jumper if desired.
- **Q/VC-Q:** Move from classic 808 hi-hat to metallic, crushed, or even oscillating tones. Modulate with external CV for evolving timbres.
- **BandPass OUT:** Use as a raw source for further processing/patching in eurorack.

---

## **Voltage Reference**

- **Gate/Trigger Inputs:** Expect +5V logic.
- **VC-Q Input:** 0–5V for resonance control.

---

## **Example Patch Tips**

- For *techno* hats: Send a gate sequence to CH GATE IN, with alternating gates to CH ACCENT for traditional 808/909 patterns.
- For *dynamic sound*: Modulate VC-Q with a slow LFO or envelope.
- *Overdrive sound*: Max LEVEL and ACCENT for punchy, distorted hats.

---

**Reference:**  
[Tiptop Audio HATS808 Manual PDF](https://tiptopaudio.com/manuals/HATS808.pdf)  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)