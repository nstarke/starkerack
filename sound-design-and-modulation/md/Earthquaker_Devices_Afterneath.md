# Earthquaker Devices — Afterneath

- [Manual PDF](../../manuals/EQD-EU-Afterneath-Eurorack-R1.pdf)

---

[Download the Afterneath Eurorack Module Manual (PDF)](https://www.earthquakerdevices.com/content/afterneath-eurorack-manual.pdf)

---

# How To Modulate the EarthQuaker Devices Afterneath for Powerful Percussive, Bass, and Pad Sounds

The **Afterneath Eurorack Module** is a unique and versatile reverb/delay effect, especially when deeply modulated via CV. Below are techniques and patch ideas to use CV, external modulation, and feedback routing to sculpt the kinds of powerful, unorthodox sounds you might crave for experimental, electronic, or bass-heavy music.

## Percussive and Distorted Sound Design

### Core Concepts
- **Percussive sounds** often need snappy, sharp envelopes or drastic pitch/rate changes.
- The Afterneath's digital architecture—particularly the **Drag**, **Diffuse**, and **Reflect** parameters—can take clean input signals and, via modulation, break them into unpredictable, glitchy rhythms with metallic or resonant tails.

### Techniques
#### 1. **Self-Oscillation for Distorted "Kick/Impact" Sounds**
- **Reflect** and **Length** above noon induce self-oscillation.
- Patch short, sharp envelopes into **Drag CV**: abrupt CV bursts will cause wild, pitch-glided booms and distorted digital "hits."
- Try putting the **Mode** in anything from classic (Unquantized) to chromatic or major scale for varied pitch intervals between hits.
- Feedback through external distortion: Patch **Reflect Send** to a distortion pedal or saturator, then back to **Reflect Return** for even more extreme, chaotic impacts and ring-modulated tails.

#### 2. **Stuttering Percussive Echoes**
- Clock or gate the **Drag CV**: feeding rhythmic gates/pulses into Drag can make the delay lines "jump," slicing your input into repeated percussive grains—add LFO to **Diffuse** to smear for metallic/repeated drum textures.

---

## Dubstep/Drum & Bass Basslines

### Core Concepts
- Dubstep and DnB basses thrive on unpredictable filtering, glitched delays, and evolving timbres.
- The Afterneath can serve as an aggressive sound-warping module even for "dry"-style bass patches.

### Techniques
#### 1. **Bass Growls via CV Pitch Quantization**
- In **Mode 4-9** (Quantized/Scales), run a bassline into the Afterneath and sequence the **Drag CV** with a stepped random voltage, a sequencer, or a keyboard.
- Let self-oscillation interact with the input: the result can be deep, pitch-quantized digital resonances that snarl and mutate.
- Use an envelope, LFO, or your bass sequence to modulate **Diffuse** or **Length** for shifting energy from dry attacks to long, droning decays.

#### 2. **Aggressive Feedback Squelch**
- Redirect **Reflect Send** through a VCF or distortion and return it.
- Sequence the cutoff or distortion gain in sync with your bassline. The feedback loop will interact with the Afterneath’s reverb/delay, generating squelchy, evolving harmonics and sidebands.

---

## Haunting Atmospheric Pad Sounds

### Core Concepts
- Pads shine when sounds are smeared, randomized, and constantly evolving.
- The Afterneath's **Diffuse**, **Length**, ambient feedback, and CV-morphing stand out here.

### Techniques
#### 1. **Evolving Clouds with Random Modulation**
- Patch a slow, random or cyclic voltage into **Drag CV** in **Unquantized** or **Pentatonic/Octave** modes. The pitch and character will drift through “otherworldly” intervals.
- Modulate **Diffuse**, **Length**, and **Mix** with slow external LFOs, S&H, or random voltage for shifting cloud-like textures.
- Set up a Pseudo-Stereo Patch: Main Out to Left, **Reflect Send** to Right, return some to an effect chain (reverb/EQ/freeze/granular), then back to Reflect Return.
- For shimmer-like pads: process Reflect Send through a pitch shifter (up an octave or two) before routing back to Reflect Return.

#### 2. **Ghostly Melodic Melts**
- With an arpeggiated input, set Mode to **Major, Minor, or Pentatonic Quantized**, and run a very slow triangle or sine LFO into **Drag CV**.
- Each note/phrase becomes a blurred, scale-locked glissando, giving the pad a spectral, drifting sense of melody.

---

## General Modulation Tips

- **All four main parameters (Drag, Mode, Diffuse, Length) accept CV and have inverting attenuators.**
    - Try bipolar LFOs for subtle or violent morphs; use external offsets to keep the modulation in the desired range.
    - The parameter knobs work as offsets; experiment with where you set them before applying CV.

- **Try the Reflect feedback loop**
    - Feedback external effects (distortion, filter, delay, bitcrusher, even another reverb!) via Reflect Send/Return for unhinged, chaotic echoes or metallic, endless ringing.

---

## Explore Further

Don’t forget: the Afterneath thrives on experimentation! Random voltage, audio-rate modulation, stepped CV, and combinations of internal and external feedback can turn any patch into a journey through wild, impossible spaces.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)