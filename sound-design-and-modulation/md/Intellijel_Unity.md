# Intellijel — Unity

- [Manual PDF](../../manuals/unity-mixer_manual_2020.04.15.pdf)

---

[**Unity Mixer Manual (PDF)**](https://intellijel.com/downloads/manuals/unity-mixer_manual_2020.04.15.pdf)

---

# Creative Sound Design with the Intellijel Unity Mixer

As a Eurorack modular synthesist, the Intellijel Unity Mixer is a powerful yet straightforward tool that can inspire creative sound design—especially when building distorted percussive sounds, aggressive basslines, or lush atmospheric pads. Below is an analysis focused on modulation and patching techniques that exploit the module's unique features.

---

## **Distorted Percussive Sounds**

### **1. Voltage Clipping & Signal Overload**
- The Unity Mixer sums incoming voltages up to a max of **10.5V**. Exceed this, and the output **clips**, resulting in a crunchy, distorted signal—perfect for punchy, distorted percussion.
- **Patching Tip:**  
  - Mix multiple envelopes, drum triggers, or audio signals with high amplitudes into a single mixer section.
  - Deliberately stack high-velocity or unattenuated envelope outputs from modules like Maths or Quadra.
  - Optional: Set both jumper(s) to unity gain (no attenuation), ensuring any signal over 10.5V gets hard-clipped.

### **2. Layering Percussive Elements**
- Patch several percussion sound sources (kick, snare, hats) into each mixer input.
- The summed output can act as a ‘parallel bus’ for further processing (into distortion, a wavefolder, or a compressor for extreme punch).
- For clean/dirty blends, use one side at -6dB and the other at unity, sending the same sources (split) and mix later with a crossfader/VCA.

---

## **Crazy Basslines (Dubstep/Drum & Bass)**

### **1. Complex CV Mixing**
- Take LFOs, envelopes, sequencer CVs, random voltages, and mix into the filter cutoff or oscillator FM input.
- With no individual level controls, combine extreme modulation depths for wild, constantly-shifting bass modulation.

### **2. Audio-Rate FM Madness**
- Sum several audio-rate signals (e.g., multiple VCO waveforms) to the FM input of a filter or oscillator, using Unity Mixer for clean, phase-correct summing.
- Pushing FM sum above 10.5V for “dirty” digital clipping artifacts—think metallic, spiky sounds often heard in neurofunk and modern bass music.

### **3. Sub + Harmonics**
- Mix clean sub (sine), with saw, pulse, or other harmonics (possibly after distortion or wavefolding) for massive, complex basses.
- Use -6dB jumper if your sources are hot, keeping the sound tight without clipping—OR run hot for intentional overdrive.

---

## **Haunting Atmospheric Pads**

### **1. Layer Modulation Sources**
- Merge multiple slow LFOs, random voltages, and envelopes to modulate filter cutoff, VCA, or effects parameters.
- This creates rich, evolving textures as subtle movement or chaos is continually blended.

### **2. Stereo Pathways (with Two Mixers)**
- Use each of the two Unity Mixer sections for left and right modulation paths.
- Feed slightly different modulation sources or levels to each, for organic stereo spread and motion.

### **3. Dynamic CV Crossfading**
- Patch several attenuated envelopes from modules like Quadratt or Triatt into the mixer, sum to a filter's FM input.
- Use as a “macro modulation” bus: global filter sweeps with many CVs, perfect for pads.

---

## **Bonus: Experimental Signal Pathways**

### **1. 6:1 Mixer Mode for Layering**
- Use the bottom output as a 6:1 mixer: stack six different sources.
- Layer six waveforms, drums, or modulations for extreme complexity.
- Patch “nothing” into output [4], sending it all to output [8].

### **2. Chained Attenuation for Sculpted Peaks**
- Enable -6dB attenuation for one or both mixers (per jumper) to tame surges
- OR deliberately double-attenuate then boost the output with a VCA, for different saturation characteristics.

---

## **Patching Examples**

**A. Distorted Percussion Bus**
```
Kick (high volume) --> In 1
Snare (moderate)   --> In 2
Clap (high)        --> In 3
Sum out (4): If >10.5V, will clip/distort for crunchy bus to compressor or reverb.
```

**B. Dubstep Bass Modulator**
```
LFO (audio rate)     --> In 1
Envelope (fast decay)--> In 2
Random voltage       --> In 3
Mix outs to VCO FM or filter for classic “wobble + chaos” basslines.
Boost levels past 10.5V if you want digital clipping razz!
```

**C. Haunting Pad Motions**
```
Very slow LFO          --> In 5
Slewed random (Woggle) --> In 6
Envelope (slow attack) --> In 7
Out (8) patches to filter cutoff, VCA, OR effects wet/dry for immersive pad morphing.
```

---

## **Extra Utility Tips**
- Since it’s DC-coupled, the Unity Mixer works with both audio and CV (unlike some mixers).
- No phase inversion means summed modulations remain “musically correct.”
- Experiment with using attenuators BEFORE the mixer for finely-tuned blends.

---

[**Unity Mixer Manual PDF**](https://intellijel.com/downloads/manuals/unity-mixer_manual_2020.04.15.pdf)

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
