# Erica Synths — Sample Drum

- [Manual PDF](../../manuals/FINAL_sample_drum_instrukcija_A4.pdf)

---

[Download the Erica Synths Sample Drum Manual (PDF)](https://www.ericasynths.lv/media/EricaSynths_SampleDrum_Manual_v1.05.pdf)

---

# Creative Ways to Use Erica Synths Sample Drum in Your Eurorack System

The Erica Synths Sample Drum is a deep, performance-oriented sampler module with loads of creative CV and performance possibilities. Here are ways to squeeze the most out of it in your modular setup:

## 1. **Smart Use of CV Inputs for Algorithmic Manipulation**
- **Random CV/Random Step Voltages:** Patch a random voltage or stepped source (like the **Mutable Instruments Marbles**, **Turing Machine**, or **Make Noise Wogglebug**) to the sample select, start point, or slice index. This creates unpredictable, generative percussion or glitchy sample rearrangement.
- **Sequencers:** Use a CV sequencer (**Malekko Voltage Block**, **Intellijel Metropolis**) for tonal variation (tune), rhythmic slicing (slice index), or sample switching in time with your sequence.

## 2. **Dynamic Drum or Percussion Voices**
- **Envelope Generators:** Patch envelopes from modules like the **Make Noise Maths**, **Intellijel Quadra**, or **ALM Pip Slope** to the Decay or Level CV input, to dynamically shape your samples based on precise performance gestures or gates from your main sequencer.
- **CVable FX Control:** Assign CV to effect parameters; use LFOs or random sources for evolving, animated effects during playback.

## 3. **On-the-Fly Sample Chopping, Live Loop Remixing**
- **Performance Mode:** Prepare 1-bar loops, slice into 8/16/32. Trigger slices from gate sequencers or clock dividers (**4ms Rotating Clock Divider**, **Pamela’s New Workout**) to create micro-variations and live “remixes” in sync with your system's tempo.
- **CV Slice Index:** Use buffered mults to send the same sequence or modulation to both the Sample Drum and another voice for tightly coordinated sample chopping and synth voice shifts.

## 4. **Hybrid Granular/Glitch Drumming**
- Use **Manual Slicing** or **Zero Crossing Auto Slicing** for click-free, granular playback.
- Randomize or CV-control playback direction and slice order (RND, BKW, FWD modes) for glitch, IDM, breakcore, or Autechre-style percussive effects.
- Pair with **Make Noise Morphagene** or **1010Music Bitbox** for stereo, higher-polyphony, or cross-sample manipulation.

## 5. **Audio-Rate CV Experiments**
- Patch high-speed LFOs, oscillators, or even audio signals to the tune or start/loop/end points for FM-style, pseudo-granular, or audio-rate effects. _Try slowly increasing the LFO speed into the audio range for wild timbral shifts._

## 6. **Live Sample Recording and Reprocessing**
- Use the module’s **live sampling** to grab fragments of your modular jams. Route an aux send or cue bus to Sample Drum input (CV3, channel 2) and immediately process/slice for instant remix, mangling, and recall.
- *Idea:* Use **XOR Electronics NerdSeq** or **Winter Modular Eloquencer** to send triggers to record new content at precise moments.

## 7. **Insertion FX, Parallel Processing, and Sidechaining**
- Send Sample Drum audio out to effects modules (**Strymon Magneto**, **Mordax Data**, **Tiptop Z-DSP**, **Endorphin.es Milky Way**) before returning to your main outs or other mixers.
- Use **VCAs** (*Intellijel Quad VCA*, *Doepfer A-132-4*) to further sculpt dynamics with envelope or modulation control.
- Apply a sidechain ducking effect with envelope followers or dedicated sidechain modules to let Sample Drum "duck" or react dynamically to other percussion.

## 8. **Stereo Imaging and Crossfades (with External Mixer)**
- Exploit the dual-channel nature of Sample Drum for live A/B performance: one-shot stabs on one channel, evolving loops on the other.
- Use a performance mixer (**WMD Performance Mixer**, **Intellijel Mixup**) for crossfading, mutes, or parallel FX sends.

## 9. **Sample-Based Synth Voice/Liquid Droning**
- Load tuned single-cycle waveforms or drone loops into Sample Drum. Use 1V/Oct into pitch for playable melodic lines.
- Modulate loop points and FX via slow LFOs for morphing pads or shifting background textures.

## 10. **Sample Drum as a Performance Hub**
- Assign the six rotary encoders for instant control of the parameters you tweak most in live jams (tune, FX, start/loop/end, decay, etc.).
- Save projects suited to different live sets/styles for instant recall during performances.

---

### Example Patches

#### **Glitch Percussion Machine**
1. Patch clock divider triggers to both TRG1 and TRG2 (polyrhythms).
2. Use Marbles or Wogglebug stepped random to CV Slice Index.
3. Assign FX mix to a spare encoder and modulate with an LFO.
4. Split the outs into a mixer, cueing one out for additional live FX.

#### **Live Loop Chopping with Sequencer Sync**
1. Load a loop, slice into 16 parts.
2. Use a pitch CV sequencer in 1V/Oct mode to select slices per step.
3. Patch a gate sequence from your main sequencer to TRIG1.
4. Try quickly recording in new audio on channel 2 (as a breakdown fill).

---

### Useful Module Types for Pairing

- Random/stepped CV generators (*Turing Machine, Marbles*)
- Sequencers with CV out (*Voltage Block, Eloquencer, NerdSeq*)
- Dedicated effects modules (*Milky Way, Magneto, Z-DSP*)
- Audio/CV mixers and VCAs (*Quad VCA, WMD Performance Mixer*)
- Clock modulation tools (*4ms Rotating Clock Divider, PNW*)
- LFOs and Envelope Generators (*ALM Pip Slope, Maths*)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
