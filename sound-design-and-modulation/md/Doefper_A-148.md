# Doefper — A-148

- [Manual PDF](../../manuals/A148_man.pdf)

---

[Download Doepfer A-148 Dual S&H Manual (PDF)](https://doepfer.de/a100man/A148_man.pdf)

---

# Creative Modulation Techniques for the Doepfer A-148 Dual S&H

The **Doepfer A-148 Dual Sample & Hold (S&H)** module is an incredibly versatile component for sculpting evolving, unpredictable, and dynamic voltages. With the 2005 revision, the option to set each half to S&H or T&H (Track & Hold) mode opens up even more sonic possibilities. Here’s how you can push this humble module for **distorted percussion**, **crazy basslines**, and **atmospheric pads** in your Eurorack system.

---

## 1. Distorted Percussive Sounds

### A. Sample Noise with Fast/LFO Triggers

- **Patch white or pink noise** (e.g., from Doepfer A-118) into the S&H input.
- **Mult a gate signal from a sequencer or drum module** to the Trigger input.
- **Take S&H Out to your VCA/Filter/Distortion**, then to audio out.

**Result:**  
Each trigger “samples” a unique noise slice—great as a percussive click, snare, or hi-hat. Add a distortion module or wavefolder after the VCA for gritty drum hits.

**TIP:**  
Modulate **Trigger input speed** with bursts/LFOs for machine-gun–like or randomized percussive patterns.

### B. T&H for Glitchy Envelopes

- Set one half of the A-148 to **Track & Hold** mode using the internal jumper.
- **Patch a fast, modulating signal** (like a crazy-wobbly LFO) to S&H In.
- **Hold briefly with short gates or audio-rate triggers** for stuttering, data-moshed envelopes.
- Feed this to a VCA’s CV, post-distortion.

---

## 2. Crazy Basslines (Dubstep/Drum & Bass)

### A. S&H on LFO for Stepped Wobble

- LFO (triangle/saw) into S&H Input.
- External clock (MIDI clock or sequencer gate, odd Euclidean rhythm, etc) to Trigger In.
- S&H Out to VCO pitch or VCF cutoff.

**Result:**  
Unique, stepped basslines and evolving filter sweeps with syncopation.

**Further Mangling:**
- Patch a heavily resonant filter (set nearly to self-oscillation) after this, and modulate cutoff with the S&H output for “formant” filtering.
- Add *FM* from S&H Out to secondary oscillator(s)—chaotic, metallic, and aggressive sounds.

### B. Layered Dual-Mode Bass

- Use both S&H halves:  
    - Upper in S&H, lower in T&H.
    - Trigger both with different clocks/resets for cross-rhythms.
- First output modulates VCO pitch. Second output modulates filter or waveshaper depth for morphing/distorted timbres.

---

## 3. Haunting Atmospheric Pads

### A. S&H with Slow Noise for Textures

- Slow random voltage/noise into S&H Input.
- Gentle, irregular triggers (West Coast-style events, or clock divisions) to Trig In.
- S&H Out blended into a filter’s cutoff or oscillator FM amount on a slow pad.

**Result:**  
Ghostly, shimmering atmospheres that meander and evolve unpredictably.

### B. Modulate Delay or Reverb Parameters

- Use S&H Out to modulate *CV-able* reverb/delay depth, time, or feedback.
- Try splitting the S&H Out to both pitch and filter CVs for subtle drifting intonation.

---

## BONUS: General Tips

- **Stacked Randomness:**  
  Chain multiple S&H modules, or bounce the output through slews (A-170) to smooth steps for portamento glides or wonkier modulations.
- **Feedback Loops:**  
  Plug the output back into another modulation source (like a VCO or noise generator), or self-patch for unpredictable behaviors.
- **LED Visuals:**  
  Use the onboard LEDs to monitor voltage states quickly when patching complex feedback/randomness setups.

---

## Further Reading & Experiments

- Try clocking S&H with **audio-rate oscillators** for bitcrush/decimation-type effects (sample rate reduction), especially on envelope or filter CV paths.
- Use the new -12V...+12V range for high-headroom, dramatic modulations.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)