# Doepfer — A-119

- [Manual PDF](../../manuals/A119_man.pdf)

---

[Doepfer A-119 Manual (PDF)](https://doepfer.de/a100_man/A119_anl.pdf)

---

# Using the Doepfer A-119 Ext. Input / Envelope Follower to Structure Full Length Eurorack Songs

## Overview

The Doepfer A-119 is much more than just an audio input preamp. By extracting **envelope** and **gate** information from external signals—vocals, guitar, drum machines, or any audio—it becomes a versatile control source for your whole system. This makes it a powerful tool for modulating, automating, and even *conducting* a eurorack patch over the span of an evolving, full-length composition.

Below are advanced strategies for using the A-119, in combination with other modules, to build arrangements, transitions, and song structures—moving beyond simple loops into complete tracks.

---

## 1. **Using External Audio as a Song-Conductor**

### a) **Dynamic Scene and Section Changes**

- **Input** a microphone with vocals (or even a drum machine loop).
- **Gate out** from A-119 triggers different sections in your patch:  
  - Patch to clock dividers/sequential switches to cycle through drum/bass/melody patterns.
  - Use the **envelope out** for slow, smooth automation (e.g., filter sweeps, reverb/delay levels).
- **Result:** You control transitions, breakdowns, and buildups simply with your voice or an outboard instrument.

### b) **Live Muting & Unmuting**

- Use A-119's envelope or gate to control **VCAs** or **mute switches** for instant drops/buildups by playing or pausing your external signal.
- Example: Stop playing/singing for a “break;” bring the beat back by starting again.

---

## 2. **Automated Modulation based on Intensity**

### a) **Mix Evolution**

- Patch the **envelope output** to a matrix mixer, affecting multiple modulation destinations (VCF cutoff, VCA gain, effects parameters, sequencer speed).
- Vary your external audio intensity for organic transitions between “verses” and “choruses.”

### b) **Rhythmic Gates and Pattern Switching**

- **Gate out** to pattern selectors, clock dividers, or sequential switch modules.
- Example: Use a handclap or a loud guitar chord to switch drum patterns, launch fills, or reset sequencers, creating variation throughout the performance.

---

## 3. **Sidechain & Ducking for Arrangement and Groove**

### a) **Classic Sidechain Pumping**

- Feed a drum machine kick or external drum loop through A-119.
- Patch **gate out** (or envelope with slew for smoothing) to the CV input of the track’s main VCA.
- Whenever the kick hits, it ducks your bass/lead/synth line, as in classic electronic tracks.
- Use for breakdown/build effect by turning the external drum loop on/off during the song.

### b) **Level-Responsive Effects**

- Use the **envelope out** to open up reverbs/delays only when vocal/guitar is loud—great for “epic” chorus effects, or pulling back for verses.

---

## 4. **Ring Mod and Audio-Rate Modulation (for Unique Transitions)**

- Use A-119 to bring vocals/guitar to modular-level, then ring modulate with a VCO (as in manual).
- Modulate the ring modulator’s output VCA with the A-119 **envelope**, so the effect is only heard while you play/sing.
- Use this for climactic sections, or as a transition effect in your song arrangement.

---

## 5. **Song Structure with Sequential Automation**

- Use **gate out** to clock a sequential switch or sample & hold.
- Every time you strike your external signal, the patch state advances: change drum sound, chord, filter routing, FX send.
- Map out a full verse-chorus-bridge structure by associating different patch routings to each step.

---

## 6. **Sampling & Looping External Input**

- Use A-119 with a sampler/looper module (e.g., Make Noise Morphagene, 4ms Stereo Triggered Sampler).
- Manually start and stop sampling/overdubbing using the **gate out** as a “record” trigger, letting you “perform” when new material enters the song.

---

## 7. **Creative Gate/Envelope Routing for Algorithmic Compositions**

- Patch the envelope output to the rate control of random/chaotic LFOs or probability-based triggers (e.g., Mutable Instruments Marbles).
- Your playing dynamically changes the randomness, complexity, or intensity of algorithmic drum lines or melodic variation, evolving across song sections.

---

## **Summary**

> **The A-119 transforms external input—voice, instruments, even processed or sampled material—into modular “control language.” By patching its envelope and gate outs creatively, it becomes the bridge between performance and composition. Use it to automate transitions, modulate effects, generate triggers for song sections, shape dynamics, and make your modular patches perform with the life and variation needed for full-length songs, not just endless loops.**

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**