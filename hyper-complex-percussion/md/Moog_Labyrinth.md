# Moog — Labyrinth

- [Manual PDF](../../manuals/Labyrinth Manual.pdf)

---

[**Moog Labyrinth User Manual (PDF)**](https://www.moogmusic.com/files/manuals/Labyrinth_Manual_Web.pdf)

---

# Using Moog Labyrinth for Hyper-Complex, Polyrhythmic Percussion

## **1. Why Labyrinth?**

Moog’s **Labyrinth** is an experimental semi-modular voice and generative sequencer designed for creative, evolving, and intricate pattern creation. With dual generative sequencers, extensive modulation, parallel/serial signal paths, and a uniquely punchy architecture (including VC wavefolder, VCF, and two analog oscillators), it's particularly suited for dense, rhythmically complex, percussive music.

---

## **2. Generating Dense Rhythmic Complexity**

### **a. Dual Generative Sequencers: Polyrhythms & Poly-metric Patterns**

- **Independence:** SEQ1 and SEQ2 each have 8 steps, independent length, and can be clocked separately (via external clocks to *CLOCK 1* and *CLOCK 2*).
- **Length & Shift:** Set SEQ1 and SEQ2 to different lengths (e.g., 5 and 7 steps) to create polyrhythms and complex time signatures.
- **Chains & Offsets:** *CHAIN SEQ* links both sequencers for up to 16 steps. In polyrhythm mode, use *write head offsets* (see button combos) to further desynchronize sequences.
- **External Clocks:** Patch separate clock sources—e.g., from a Euclidean rhythm or random burst generator—to push the sequencers into interlocking, unusual grooves.

### **b. Corrupt—Evolving and Disrupting Patterns**

- Use the **CORRUPT** knob to create morphing patterns: set “just above 12 o’clock” to evolve both voltage and rhythm, adding unpredictability and complexity.
- Save stable states with **BUFFER**; let sequences mutate, then recall for dramatic “glitch” or tension-release effects.

---

## **3. Percussive Sound Design Techniques**

### **a. Parallel Voice Engine—VCW + VCF Signal Paths**

- **Wavefolder (VCW):** Push VCW FOLD and experiment with asymmetry (VCW BIAS) for snappy clicks, metallic pings, or noisy analog transients.
    - **Envelope Fast Decay:** Route EG1 (fast decay) to VCW FOLD for punchy percussive attack.
    - **Sequencer Modulation:** Route SEQ1 CV to VCW FOLD for step-by-step brightness/drive modulation, making each hit distinct.
- **VCF Path:** Push resonance, and automate *CUTOFF* with SEQ2 or EG1 for dramatic, vowel-like filter percussion or “snare” sweeps.

### **b. Mixer Drive and Crossfading**

- Overdrive the **MIXER** for saturation above 12 o’clock—adding punch and analog sizzle to every drum hit.
- Use **BLEND** or automate it (via panel, envelope, or CV) to dynamically crossfade between parallel and serial routing, or switch timbres in real-time for fills and unique accents.

### **c. Ring Modulation & Noise**

- Mix in **RINGMOD** for metallic clangs or bell percussion.
- Carefully shape **NOISE** and use the tone control for hi-hats, shakers, or pronounced attack elements.
- Patch trigger out into **VCO 1V/OCT** for metallic hi-hats, as suggested in the “Spiral Enigma” preset.

---

## **4. Using the Utility Mixer (U MIX) and Patchbay for Further Complexity**

- Submix oscillators and noise, or merge Labyrinth outputs with external triggers/CVs through the patchbay.
- Use *BIT FLIP CV* inputs to rhythmically turn individual sequencer steps on/off using external modulation—great for generative stutter or burst effects.
- Route EG2 or external envelopes to VCA CV for “choked” drum hits, dynamic accents, or staccato bursts.

---

## **5. Advanced Applications & Eurorack Integration**

- **Clock Inputs:** Run SEQ1 and SEQ2 from different (or related but phase-shifted) clocks in your rack for advanced polymeters. Try Euclidean, triplet, or random clocks.
- **MIDI Sync:** Use MIDI clock or external drum sequencers to synchronize, then push or pull steps for off-kilter grooves.
- **CV Outputs:** Use SEQ1/SEQ2 CV out as pitch, modulation, or even cross-modulate percussion parameters in external modules for multi-layered drum machines.
- **Envelope Outs:** Use EG1 or EG2 outputs to externally trigger other percussive voices or effects in your system—locking multiple modules to Labyrinth’s generative patterns.

---

## **6. Patch Examples for Unique, Punchy, Percussive Use**

### **Example 1: Polyrhythmic Metallic Kit**
- SEQ1 length: 5. SEQ2 length: 7. Clocks: independent.
- MIXER: Overdrive both VCO and Ringmod.
- VCW FOLD modulated by EG1 (short decay, high modulation).
- BLEND automated by another fast LFO for rapidly shifting voicings.

### **Example 2: Mutating Glitch Drums**
- CORRUPT full, SEQ2 triggers modulate Envelope Decay (EG2 via U MIX).
- Rout noisy signal to VCF→VCW order; modulate BLEND
- Patch BIT FLIP inputs to a burst generator for “random fill” glitch moments.

---

## **7. Tips for Extra Percussive Impact**

- Patch fast, snappy external envelopes or LFOs to FOLD, VCF, VCAs.
- Experiment with high resonance and filter morphing for liquid-like, vocal drum timbres.
- Use the quantizer to lock sequences to non-standard scales for melodic drums.
- Modulate VCO pitch with per-step voltages for tonal drums and “melodic percussion.”

---

**Reference:**
[Moog Labyrinth Official Manual PDF](https://www.moogmusic.com/files/manuals/Labyrinth_Manual_Web.pdf)

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)