# 4ms — Rotating Clock Divider

- [Manual PDF](../../manuals/RCD-manual-1.2.pdf)

---

[4ms Rotating Clock Divider User Manual PDF (via 4ms company)](https://4mscompany.com/p.php?p=180&)

---

# Creative Patch Ideas for the 4ms Rotating Clock Divider (RCD)

The 4ms Rotating Clock Divider is a highly flexible module that can serve as the rhythmic heart of a Eurorack system. Its unique clock division, rotation, reset, and spread features open it up to a huge range of creative clocking techniques, sequencing manipulation, and generative rhythms. Here are some patch ideas and module combinations to get the most out of the RCD:

---

## **1. Polyrhythmic Trigger Sequencing**  
**Patch Concept:** Use the multiple divided outputs to create complex rhythms.

- **Modules:**  
  - Drum modules (e.g., Hexinverter Mutant Drums, ALM Busy Circuits Akemies Taiko, Tiptop Audio drum modules)
  - Step sequencer or trigger sequencer
  - Mixer for gate/trigger summing (optional)

**How:**  
Patch different RCD outputs (/3, /5, /6, etc.) directly into drum module trigger ins. This generates overlapping, evolving polyrhythms out of a single master clock. Fiddle with the "Rotate" CV (perhaps with an LFO, random generator, or sequencer) to shift all rhythms in real time! Patch one divided output to a sequencer’s clock in and another to a kick, for shifting groove relationships.

---

## **2. Probabilistic & Generative Audio Events**  
**Patch Concept:** Add controlled randomness for generative music.

- **Modules:**  
  - Mutable Instruments Branches, WMD Probabilty Javelin (probability/skipping modules)
  - Mutable Instruments Marbles (random/generative trigger generator)
  - Doepfer A-149-1/2 or other random voltage sources

**How:**  
Use one or more RCD outputs to drive probabilities in a module like Branches (e.g., /7 or /8), so events only fire on certain steps. Rotate CV input can be sequenced or randomly modulated for evolving rhythmic probabilities. You can even reset the RCD with another divided output for generative rhythm cycles.

---

## **3. Synchronized but Evolving LFO/Envelope Triggers**  
**Patch Concept:** Trigger multiple envelopes or LFO syncs for coordinated modulation.

- **Modules:**  
  - Intellijel Quadra, Make Noise Maths, ALM Pip Slope, or other envelope/LFO modules
  - Oscillators or Filter modules (for modulating timbre, amplitude, etc.)

**How:**  
Send RCD outs to envelope/LFO trigger ins. The diverse clock divisions create movement in filter cutoff, pitch, or amplitude that’s still musically tied to the master clock. Rotating or resetting brings instant variation while staying tight to the tempo.

---

## **4. Clocking Multiple Sequencers or Effects**  
**Patch Concept:** Clock several sequences with shifting offsets.

- **Modules:**  
  - Intellijel Metropolis, Make Noise Rene, Arturia BeatStep Pro, or other sequencers
  - Tap-tempo delay or synced effects modules (e.g., 4ms Dual Looping Delay, Intellijel Rainmaker)

**How:**  
Drive multiple external sequencers or delay/sync inputs with different divisions. Rotate CV shifts all sequences’ placement instantly, causing abrupt rhythmic remixes.

---

## **5. Drum Machine Remixing/Probability Manipulation**  
**Patch Concept:** Insert the RCD before a drum sequencer for glitchy, chopped, or evolving beats.

- **Modules:**  
  - Any step sequencer with external clock in (e.g., Erica Synths Drum Sequencer, Tiptop Circadian Rhythms)
  - WMD Chimera, Hexinverter Mutant Rimshot, etc.

**How:**  
Drive the sequencer’s clock with a nonstandard divided output, rotating for groove variation, or reset from a longer clock to induce bucked, swung, or chopped feel in the beats.

---

## **6. Advanced Euclidean and Spread Rhythms**  
**Patch Concept:** Create spaced, musical divisions via Spread mode.

- **Modules:**  
  - Euclidean trigger modules (e.g., vpme.de Euclidean Circles, Mutable Grids)
  - Drum modules or sequencers

**How:**  
Turn on Spread mode and clock drums or accent triggers with musically useful divisions (e.g., /4, /8, /12, /16). Rotate to explore tightly grouped or widely spaced steps. Perfect for minimal techno and IDM grooves.

---

## **7. Frequency Division in Audio-Rate Patches**  
**Patch Concept:** Use high-frequency clock input and abuse RCD as a subharmonic generator.

- **Modules:**  
  - VCO (e.g., Intellijel Dixie II+, Mutable Braids, etc.)
  - Audio mixers and distortion FX

**How:**  
Feed a square wave VCO to the RCD's clock input. The outputs provide stepped-down subharmonic square waves (octaves and divisions of the original frequency). Can be used as audio-rate clocking for Karplus-Strong, pseudo-chord creation, or gritty drone textures.

---

## **8. Master Clock Distribution and Reset**  
**Patch Concept:** Keep a patch in sync with regular global resets.

- **Modules:**  
  - Pamela's New Workout, ALM Busy Circuits Pamela's Pro Workout (master clock/generator)
  - Sequential switch (e.g., Doepfer A-151 for patch switching on reset)

**How:**  
Patch a divided RCD output (like /16 or /32) to the reset inputs of sequencers or clocked effect modules so all sync to the same “downbeat” or phase point as the global clock. Use CV Reset input for more controlled, performative global resetting.


---

## **Bonus: Hands-Off Variation with CV Sources**
- **Use LFOs, random voltages (Wogglebug, Turing Machine), step sequencers, or even envelope outs to the Rotate CV or Reset CV inputs for shifting, “alive” clock architecture.**

---

### **Module Pairing Recommendations**
- **CV sources:** Intellijel Quadrax, Maths, Mutable Instruments Stages/Marbles, Malekko Voltage Block  
- **Random Generators:** Make Noise Wogglebug, SSF Ultra-Random Analog  
- **Logic/Utilities:** Mutable Instruments Kinks, Intellijel OR/AND, Doepfer A-166  
- **Clock Manipulators:** Pamela’s New Workout, ALM mmT, 4ms Shuffling Clock Multiplier  
- **Drum/Trigger Receivers:** Any drum synth, envelope, or sequencer module

---

### **General Tips**
- Experiment with Spread mode ON vs OFF for very different feels.
- Use GATE vs TRIGGER output mode to change the way downstream modules respond.
- Invert counting (up/down) for pattern inversion.
- Consider using the RCD Breakout for more live control.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)