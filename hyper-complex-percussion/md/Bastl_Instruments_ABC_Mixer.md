# Bastl Instruments — ABC Mixer

- [Manual PDF](../../manuals/manual-abc-web.pdf)

---

[ABC Mixer Manual (PDF)](https://bastl-instruments.com/content/manuals/ABC_manual.pdf)

---

# Using the Bastl Instruments ABC Mixer for Hyper-Complex Percussion in Eurorack

As a Eurorack modular synthesizer musician seeking densely rhythmic & hyper-complex percussion, here’s how you can leverage the **Bastl ABC Mixer**—designed as a 6-channel audio/CV mixer—to achieve intricate polyrhythms, odd time signatures, and punchy, evolving sequences.

---

## Core Capabilities of the ABC Mixer
- **6 inputs (A–F), each with gain control** (0–1)
- **2 outputs:** `A+B+C` and `D+E+F` (can sum to one 6-channel mix if only using one output)
- **Switchable AC/DC coupling** (via solder jumpers on rear): supports both audio *and* CV signals
- **Normalization jumpers** for routing (A→D, B→E, C→F) — powerful for stereo splitting or dual-layer mixes

---

## Creative Percussive Use-Cases

### 1. **Layering Percussion for Dense Grooves**
- Patch 6 unique percussion voices (e.g., kick, snare, rim, hat, click, glitch) to the 6 inputs.
- Mix complementary voices (e.g., A: Kick, D: FM Kick; B: Snare, E: Clap) into the two output buses, allowing for thick, composite drum sounds.
- Use the normalization jumpers to stack or split voices for stereo imaging or polyrhythmic accents.

### 2. **Polyrhythmic Routing & Stereo Tricks**
- Use the dual outputs (`A+B+C` as left, `D+E+F` as right) and normalization to build polyrhythms—say, a 4/4 pattern in A+B+C and a 5/4 or 7/8 pattern in D+E+F. Use a switch or step-sequencer to modulate which voices are summed to which outputs for phasey, interlocked beats.
- With normalization, one trigger can send similar sounds to both buses, but you can mix them individually.

### 3. **Dynamic Muting & Accent Control**
- Use the gain knobs as manual performance tools: fade voices in for fills, punchy one-shots, or mutes to break up loops with surprising silences or sudden complexity.
- Rapid tweaking during live jams lets you accent polyrhythmic hits by temporarily maxing a noise burst or click.

### 4. **CV Mixing for Evolving Patterns**
- If you patch the module as a CV mixer (modifying for DC coupling):
  - Mix several stepped/random/Euclidean CV sources (gates, envelopes, logic signals) to create wild composite triggers or modulation curves that can be sent to percussion modules’ trigger/decay/timbre inputs.
  - Use a mixture of rhythmic gates in different time signatures (e.g., input A: 3-step rhythm, B: 4-step, C: 5-step), and sum into outputs to create CV "polyrhythm" clocks or probability-based triggers for percussion.

### 5. **FM/AM Audio Rhythmic Processing**
- Run audio-rate percussion sounds through some inputs and use the gain controls for distortion/saturation tricks.
- Alternate between audio mixing for dense textures and fast-slew envelope/CV mixing for clicky, punchy percussion.

---

## Tips for Unique, Punchy, Complex Percussion
- **Use AC-coupled mode for tight, poppy transients; switch to DC coupling for CV mangling.**
- **Patch in audio signals with transients that have differing lengths and positions to create accidental swing or groove.**
- **Mute and unmute channels in sync and off-sync with the master tempo for stutter and fill effects.**
- **Use the normalization jumpers to "mirror" polyrhythmic material across both outputs for stereo motion.**
- **Experiment with feedback loops by cross-patching outputs back through further processing before returning to an input.**
- **If your percussion voices have individual accent ins, route a mixed, complex CV or audio gate output to those for driven groove and punch.**

---

#### Further Exploration
- Try sending **post-mixer outputs to VCAs/effects** (e.g., ring mod, saturation, reverb) and use rhythmic gating to carve new grooves from the sum.  
- Combine the ABC Mixer with clock dividers, logic, Euclidean sequencers, and probability generators for ever-morphing patterns.
- Use feedback: take one of the outputs, process (distort, wavefold, filter), and patch back in to an input—carefully—for evolving percussive soundscapes.

---

**Full Manual:** [ABC Mixer Manual (PDF)](https://bastl-instruments.com/content/manuals/ABC_manual.pdf)  
**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**