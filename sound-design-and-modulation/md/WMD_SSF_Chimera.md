# WMD SSF — Chimera

- [Manual PDF](../../manuals/Manual_v1.2.pdf)

---

[**WMD Chimera Metallic Percussion Synthesizer Manual (PDF)**](https://wmdevices.com/pages/support)

---

# Creative Modulation Techniques for the WMD Chimera Eurorack Module

The WMD Chimera is a flexible metallic percussion synthesizer, capable of everything from sharp, metallic hits to deep, shifting atmospheres. Below are some techniques and patch ideas to create **distorted percussive sounds**, **crazy basslines**, and **haunting atmospheres**, leveraging external modulation sources (e.g., LFOs, envelopes, sequencers, other modules).

---

## 1. Distorted Percussive Sounds

- **Density & Decay Modulation**:  
  Patch a fast random voltage or stepped LFO into the DENSITY CV to vary grain count per trigger dynamically. Modulate DECAY with an envelope output tied to a rhythm source, allowing each hit to have different decay lengths.
- **Surface Type Scanning**:  
  Use a slow LFO or a sequence to scan the SURFACE CV, morphing between metallic textures with every hit.
- **FX and FX AMT Crush**:  
  Modulate FX AMT with a fast square or random LFO and set FX to quality or sample rate reduction mode for digital distortion. Try turning FX comb filtering on and use an envelope to sweep FX AMT for wild flanging metallic distortions.
- **Choke Input for Glitchiness**:  
  Trigger the CHOKE input with offbeat pulses or a clock divider to force abrupt cuts—ideal for choppy, glitchy percussive breaks found in IDM, breakcore, and distorted techno.
- **Accent Pulses for Crunch**:  
  Use a trigger sequencer to send accents on selected steps, pushing the module into harder, almost clipping percussive transients.

## 2. Basslines for Dubstep & Drum & Bass

- **PITCH Mod Sequencing**:  
  Use a CV sequencer to modulate PITCH in bass line patterns. Its 5-octave span makes deep subs and clangorous mids possible, especially when combined with high DENSITY and short DECAY.
- **Envelope Pitch Decay (Wobble Effect)**:  
  Modulate the ENVELOPE amount with a synced LFO so pitch bends with each step—set to negative for disorienting Doppler bends or positive for classic video-game laser sweeps. For true "wobble bass," sweep pitch envelope and FX/filter parameters in tandem.
- **Haunted Overdriven Bass**:  
  Bring in external overdrive/distortion after the Chimera output for additional bass growl. Feed the VCA input with a modulated envelope for dynamic amplitude ducking in time with your kick or snare.
- **Comb Filter FX for Zappy Bass**:  
  Route a fast, envelope-shaped modulation to the FX AMT input in comb mode. This will notch the harmonics in moving patterns, reminiscent of zappy, bass-textured DnB sounds.

## 3. Haunting Atmospheric Pads

- **Maxed Density & Decay for Textures**:  
  Set DENSITY and DECAY high for long, shimmering washes. Patch a slow, smooth LFO to DECAY or SURFACE to make the pad morph over time.
- **Surface Morph Modulation**:  
  Use a sample-and-hold or random LFO to automate moving through different SURFACE types, creating eerie, ever-changing metallic tones.
- **Unquantized Pitch Drones**:  
  Send a slowly changing CV (using a random smooth LFO) to PITCH. Combine with occasional pitch envelope modulation for organic, otherworldly drift and detuning.
- **Self-Oscillating FEEL Mode for Generative Textures**:  
  Use the last FEEL mode for unpredictably unique textures with each trigger. With DECAY at max, the sound stretches out for endless droning metallic atmospheres.
- **FX Modulation for Haunt**:  
  Slowly modulate FX AMT (in digital reduction or comb mode) for shimmering, spectral artifacts.

---

## Input Modulation Suggestions

- **LFO to PITCH/FX AMT:** Add vibrato, metallic flutter, or comb filter movement.
- **Random or S&H to SURFACE:** Textural movement over time.
- **Envelope to DECAY/DENSITY:** Rhythmic dynamic changes for evolving hits or pads.
- **Rhythm Triggers to ACCENT/CHOKE:** Create unpredictable rhythmic structures.

### Pro-Tip: Chain the Chimera into a granular or reverb module after for even more spectral pad ambience or menacing percussive spaces.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
