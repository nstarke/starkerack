# After Later Audio — Ornament and Crime

- [Manual PDF](../../manuals/ornament and crime.pdf)

---

[Ornament & Crime v1.3 Firmware User Manual (PDF)](https://ornament-and-cri.me/user-manual-v1_3/)

---

# How to Use the Ornament & Crime to Build Full-Length Eurorack Songs

Ornament & Crime (“o_C”) is not just a clever quantizer or utility—it’s a deep, polymorphic toolkit that can drive structure, variation, and musical storytelling in a Eurorack system. Below, you’ll find practical strategies to go beyond catchy loops and into song-form, using o_C as the backbone or heart of your modular compositions.

---

## Core Concepts for Song Construction

### 1. **Scenes, Sections, and Recallable States**

- **Presets/State Save**: The o_C can save the state of all its apps and channels. Use this as an instant “scene change”—moving from verse-like states to chorus-like states with a long press of the encoder, recalling saved setups.
- **Manual or CV Scene Control**: Assign a CV (from another module like a sequencer, manual controller, or Planar/Vector joystick) to modulate parameters or even switch apps/states to jump between parts—e.g., swapping from melody lines to quantized harmonies or changing clock divisions.

### 2. **Self-Generating and Evolving Structures**

- **Internal Sources**: Use o_C’s internal bytebeat, Turing Machine, logistics, or integer sequence generators as non-repeating, evolving sources for melody/bass/rhythm, avoiding static repetition.
- **CV Assignment**: Modulate sequence length, active note mask, clock division, or quantizer root in real time, either manually or with slow modulation, to introduce gradual change and “movement” across sections.

### 3. **Euclidean and Polymetric Rhythms (Piqued, Harrington 1200, Sequins, Acid Curds)**

- Harness Euclidean rhythm generation or sequence cycling to create rhythmic sections/variations: 
  - **Intro:** Sparse rhythms, longer Euclidean cycles.
  - **Verse:** Denser fills.
  - **Chorus:** Polyrhythms (Euclidean masks + fast clocks).
- Use envelope segments as rhythmic CV sources elsewhere—self-patching or routing to VCA/VCF, or triggering/clocking external envelopes.

### 4. **Chord Progression & Harmonic Movement**

- **Harrington 1200 & Acid Curds:** Control chords, inversions, and progressions; automate these with manually advanced triggers, clock dividers, or CV assigned to progression or mode.
    - Example: One progression for “verse,” another for “chorus,” cycling through or gating between them.
- Output root/chord CVs to voice multiple oscillators/VCOs for rich harmonies, or trigger chord changes via external gate sources (gestural performance, sequencer gates, or MIDI-to-CV modules).
  
### 5. **Melodic Structures and Melodic Variation (Sequins, Quantermain, Meta-Q)**

- Use **Sequins** for up to 64-step melodies or bass lines, chaining them for A/B/C sections.
    - Assign CV to step, length, mask, clock rate—controlled by other sequencers/LFOs/programmed modulation sources to vary melody over time.
- Employ **Meta-Q / Quantermain** to continuously or step-wise quantize incoming voltages, shifting scales, roots, masking notes for modal change, or variation, again assignable to external CV or LFOs for progression and development.

### 6. **Automation of System Parameters**

- Self-patch outputs: Use o_C’s own modulation or logic outputs (from say, Piqued envelopes or random sources) to control or modulate its own settings or those of other modules (via CV attenuators or logic).
- External modulation: Route LFOs, random, or stepped CV into o_C’s assignable parameters for emergent, non-repetitive structure (slow LFOs for subtle change; fast CV for ratchets, abrupt scene changes).

---

## Concrete Song-Building Techniques

### **A. Multichannel Song Parts from a Single o_C**

1. **Drums/Percussion:**  
   - Use Piqued for Euclidean trigger envelopes—patch out to EG/VCA for percussion sources or send gates to external drum modules.
2. **Bass Line:**  
   - Use Sequins as a 16+ step bass CV sequencer, or Quantermain to quantize random CV to a stable bass line.
3. **Lead & Harmony:**  
   - Harrington 1200 for chords, Quantermain for melody. Both can share the same clock, or intentionally de-sync for more complex phrasing.
4. **Automated Transitions:**  
   - Assign CV from a macro controller, manual switch, envelope, or slow LFO to swap chord progressions, sequence chains, or root notes.
   - Use the CV-to-slot system in Meta-Q or Sequins to “flip” between different sequences or masks.

### **B. Sectional Song Development**

- **Verse:**  
  - Activate slot 1 in Sequins with a basic scale and rhythm; play a specific chord progression on Acid Curds; simplified rhythm on Piqued.
- **Chorus:**  
  - Switch to slot 2 in Sequins, use a different pattern; swap Acid Curds progression; open up Piqued’s rhythm or introduce ratchets.
- **Bridge:**  
  - Use randomized or Turing-sourced quantization, add logic/chaos modulations to pitch or rhythm, etc.

### **C. Live Performance & Improvisation**

- Leverage state save/recall to prepare song sections in advance.
- Use external manual controllers (Pressure Points, Planar) to live-modulate o_C parameters.
- Modulate into and out of chaos—LFO sweeps, ramp-up LFSR “random” sources, and gradually restrict scale masks back to consonance for dynamic tension/release.

---

## Example Patch for a Full-Song Structure

**Setup:**
- Channel A: Drums (Piqued envelopes trigger VCAs/drum modules)
- Channel B: Bassline (Sequins, quantized & stepped)
- Channel C: Chord CV (Acid Curds or Harrington 1200 feeding three VCOs for chords)
- Channel D: Lead (Quantermain, quantizing modulated LFO for evolving melody)

**To Create Sections:**
- Use external switch/macro controller to change:
    - Sequins sequence slot (bass)
    - Chord progression slot (chords)
    - Quantizer root/note mask (lead)
    - Piqued Euclidean fill/length (rhythm density)
- Fade sections by using attenuverters/VCA on CV controlling o_C parameters, for discrete or slow morphing transitions.

---

## Supporting Tips
1. **Self-Referencing & Cross-Modulation:** Patch o_C’s outputs as CV sources for its own parameters (recursive structure).
2. **Automation via Other Modules:** Integrate with external sequencers, voltage memories, or complex random sources for higher structure (8-step switch, WMD Performance Mixer for macro control, etc.).
3. **Manual Performance:** Prepare scene changes, and play transitions live by holding, releasing, or switching encoder/parameters at moments of highest drama.

---

By combining these techniques, the Ornament & Crime can act as a central “brains” for not only starting strong musical ideas, but evolving them to become cohesive, full-length songs—automatically, performatively, or in hybrid style.

---

[Manual PDF - Ornament & Crime v1.3](https://ornament-and-cri.me/user-manual-v1_3/)  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
