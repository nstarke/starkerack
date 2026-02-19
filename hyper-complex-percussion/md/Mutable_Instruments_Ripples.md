# Mutable Instruments — Ripples

- [Manual PDF](../../manuals/Manual - Mutable Instruments Documentation.pdf)

---

[Mutable Instruments Ripples 2020 Manual (PDF)](https://mutable-instruments.net/modules/ripples/manual.pdf)

---

# Generating Densely Rhythmic, Hyper Complex Percussion with Mutable Instruments Ripples

Mutable Instruments Ripples is primarily a multimode filter, but with creative patching, it can become a key tool in designing punchy, complex, and percussive sounds within intricate rhythmic contexts, such as polyrhythms and odd time signatures. Here’s how you can exploit Ripples to yield unique, dynamic, and rhythmically intense results.

---

## 1. **Ripples as a Percussive Voice**

Although Ripples is a filter, it can self-oscillate when resonance is increased (see **Control C**). This transforms it into a sinewave oscillator capable of producing clear, pitched percussive sounds, especially kicks, toms, and congas.

### **Self-Oscillating Kick Drum**
- **Patch:** No audio input; RES (C) at 75–100%
- **Envelope:** Patch a fast, snappy envelope (from a sequencer or modulation source) to the V/OCT input for pitch-modulated "kick" transients.
- **Cutoff Sweep:** Use the envelope to also modulate CUTOFF (A) for added thump.
- **VC LP Gain:** Modulate the LEVEL CV input with another envelope for amplitude shaping. The built-in VCA means a second VCA is not needed.

### **Snare/Clap Timbres**
- Mix in noise from another source to one of the audio inputs, alongside self-oscillation, and process both through Ripples.
- Use the BP output for snappier or harsher attacks.

---

## 2. **Filter Percussion with Audio Inputs**

Ripples excels at taking complex audio signals (like layered noise, FM, or oscillator clusters) and sculpting them into percussive hits.

- **Complex Input:** Patch dense noise bursts, short oscillator blips, or prepared percussive loops.
- **Rhythmic Modulation:** Use fast, staggered CVs from a modulation sequencer or clocked random source to the cutoff, resonance, and VCA input. For polyrhythmic complexity, these CVs should be derived from rhythm sources in different time signatures or clock divisions (e.g., 4:3, 5:4).
- **Overdrive:** Push Input 1 level (D) high for soft-clipping, instilling extra punch and grit.

---

## 3. **Dynamic Filtering for Rhythmic Variation**

Ripples' smooth and musical resonance, voltage-controllable cutoff, and switchable slopes make it ideal for evolving, dynamic filtering:

- **Patterned Modulation:** Send rhythmic stepped CVs (e.g., from a trigger sequencer’s accent, or from a clocked random generator) to the cutoff CV and resonance CV.
    - Try Euclidean sequencers, polyrhythmic LFOs, or probability-based trigger generators.
- **Filter Slope Switching:** Manually or via coordinated hand movement, flip the slope switch between phrases for dramatic contrast (e.g., alternate 2-pole/4-pole responses every X bars in a complex cycle).
- **Stereo/Layered Percussion:** Mult the input signal, process with parallel Ripples channels in different modes (HP, BP, LP), sequence their cutoffs with different length patterns (e.g., 7-step for HP, 5-step for BP), and then recombine for stereo or multi-layered percussion voices.

---

## 4. **Using All Three Outputs Creatively**

- **Parallel Processing:** Use HP for clicky, snappy tops; BP for snare-like midrange; LP for deep body. Sequence, mix, and layer all three outputs to sculpt dense, multi-timbral percussion.
- **VC LP Output as Accent:** Exploit the VCA control for the LP out to accent hits rhythmically—send an accent envelope from your complex clock/gate source here.
- **Frequency Modulation:** Use E (attenuverter) to inject bipolar CV from an LFO or sequencer for time-warped filter cutoff motion, enhancing groove complexity.

---

## 5. **Advanced Tips for Maximum Rhythmic Density**

- **Nested Polyrhythms:** Program your mod sources (LFOs, envelopes, sequencers, random CV) to different clock divisions or non-aligned lengths; route these to cutoff, res, and LP gain for intersecting rhythms.
- **Gated Sweep Percussion:** Sweep the filter with a random CV, but only activate it on certain triggers/gates for micro-accented textures.
- **Feedback/Resonance "Rattles":** Modulate the resonance at audio rates or with a quick LFO for inharmonic, metallic percussion.

---

## **Summary Patch Example: Polyrhythmic Filter Percussion**

1. **Patch:** Send an audio mix of noise and short oscillator pings to INPUT 1.
2. Use three different envelope generators/stepped random sources at unique clock divisions:
   - EG1 (7-step) → CUTOFF CV
   - EG2 (5-step) → LEVEL CV (VCA for LP out)
   - EG3 (4-step) → RESO CV
3. Use the LP out as the main percussion body, mixing in BP and HP as needed for added snap or crackle.

---

**Unleash hyper-rhythmic percussive power by pairing Ripples with creative, clocked mod sources!**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)