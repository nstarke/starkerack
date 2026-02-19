# Vermona — Melodicer

- [Manual PDF](../../manuals/melodicer manual en 1.1 web.pdf)

---

[Download the VERMONA meloDICER User Manual (PDF)](https://www.vermona.com/fileadmin/manuals/MeloDICER_UserGuide_EN.pdf)

---

# Using meloDICER for Dense, Hyper-Complex Percussion and Rhythmic Patterns

The **VERMONA meloDICER** is a stochastic sequencer, capable of generating patterns that range from minimal randomness to full chaos. While it is designed primarily for melodic sequencing, its feature set can absolutely be pushed into the territory of highly intricate, layered, and evolving percussion sequences — including polyrhythms and odd meters.

Below I detail techniques and strategies, based on the manual, for utilizing meloDICER as a *rhythmic brain* in a percussion-focused Eurorack setup.

---

## 1. **Strategic Use of the Rhythm Section**

### **Main Controls: NOTE VALUE, VARIATION, LEGATO, REST**
- **NOTE VALUE:** Sets the base note subdivision. Use 1/8, 1/16, or even 1/32 for rapid-fire rhythms.
- **VARIATION:** Turn this up to introduce *random additional subdivisions*, leading to complex, unpredictable syncopation.
- **LEGATO:** If you want some hits to be "tied" together for double/triple hits (like flams or rolls), increase LEGATO. For classic drum trigger behavior, keep it low.
- **REST:** Crank this up to sporadically remove steps, introducing holes and breath to ultra-dense rhythms.

### **Access More Subdivisions:**
By default, triplets and 1/32 notes in VARIATION are off.  
**To enable them:**
1. Enter EDIT mode (`E` button).
2. Select parameters 6 and 7.
3. Activate triplets and/or 1/32 as desired.
Now VARIATION can randomly access these, opening the door to tuplets and more polymetric rhythms.

---

## 2. **Polyrhythms and Odd Meters**

### **Pattern Length Manipulation for Odd Time Sigs and Polyrhythms**

- **Set pattern length:** Hold `4` or `6` (first/last step) and use the encoder to select arbitrary boundaries.
    - Example: Set pattern length to 5 or 7 or 11 1/16 notes, creating cycles that don’t fit standard 4/4.
- **Move the range:** Hold both `4` and `6`, turn encoder to offset start point for phase-shifted loops (Steve Reich style).

- **Combine with external clocks:** Use irregular external clocks (e.g., 5/8 or 7/8 pulse patterns) into CLK IN to push the meloDICER into non-4/4 domains.

---

## 3. **External Clocking and DAW Sync**

- Use external, non-4/4 clock sources to make meloDICER sequence on top of polymetric, polyrhythmic, or complex time signature backbones.
    - Example: Run a Euclidean or Turing Machine-based trigger sequencer into CLK IN for “irrational” pulse grids.

---

## 4. **Dense Percussion: Utilizing CV and GATE Outputs**

- **GATE OUT**: Drives percussive envelopes, VCAs, or directly triggers drum modules.
- **1V/OCT OUT**: Route to percussion modules with pitch input to create “melodic” perc or to modulate pitch/folder/timbre for punchiness.

#### **Innovative Voice Routing Ideas:**

- Use fast pattern lengths (3, 5, or 7 steps) with active VARIATION and REST to generate stuttering breakcore-style hi-hats or snares.
- Send 1V/OCT to a percussive synth’s pitch (e.g., BIA, Plonk) for zappy, FM-drum-style lines with evolving pitch for each trigger.

---

## 5. **Sculpting Variability: Dice vs. Realtime Mode**
  
- **Dice mode:** Press DICE to lock in generated patterns for tight loops. 
- **Realtime mode:** Hold DICE (LED off) for always-evolving generative sequences—good for unpredictable fill/drum solo variation.
- **Rhythm & Melody independence:** Lock one section to a loop (e.g., dense rhythm grid) while leaving the other in free-random mode.

---

## 6. **CV IN for Algorithmic Modulation**
  
- Assign LFO, S&H, or other modulation sources to meloDICER’s CV INs to morph NOTE VALUE, VARIATION, LEGATO, and REST in real time.
- Patch sequencer or envelope to CV IN2 for CV-controlled rhythmic modulation: e.g., more REST in some bars, more VARIATION in others.

---

## 7. **Advanced Drum Techniques**

- **Gated MUTE and Pattern Restart:** Use GATE IN 2 for rhythmic drop-outs, kill-switch fills, or instant reset-to-start variations.
- **LOCK mode:** Prepare new patterns scaled to intensity or groove, then punch them in at the drop for live “scene” changes.

---

## 8. **Quantizer/Alternative Modes**
  
- **Seq + Gate mode:** Use an external drum sequencer to clock meloDICER’s melody (which you send to percussion modules for tuned percussion).
- **Quantizer 1/2:** Quantize CV from another random or pattern source for “in-scale” pitch percussion or glitchy pitch routings.

---

## 9. **Saving/Recalling Insanity**

- Save your best chaotic/rhythmic patterns and reload for live sets.
- Patterns include random seeds, so you can recall *precise* rhythms that sound algorithmically wild.

---

### **Summary Table: meloDICER for Advanced Rhythms**

| Function                        | Application for Percussion                   |
|----------------------------------|----------------------------------------------|
| Triplet/1/32 Variation           | Polyrhythms & odd subdivisions               |
| Pattern length/offset            | Odd meters, phase cycles                     |
| External clock (odd pulses)      | Polymeter, generative irregularity           |
| REST/LEGATO randomization        | Sporadic drop-outs, rolls, burst effects     |
| CV IN modulation                 | Dynamic intensity, "humanize" machine beats  |
| Locked vs. free random modes     | Repeat fills vs. evolving chaos               |
| Pattern save/recall              | Live performance transitions                 |


---

## Example Patch (Eurorack Context)

1. **GATE OUT** ➔ Envelope Generator ➔ VCA ➔ Noise or Drum Voice
2. **1V/OCT OUT** ➔ Drum module with pitch/frequency control for ghost notes/tuned perc
3. **External Clock IN**: Use Euclidean sequencer with 5/8 or 7/8 rhythm for polyrhythms
4. **Pattern Length**: Set to 11 steps for evolving patterns
5. **CV IN 2**: Envelope or LFO for morphing VARIATION and REST on the fly

---

## Resources

- [Download the VERMONA meloDICER User Manual (PDF)](https://www.vermona.com/fileadmin/manuals/MeloDICER_UserGuide_EN.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
