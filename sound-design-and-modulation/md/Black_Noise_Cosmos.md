# Black Noise — Cosmos

- [Manual PDF](../../manuals/BLACK-NOISE_COSMOS_User-Manual_V1.pdf)

---

[**Download the COSMOS Manual PDF**](sandbox:/mnt/data/COSMOS_User_Manual_V1.0.pdf)

---

# COSMOS: Eurorack Modulation & Sound Design Strategies

Based on the COSMOS manual, here are focused approaches to coaxing **distorted percussion**, **crazy basslines** for DnB/dubstep, and **haunting pads**. The COSMOS’ deep analog logic, signal folding, rectification, and flexible CV routing make it a wild processor for modular explorers.

---

## 1. **Distorted Percussive Sounds**

### a) Clamping VCA (p. 21, "Clamping VCA")
- **Patch:** Send a short envelope or percussive noise burst to the X input. Patch a fast, snappy envelope (from Maths, Function, or similar) to the Y input. Use the **inv. TZ CLIP** out for your sound.
- **Modulate:** Use the envelope's decay CV to create transient shaping. Increase the envelope depth for harder, squashed distortion.
- **Enhance:** Add an offset before the Y input for more extreme clamping/distortion, making the percussive attack even sharper. Try the touch pads to introduce manual "hits".  
- **Character:** This introduces analog distortion that enhances percussive transients—great for techno/dubstep snares, glitch kicks, or metallic rimshots.

### b) Full-Wave Rectifier (p. 18, "Full-Wave rectifier")
- **Patch:** Send your drum audio into X, the corresponding inv out to Y. Take the MAX output for a fully-rectified, harmonic-rich drum sound.
- **Modulate:** Use a fast LFO or another envelope on the offset CV to dynamically "bend" the harmonics for each drum trigger.

### c) Complex Ring Modulation (p. 23, "Complex ring modulation")
- **Patch:** Use two VCOs or drum signals, routed through attenuators/offsets into the X and Y inputs.  
- **Modulate:** Use envelopes or stepped random CV into the offset/attenuator modules for shifting metallic clang and broken digital-sounding percussion.

---

## 2. **Crazy Basslines (Dubstep/Drum & Bass)**

### a) TZ Clipper - XOR Logic (p. 14)
- **Patch:** Send a triangle or sawtooth from a VCO into X, a sub-octave square or LFO or another VCO into Y.
- **Modulate:** Modulate the frequency and offset of the Y input for constant movement. Self-patch the COSMOS outputs to other parameters for complex chaos.
- **Output:** Use the **TZ CLIPPER** or **XOR** out for gnarly, squelchy, phase-inverting, FSU-style tones typical of modern DnB/Dubstep.

### b) Harmonic Wave Shaper (p. 28)
- **Patch:** VCO into X. Send **TZ clipper gate** out through a fast slew or LPG, then negative offset to Y. Take **TZ CLIPPER** out.
- **Modulate:** Use sequencer, LFO, or envelope into slew time and offset CV for "punching," folding, and tearing basslines.

### c) Self-Oscillation & Feedback (p. 24)
- **Patch:** XNOR gate out > X input. Add slew or filter in the feedback for pitch control.
- **Modulate:** Use envelopes, random sources, or touch plates to add fiery, spiky, unpredictable movement to your basses.

---

## 3. **Haunting Atmospheric Pads**

### a) Envelope Combiner (p. 33)
- **Patch:** Layer two independent slow envelopes into X and Y. Take the **MAX** or **MIN** output for a morphing, organic pad shape.
- **Modulate:** Use slow LFOs to vary envelope parameters over time. Send additional LFOs or envelopes to input offsets for swelling movement.

### b) Window Comparator (p. 20)
- **Patch:** Patch a gently moving LFO or drone oscillator through an offset generator into X; the inv-X out, also through an offset, into Y. Take the OR gate out for a gated pad signal.
- **Modulate:** Slowly modulate the offsets (window center/width) for evolving, ghostly gating and harmonic shifts.

### c) Full-Wave Rectifier + Envelope Follower** (pp. 18, 34)
- **Patch:** Layer atmospheric samples or field recordings into X, inv out to Y. MAX output through a fast slew/LPG for an evolving, cloud-like control voltage or re-shaped drone.
- **Modulate:** Use the CV outs to modulate filters, reverbs, or other ambient processors.

### d) Touch Plates for Expressive Modulation
- Keep one or both inputs unpatched and use touch plates to bring in subtle or dramatic voltages. Great for slowly morphing pads with hands-on control.

---

## General Modulation Tips

- **Self-Patching:** Experiment with COSMOS’ own outputs modulating its own inputs for complex, self-organizing textures.
- **Logic Gates for Rhythms:** Use trigger/gate outs and their NOT/falling-edge versions to set up shifting, polyrhythmic modulations across your voices and FX.
- **CV-Controlled Offsets:** Always exploit GOMA or similar for live CV-driven offsetting, making every effect dynamic.

---

#### Experiment! The COSMOS is an analog computer-in-miniature—patching is open-ended, unpredictable and often yields surprising musical gold.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)