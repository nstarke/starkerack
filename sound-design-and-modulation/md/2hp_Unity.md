# 2hp — Unity

- [Manual PDF](../../manuals/2hp_Unity.pdf)

---

[Unity Mixer Manual (PDF)](https://2hp.com/wp-content/uploads/Unity_Manual.pdf)

---

# Creative Modulation Techniques with the Unity Mixer

The **Unity** is a compact, dual-channel utility mixer by 2hp, with three flexible modes: Averaging, Unity, and Split. By taking advantage of its normalling, summing, and mode functions, you can generate complex, expressive, and even *unhinged* modulation for a variety of wild sound design objectives. Below are techniques tailored to:

- **Distorted Percussive Sounds**
- **Dubstep/Drum & Bass Basslines**
- **Haunting Pads and Textures**

---

## 1. Creating Distorted Percussive Sounds

**Goal:** Fuse envelopes, noise, and audio-rate CV in ways that clip, fold, and punch through a mix.

**Patch Ideas:**
- **Audio-rate Mixing:**  
  *Patch three short envelopes (from different EGs or drum modules), or mix a snappy envelope, a noise source, and an audio-rate oscillator (square wave works well) into the top three inputs.*
  - Set the **Mode Toggle** to **Averaging** or use **Split Mode** if wanting three audio signals summed and balanced in loudness.
  - Overdrive** downstream modules (VCAs, filters, distortions) using the summed output—mixed transients can create punchy, complex percussion, especially when levels sum to clipping.
- **Stacked Percussive Textures:**  
  Use the normalling feature: leave Out 1 unpatched and patch additional percussion triggers or audio into the lower mixer. The merged signal at Out 2 can be fed into a distortion pedal, wavefolder, or wave rectifier for brutal, textural timbres.

> **Tip:** Mix envelope and drum signals at *unity gain* for maximum gain-staging into waveshapers; use *averaging* to keep the mix tight and less “blown out.”

---

## 2. Crazy, Animated Basslines (Dubstep/Drum & Bass)

**Goal:** Animate a bass voice with multiple modulation sources for rhythmic, morphing, and unpredictable movement.

**Patch Ideas:**
- **Wobble Source Mixer:**  
  Mix multiple LFO shapes (triangle, saw, stepped random) into a single animated CV for controlling a VCF or waveshaper cutoff. **Unity Mode** is perfect here—the summed result produces wild, evolving filter or FM movement.
- **Dual-Mode Signal Animation:**  
  Use **Split Mode:** top mixer for LFOs/envelopes to modulate *one* filter, bottom for audio-rate oscillators or audio-CVs (ringmod outputs, subosc) to modulate a *second* filter or VCA. Crossfade between the two for evolving, gnarly “talking” basslines.
- **Serial CV Distortion:**  
  Mix a slow envelope, audio-rate oscillator, and noise into the same mixer at **unity gain**; the resulting sum can have unpredictable spikes and artifacts, perfect for driving bass distortion or modulation FX.

> **Tip:** Sending summed modulation to *both amplitude and filter* (via separate VCAs/VCFs) will create basses that “snarl,” “growl,” or “stutter” like those in high-energy electronic genres.

---

## 3. Haunting Atmospheric Pads

**Goal:** Build deep, shifting pads and textures via serial modulation and subtle signal blending.

**Patch Ideas:**
- **CV Texture Mixer:**  
  Mix two or three slow LFOs or looping envelopes with subtle differences into one mixer. In **Averaging Mode**, the slow modulations gently undulate—patch this to the mod input on a large reverb, delay time, or wavetable position for pads that shimmer and drift.
- **Mix Audio into Modulation:**  
  Use **Split Mode:** in the top mixer, blend LFOs/envelopes; in the bottom, blend faint audio signals (sine or triangle waves) to quietly modulate effect parameters (e.g., reverb decay, filter resonance). The interaction between audio and CV sources introduces ghostly, complex modulation patterns.
- **Chaining Mixing for Massive Mod Sources:**  
  Leave first output unpatched so signals from both mixers are combined at Out 2. Use the 6-to-1 function to sum a variety of random, audio, and LFO modulation sources for huge, evolving macro-modulation.

> **Tip:** Smoothing the output from the Unity mixer (with a slew/lag processor or lowpass filter) can turn even sharp, stepped sources into ethereal, morphing pad movements.

---

## Additional Creative Tricks

- **Feedback Mixer:**  
  Mult an output (e.g., from an effects module) back into one of the mixer inputs—tiny adjustments create howling, chaotic feedback textures. Use the **Averaging** mode to tame the feedback.
- **CV Controlled Dry/Wet:**  
  Use two mixers—one for dry, one for wet signal—and toggle between them with the Mode Switch. Patch the summed output to a VC crossfader for smooth, automatable blending.

---

## Reference

- [Unity Mixer Manual (PDF)](https://2hp.com/wp-content/uploads/Unity_Manual.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

*Explore, experiment, and patch wildly!*