# 2hp — MMF

- [Manual PDF](../../manuals/2hp_MMF.pdf)

---

[Download the MMF Module Manual (PDF)](https://www.tesseractmodular.com/uploads/1/0/9/6/109692205/mmf_manual.pdf)

---

## Using the Tesseract Modular MMF for Complex Rhythmic & Percussive Music Creation

The **Tesseract Modular MMF** is a 2HP analog multimode filter with low pass (LP), high pass (HP), and band pass (BP) outputs, featuring voltage-controlled cutoff (Freq) and resonance (Reso). Here’s how you can use it to sculpt hyper-complex, densely rhythmic percussion:

### Patch Ideas for Dense, Complex Percussion

#### 1. Multimode Output Exploitation
- **Parallel Percussion Routing:** Send a simple noise source, drum mix, or even a complex oscillator into the INPUT. Route LP, HP, and BP outputs to separate VCAs or mixers. Each output shapes the sound differently (LP for punch, HP for click, BP for snap), allowing you to craft layered percussive elements from one source.
- **Create Rhythmic Contrast:** Use each output in a different sequence or at different stages in your patch—eg., BP to a reverb for 'ghost notes,' LP for thuddy kicks, HP for sharp hats.

#### 2. Complex, Syncopated Filter Modulation

- **Tempo-Synced Modulation:** Patch sequencer or clocked modulation sources (like a random stepped LFO) into the FREQ and RESO CV inputs. To make this polyrhythmic, use multiple independent clock/divider or trigger sources in different time signatures (e.g., one modulator at 5/4, another at 7/8).
- **Euclidean Patterns:** Use a Euclidean or probability-based sequencer to send sharp envelopes or stepped voltages to FREQ, rhythmically opening and closing the filter. This can create rapidly shifting, complex percussive effects.
- **Modulate Resonance for Percussive Ping:** Use short envelopes or triggers in odd meter to the RESO input, so it rhythmically self-oscillates or rings in unique patterns.

#### 3. Percussive “Voice” Patch

- **Filter as a Drum Synth:** Ping the filter—patch a snappy, short envelope or a trigger directly to the AUDIO INPUT with little or no input signal. Adjust FREQ and RESO (and their CVs) for percussive blips, metallic hits, or synthetic toms. Modulate these with non-standard meters or polyrhythms for hyper-complex drum sounds.
- **Voltage-Controlled Timbre:** Combine parameter automation (from sequencers or LFOs in odd divisions) with fast FREQ/RESO modulation to morph between percussive timbres and rhythmic motion.

#### 4. FX and Signal Processing

- **Granular Percussion:** Process external drum loops or acoustic percussion, then modulate the filter with per-track envelopes or triggers in complex meters. Send the MMF’s outputs to delays/panners for even more rhythmic density.
- **Layer with Other Filters:** Parallel-process with other filters sequenced in different rhythmic subdivisions, then layer or crossfade for ultra-rich, syncopated results.

---

### Unique, Punchy, and Percussive Manipulation Tips

- **Filter Mod Depth:** Use attenuators/offsets or VCA control for FREQ/RESO CV-ins to ensure deep, punchy sweeps or sharp, fast filter movements for each trigger/gate in your sequence.
- **Dynamic CV Switching:** Use a sequential switch to rapidly cycle different modulation sources into FREQ/RESO for unique percussive movement.
- **Feedback Techniques:** Patch the BP or HP output back into the input through an attenuator—this can create wild self-oscillating percussion or snappy resonant effects.
- **Dynamic Wet/Dry:** Crossfade between raw and filtered signals in time with your sequenced patterns for “ghost” echoes, evolving fills, or stutter effects.

---

**Manual Reference:**  
- *Freq* accepts -8V to +8V for cutoff sweeps.
- *Reso* accepts -5V to +5V for resonance sweeps.
- All outputs are simultaneously available, making parallel processing easy.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)