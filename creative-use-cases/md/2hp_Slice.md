# 2hp — Slice

- [Manual PDF](../../manuals/2hp_Slice.pdf)

---

[**2hp Slice Manual PDF**](https://twohp.com/manuals/slice_manual.pdf)

---

## Creative Uses for the 2hp Slice in Eurorack Systems

The **2hp Slice** is a compact, clockable beat repeat and glitch effect engine—perfect for creative audio manipulation. Here are inventive ways to exploit its potential, both with specific modules and general Eurorack module types:

---

### 1. **Live Drum Glitching**
**Combine With:**
- **Mutable Instruments Peaks/ALM Busy Circuits Pam’s New Workout (Pamela's)** (Clock/Trigger source)
- **TipTop Audio ONE, Erica Synths Sample Drum** (Sample/Drum modules)

**Patch Idea:**
- Use a drum or percussion loop as the input to Slice.
- Feed clock and/or triggers from a sequencer or clock divider (e.g., Pam’s New Workout) to precisely control when the beat repeat activates.
- Modulate the Size CV with a stepped random CV (e.g., Mutable Instruments Marbles, or Doepfer A-118) for unpredictable repeat sizes.

**Result:**  
Live, rhythmically-locked glitch effects—great for fills, triplet rolls, or granular breakdowns in percussion-heavy patches.

---

### 2. **Experimental Granular Textures**
**Combine With:**
- **Make Noise Morphagene / 4ms Stereo Triggered Sampler** (Tape/Looper modules)
- **Qu-Bit Chance / WMD/SSF Modbox** (Random/Modulation sources)

**Patch Idea:**
- Use long, evolving audio samples as Slice’s input.
- Randomize the Size parameter via LFO or sample & hold to "scan" beat repeat sizes.
- Occasionally freeze the buffer manually or automate the Trig input with irregular gate bursts from a random gate generator.

**Result:**  
Unpredictable, stuttering textures reminiscent of classic glitch and IDM production techniques.

---

### 3. **Creating Polyrhythms and Odd-Time Grooves**
**Combine With:**
- **Intellijel Steppy / 4ms Quad Clock Distributor** (Multichannel sequencers)
- **Mutable Instruments Grids / Euclidean Circles** (Rhythm generators)

**Patch Idea:**
- Use multiple copies (multisplitted audio) of a groove or synth riff, processed through different clock rates and Size settings on Slice.
- Switch between including/excluding triplets via the toggle for instant polyrhythmic shifts.

**Result:**  
Layers of repeating fragments that weave in and out of sync—ideal for mathy grooves or unique breakdowns.

---

### 4. **Glitching Melodies and Vocals**
**Combine With:**
- **Intellijel Shapeshifter / Make Noise DPO** (For melodic synth lines)
- **2hp Play, Endorphin.es Two of Cups, or similar micro sampler** (For vocals)

**Patch Idea:**
- Run melodic or vocal lines into Slice.
- Use an envelope follower (e.g., Mutable Instruments Ears or Doepfer A-119) to derive gates from audio peaks, which then trigger the repeat gate input—creating glitch slices "in rhythm" with the natural dynamics of the source.
- Use an external pitch CV randomizer to modulate the Slice size for subtle or extreme pitch/rhythm manipulation.

**Result:**  
Intricate, dynamically triggered pitch-mangling and micro-looped vocal or synth phrases.

---

### 5. **Feedback Loop Destruction**
**Combine With:**
- **2hp Loop / Bastl Instruments Spring reverb / Doepfer A-189-1 Bit Modifier** (Loop recorders, Signal destructors)
- **Mixers/VCAs**

**Patch Idea:**
- Patch the output of Slice back into a loop station, delay, or bit crusher.
- Modulate Slice trigger/size in sync with the loop, or at odds for unstable results.
- Adjust feedback amount with a VCA for controlled chaos.

**Result:**  
Self-oscillating, evolving loops full of digital artifacts and abrupt rhythmic stutters—a great way to spice up drones or ambient patches.

---

### Generic Module Type Suggestions

- **Clock/Random Generators:** (Pamela’s New Workout, Mutable Marbles, Doepfer A-160)
- **Samplers/Recorders:** (2hp Play, TipTop ONE, 4ms STS, Make Noise Morphagene)
- **Drum Modules:** (ALM Akemie’s Taiko, Erica Synths Drum Mixer)
- **Sequencers:** (Intellijel Metropolix, Arturia Keystep Pro)
- **CV Modulation:** (LFOs, Random, Sample & Hold, Complex Function Generators)
- **Envelope Followers:** (Mutable Ears, Doepfer A-119)
- **Effect Processors:** (Loopers, Delays, Bitcrushers)

The 2hp Slice thrives on **clock and CV modulation**—get creative with tempo divisions/multiplications, feedback routings, and dynamic gate triggering to unlock maximum glitchy fun in your modular rig!

---

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**