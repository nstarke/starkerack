# Bubblesound — HexVCA

- [Manual PDF](../../manuals/bubblesound.pdf)

---

[**HEXvca Manual (Bubblesound)**](https://www.bubblesound-instruments.com)

---

## Using HEXvca for Dense, Complex Rhythmic & Percussive Patches

The **Bubblesound HEXvca** is a six-channel voltage-controlled amplifier (VCA) with flexible normalization, mix outputs, linear/exponential switching, and DC-coupled inputs for both audio and CV. While it is not a voice or effect on its own, it is an **essential utility for routing, sculpting, and animating both audio and control voltages**—especially potent in dense, polyrhythmic, and complex percussion setups. Here’s how to exploit its strengths:

### 1. Modular Polyrhythmic Percussion Routing

#### a. **Assigning VCAs to Percussion Voices**
- Route six different percussive sound sources (drums, metallic hits, noise bursts, modular drum synths) into the six HEXvca inputs.
- Patch separate or shared envelopes/LFOs/gate bursts to their respective CV inputs.
- Use the jumpers on the back to normalize CVs, allowing one gate or envelope to trigger multiple VCAs for tightly related patterns or "flams."

#### b. **Complex Accent Patterns (using the Exp/Linear Switches)**
- Assign different VCA response curves: Use exponential for snappier transients (kicks/snares), linear for smoother hits (hats, shakers).
- Modulate the CV with rhythmic LFOs, stepped random voltages, or Euclidean/chaotic gates for organic, “swung” micro-timing.

#### c. **Creating Polyrhythms & Unusual Rhythmic Structures**
- Feed in multiple complex rhythmic control voltages (such as from a trigger sequencer or random CV generator) into different VCAs’ CV inputs.
- Use cross-normalization jumpers so a single polyrhythmic CV can gate multiple percussive voices at offset rhythms—ideal for 5-against-7 time, etc.

---

### 2. Using the Built-in Mixer for Rhythmic Layering

- Utilize the **1-3, 4-6, and 1-6 mix outputs** to blend clusters of percussive voices into “macro” percussion channels.
- Apply different CV patterns to overlapping groups (for example, channels 1, 3, 5 running in 7/8; 2, 4, 6 in 5/4) and sum to the main mix for composite polyrhythms.

---

### 3. Dynamic, Punchy Percussive Manipulation

#### a. **Rhythmic Gating and Chopping**
- Use short, sharp envelopes or triggers to “chop” sounds for hyper-articulated rhythms or glitch percussion.
- Try 1V/oct or sequencer gates into the CV inputs for “melodic” gating or accent randomization.

#### b. **Crossfade Percussive Textures**
- Patch two or three sources (e.g., metallic digital drum, saturated analog hit, noise burst) into adjacent VCAs, using their VCAs’ CVs to rhythmically blend and morph textures.

---

### 4. Make it Unique, Punchy, and Percussive

- Use very short, high-voltage envelopes for instant “thwack”; modulate amplitude dynamically with random or cyclical CV for an organic, always-shifting groove.
- Patch CV into both the input and CV of a VCA for amplitude-modulated AM/ringmod-style percussive clangs (DC-coupled design supports audio-rate CV for wild effects).
- Try signal path “feedback” by routing the mixer output back into an audio input (careful with gain staging) for smashed, dirty parallel compression effects.

---

### 5. Pro-level Tips

- The **SSM2164 VVCA chips** deliver super low noise and headroom—so don’t be afraid to run hot transient signals for crisp punch.
- The module is only 7HP: Use multiple HEXvcas in a single skiff for high-density rhythmic matrixing.

---

### Summary

The HEXvca is more than a utility; in a dense rhythmic patch, it becomes a core tool for sculpting, gating, accenting, layering, and dynamically remixing percussion. It’s at its most powerful when paired with sequencer gates, complex clocks, random CV, and multichannel envelopes/LFOs. Use the normalization and built-in mixer to wring maximal complexity and “liveness” from your patch.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)