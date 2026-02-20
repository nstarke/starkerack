# Bubblesound — HexVCA

- [Manual PDF](../../manuals/bubblesound.pdf)

---

[HEXvca Manual PDF](https://www.bubblesound-instruments.com)

---

# Creative HEXvca Modulation Techniques for Unique Synth Sounds

## Overview

The HEXvca by Bubblesound is a versatile 6-channel voltage controlled amplifier (VCA) module with both linear and exponential response options, normalized CV paths, and flexible mixing capabilities. This makes it especially well-suited for crafting precise modulation, dynamic mixing, and audio/CV interfacing—perfect for the dynamic, aggressive, and atmospheric sounds found in modern electronic music. Below you’ll find patching and modulation techniques targeting:

- **Distorted Percussive Sounds**
- **Dubstep/Drum & Bass Basslines**
- **Haunting Atmospheric Pads**

---

## 1. Distorted Percussive Sounds

#### Classic Drum Machine Punch with Overdrive Flavor

- **Audio Input**: Feed drum/click samples, short synth hits, or external audio sources into one or several VCA inputs.
- **CV Source**: Patch sharp, snappy envelopes (e.g., Maths, Function, or simple Attack/Decay EGs) into the CV inputs.
- **Exponential/Linear Response**: Set the channel’s CV mode to **Exponential** for more punch and “snappy” volume shape.
- **Normalization**: Use input normalization (set via rear jumpers) so one envelope can simultaneously control multiple VCAs for layered transients.
- **Internal Mixing & Distortion**: Take the summed output from 1–3, 4–6, or 1–6 and send to a wavefolder, overdrive, or external distortion module.  
  - **Tip:** Use a hot input level to push the SSM2164 into gentle saturation, or boost output via a mixer for analog “grit.”

---

## 2. Dubstep/Drum & Bass Basslines

#### Growling, Rhythmic Modulation and Multi-Layered Bass

- **Audio Input**: Route up to 6 saw/square/triangle waveforms (from several VCOs or a complex VCO with multiple outs) into the VCA inputs.
- **CV Source**: Use LFOs, sequenced stepped voltages, and envelope followers for dynamic movement.
  - **Fast LFO:** For classic “wobble”. Try shapes like triangle, sine, ramp for different feels.
  - **Steppy/Random CV:** Patch sample & hold, or sequencer outputs for unpredictable modulation.
- **Mixing**: Use the group outs (1–3, 4–6) to split bass layers for separate processing (e.g., one group to a lowpass filter for sub, another to a comb filter for mid/top end).
- **Morph Uniquely**: Use the hex VCA’s normalization to apply one moving LFO across many VCAs for polyrhythmic “multi-wobble” effects.
- **Exponential Response**: For maximum movement and punch.

---

## 3. Haunting Atmospheric Pads

#### Layering, Dynamic Envelopes, and Evolving Textures

- **Audio Input**: Fill each VCA with a different drone or wavetable oscillator—subtle detuned intervals add depth.
- **CV Source**: Use ultra slow envelopes, random LFOs, or even a looping attenuated envelope generator to control each VCA.
  - **Linear Response:** Keeps volume transitions smooth and ambient.
  - **Normalization:** Assign one looping envelope to multiple VCAs for gentle, synchronized swells.
- **VCAs for CVs**: The HEXvca is DC-coupled, so patch slow LFOs or random CV through VCAs to modulate other modules, making the soundscape evolve organically.
- **Mix Output**: Summed outputs are perfect for a lush, layered sound sent to reverbs and delays.

---

## Additional Tips

- **Use with HEXar**: If you own a HEXar, connect via the included ribbon cable for playability without patch cables—ideal for live tweaking.
- **Patch Feedback**: Route some mix output through effects and back to an input for wild, self-oscillating textures.

---

## Conclusion

The HEXvca shines as a flexible hub for amplitude modulation and mixing in your eurorack system. Creative use of its normalization, mix architecture, and CV modes opens up sophisticated sound design with minimal patching—perfect for anybody producing aggressive bass music or lush soundscapes.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)