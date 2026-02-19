# 2hp — Turing Machine

- [Manual PDF](../../manuals/TM_Manual.pdf)

---

[**TM (2hp) Module - Manual PDF**](https://2hp.com/manuals/TM.pdf)

---

## Creative Patch Ideas for the 2hp TM Module

The 2hp TM (Turing Machine) is a compact and flexible probabilistic random sequence generator. With probability, sequence length, and amplitude controls, it can deliver everything from wild random CV to quantized melodic sequences. Here’s how you can creatively extend its core functionality by combining it with other Eurorack modules:

---

### 1. **Generative Melodies with a Quantizer**
- **Patch Idea:** Send TM’s OUT to a **quantizer** (e.g., **Intellijel µScale II**, **Doepfer A-156**). The quantizer will constrain TM’s random voltages to musical notes.
- **Benefit:** Produces endless evolving melodies that stay in key. You can further refine the "randomness" by adjusting TM’s probability knob.

### 2. **Controlled Random Modulation**
- **Patch Idea:** Patch TM OUT to modulate a filter cutoff (**VCF**), wavefolder, or oscillator pitch CV. Trigger TM with an irregular gate source (e.g., **4ms QCD**, **Pam's New Workout**).
- **Benefit:** The probability and sequence length become hands-on tools for controlling how stable or chaotic your modulation is—great for generative textures or shifting atmospheres.

### 3. **Probability-Driven Sequencing**
- **Patch Idea:** Use TM as a CV source for a **sequencer’s** transpose input (e.g., **Make Noise René**, **Arturia Keystep Pro** CV IN).
- **Benefit:** Introduces semi-random melodic variations layered over traditional sequences, making rigid patterns more expressive and alive.

### 4. **Rhythmic Randomization**
- **Patch Idea:** Mult TM OUT to multiple destinations (using a passive or buffered mult), modulating several drum module parameters at once (e.g., pitch, decay, or timbre on modules like **Mutable Instruments Plaits** or **Noise Engineering Basimilus Iteritas**).
- **Benefit:** Each trigger can subtly re-shape your drum sounds, resulting in non-repeating and organic beats.

### 5. **Randomized Harmonic Chords**
- **Patch Idea:** Send TM OUT through an **analog shift register** (like **Doepfer A-152** or **Mutable Instruments Branches**) to generate related, shifting harmonic intervals.
- **Benefit:** You can use the shifted outputs to drive a bank of oscillators tuned to harmonize, for lush and strange random chord progressions.

### 6. **Probability-Locked Sequence as CV LFO**
- **Patch Idea:** Turn probability all the way right (0%) to lock the sequence, then vary the number of steps. Use OUT as a stepped CV LFO to modulate parameters like reverb mix (e.g., **Make Noise Mimeophon**) or a granular sampler’s position.
- **Benefit:** Interesting for “pseudo-repeating” modulation that isn’t strictly cyclic—great for slow evolving pads and textures.

### 7. **Probability Morphing with External CV**
- **Patch Idea:** Modulate the PROB control with a slow LFO or envelope, sweeping between random and locked sequences over time (try **Mutable Instruments Tides** or **ALM Pamela’s Pro Workout**).
- **Benefit:** Lets randomness itself ebb and flow, introducing emergent structure and variation to your patches.

### 8. **Live Performance Tweaks**
- **Patch Idea:** Map STEPS or AMP to tactile or performative CV controllers (like **Planar2** or **Pressure Points**), for real-time manipulation of how much randomness hits your patch.
- **Benefit:** Instant hands-on control and playability, ideal for improvisation or subtle dynamic changes during a live set.

---

## **Generic Module Pairings**

- **Quantizer** (for melodic context)
- **Low Pass Gate / VCF** (random timbral movement)
- **Sequencer** (injecting randomness)
- **Clock Generators/Dividers** (complex rhythms)
- **Switches/Multiples** (spread TM CVs across voices)
- **Sample & Hold / Analog Shift Register** (complex random motion)
- **Envelope Generator** (dynamic amplitude control via TM OUT)

---

The TM module’s small size belies its versatility and generative power—its randomness, if tamed and contextualized with these companion modules, becomes a source of endless creative variation.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)