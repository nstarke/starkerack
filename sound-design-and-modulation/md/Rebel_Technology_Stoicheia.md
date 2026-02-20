# Rebel Technology — Stoicheia

- [Manual PDF](../../manuals/Stoicheia – Rebel Technology.pdf)

---

[Stoicheia (Στοιχεῖα) Euclidean Sequencer Manual PDF](https://raw.github.com/pingdynasty/EuclideanSequencer/master/EuclideanSequencerSchematic.png)

---

## Rebel Technology Stoicheia – Creative Modulation Guide

The Rebel Technology Stoicheia (Στοιχεῖα) is a dual Euclidean sequencer designed to generate complex rhythmic patterns from input trigger signals. By combining its unique Euclidean sequencing with creative patching and CV modulation, you can coax everything from crushed, distorted percussion to wild bass rhythms and shimmering atmospheres. Here’s how to push its capabilities for your modular music:

---

### Module Overview

**Main Modulation Points:**
- **Two independent Euclidean sequence channels (A and B)**
- **Sequence Length (1–16 steps)**
- **Number of Fills (active steps per cycle)**
- **Rotation (sequence offset)**
- **Modes:** Trigger, Alternating, Chained
- **Clock inputs (external, LFOs, gates, audio!)**
- **CVable via external modulation (using supporting modules or hands-on control)**

---

## 1. Distorted Percussive Sounds

### **a. Clock Modulation with Audio-Rate Signals**
- **Patch a drum voice or sample module to the output of Stoicheia.**
- **Feed the clock input a square wave or fast LFO, OR experiment with audio-rate clocks (oscillator square wave, noise bursts).**
- **Result:** Audio-range clocks can turn Steicheia’s output into glitchy, harsh digital noise bursts and pseudo-bitcrushed rhythmics.
- **Tip:** Patch clock through a VCA modulated by an envelope to shape percussive “grit” on each trigger.

### **b. Live Fills Modulation**
- **Modulate the “Fills” knob with a slewed random CV or sequencer.**
- **Result:** Polyrhythmic fills and stuttering, irregular percussion—great for breakbeats and industrial hits.
- **Tip:** Rapid fill changes create metallic machine-gun or granular snares.

### **c. Rotation Knob Twisting**
- **Randomly or rhythmically sweep the “Rotation” knob.**
- **Combined with fill/length modulation, this will create morphing, non-repetitive hits and fills—ideal for distorted IDM and d’n’b percussion.**

---

## 2. Crazy Basslines (Dubstep, Drum and Bass)

### **a. Sequence Bassline Gate Patterns**
- **Send Stoicheia’s outputs to an envelope or VCA opening a bass oscillator.**
- **Use Chained Mode:** Sequence A = 12, Sequence B = 4, total 16 steps with off-kilter Euclidean fills.
- **Result:** Bassline triggers with non-square, “wonky” groove.

### **b. Modulate Length and Fill via CV**
- **If you have a CV controllable version or can hack the panel, use LFOs or sequencers patched to the length/fill controls for A/B.**
- **Result:** Syncopated, “alive” step-sequenced bass that twists between rigid and loose, mechanical and organic.
- **Try:** Random CV for fills = classic “wobble” bass patterns.

### **c. High-Rate Clock Tricks**
- **Patch a very high-frequency clock (audio rates) to Stoicheia, run its gate to an oscillator FM input or to a filter’s trigger/FMOD.**
- **Result:** Rhythmic digital distortion, stutters, and aliasing effects for neurofunk growls and reese basslines.
- **Patch both A and B outputs to two oscillators for polyrhythmic bass duets.**

---

## 3. Haunting Atmospheric Pads

### **a. Use for Slow, Evolving Gates**
- **Patch an ultra-slow LFO or clock divider to the clock inputs.**
- **Set long sequences (e.g., 13 or 15 steps) with sparse fills for unpredictable pads (E(3,13), E(5,15), etc.).**
- **Send outputs to LPGs or long envelopes controlling pad swells.**
- **Result:** Rhythmic, ghostly patterns that never quite repeat—great for ambient music.

### **b. Chained or Offset Polyrhythms**
- **Set different rotations on A/B, use both to trigger multiple voices panned left/right for evolving stereo movement.**
- **Live-modulate rotation for “shimmering” effect as pad hits drift in and out of sync.**

### **c. Turn Fill/Length while Freezing Rotation**
- **Hands-on (or with attenuation and CV) sweep fills and lengths slowly while keeping rotation steady.**
- **Result:** Slowly shifting textural patterns, like ritual bells or distant thunder.

---

## Tips & Tricks

- **Audio Clocking:** Don’t be afraid to use audio oscillators, noise, or unpredictable sources for the clock input—results can be wild, from harsh pulses to organic sounds.
- **Reset Input:** Use external modules to reset both sequences in sync with other events, e.g., with the downbeat of a loop.
- **Chained Mode:** Allows beyond-16-step polymetric sequences—perfect for generative or long-form music.
- **CV Modulation:** Theoretically, you can hack the hardware or use external voltage-to-pot adapters to automate all parameters.

---

## Further Exploration

- **Firmware hacking:** Since Stoicheia is open source, you can flash or customize its behavior if you’re handy with code/AVR.
- **Use CV randomizers and logic modules to inject even more change and chaos into your gate patterns.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)