# Hexinverter — Orbitals

- [Manual PDF](../../manuals/hexinverter-orbitals.pdf)

---

[Hexinverter Orbitals User Manual PDF](https://www.hexinverter.net/wp-content/uploads/2015/05/Orbitals_User_Manual_v104.pdf)

---

# Generating Dense, Hyper-Complex Percussion with Hexinverter Orbitals

As a eurorack musician, **Hexinverter Orbitals** is an outstanding module for driving dense, intricate rhythmic and percussive sequences—especially when aiming for complex polyrhythms and evolving pattern structures. Here’s how you can harness the features described in the manual:

---

## 1. **Dual (or 16-Step) Sequencing**

- **Polyrhythms:**  
  Operate Orbitals as two independent 8-step sequencers. Send each sequencer’s **gate output** to trigger different percussion modules (e.g., kick, snare, hats). By setting different sequence **lengths** (e.g., 5 steps for A, 7 steps for B), you create natural polyrhythms as the sequences only align after 35 steps.
- **Complex Patterns:**  
  Switch to 16-step mode to program more elaborate percussion patterns. Combine this with sequence length controls to experiment with truncated/extended rhythms (e.g., set A to 11 steps, B to 13).

---

## 2. **Advanced Step Modes**

- **Random & Pendulum:**  
  Use **RND (random)** mode for one sequencer for glitchy, evolving percussion, and **PND (pendulum)** mode for the other to bounce between linear and reverse for organic time-feel shifts.
- **Voltage Addressed Stepping:**  
  Feed unpredictable (LFOs, sample & hold, other random CVs) into the **RST/CV inputs** in “CV” or “CLK” mode to allow the step addressing (and thus, rhythm) to follow complex or modulated patterns.

---

## 3. **Custom Clocking & Time Signatures**

- **External Clocks:**  
  Use complex, non-standard clocks (Euclidean, clock dividers/multipliers, or hand-programmed rhythms) into each sequencer’s **CLK IN** to generate asymmetrical rhythms and custom time signatures.
- **Internal/External Clock Asymmetry:**  
  Clock A and B with different sources or rates for shifting polyrhythms, or clock one internally and the other externally for controlled chaos.

---

## 4. **Gate and CV Programming**

- **Gate Length Tuning:**  
  Use the **GATE knobs** per channel to vary step lengths—ideal for tying gates across steps or creating sudden rolls/bursts.
- **Strategic Gate Steps:**  
  Set specific steps’ gate switches ON/OFF to carve out intricate rhythms, rests, ghost notes, or fills.
- **Gate Outputs as Modulation:**  
  Use the sequencer’s gate outs not just for triggers, but to rhythmically modulate other parameters (VCAs, filters, effect depths) in time with percussion.

---

## 5. **Sync and Transposition for Evolution**

- **SLAVE B>A Switch:**  
  When you want tightly related, evolving patterns, synchronize Sequencer B’s clocking, reset, and run controls to Sequencer A. Allows for tandem evolution or instantly flipping back to independent operation.
- **Transpose Percussion:**  
  Use the **TRANS A input** to shift the CV output, transposing percussion for melodic/rhythmically shifting hits if using pitch-responsive drum sources.

---

## 6. **Voltage Range and Bipolarity**

- **Voltage Ranges:**  
  Set jumper output ranges (see [manual p.8](https://www.hexinverter.net/wp-content/uploads/2015/05/Orbitals_User_Manual_v104.pdf)) to work perfectly with even the oddest drum/CV modules—±2.5V, ±5V, or unipolar 0–5/10V.
- **Bipolar CV for layered modulation:**  
  Use the bipolar mode to modulate drum tuning, morphing, or waveshaping per step for extra animated percussion.

---

## Example Patch Ideas

1. **Polyrhythmic Drums:**  
   - Seq A: 5-step (kick triggers), Seq B: 7-step (snare/hats)  
   - Different clock rates  
   - Random mode on Seq B for glitch fills

2. **CV-Modulated Drums:**  
   - Output CV from a sequencer to pitch/timbre input of a percussion module  
   - Toggle gate switches so only some hits are accented or modulated

3. **Fractal/Euclidean Patterns:**  
   - Use clock dividers/multipliers upstream for complex pulse streams  
   - Route sequencers’ CLK OUTs into logic modules for even wilder layers

---

## Tips:

- **Stacked Patterns:** Use additional logic modules, VCA chaining, or envelope retriggers for layering and further densifying rhythms produced by Orbitals.
- **Manual Performance:** Use the RESET and RUN switches or trigger inputs for real-time fills, breaks, and resets during live performance.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
