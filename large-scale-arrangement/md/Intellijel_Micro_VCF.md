# Intellijel — Micro VCF

- [Manual PDF](../../manuals/uvcf_manual_2021.08.15.pdf)

---

[Intellijel µVCF Manual PDF](https://intellijel.com/downloads/manuals/uVCF/uVCF_manual_2021.pdf)

---

# Using the Intellijel µVCF in Full-Length Eurorack Songs

Creating a full-length song in a modular Eurorack system often moves beyond patching impressive loops or riffs—you need structure, variation, transitions, and evolving timbres. The Intellijel µVCF (micro Voltage Controlled Filter) is a compact, pristine-sounding analog state variable filter that can become an essential part of this process. Below are practical, creative strategies for using the µVCF in full song creation, focusing on its strengths and how it can interact with the rest of your system to help you move from loops to finished pieces.

---
## 1. Dynamic Timbre and Scene Changes

**Automate Filter Cutoff for Progression**

- Use the µVCF’s FREQ input and modulate with slow LFOs, sequencers, or envelopes to create evolving timbral shifts through different song sections (intro, verse, chorus, breakdown).
- Example: Patch an LFO to FM2 (with the bipolar attenuator for movement) and an envelope or step sequencer to FM1 (tracks 1V/oct for melodic/filter sweeps) to make drastic changes between sections.
- Assign your main bass or melodic voice to the µVCF, and automate cutoff and/or resonance for drops, breakdowns, and builds.

---

## 2. Morphing Between Texture Types

**Simultaneous Outputs for Transitions**

- Take advantage of the µVCF’s simultaneous outputs (lowpass, bandpass, highpass). Route them to different VCAs or effects chains.
- Fade between outputs using a crossfader, manual switches, or CV-controlled VCA matrix. This lets you shift a part’s character—e.g., intro in bandpass, drop in full lowpass.
- Example: Use BPF in a reverb-heavy aux send for “distant” moments, then switch the main mix to LPF for a “close-up” impact.

---

## 3. Percussion and Resonant Elements

**Self-Oscillation for Percussive Tones**

- With Q (resonance) turned up and no input, the µVCF self-oscillates and can act as a sine VCO. Sequence the filter’s pitch via FM1 (1V/oct).
- Use this for tuned percussion, sub-bass drops, or melodic lines that blur the boundary between percussion and synth.
- Routinely change filter resonance or modulate with envelopes to morph the tonal character, giving you new sounds for different song sections.

---

## 4. Movement and Rhythmic Interest

**Filter FM for Animated Textures**

- Send audio-rate modulation (from a VCO or a burst generator) into FM2 for wild, animated textures that aren’t easily replicated by more static patches.
- Use envelopes or sequencer-driven gates to open up the filter only at particular moments (e.g., last beat of every 8th bar), creating anticipation and release.

---

## 5. Filter as a Song Structuring Tool

- Patch drums, drones, or entire submixes through the µVCF to “mute” or “unmute” frequency bands. Great for building tension (progressively closing the LPF in a breakdown) or sudden impact (opening aggressively at a drop).
- Use performance controls (manual tweaks, pressure sensors, external MIDI-to-CV via a controller) to play the filter live.

---

## 6. Using Multiple Filter Outputs for Stereo Imaging or Layering

- Send LPF and HPF outputs to different sides of a stereo field, or EQ differently to create movement without losing low end or adding harshness.
- Layer processed (FXed) versions alongside dry outputs for depth and space in mix.

---

## Workflow Tips: Beyond the Loop

- **Scenes & Mutations:** Create multiple scenes in your patch—e.g., Scene A uses bandpass with moderate Q and slow LFO, Scene B uses LPF fully open with audio-rate FM, Scene C introduces filtered noise for breakdowns.
- **Hands-On Transitions:** Use manual filter control on the µVCF for performance “macro” movements—big sweep to mark song transitions, or rapid Q increases to signal breakdowns.

---

# Example Eurorack Song Structure Using µVCF

1. **Intro:** Filtered noise or pads through HPF/BPF, slowly opening FREQ.
2. **Verse:** Sync bass through LPF, automate filter for evolving warmth.
3. **Chorus:** Open LPF, increase resonance; add FM for brighter, animated texture.
4. **Breakdown:** Self-oscillate, sequence filter pitch for melodic sine tones.
5. **Build:** LFO sweeps FREQ, resonant peaks become more pronounced.
6. **Drop:** All outputs open, full mix, FM at audio rates for energy.
7. **Outro:** Slowly close FREQ, fade to noise through HPF.

---

## Combination Ideas With Other Modules

- Pair with a **sequencer** for stepped filter movements that follow musical events.
- Patch outputs into a **reverb/delay** or granular FX for more spacious transitions.
- Use with a **CV-controlled switch or matrix** for scene changes—swap which voice is being filtered live.
- Combine multiple µVCFs for complex parallel processing (bass/lead/FX individual filtering for song arrangement).

---

## Final Thoughts

The µVCF isn’t just a utility—it’s a flexible tone-shaper, performance tool, and composition engine. Use its precision and routing flexibility to create musical structures, dramatic transitions, and evolving textures that turn your modular jams into cohesive, expressive songs! Experiment with multi-output patching and dynamic control to keep listeners engaged from intro to outro.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)