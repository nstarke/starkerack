# Worng Electronics — Vector Space

- [Manual PDF](../../manuals/Vector Space Manual v1.00.pdf)

---

[Download the WORNG Electronics Vector Space Manual (PDF)](https://static1.squarespace.com/static/581c4e5c5016e1db504461d8/t/5e4da639efd4f5444d7de05e/1582163769798/VectorSpace_Manual.pdf)

---

# Using the WORNG Electronics Vector Space for Densely Rhythmic, Hyper-Complex Percussion in Eurorack

As a modular synthesist, the WORNG Vector Space is a uniquely powerful tool for sculpting polyrhythmic, polymetric, and deeply intertwined percussion and rhythm sequences. Here’s how you can unlock its dense rhythmic potential:

## 1. **Polyrhythmic & Complex Gate/Trigger Generation**

#### **Patch Concept: “Rhythm Splintering”**
- **What you’ll need:** Three clock, trigger, or gate sources each running at different rates or time divisions (e.g. 5, 7, 9).
- **How to patch:**
  1. Patch each clock/gate stream into the i, j, and k inputs of the Vector Space. Use a mix of clock generators, sequencer triggers, or LFOs with pulse outputs.
  2. Experiment with the input voltage switches (++/+-) to transform the polarity and offset of the incoming signals.
  3. Use the **Cube Outputs** as complex gate/trigger outputs: They will present logical AND/OR/XOR/NOT-style combinations of the inputs, but with phase relationships and analog blending—so not simply digital logic, but richer, more nuanced gate blends.
  4. The **Plane Outputs** offer even more intricate, rectified and summed combinations—perfect for non-standard triggers and “ghost” hits.

- **Application:** Patch these outputs into drum modules, percussive sound VCAs, end-of-chain effect gates, or envelope triggers. You’ll quickly create “impossible” time signatures and evolving polyrhythms.

---

## 2. **CV Modulation for Rhythmic Complexity**

#### **Patch Concept: “Fractal Envelopes”**
- Patch multiple asynchronous LFOs, random gates, or looping envelopes into the Vector Space inputs.
- Send several outputs (particularly Planes and Spheres) to modulate parameters like decay, pitch, filter cutoff, or effect amounts in your percussion voices.
- This layering multiplies micro-variation, adding “human” shuffle, groove, and constantly morphing accents to your percussion.

---

## 3. **Self-Patching Feedback Rhythms**

#### **Patch Concept: “Recursive Drumming”**
- Patch selected outputs from the Vector Space back into clock divider/multiplier CV inputs, or to modulate LFO rates that re-enter the Vector Space.
- This creates feedback/chaos loops, where the timing structures feed on themselves for evolving, unpredictable rhythms.

---

## 4. **CV-Controlled Probability & Swing**

- Use the **Sphere** output (with its summed, rectified, and net-distance approach) to control probability/skipping modules or VCAs.
- The complex, ambiguous blend of your three inputs will create “weighted” gates and CVs, great for probability-based rhythm or “random accents.”

---

## 5. **Voice/Effector Use: Making Percussion Unique, Punchy, Percussive**

- *If* you’re running audio through Vector Space, try feeding short, percussive tones (e.g. sine pings, metallic FM pulses, glitches) into i/j/k. The output blends will create metallic clangs, distorted syncs, AM/FM hybrids, and mysterious timbres otherwise hard to achieve.
- The **Cube** outputs yield phase-varied combinations (think of syncopated stack-ups), while the **Plane** outputs add upper harmonics for aggressive, punchy attack. 
- Use the modulation outputs (especially those with LEDs flickering rapidly) to amplitude or filter-modulate your percussion audio for extra punch and complexity.
- Don’t forget to audition via an envelope follower and external VCA to emphasize dynamic punchiness.

---

## 6. **Concrete Example Patch for Ultrarhythmic Percussion**

1. **Inputs:**
   - i: Euclidean gate sequence (e.g. 5 steps in 16).
   - j: LFO square, free-running at non-multiplicative rate.
   - k: Chaotic stepped random voltage (clocked independently).

2. **Cube Outs:**
   - Patch four Cube outputs to trigger kick, snare, hat, and percussion sound sources. Each will rumble with offset timing and shifting polyrhythm.

3. **Plane Outs:**
   - Use Plane outs as accent triggers or to modulate decay/release amounts on your drums, creating shifting ghost notes and fills.

4. **Sphere/UnSphere:**
   - Use these as modulation for probability/swing (via a CV-able Bernoulli gate or swing generator), so that swing and randomness evolves with the overall “vector” motion in rhythm space.

---

## Tips for Extreme Percussion with Vector Space

- Use offset switches as live manipulation tools while recording or performing.
- Patch some outputs to amplitude or timbre CV of percussion voices for wild, organic, living digital percussion.
- Repatch frequently—small inputs changes can lead to major rhythmic breakthroughs.

---

The WORNG Vector Space is not simply a utility but a central nervous system for generative and polyrhythmic percussion—the more unstable, offset, and cross-modulated your inputs, the more singular your rhythmic output!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)