# Qu-Bit — Synapse

- [Manual PDF](../../manuals/Synapse.pdf)

---

[Qu-Bit Synapse Manual (PDF)](https://qu-bit-electronix.com/manuals/Synapse_Manual.pdf)

---

# Using the Qu-Bit Synapse for Unique and Extreme Sound Design

**Qu-Bit Synapse** is an extremely powerful crossfading, switching, and mixing utility that can be turned into a creative sound processor for intense modulation, mangled audio, wild basslines, glitched percussion, and evolving pads. Here’s how you can use it to achieve the types of sounds you described, referencing the features, functions, and methods as outlined in the manual.

---

## 1. Distorted Percussive Sounds

### **Key Techniques**
- **Crossfade Audio and CV**: Patch fast envelopes or stepped random voltages into crossfade CVs for sharp, dynamic percussive movements between extreme signals or between dry/wet distorted signals.
- **Internal Modulation/LFOs**: Use Synapse’s internal triangle LFOs for additional rhythmic modulation.
- **Scatter Function**: Rapidly shuffle output routing for glitchy drum fills.
- **Sum Outputs & Click-less Switching**: Layer or slam multiple signals together.

### **Patch Idea: Machine Gun Snares/Glitch Drums**
1. **Inputs**: Route snare and hi-hat audio to A/B inputs of one or more channels.
2. **Crossfade CV**: Mult a fast-decay envelope, clocked random, or stepped LFO as CV to rapidly morph between these sources with per-hit or per-step variation.
3. **Scatter/Advance**: Clock or manually trigger the **Scatter** or **Advance** inputs in time with your sequence for rapid, stuttering, or 'random break' effects.
4. **Inertia**: Drop to zero for instant switching, or add slew (0-5s) for smeared tails and transient blurring.
5. **Sum Outputs**: Mix the percussion for further distortion/overdrive downstream or to create composite, overblown hits.

---

## 2. Dubstep & Drum and Bass Bassline Madness

### **Key Techniques**
- **Dynamic Routing**: Use Terminal and Scatter to swap bass paths through distortion, filters, or parallel effects.
- **LFO Relationships & Frequency**: Modulate crossfades at audio rates for FM or AM basses.
- **+5V DC Offset**: Use Synapse as a stored voltage sequencer for wild pitch or folded modulation.

### **Patch Idea: Wobble, Growl, and Talking Bass**
1. **Bass Source Routing**: Feed clean and distorted (or filtered/unfiltered) bass signals to A/B of one channel.
2. **Crossfade CV**: Use envelopes, synced LFOs, or sequencer gates to automate ’wobble’ between bass treatments.
3. **Internal LFOs**: Set LFOs into the audible spectrum (~1kHz) and use them to rapidly modulate crossfade, generating vocalic, AM/FM bass textures.
    - Set LFO relationship to **Cascading** or **Alternating** for rhythmic, evolving bass.
4. **Live Routing**: Trigger **Scatter** at fills or drops for a sudden, randomized path-swapping 'talk' effect.
5. **DC Offset**: Engage +5V mode, using Synapse to inject clean control voltages or pitch steps for extra-wild modulation or for turning a channel into a step-sequencer.

---

## 3. Haunting Atmospheric Pads & Soundscapes

### **Key Techniques**
- **Slow LFO and Fade Automation**: Use slow, phase-shifted internal LFOs for evolving textures.
- **Memory Locations**: Store sections of evolving crossfade blends for live recall.
- **External CV**: Morph between droning OSCs, reverbs, granular, and field recordings via crossfade CVs or memory transitions.
- **Inertia**: Max out inertia for gliding, organic motion.

### **Patch Idea: Ghostly Pads with Evolving Motion**
1. **A/B Inputs**: Feed contrasting pad textures (analog drone vs. digital reverb, etc.) to each channel.
2. **Internal LFO Amplitude/Frequency**: Set LFOs all at different amplitudes and to **Phase Offset** or **Synchronous** for drifting stereo or quadraphonic movement.
    - LFOs modulate crossfade into evolving blends and shifting presence.
3. **Memory Banks**: Save several crossfade scenes with subtly different A/B blends.
    - Transition between them live for 'sectional' atmospheres, using high inertia for seamless morphing.
4. **Sum Outputs**: Combine pads for super-rich, wide mixes.
5. **Randomization**: Occasionally randomize LFO and memory for serendipitous ambient events.

---

## **Extra Tips**

- **Click-less Switching**: Keep enabled for smooth audio paths in pads, disable for sharp attack in percussion.
- **Per-Channel Master Volume**: Use to balance layers or attenuate wild waveforms/distortion mixtures.
- **Creative CV Routing**: Use Synapse not just for audio, but complex CV re-routing and automation (ex. LFOs into FX, sequencer signals to different destinations per memory or switch state).

---

## **Conclusion**

Qu-Bit Synapse can act as a mutant VCA, animated switch, hybrid mixer, crossfader, and more — try CV'ing everything, stacking memories, and blending between internal and external modulation for truly unique sounds.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)