# Erica Synths — Clap

- [Manual PDF](../../manuals/CLAP_manual.pdf)

---

[Download the Erica Synths Clap Manual (PDF)](https://www.ericasynths.lv/media/Clap_v1_02_manual.pdf)

---

# Erica Synths Dual Drive: Experimental Modulation Ideas

As a Eurorack musician focusing on percussive distortion, aggressive basslines, and haunting atmospheric pads, the Erica Synths Clap module offers a lot of creative modulation possibilities. Here’s how you can push its sound boundaries:

## **Module Recap**

**Controls & Inputs:**
- **Tone:** Master tone for the clap (has CV attenuator)
- **Decay:** Decay time for the clap (controllable)
- **TRIG/ACC:** Trigger for hits and accent (max level with +10V to ACC input)
- **Tone CV:** Modulate tone
- **Output:** Audio out

## **Modulation Tips by Sound Type**

### **1. Distorted Percussive Sounds**

- **Patch Idea:** Feed a snappy, fast envelope or LFO into the **Tone CV** input.
  - *Why?* Constantly shifts the timbre, making each clap hit sound spiky and more “distorted.”
- **Use an analog distortion, wavefolder, or the Erica Dual Drive post-Clap output** to add harmonics and texture.
- **Accentuate Randomness:** Run randomly-timed triggers into **TRIG** for unpredictable, glitchy beats. Use a stepped random or Turing Machine sequence into **Tone CV** for morphing harshness.
- **Extreme Decay Sweeps:** Modulate **Decay** knob in real time or with CV (via external sequential switch or LFO) to morph between gated plips and long, noisy bursts.

### **2. Crazy Basslines (Dubstep, Drum & Bass)**

- **Substitute for Oscillator:** Using the noisy “clap” as an oscillator source.
  - Patch a very fast trigger/gate sequence into **TRIG** (audio rate or near-audio rate).
  - Heavily modulate **Tone** and **Decay** with LFOs or sequencers synchronized to your bassline pattern.
- **Accent Control for Movement:** Program accents in your CV sequencer or via gate merges to make some hits “pop” (send +10V to **ACC**).
- **Filter + Distortion:** Route module output through a resonant lowpass filter and then a distortion/wavefolder for squelchy, growling digital sounds.

### **3. Haunting Atmospheric Pads**

- **Modulate Decay for Texture:** Send a slow, undulating envelope or random LFO to **Decay CV** for evolving noise shapes.
- **Layer Multiple Clap Modules or Multed Outputs:** Each with slightly shifted **Tone** and **Decay** (modulated slowly) to create dense, spectral textures.
- **Reverb + Delay:** After output, send to lush reverb/delay for atmospheric wash.
- **Drone Techniques:** Trigger the clap at audio-rate with fast LFOs or random triggers, and use a slow LFO or envelope on **Tone CV** for evolving pads. Try leaving decay long and letting sounds overlap into clouds of shifting noise.

## **General Tactics**

- **Accent Dynamics:** Don’t leave the **ACC** input static; modulate it for subtle “ghost notes” or massive hits.
- **Rhythmic Complexity:** Use clock dividers/multipliers to sequence unusual trigger patterns into **TRIG**.
- **CV Control Morphing:** Keep modulation sources moving—LFOs, random, sequencers, envelopes all bring the sound to life.
- **Feedback/Resample:** Send output to a sampler/looper, cut and resample with external DSP/fx for building complex, layered textures.

---

> **Manual PDF:** [Erica Synths Clap Manual (PDF)](https://www.ericasynths.lv/media/Clap_v1_02_manual.pdf)  
> **Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**