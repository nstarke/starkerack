# Tiptop Audio — HATS808

- [Manual PDF](../../manuals/Tiptop_Audio_HATS808_ns.pdf)

---

[Download the HATS808 Manual PDF](https://www.tiptopaudio.com/manuals/hats808.pdf)

---

# Creative Modulation Strategies for Tiptop Audio HATS808  
_Analysis by a Eurorack Synthesist_

The Tiptop Audio HATS808 is a deep, analog hi-hat module with many unique modulation opportunities. With its added voltage-controlled resonance (Q/VC-Q), enhanced gain staging, and independent accent control, it is capable of far more than classic hi-hat duties. Let’s dive into ways you can leverage this module for distorted percussion, warped dubstep/drum & bass basslines, and eerie atmospheric textures.

---

## 1. Distorted Percussive Sounds

#### Utilize the Overdrive (HOT GAIN)
- **LEVEL Knob:** Set the LEVEL to max; this pushes the output into hot, saturated territory.
- **ACCENT Knob:** Also max this out, or modulate with high-velocity triggers for further punch and harmonics.

#### External Clipping/Distortion
- Patch the HATS808 output into an external wavefolder, distortion, or even guitar pedals for increased bite.

#### VC-Q Modulation
- Use an LFO or envelope to modulate the VC-Q input. Rapid, snappy envelopes (from maths/function generators) will cause the band-pass filter resonance to sweep, creating metallic, tearing or “laser-like” textures.
- You can also try audio-rate modulation (patch an oscillator into VC-Q). This will create ring-mod and digital/bitcrush-style artifacts due to the filter entering self-oscillation and chaotic behavior.

#### Choke & Accent Tricks
- For rhythmic stutters, sequence repeated CH triggers with offset or random accents. Use accent modulation to induce unpredictably distorted, clipped attacks on some beats.

---

## 2. Crazy Bassline Generation (Dubstep/DnB)

#### BandPass Out for Bass
- Use the **BandPass OUT** as a raw oscillator: Patch it into a VCA, filter, and envelope controlled by your sequencer.
- Crank the Q knob—when past a certain point, the internal filter begins to oscillate. Try holding the Open Hat for longer decays; this produces a droning, bassy tone that’s somewhere between a kick, snare, and metallic waveform.

#### Audio-Rate VC-Q FM
- Feed a VCO or noise source into the VC-Q input. With high Q settings, the band-pass filter will track this CV, giving you aggressive, vocal/squelchy or growling bass—especially effective if clock-synced to your sequencer.

#### Envelope Modulation
- Mult a drum envelope or LFO to the VC-Q; sweep the Q at bass rates for wobble bass. Longer envelopes modulating Q give you strong moving bass textures—just like dubstep wobs.

#### Extreme Choke Disabling
- Disable choke on the HATS808 (jumper on PCB as described). This allows the Open Hat/“bass oscillator” to decay fully, sustaining distorted tones—good for droning notes or basses.

---

## 3. Atmospheric Pad/Texture Design

#### BandPass Raw Source
- The BandPass OUT is a wonderful metallic/spectral sound source. Run it into a long-decay envelope-controlled VCA, reverb, and/or granular modules for textural pad layers.

#### VC-Q with Slow Modulation
- Patch a slow LFO, envelope follower (from a field mic, contact mic, etc.), or S&H into VC-Q for gentle, evolving changes in resonance—making shimmering or haunting sound beds.

#### Self-Oscillation Drones
- Push Q to self-oscillation territory. Carefully tune the decay/hold with external envelopes. Add reverb and delay for cavernous, bell-like atmospheres.

#### Feedback Loop
- Route the output of BandPass OUT back into a mixer channel, and route some of this back into the VC-Q, optionally passing through a delay or phaser first. Carefully controlled, this feedback creates eerie, evolving metallic atmospheres.

---

### Bonus Utility: External Modulation and Processing
- HATS808 responds well to CV from unusual sources:
  - **Random Voltages/S&H:** For unpredictable timbral shifts.
  - **Envelope Followers:** To impart movement from external audio into the percussive sound.
  - **Sequencer Gates/CV:** For classic rhythmic modulation of ACCENT, LEVEL, and VC-Q.

### Patch Examples

```text
* Distorted Perc Shot:
  OH OUT → Overdrive → Mixer
  ACCENT IN: Envelope with peak at attack

* Wobble Bass:
  BANDPASS OUT → VCA → Filter
  VC-Q IN: Sine VCO (audio-rate)
  Decay: Long

* Haunting Pad:
  BANDPASS OUT → VCA (long envelope) → Reverb → Output
  VC-Q IN: Slow S&H or LFO
```

---

Explore unconventional patching—remember, modulation is key to unique timbres. The HATS808 isn’t just a hi-hat, it’s a wild source of analog energy for the curious.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)