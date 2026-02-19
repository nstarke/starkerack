# Wenzellabs — NSA Selector

- [Manual PDF](../../manuals/wenzellabs_the_NSA_selector_ the NSA selector eurorack module.pdf)

---

[NSA Selector Manual (PDF)](https://github.com/wenzellabs/the_NSA_selector/raw/main/README.md)  
*If the above link doesn't work, [view the Github page here](https://github.com/wenzellabs/the_NSA_selector)*

---

# Using the NSA Selector for Hyper-Complex, Densely Rhythmic Percussion in Eurorack

The **NSA Selector** is not a traditional voice, oscillator, or standard effects module. Instead, it is a network-to-audio converter that taps raw Ethernet traffic, translates network data (at the physical, not protocol level) into a 4-bit, 25MS/s audio stream, and spits it out as audio. This opens up a **new world** of using *network activity* as a source of wild, unpredictable, or programmable rhythmic complexity.

## What The NSA Selector Is

- **Not an audio interface**: It doesn’t play back audio files (no MP3, WAV, etc. playback).
- **Network stream to audio**: Any data packet on the network can form the audio stream—ideal for taking advantage of the *density and complexity* of network traffic as a random or controlled audio/percussive source.
- **Eurorack format, 4HP**, audio output, dual Ethernet in/out.

## Generating Dense, Complex Percussion with the NSA Selector

### 1. **Harness Network Activity for Percussion**

- Patch the audio output of the NSA Selector directly to a VCA, filter, or distortion.
- Run actual **network traffic**, triggers, or patterns using tools/scripts on your computer, and use these *as a percussive "sequencer"*.
- **Methods:**
    - Use the *sequencer shell script* (provided in the repo) to send ping bursts at complex, programmable intervals; network packet sizes/spacing will directly shape the rhythm.
    - Transfer large, uncompressed images (*.bmp*) or other files for continuous bursts of network noise — the file size, structure, and transmission method will shape the rhythmic activity!
    - Run or write custom scripts to output traffic in arbitrary, algorithmic, generative, or polyrhythmic pulse streams.
    - Trigger multiple devices on the network to talk at polyrhythmic or odd-time intervals (especially with multiple scripts running at odd timer divisors).

### 2. **Embrace Polyrhythms & Complex Timings**

- **Desynchronize** multiple traffic sources (for example, multiple computers, VMs, or scripts) running at cycles that relate by complex ratios (e.g., 7/8 vs 9/8 vs 13/8): the composite traffic will organically create dense, interlocking polyrhythms.
- Change packet size, intervals, source/destination pairs; these all skew the resulting rhythm, producing off-kilter grooves.
- Use tools like `ping`, `netcat`, or custom UDP/TCP spamming scripts with variable timings to "play" the network as your percussion generator.

### 3. **Enhance & Sculpt Percussive Complexity in the Modular System**

- **Processing:** Patch NSA Selector’s output through:
    - **Envelopes/VCA:** Use an envelope follower to extract rising/falling dynamics out of the noise for punchy, squelchy percussive accents.
    - **Filters:** Sculpt the noise to sweep or emphasize certain frequency bands that correspond to desired percussive elements.
    - **Distortion/Wavefolder:** Crunch the network noise for extra punch and sizzle.
    - **VCAs/Gates:** Use sidechained gates to chop up the noise or isolate traffic bursts as discrete drum hits.
- Use as an **audio-rate modulator** to introduce digital "texture" into otherwise-acoustic percussion sources—try ring modulation or AM with more traditional drum voices for glitchy, NSA-infused percussion.

### 4. **Unique & Punchy Voice Design Tips**

- **Layering:** Mix NSA Selector with other percussive sources—use as a transient, a noise burst, or add texture/ambience.
- **Feedback:** Route the output into a delay or effect, then back into your network setup (by broadcasting the audio back as traffic for recursive, evolving rhythms).
- **MIDI/Software Sync:** Develop a custom script to send network "hits" from a MIDI sequencer, channeling your DAW or controller’s polyrhythmic chops directly into the NSA Selector.

### 5. **Random/Chaotic Percussion Approach**

- Plug the module onto a network used by other people/devices for unpredictable, stochastic percussion sourced from *real-world* events.
- Map the density of traffic to filter cutoff, envelope, or other CV-able parameters, for *network-to-control-voltage* mapped complexity.

---

## **Recommended Patch Example**
```
NSA Selector Audio Out
  → Mult
  → VCA #1         → Channel 1 Mixer (main percussion)   → Output
  → Bandpass Filter → VCA #2 (Env Follower’d)            → Fuzz → Mixer (snare/grit layer) → Output
  → Envelope Follower (from original out) → CV for VCA/Gate/Envelope Retrigger

NSA Selector Audio Out
  → Sequencer Input (sample-and-hold or logic) for generating random triggers
```

---

> **Explore deeply: “Be creative!”**  
> The manual stresses experimentation: This module is meant for unique, one-of-a-kind rhythmic and percussive effects that break the grid. The intersection between networking and Eurorack is the sound of techno-anarchy!

---

[GitHub: Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)