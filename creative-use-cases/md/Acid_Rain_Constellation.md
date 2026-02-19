# Acid Rain — Constellation

- [Manual PDF](../../manuals/Constellation_Manual_Firmware_1.1_4.7.2025.pdf)

---

[Constellation Firmware V1.1 Manual (PDF)](attachment:Constellation_Firmware_V1.1_Manual.pdf)

---

# Creative Patch Ideas for Acid Rain Constellation V1.1

The **Acid Rain Constellation** is not just a trigger sequencer—it’s a powerful rhythmic brain for Eurorack systems. By harnessing its Euclidean, probabilistic, and layered pattern engines, you can create deeply evolving polymetric and polyphonic rhythms. Below are some creative patch tips and module recommendations for pairing with Constellation, using the features detailed in the manual.

---

## 1. **Dynamic Drum Kits & Percussion Ensembles**

**Patch Idea:**  
Use Constellation's eight channels to trigger a range of drum voices and percussion modules. Each channel can have its own complex pattern, bursts, and probability:

- **Kick Drum:** Constellation Ch1 → Mutable Instruments Peaks/Intellijel Plonk/Any analog kick.
- **Snare/Clap:** Ch2 → Tiptop Audio SD808/Noise Engineering Ruina Versio.
- **Hi-Hats (Closed/Open):** Ch3/4 → ALM Tangle Quartet, WMD Crater, or Pico Drum.
- **Misc Percussion (Rimshot, Cowbell, etc.):** Ch5–8 → Erica Synths Pico Drums, Noise Engineering Basimilus Iteritas.

**Creative Twist:**  
Randomly modulate the ‘chance’ or ‘burst’ of one percussion channel using external CV from a S&H or LFO source for quasi-generative fills.

---

## 2. **Generative Melodic Triggers & Sample Mangling**

**Patch Idea:**  
Connect Constellation outputs to the trigger inputs of a modular sampler (like **Morphagene**, **1010 Music Bitbox**) or to CV-addressable quantizers/sequencers (**Make Noise Rene**, **Malekko Voltage Block**).

- Use Euclidean patterns to drive melodic sample re-triggers, glitch processing, or generative gate chains.
- Assign Constellation’s outputs to gate the step advances of sequencers for non-linear melodic movement.

**CV Inputs Augmentation:**  
Patch slow LFOs (Intellijel Quadratt, Xaoc Batumi) into CV Inputs to modulate pattern length or rotation, making patterns morph organically with time.

---

## 3. **Polyrhythmic Gates for West Coast Synthesis**

**Patch Idea:**  
Feed various Constellation outputs as gates for complex function generators (**Make Noise Maths, Befaco Rampage**), low pass gates (**LxD, Verbos LPG**) or envelope generators that shape the modulation of FM/ring modulation voices.

- Use the flip-flop (flop) function for generating long/short gates to control LPG open/close for percussive versus sustained plucks.
- Employ different channel clock divisions for true polyrhythmic generative west coast percussion.

---

## 4. **Sequence Probability and ‘Controlled Random’ Performance**

**Performance Technique:**  
- Assign ‘chance’/‘ratchet’/‘burst’ parameters to manual CV input controls or foot-pedals for live “on–the-fly” fill creation, glitch moments, or breakdowns.
- Use channel muting/soloing along with the ‘live mode’ to instantly switch up groove sections during performance—think finger-drumming entire rhythm scenes.

---

## 5. **Euclidean Clock & Rhythm Distribution for Entire Racks**

**Patch Idea:**  
Use the internal clock as the master, or receive external clock from **Pamela’s New Workout** (for clock sync, swing, or shuffled groove).
- Use Constellation’s clock/gate outputs to slave multiple sequencers, clock dividers (4MS Rotating Clock Divider, Doepfer A-160-2), or event processors (Westlicht Performer, Hermod).

**Sync/Reset Nuance:**  
Clock and reset everything from Constellation to keep rhythmic structures tight across complex setups, leveraging its robust clock predict/reset management.

---

## 6. **CV-Controlled Save Slot Changes and Scene Morphing**

**Patch Idea:**  
Use the new CV input assignment for ‘load’ to trigger instant recall of entire rhythmic scenes from other modules capable of generating gates at key moments (e.g. End of Cycle output from a function generator).  
- Seamlessly jump between different saved drum patterns or polymetric grooves—great for live sets.

---

## 7. **Injecting Probabilities into Traditional Step Sequencers**

**Patch Idea:**  
Sync a step sequencer (e.g. **Intellijel Metropolis**, **Winter Modular Eloquencer**) from Constellation’s clock out, but occasionally override expected step triggers by mixing in an irregular Euclidean pulse from Constellation into the step input.

- Intermittently “skip” or accent certain steps of a linear sequence for controlled randomness.

---

## 8. **Microtiming and Human Groove**

**Patch Idea:**  
Leverage Constellation’s per-output microtiming (channel clock rotate/delay) to offset triggers, mimicking swing or flam, and manufacturing microgrooves.

- Use this to create shuffle on hats, slightly early/late snares, or polymetric “push” in polyphonic voice triggering.
- Assign modulation to width for varying gate lengths and making phased, evolving gate pulses for modulating filters/envelopes.

---

## 9. **Self-Modulation and Cross Modulation**

**Patch Idea:**  
Use a channel’s output to clock/modulate the CV input of another channel or pattern, creating recursive rhythmic structures (e.g., Ch8 triggers CV Input 1, which modulates Ch1 ‘length’ or ‘chance’).

---

## 10. **Generative Breakbeat/Glitch Textures**

**Example Patch:**  
- Patch outputs with high burst/ratchet/random settings into fast attack envelope generators.
- Send envelopes to amplitude-modulate samples, granular processors, or wavefolders (e.g. **Make Noise Mimeophon**, **Qu-Bit Nebulae**, **SSF Entity Ultra-Kick**).

---

### Interesting Module Pairings

- **Pamela’s PRO Workout:** Tight master clock, groove templates, randomization.
- **Winter Modular Eloquencer, Hermod, Nerdseq:** Step sequencer brain, great for integrating with advanced rhythm.
- **Mutable Instruments Branches:** Probability gate processor, stacks with Constellation’s chance for multi-level randomness.
- **4MS QPLFO, Batumi:** Slow evolving modulation, perfect for CV inputs.
- **Erica Synths Drum Modules, Noise Engineering percussion:** For deep drum voice variety.
- **Intellijel Plonk, 2hp Pluck:** Expressive percussive synthesis engine sources.

---

## General Creative Tips

- **Layer simple and complex:** Use some channels for bread-and-butter “foundational” meters (4/4), and others for sparse, random, polyrhythmic accents—this generates both familiarity and surprise.
- **Scene juggling:** Use live mode and CV scene recall for performance—treat Constellation as a “groove box” brain for your modular set.
- **Probability and modulation:** Routinely switch up which parameters respond to CV or random gates to avoid repetition and maximize surprise.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)