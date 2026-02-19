# Doepfer — A-135-1

- [Manual PDF](../../manuals/A135_man.pdf)

---

[Doepfer A-135 VC-Mixer Manual (PDF)](https://doepfer.de/a100man/A135_anl.pdf)

---

## Using the Doepfer A-135 VC-Mixer for Dense & Complex Percussion

As a eurorack artist aiming for hyper-complex, polymetric percussion, the **A-135 VC-Mixer** isn't just a utility—it's a dynamic performance and sequencing tool. Here’s how you can harness this voltage-controlled mixer for rhythmic intensity:

---

### Core Features to Exploit

- **Four Independent, Linear VCAs**: Each input is independently mixed with CV-controllable volume.
- **CV Control for Each Channel**: The CV inputs (with their attenuators) let you rhythmically gate/morph each sound using external trigger, LFO, envelope, or sequence sources.
- **Manual Gain Offset**: Push channels into constant "open" or use as a bias for bipolar CVs (great for morphing or creating asymmetrical patterns).

---

### Percussive Applications & Unique Techniques

#### 1. **Dynamic Voice Summing for Polyrhythms**

- **Patch** 4 separate percussion voices (TR-808/909 modules, synthesized percs, sample players, or even heavily filtered noise/oscillators) into the 4 audio inputs.
- Use a complex trigger or gate sequencer (e.g., Mutable Instruments Grids with Euclidean patterns, or Pamela’s New Workout) to send gates/LFOs/envelopes to the CV inputs of each channel.
    - **Example**: Channel 1 = regular 4/4 kick, Channel 2 = 5-step hat pattern, Channel 3 = 7-step snare hits, Channel 4 = 11-step FM clang.
- **Result**: The overall output is a blend of polyrhythms, constantly morphing as your CV sources interact.

#### 2. **Rhythmically Gating Audio Sources**

- **Send audio-rate triggers or audio snippets** to the audio ins and gate them with fast envelopes.
    - Use short, snappy envelopes (from an A-140, Maths, or Falistri) triggered by advanced sequencer logic (e.g., OR/AND/XOR clocks, or even probability triggers).
- Use LFOs or random CVs (A-118, A-148) to toggle or pulse the channels, dynamically muting/unmuting rhythmic fragments and textures for generative results.

#### 3. **Morphing, Randomized, or "Animated" Drum Patterns**

- Patch CVs from sequencers with clock divisions/multiplications, random gates, or irregular LFOs.
- Randomly modulate the Gain controls to let quiet percussion "peek" through—this is great for **ghost notes** or *micro-dynamics*.
- Run a morph CV (A-144 Morph Controller, Planar, or joystick module) into all four channels—crossfade complex percussive parts for live morphs.

#### 4. **Percussive "Ring-Mod" Style FX**

- Feed an audio-rate percussion signal (e.g., a hi-hat or metallic sound) into the CV input of a channel, with another drum sound at the audio input.
- You’ll get wild, AM/ringmod-like percussion that’s highly dynamic and gritty—perfect for punchy, off-kilter drums.

#### 5. **MIDI-CV and Cross-Platform Complexity**

- Use MIDI-to-CV modules to send algorithmic, polyrhythmic MIDI controller data into CV ins.
    - Example: Mod Wheel controls snare level, Pitch Bend morphs between channels, velocity accentuates hats—all clocked from DAW or an external sequencer.

#### 6. **Patch Example for Extreme Complexity**
```plaintext
[Kick Module] ----> Audio In 1
                        /      \
[Trigger Sequencer A]-- CV In 1 (Euclidean 4/4)
[FM Snare] ---------> Audio In 2
                        /      \
[Trigger Seq B] ----- CV In 2 (7/8 pattern, irregular gates)
[Sample Player] ----> Audio In 3
                        /      \
[Random S&H] ------- CV In 3 (for digital artifacts)
[Filtered Noise] ---> Audio In 4
                        /      \
[LFO+Envelope] ------ CV In 4 (morphs at odd divisions)
> To FX and Master Out!
```

---

### Tips for Punch, Uniqueness, and Percussive Impact

- **Use Short, Snappy CVs**: Decay envelopes, tight triggers, and steep random gates create sharp, percussive transients.
- **Exploit Gain Offsets for Ghosts**: Subtle boost lets quieter hits through, perfect for groove nuances.
- **CV Over Audio for FM**: For truly broken/glitchy sounds, route audio signals as CVs, not just control voltages.
- **Cascade More VCAs!**: Chain another quad VCA for multi-stage Gating/AM, driving even wilder textures.
- **Feedback Loops**: Mix VC-Mixer out back into a percussive modulator for recursive complexity.

---

### More Possibilities

- **Morph Percussion with A-144 or Planar**
    - Achieve single-knob crossfading and quirky rhythm morphs across four voices.
- **Automate via DAW/External MIDI**
    - Deep integration for generative, superhuman-precision percussion automation.

---

- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)