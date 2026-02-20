# Noise Engineering — Sec Ruina

- [Manual PDF](../../manuals/Seca Ruina - Noise Engineering Documentation.pdf)

---

[Seca Ruina Manual PDF](https://manuals.noiseengineering.us/sr/)

---

# Creative Modulation Techniques for Noise Engineering Seca Ruina
The Seca Ruina is a compact 6HP multiband distortion module for Eurorack, splitting your input into three frequency bands—high, mid, and low—with independent drive controls, CV inputs, and individual outputs. It also features a universal drive CV and an onboard VCA. This makes it ideal for sculpting complex timbres, wild modulations, and thick percussive and atmospheric tones.

Below are patch ideas and modulation strategies tailored to producing **distorted percussion, crazy basslines, and haunting pads**.

---

## 1. **Distorted Percussive Sounds**

### Technique
- **Input Source**: Feed short, punchy sounds (drum modules, samples, or percussive synth stabs) into the **In** jack.
- **CV Modulation**:  
  - Patch an envelope (from your drum trigger) into the **Sum CV input**. This will turn the Seca Ruina into a VCA, shaping both amplitude and drive.  
  - For extreme effects, patch separate envelopes or fast LFOs into the **High, Mid, and Low CV inputs** to vary the drive amount per band as the drum hits.
- **Knob Tweaking**: Start with one or more bands set to high drive; adjust the bands for desired crunch.
- **External Processing**: Take the **individual band outputs** and treat each band separately (e.g., adding reverb to the highs, bitcrushing the mids, or saturating the lows).

### Results
- Tunable drive and punch per frequency region.
- Rhythmic distortion “envelopes” that evolve with each hit.
- Individual bands can be further processed—for example, overdriven highs with filtered, clean lows.

---

## 2. **Crazy Dubstep/Drum & Bass Basslines**

### Technique
- **Input Source**: Use a complex oscillator (e.g., Loquelic Iteritas or a classic subtractive voice) for rich harmonics.
- **CV Modulation**:
  - Patch intense, synced LFOs or sequenced CVs (sample & holds, stepped voltages) into the **Low and Mid drive CVs**.  
  - For "talking" basses, send envelopes or fast, random LFOs into the **High band drive** for occasional extra sizzle.
  - Use the **All drive CV** for envelopes tied to accent triggers or for wobble movement.
- **Performance**: Tweak drive knobs as you play to morph tone and aggression.
- **Splitting**: Use the individual band outs. Route the lows through a compressor, mids through phaser/flanger, and highs through an exciter or delay.

### Results
- Basslines that grind, wobble, and “talk.”
- Hits on different beats produce different distortion textures by CV-automating drive per band.
- Layered, multi-band distortion with external effects for rich, modern bass textures.

---

## 3. **Haunting Atmospheric Pads**

### Technique
- **Input Source**: Use chordal samples, lush synth pads, or drones.
- **CV Modulation**:
  - Patch smooth, very slow LFOs or fluctuating random voltages to the **High, Mid, and Low drive CVs** for gentle, evolving distortion character shift.
  - Subtle modulation of the **Sum drive CV** with a slightly slower LFO for breathing dynamics.
- **Interface**: Keep drive knobs at moderate to low settings for subtle harmonic movement.
- **Output Processing**: Take the **Sum out**, and run it through vast reverbs, delays, or granular processors for cinematic spaciousness.

### Results
- Pads with subtle, spectral motion and unpredictable harmonic changes.
- "Ghostly" textures as the bands interact and distort artifacts shift in and out of the mix.
- Can control harshness/intensity by dialing in more drive or speeding up LFOs for more agitation.

---

### Additional Tips

- **Dynamic CV Control**: Because Seca Ruina’s CV ins are 0–5V, you can use a sequencer or controller to swap between soft, rich, and abrasive textures in real-time.
- **Patch Example**: For hyper-detailed control, send CV from a sequencer to each band, and random gates to the “All” input, letting rhythms shift and morph unpredictably.
- **Live Tweaks**: Hands-on tweaking while modulating with CV gives an organic, performance-verifiable result—perfect for live improvisation or wild sound design.

---

For more technical details or inspiration, check out the full manual:
[Seca Ruina Manual PDF](https://manuals.noiseengineering.us/sr/)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)