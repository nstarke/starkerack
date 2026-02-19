# Sea Side Modular — Proteus

- [Manual PDF](../../manuals/ProteusManual.pdf)

---

[Download the Seaside Modular Proteus Manual (PDF)](https://seaside.digital/proteus/proteus_manual.pdf)

---

# Creative Uses for Seaside Modular Proteus in Eurorack Setups

The Proteus is a generative melodic sequencer with probabilistic and “humanized” algorithms, making it an endlessly versatile source for melodies, triggers, and evolving patterns. Here’s how you can creatively use Proteus in a Eurorack setup:

---

## 1. **Melodic Generative Voice**
   - **Basic patch:** Proteus V/OCT ➔ VCO (e.g. ALM MCO, Mutable Plaits) ➔ VCF ➔ VCA ➔ Output; Proteus GATE OUT ➔ Envelope Generator (e.g. Make Noise Maths) ➔ VCA.
   - **Tip:** Use different scales and pattern bank features to quickly switch mood and tonality during performance.

## 2. **Melody Modulation with External CV**
   - **Modulation:** Send random or evolving CV to Proteus parameters (DENSITY, COMPLEXITY, PATIENCE, etc.) using modules like ALM Pamela’s New Workout, Mutable Stages, or Make Noise Maths.
   - **Result:** Melodies morph over time, providing organic movement.

## 3. **Interactive Mutations**
   - **Performance:** Patch gate/trigger outputs from a performance-oriented controller (e.g., Intellijel Tetrapad, Make Noise Pressure Points) to the NEW or NEXT jacks to force new melodies or cycle through pattern slots on demand.

## 4. **Clock Manipulation and Experimentation**
   - **Non-standard rhythms:** Use clock divider/multiplier modules or irregular clocks (e.g., 4ms QCD, Pamela’s New Workout, or random clocks from Mutable Marbles) into GATE IN for polyrhythms or euclidean patterns.

## 5. **Layered Voices/Polyphony**
   - **Double/triple melodic layers:** Run Proteus V/OCT OUT through a precision adder (e.g., Doepfer A-185-2) for harmonized lines, or use a quantizer downstream (e.g., Intellijel Scales) for harmonies.
   - **Tip:** Use two voices—one dry, one slewed (add slew via a module like Mutable Instruments Tides or Doepfer A-171-2)—for melodic counterpoint.

## 6. **Probability-Based Percussion**
   - **Gate output to percussive voice:** Patch GATE OUT to a percussive module or drum synth (e.g., Mutable Peaks, WMD Crater).
   - **Use density and sleep:** Set DENSITY to lower to create less dense, shifting patterns, or use SLEEP for rhythmic gaps.

## 7. **Generative Song Structure**
   - **Pattern Bank + Scene Control:** Use external sequential switches (e.g., Doepfer A-151, Erica Synths Sequential Switch) to switch between multiple melodic outputs, each with unique Proteus patterns or scales, forming “parts” of a composition.

## 8. **Generative Ambient / Drone Work**
   - **Melodic drone:** Patch through plenty of reverb & fx (e.g., Make Noise Mimeophon, Strymon Magneto).
   - **Octave & mutate:** Let Proteus’ mutate/octave parameters wander for shifting pads.

## 9. **Melody Quantization/Non-Quantized Synthesis**
   - **Patch through or around external quantizers:** Proteus can be quantized or not; but for “microtuning” or Scala scales, combining Proteus with Disting mk4/Hemisphere Suite or ADDAC207 Intuitive Quantizer can yield Slendro, Just Intonation, or user-drawn scales.
   - **Layer quantizers:** Send Proteus CV into a quantizer locked to a different scale for complex melodic interplay.

## 10. **Logic-Based Harmony and Counterpoint**
   - **Logic Processing:** Run GATE OUT and/or generated melodies through logic modules (e.g., Mutable Kinks, Doepfer A-166 Dual Logic) to derive new rhythmic or melodic material triggered only on particular combinations/changes in Proteus sequence.

## 11. **CV Memory Morphs**
   - **Morph between patterns:** Save versions of a melody at different moments in Pattern Bank, and step/blend between them using the NEXT jack and external latching switches or even sequential control voltages.

## 12. **Experimental Percussion or Voltage Source**
   - **Non-melodic applications:** Use Proteus OUT (tuned to atonal or custom microtonal scales, or with low density and short sequences) to modulate parameters in other modules—VCFA cutoff, delay time, granular fx—using pitch as a generic control voltage.

---

## **Module Recommendations**
- **Random Sources:** Mutable Marbles, Toppobrillo Sport Modulator 2
- **Slew-Filled Voices:** Make Noise Maths, Doepfer A-171-2
- **Quantizers:** Intellijel Scales, Disting mk4, ADDAC207
- **Switches:** Doepfer A-151, WMD Sequential Switch Matrix
- **Percussive Voices:** Mutable Peaks, Tiptop 808/909 series, Noise Engineering Basimilus Iteritas Alter
- **Reverb/Delay:** Strymon Magneto, Make Noise Mimeophon, Mutable Beads

---

## **Generic Patch Ideas**
- Stack two melodies (Proteus + other sequencer) into a mixer for “duet” textures.
- Use Proteus patterns to control not pitch, but complex timbre changes: send CV to LPG, filter cutoff, reverb mix, etc.
- Use “sleep” or “density” at minimum for random emphasis—sharp trigger patterns for glitch or IDM effects.

---

**Link:** [Manual PDF](https://seaside.digital/proteus/proteus_manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)