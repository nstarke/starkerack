# Doepfer — A-121-3

- [Manual PDF](../../manuals/A-121-3 12dB Multimode Filter (slim version).pdf)

---

[**Doepfer A-121-3 12dB Multimode Filter Manual** (HTML; no official PDF)](https://doepfer.de/a1213.htm)

---

# Using the A-121-3 Multimode Filter for Dense, Rhythmic, and Complex Percussion in Eurorack

The **Doepfer A-121-3 12dB Multimode Filter** is a highly compact and versatile multimode filter. You can use this module not only as an effect, but also as a unique drum/percussion voice by exploiting its self-oscillation abilities and its wide, voltage-controlled cut-off and resonance.

## **Key Features for Percussive & Rhythmic Patch Ideas**

- **-12 dB/octave Multimode (LP, HP, BP, Notch) Simultaneous Outputs**
- **Voltage-Controlled Cut-off and Resonance (Q)**
- **Self-oscillates for sine percussion**
- **Manual input level, filter Freq, resonance controls**
- **Compact 4HP**

---

## **Techniques for Rhythmic, Polyrhythmic, and Complex Percussion**

### **1. Percussive Filtering for Dense Rhythms**

- **Patch Variation:**  
  Run complex drum or noise sources (digital or analog) into the audio IN of the A-121-3.  
  Use fast, percussive envelopes (from clocked modulation sources) into CV1 and/or CV2 (with attenuator) to rhythmically modulate cut-off.
  - The two FM inputs allow you to layer envelopes (e.g., hi-hats with sharp, quick mod; toms with slower, variable CVs)
  - Stereoize drums by using LP for one side, HP for another, morphing filtered signals using panning.

### **2. Polyrhythmic Resonance Modulation**

- **Modulate Resonance (Q):**
  - Use triggers from odd divisions (e.g., 3/16, 7/16) to periodically open up resonance just on certain drum accents. The CQ input is not attenuated, so use external attenuators or bipolar offsets for subtle changes.
  - Pair this with sequencers or function generators set to different clock divisions for immediate polyrhythmic results.

### **3. Self-Oscillation for Sine Percussion**

- When you turn up the Q to self-oscillation, the filter produces a stable sine.
  - **Kick Drums:** Use a trigger or short envelope on the cut-off CV, and use Level to saturate/clipping for punch. Extra drive (input level past 5) makes for snappy, clicky drums.
  - **Toms/Bells:** Patch a sequencer or random stepped CV for cut-off, pair with short/long envelopes for pitch decay, and hit the filter with polyrhythmic gate sequences. Resonance modulation acts like FM, yielding zappy, metallic percussive hits.

### **4. Notch/Bandpass for Unique Percussive Tones**

- Layer several filter outputs (LP, BP, HP, Notch) through VCAs, each triggered by a different rhythm—create complex, dynamic timbres.
- Notch output gives hollow, phasing "blips" great for glitch percussion or layered with hats/claps.

### **5. Input Overdrive for Punch**

- Increase the Level knob past 5 for intentional distortion/clipping, especially useful for making anemic drum sources hit harder.
- Create variation by CVing the input Level via external VCA, under control of burst/gate patterns for rhythmic distortion.

### **6. Clock/CV Modulations for Hybrid Drum Machines**

- Use LFOs, stepped randoms (Sample&Hold), or fast, euclidean rhythms as modulation sources for CV1/CV2.
- Combine with analog logic processors: AND, OR, XOR complex trigger sources into bursty cut-off modulation.

### **Patching Example: "Polyrhythmic Filter Percussion"**

```markdown
Drum Source (or White Noise) → A-121-3 AUDIO IN

Polyrhythmic Envelope 1 (3/16 clock) → CV1 (cut-off FM)
Polyrhythmic Envelope 2 (5/16 clock, slower) → CV2 (attenuate w/ FCV2 for depth)
Euclidean/Random Gates → CQ (external attenuator or offset module for subtlety)

Mix and layer LP, BP, and Notch Outs → Multiple VCAs → Stereo Mixer
Each out is VCA’d with another rhythm — instant cross-rhythmic percussion layer

Crank Q to max > Self-oscillation: Patch triggers (1, 2, 3, 5 beat clocks) to cut-off CV/Level for tuned sine drums
```

### **Tips for Punchiness and Uniqueness**

- Use audio-rate modulation into CV inputs for metallic, "FM percussion" effects.
- Stack filter outputs with slight delay or phase offset for “slapback" snare/hats.
- Routinely overdrive input and modulate resonance for transient smacks and spectral sweeps that cut through dense mixes.

---

## **Summary Table**

| Output Types | Use for             | Rhythmic Ideas                                  |
|--------------|--------------------|-------------------------------------------------|
| LP           | Kicks, toms, bass  | Envelope pitch + decay, clocked Q sweep         |
| HP           | Snares, hats, rims | Fast LFO/Env on cut-off, CV w/ burst patterns   |
| BP           | Wood/metal clacks  | Quick decay, polyrhythmic mod, layering         |
| Notch        | Zappy Fx, claps    | Euclidean Q mod, crossfade w/ hats or snare mix |

---

## **Manual Link**

[Doepfer A-121-3 Manual (HTML)](https://doepfer.de/a1213.htm)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)