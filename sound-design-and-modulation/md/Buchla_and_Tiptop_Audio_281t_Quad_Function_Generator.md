# Buchla and Tiptop Audio — 281t Quad Function Generator

- [Manual PDF](../../manuals/Buchla_&_Tiptop_Audio_281t.pdf)

---

[**Quad Function Generator - Model 281t Manual PDF**](https://tiptopaudio.com/manuals/281t.pdf)

---

# Creative Patching with the 281t Quad Function Generator

The Buchla/Tiptop Audio 281t is an extremely flexible envelope and function generator for Eurorack that can be used in classic and experimental ways. Below are some techniques and ideas for modulating the module to produce **distorted perc** sounds, **aggressive basslines** (a la dubstep/drum & bass), and **haunted pads**.

---

## 1. **Distorted Percussive Sounds**

**Key principles:**  
- Ultra-fast attack/decay times for “snappy” envelopes  
- Self-cycling for repeating hits  
- Feedback, FM, and wavefolding for distortion

### Example Patches

- **Drum Synth:**
  1. Set a channel to **Cyclic** mode with the attack/decay times set to very fast (~0.001-0.1s).
  2. Patch output to a VCA or as an envelope for a drum voice.  
  3. Use the transient pulse output as a trigger for other modules (e.g. noise burst, filter ping).
  4. Self-patch the pulse output to its own trigger input for feedback-driven clicking/glitchy hits.

- **Distortion via Feedback:**
  - Patch the channel’s output to a distortion or wavefolder module, or even back into its own CV input for self-modulating, unstable envelopes.

- **Layered Perc:**
  - Use two generators in quadrature to trigger two different drum sounds slightly out of phase for a “flam” effect.

---

## 2. **Crazy Basslines (Dubstep, DnB)**

**Key principles:**  
- Exponential envelope shapes for filter sweeps  
- Complex envelope chaining and cross-modulation  
- Rhythmically synced cycling

### Example Patches

- **Woozy Bass “Wobble”:**
  1. Use one function generator in **Cyclic** mode with a mid-to-slow decay (~0.2-1s).
  2. Use the envelope output to modulate a VCF cutoff (or a wavefolder’s index for even more grit).
  3. Use the **Attack/Decay CV inputs** for envelope-shape modulation, feeding them step sequencer or LFO CV for evolving rhythmic movement.

- **Envelope Self-Sync:**
  - Use the **Cycle jack** to rhythmically sync the envelope cycling to your clock, creating gated, stepped wobble patterns.
  - Patch “quadrature” mode for stereo, phase-shifted filter modulations.

- **Aggressive FM Basses:**
  - Use two envelopes in quadrature to modulate both pitch and filter cutoff of a bass oscillator separately, or cross-modulate one envelope with the output of another.

---

## 3. **Haunting Atmospheres and Pads**

**Key principles:**  
- Long, evolving envelopes  
- Chain/cascade multiple channels for multi-stage shapes  
- Subtle cross-modulation for complexity

### Example Patches

- **Layered CV Pads:**
  1. Set all four channels to **Sustained** mode, with long attack/decay times (~2-10s).
  2. Sum two or more envelope outputs to control VCA amplitude for a slowly undulating pad.
  3. Use another channel to modulate filter resonance or a reverb send for ethereal drifting.

- **Ghostly Cross-Modulation:**
  - Patch A’s output to B’s attack CV, and B’s output to A’s decay CV for undulating, unpredictable envelope shapes.
  - Use an LFO or slow sequence to “ride” the cycle time or decay, evolving the atmosphere.

- **Quadrature Texture:**
  - With generators A & B (and/or C & D) in quadrature, pan their outputs left/right for stereo, phase-shifted evolving drones.

---

## **General Tips**

- **Pulse Output for Sequencing:**  
  Use the pulse output at the end of the decay stage to trigger new events or envelope stages for complex, self-generating patches.

- **CV in for Unusual Envelopes:**  
  Inject noise, slow LFOs, or even audio-rate signals into the CV inputs for glitchy, stepped, or audio-reactive modulation curves.

- **Extreme Settings:**  
  Use the full range of the .001s–10s attack/decay to morph between microclicks and slow surges.

---

## **Patch Example: Distorted Perc Hit Generator**

```
281t Ch1 OUT → Wavefolder IN
Wavefolder OUT → VCA → Mixer
281t Ch1 PULSE OUT → 281t Ch1 TRIG IN (self-cycling feedback)
281t Ch1 DECAY CV IN ← Random CV
Decay knob: 9 o’clock, Attack: minimum
Cycle mode: ON
```

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)