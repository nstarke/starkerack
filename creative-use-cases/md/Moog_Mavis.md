# Moog — Mavis

- [Manual PDF](../../manuals/MAVIS_MANUAL_V2_06.27.2022.pdf)

---

[Download the Moog Mavis User Manual (PDF)](https://www.moogmusic.com/sites/default/files/2023-05/Moog%20Mavis%20Manual%20v2.0_0.pdf)

---

# Creative Eurorack Patching Ideas with the Moog Mavis

The Moog Mavis is a highly flexible analog semi-modular synth that seamlessly integrates into Eurorack systems. Here are some creative ideas for using Mavis as part of a modular setup, based on its manual and unique feature set:

## 1. **Mavis as a Harmonic Modulator/Processor**
- **Wavefolder as a Flavor Tool:** The built-in wave folder is unique in the Moog lineup. Try patching external sound sources (oscillators, drum sounds, or entire mix stems) into the FOLD IN (Wavefolder input) for analog flavor and added harmonics. Adjust the FOLD knob or modulate it with an LFO or envelope for evolving textures.
- **Recommended Pairings:** Use with a complex oscillator (e.g., Make Noise DPO, Endorphin.es Furthrrrr Generator), percussive sources, or spoken word samples for aggressive timbral shaping.

## 2. **Utility Mixer and Attenuator for Creative Routing**
- **ONE+TWO Mixer:** Use this as a handy submixer for combining CV or audio. Try mixing two mod sources (like LFO + random) before sending to a parameter on another module.
- **Attenuator:** Tame hot CV signals from other “loud” Eurorack modules before feeding into the Mavis or vice versa.

## 3. **Mavis as a Second (or Modulation) Oscillator**
- **Audio Rate LFO Trick:** With its LFO able to reach audio rates (up to 550Hz), Mavis can double as a voice in an FM patch. Send audio-rate LFO out to another VCO’s FM input for classic FM clang or metallic tones.
- **Sync Opportunities:** Patch gate or clock signals into the LFO RATE input for tempo-synced effects, or use the VCO as a steady modulator for other gear.

## 4. **Sample & Hold Magic**
- **Random CV Generation:** Use the built-in Sample & Hold, sourcing the VCO (preferably a ramp/saw for wider voltage spread) and clocking it from a rhythmic LFO or external clock. Send the output to filters, oscillators, or effects modules for stepped randomness.
- **Custom Sourcing:** Patch a different random or chaotic CV source (e.g., Joranalogue Compare 2, Mutable Instruments Marbles) into S+H IN for tailored randomness.

## 5. **Filter & VCA as High-Quality Processing**
- **External Signal Filtering:** Use Mavis’ classic Moog ladder filter to process drums, external oscillators, or noisy field recordings. Modulate cutoff with the EG for dynamic sweeps or from external CV for unique filter motion.
- **Dynamic Control:** Patch other envelopes (e.g., Make Noise Maths, Intellijel Quadra) or LFOs into VCA CV input for level automation or tremolo effects.

## 6. **Patchbay for Modular Interplay**
- **MULT Outputs:** Split control voltages to send keyboard, LFO, or S&H signals to several destinations within your rack: pitch, filter, modulation, etc.
- **Feedback/Resonance Loops:** Try routing VCA or VCF outputs into external delays, distortion, or reverb, and then back into the Mavis’ wavefolder or VCF for feedback and dubby soundscapes.

## 7. **Mavis as a Standalone Voice for Sequencing**
- **Sequencer Control:** Use a Eurorack sequencer (e.g., Make Noise 0-CTRL, Arturia Keystep Pro, or any CV/gate sequencer) to play the Mavis by patching Pitch CV to 1V/OCT and Gate to GATE in. Layer Mavis with other modular voices for polyphonic or duophonic textures.

## 8. **Eurorack Drum Processing**
- **Drum Overdrive:** Patch drum machine or modular drum module outs into the FOLD IN and/or VCF. Use the envelope follower output of a module (like Mutable Instruments Ears) to modulate the filter or fold amount for dynamic response.
- **Glitch Textures:** Send high-speed random CV from Mavis’ S&H to trigger or modulate percussive voices (Hexinverter Mutant Drums, Noise Engineering Basimilus Iteritas Alter).

## 9. **Drone and Ambient Generation**
- **Self-oscillation:** Crank resonance on the filter for sine-based drones; modulate with Mavis’ EG or an external LFO for ambient sweeps.
- **Glide and Scale:** Use the Glide and KB Scale for portamento effects and microtonal experimentation when controlling other gear.

## 10. **Creative Modulation Source**
- **Envelope, S&H, and LFO Outputs:** Patch any of these to control other modules in your system. For example, send EG out to modulate the decay time on a reverb, or S&H to a wavetable position on a digital oscillator.

---

### Some Module Type Recommendations for Expanded Patching:

- **Complex Oscillator:** For advanced FM and cross-modulation (DPO, BIA, Furthrrrr).
- **Digital Noise/Random Source:** For richer S&H patterns (Mutable Marbles, SSF Ultra-Random Analog).
- **Multi-Mode Filter:** Parallel processing with Mavis filter (WMD C4RBN, Intellijel Polaris).
- **Stereo/Spatializer Effects:** Mavis only outputs mono—add a stereo reverb (Happy Nerding FX Aid, Make Noise Mimeophon) downstream for immersive results.
- **Sequencer/Controller:** For hands-off melodic duties (Make Noise 0-CTRL, Intellijel Metropolix).
- **Envelope Followers/Comparators:** For dynamic or gated interaction with external audio (Mutable Ears, Joranalogue Compare 2).

---

## Bonus: Patching Shortcuts

- Use Mavis’ built-in MULTs to distribute random or mod CV across your rack without using up valuable passive multiples.
- With ONE LVL knob, offset signals coming from other modules—great for fine-tuning pitch or filter CVs.

---

Explore, experiment, and have fun breaking signal paths! Mavis is as much a source as a processor and utility hub, gifted for hybrid east-coast and west-coast synthesis approaches.

---
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)