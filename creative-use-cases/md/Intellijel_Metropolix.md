# Intellijel — Metropolix

- [Manual PDF](../../manuals/metropolix_manual_v1.4_2022.04.04.pdf)

---

[Metropolix Manual PDF](https://intellijel.com/downloads/manuals/metropolix/Metropolix_Manual_v1.4.pdf)

# Creative Modular Patching Ideas With Intellijel Metropolix

As a Eurorack musician, the Intellijel Metropolix is a goldmine for live performance, generative music, and modular experimentation. Its unique sequencing approach, deep modulation options, and multi-track architecture enable wild creative combinations—especially when paired with other modules. Below you'll find a selection of creative ideas, patch strategies, and some module recommendations to inspire fresh musical and performative directions.

---

## 1. **Dual Voice Counterpoint with Complementary Sound Engines**

**Concept:**  
Exploit Metropolix's independent tracks (TRK 1 and TRK 2) to generate harmonically related yet rhythmically distinct melodies.

- **Suggested Combo:**  
  - [Make Noise STO](https://makenoisemusic.com/modules/sto) (TRK 1)  
  - [Mutable Instruments Plaits](https://mutable-instruments.net/modules/plaits/) (TRK 2)

- **Technique:**  
  - Set differing playback ORDER, LEN, and DIV for each track, creating intertwining counterpoint lines.
  - Use the same clock for tight timing, or clock TRK 2 at an odd division for polymetric interplay.
  - Run each through different effects (e.g., reverb for one, delay for another) to maximize separation.
  - For generative harmonic shifts, modulate the scale or root globally, or sequence User Scales via MOD lane/AUX.

---

## 2. **Sequencer-Driven Rhythmic Effects**

**Concept:**  
Harness per-stage gate, probability, and ratchet control to trigger non-pitch events, like rhythmic gating of effects or VCAs.

- **Suggested Modules:**  
  - **VCAs:** Intellijel Quad VCA, ALM Tangle Quartet  
  - **Effects:** Mutable Instruments Clouds, Strymon Magneto (using sequenced triggers for freeze/record)

- **Technique:**  
  - Assign OUT A or B to a MOD lane or track's CV lane set to "Gate Toggle."
  - Patch OUT A/B to a VCA CV input for rhythmic amplitude modulation or to a CV/gate-enabled effect.
  - Use per-stage probability for morphing, semi-random muting of effects.
  - Modulate ratchets to create fast, chopped FX bursts or granular freezes.

---

## 3. **Complex CV Modulation of External Parameters**

**Concept:**  
Sequence envelopes, LFO speeds, filters, or any CV-controllable parameter with Metropolix's MOD lanes.

- **Suggested Module Types:**  
  - **Filters:** Mutable Ripples, Tiptop Forbidden Planet  
  - **Envelope Generators:** Maths, Zadar  
  - **Waveshapers, Function Processors:** Befaco Rampage, Intellijel Bifold

- **Technique:**  
  - Assign MOD Lanes to OUT A/B (set to "Mod").
  - Design evolving or stepped CV shapes/per stage in the MOD lane.
  - Assign per-stage voltage ramps (smooth or abrupt) to subtly morph tone or envelope times on each step.
  - Use the "ramp" mode for smooth transitions, "step" for abrupt changes—great for sample & hold effects.

---

## 4. **Generative Self-Modulation and Feedback Networks**

**Concept:**  
Metropolix's internal modulation (via MOD lanes, AUX inputs, or randomized parameter features) can feedback on itself to create evolving patches.

- **Advanced Patch Example:**  
  - Assign MOD Lane 2 to modulate TRK 1's probability or playback order.
  - Patch a random voltage source (like Wogglebug or Marbles) into AUX X, assign X to modulate LEN or swing.
  - Use Z output to reset accumulator or swap track outputs mid-pattern.
  - Periodically randomize a stage’s settings live using ALT + AUX buttons for controlled chaos.

---

## 5. **Polyphonic or Chordal Eurorack Using Quantized CV Lanes and Multiple Oscillators**

**Concept:**  
Use CV lanes and/or multiple tracks/LFOs to control more than two voices for richer harmonic content.

- **Suggested Module:**  
  - Tiptop Audio Poly2 or Mutable Instruments Polyphonic OSCs

- **Technique:**  
  - Align MOD lane voltages (by hand or via user scales) for chord voicing.
  - Sequence roots with TRK 1, thirds or fifths with MOD lanes out to quantizer/extra oscillators.
  - Use external precision adders (e.g., Doepfer A-185-2) to sum CVs for more complex chords.
  - Modulate scale or root note for dreamy chord progressions.

---

## 6. **Morphing Percussive Sequences**

**Concept:**  
Animate percussion by using MOD lanes or track CVs to control drum module parameters.

- **Suggested Drum Modules:**  
  - Endorphin.es BLCK_Noir  
  - Mutable Instruments Peaks  
  - Erica Synths Pico Drums

- **Technique:**  
  - Assign per-stage ratchets for fast rolls.
  - MOD lanes to tune, decay, or effect depth on drum modules.
  - Use gate outputs for parameter locking, triggers, or accent inputs.

---

## 7. **MIDI and DAW Integration**

**Concept:**  
Use Metropolix's MIDI features to sequence or modulate external synths, drum machines, or virtual instruments.

- **Technique:**  
  - Route MIDI through the USB port (optionally using the Intellijel USB Extender).
  - Assign MOD lanes or CV lanes to output CCs for dynamic control of soft synths or hardware.
  - Sequence DAW drums or samples via trigger outputs.

---

## 8. **Expander Magic**

**Concept:**  
Expand Metropolix with a Gx/Qx for up to 8 additional gates—ideal for triggering drum modules, events, or clocking other sequencers.

- **Suggested Uses:**  
  - Trigger drum steps, clock Bastl Popcorn, reset other sequencers, or use stage gates for live performance macros.
  - Use probability clocks for generative rhythms and textures.

---

## 9. **Performance Gestures & Live Jamming**

**Concept:**  
Set up CTRL knobs for macro-performance controls such as Trk Out Swap (for instant voice swapping), Probability ±, or Slide Amount for acid-infused lines.

- **Technique:**  
  - Prepare a set with "Thru" or "Jump" preset options for instant recall of previous jams.
  - Live randomize via ALT + AUX for "happy accident" fills or improv breaks.

---

### **Patch Note**
- Chain multiple patch ideas: e.g., poly-sequencing and CV modulation of filters for animated, harmonically rich modular drones with glitchy drum accents.
- Always remember to experiment with sequence order, stage skip, and accumulator functions for non-repetitive, emergent music.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)