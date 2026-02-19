# 2hp — Pluck

- [Manual PDF](../../manuals/2hp_Pluck.pdf)

---

[2hp Pluck Manual PDF](https://2hp.com/wp-content/uploads/2019/12/Pluck_Manual.pdf)

---

## Creative Ways to Patch 2hp Pluck in Your Eurorack System

**2hp Pluck** is a 2HP-wide, Karplus-Strong algorithm-based string voice, designed for physical modeling synthesis with up to four voices of polyphony. It's super compact but very powerful — making it an ideal tool for adding plucked string timbres and "acoustic-esque" textures to your rack. Here are some creative patch ideas, along with suggestions of other modules (both specific and generic) that combine brilliantly with Pluck.

---

### 1. Polyphonic Sequencing & Chord Stabs

- **Idea:** Take advantage of Pluck’s four-voice polyphony for melodic content, arpeggios, or chord stabs.
- **How:** Use a polyphonic MIDI-to-CV converter (e.g., **MIDI 1U from Intellijel**, or **Polyend Poly**) to send polyphonic gates and CVs to Pluck’s V/Oct and Trig.
- **Patch:** Connect up to four gate/CV lanes; play chords or arpeggios from your DAW or MIDI keyboard. You could transpose the root with a sequencer or quantizer for more complex progression.

---

### 2. Physical Modeling Percussion

- **Idea:** Use Pluck as more than just a "string voice." With short decay and high damping, it can sound like percussive hits, wooden blocks, or even synthetic drums.
- **How:** Patch random or Euclidean gate patterns from a trigger sequencer (e.g., **Pamela's Pro Workout**, **Mutable Instruments Grids**) to Trig. Modulate DAMP/DECAY (with LFOs, envelopes, or random sources) to emulate natural subtle variations.
- **Patch:** Clock Pamela’s into Pluck’s TRIG, send random CV (e.g., from **Wogglebug**, **Turing Machine**, or **Marbles**) into DAMP and DECAY. Output can be processed through short stereo delays for extra realism.

---

### 3. Expressive, Modulated Strings

- **Idea:** Use envelopes or complex LFOs to modulate DAMP and DECAY, providing dramatically shifting timbres.
- **How:** Try assigning separate envelopes to DAMP and DECAY, with an expressive controller (e.g., **Make Noise Maths**, **Intellijel Quadrax**, or **ALM Pip Slope**).
- **Patch:** Use a pressure CV from a touch controller (e.g., **Make Noise 0-CTRL**) to DAMP, and let a longer envelope modulate DECAY. Gesture-based performance is very rewarding here.

---

### 4. “Strummed” Chords with Switches/Sequential Gate Controllers

- **Idea:** Use manual gate generators/switches (e.g., **Intellijel Tetrapad**, **Doepfer A-182-2**, or **Mutable Instruments Mutable Grids**) to “strum” chords or trigger fast arpeggios, playing Pluck almost like a real instrument.
- **How:** Patch sequential gates to the TRIG input and quantized CVs to V/Oct.
- **Patch:** A quantizer or pitch CV selector can step through a chord; a switch controller can fire triggers in a rhythmic pattern.

---

### 5. Processing the Output

- **Idea:** Run the sharp, plucked output to FX for new timbres.
- **How:**
  - **Reverb:** Emphasize the naturalistic quality (e.g., **Make Noise Mimeophon**, **Strymon Magneto**, **Erica Synths Black Hole DSP**).
  - **Filter:** Sweepable low-pass for duller or "muted" string sounds.
  - **Ring Modulation or Wavefolder:** Get harmonically dense, metallic, or prepared-piano effects (**Doepfer A-133**, **Intellijel Bifold**, **Ring Modulator**).
- **Patch:** Output → FX → Mixer; try CV controlling effects (e.g., reverb decay, filter cutoff) in time with Pluck’s damping for shifting spatial illusions.

---

### 6. Algorithmic/Generative Pluck Playing

- **Idea:** Use random or generative gate sources (e.g., **Mutable Instruments Marbles**, **ALM Pamela’s Pro Workout**, **Ornament & Crime** in gate sequencing modes) to create ever-changing melodic figures or textures.
- **How:** 
  - Random gates → TRIG.
  - Quanitized random or generative voltages → V/Oct (for melodic lines).
  - Slow random or S&H → DAMP/DECAY (for organic movement).
- **Patch:** Let the system surprise you with evolving pseudo-acoustic patterns.

---

### 7. Layering with Other Voices

- **Idea:** Stack Pluck with subtractive or FM synths for a hybrid string lead.
- **How:** Mult your gate/CV signals to Pluck and another voice (e.g., **Mutable Instruments Plaits**, **2hp VCO** + VCF/VCA).
- **Patch:** Mix both signals together or layer through a crossfader for morphing timbres—e.g., string/plucked attack and sustained analog pad.

---

### Module Compatibility (Quick Reference)

- **Sequencers:** Make Noise Rene, Malekko Voltage Block, Intellijel Metropolis
- **Random CV:** Mutable Instruments Marbles, Turing Machine, Noise Tools
- **Envelopes & LFOs:** Maths, Quadrax, Batumi
- **Effect Modules:** Mimeophon, Magneto, Black Hole DSP, Erica Fusion Delay
- **Polyphonic Gate/CV:** Polyend Poly, MIDI 1U

---

### Final Tips

- **Attenuate CVs** before sending to DAMP/DECAY for more subtlety. Many modules output stronger CV ranges than you need: use an attenuverter or mixer if things get too wild!
- **Experiment with feedback** by routing Pluck’s output into a delay or reverb with a feedback path—imitating resonant instruments or prepared pianos.
- **Acoustic Emulation:** Patch Pluck through an EQ, then a reverb with early reflections for extreme realism.

---

For full details, check the [Full 2hp Pluck Manual (PDF)](https://2hp.com/wp-content/uploads/2019/12/Pluck_Manual.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)