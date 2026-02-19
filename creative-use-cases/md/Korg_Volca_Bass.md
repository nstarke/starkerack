# Korg — Volca Bass

- [Manual PDF](../../manuals/Korg-Volca-Bass_manual.pdf)

---

[Download the Korg Volca Bass Manual (PDF)](https://cdn.korg.com/us/support/download/files/d1e7d195049fd25301b82e3b9b7c4c90.pdf)

---

# Creative Eurorack Patch Ideas Using the Korg volca bass

The Korg Volca Bass is a portable, analog bassline groovebox with 3 VCOs, 1 VCF, 1 VCA, EG, and LFO. While not a "true" Eurorack module, the Volca Bass can be easily interfaced with modular synths via MIDI, audio, and sync connections. Here are some patching ideas and module combinations to maximize creative potential with the Volca Bass in your modular system:

## 1. _Analog Sync for Rhythmic Precision_

**Idea:**  
Use the Volca Bass’s SYNC IN/OUT jacks to synchronize its sequencer with your modular rig. This lets you lock Volca sequences to Eurorack triggers.

**How:**
- Connect SYNC OUT from Volca Bass to a clock divider (e.g., 4ms Rotating Clock Divider) or a trigger sequencer.
- Send that divided or transformed clock into further Eurorack modules, e.g., drum sequencers or clocked effects.

**Result:**  
Synchronized basslines tightly integrated with modular rhythmic structures.

---

## 2. _Resampling and Wave Shaping with Modular FX_

**Idea:**  
Treat the Volca Bass as a sound source and process its output through modular effects, waveshapers, or filters.

**How:**  
- Patch the Volca’s headphone/audio out into a Eurorack input module (e.g., Intellijel Audio Interface II or Befaco Instrument Interface).
- Route that signal into a waveshaper/folder (e.g., Tiptop Fold Processor, Serge Wave Multiplier) for timbral roasting.
- Further sculpt with a Eurorack VCF and modulate with modular envelopes or LFOs (make manual filter sweeps for dubby effects).

**Result:**  
Growling, saturated, or broken-volca timbres far beyond the onboard filter.

---

## 3. _Volca LFO as Modulation Source for Eurorack_

**Idea:**  
Use the Volca’s LFO, which can be synced to its EG/trigger, to modulate modular parameters.

**How:**  
- Take the audio output, filter for just the LFO range (Bandpass or Envelope Follower/Comparator module), and repurpose as a CV source to modulate other modules.

**Result:**  
Pseudo-random or musical modulation, synced with your Volca sequences, affecting Eurorack filters, VCAs, or even tempo.

---

## 4. _Sequencer Paraphony: Oscillator Voice Splitting_

**Idea:**  
Volca Bass allows the three VCOs to be controlled separately (FUNC+STEP 1/2/3 for grouping). This can be creatively routed:

**How:**  
- Sequence the VCOs paraphonically (bass, lead, and faux chord) and route Volca’s output through a modular auto-panner (e.g., Make Noise Rosie), sending different VCO groupings to different effects or speakers.
- Use MIDI-to-CV (e.g., Mutable Yarns, or Expert Sleepers FH-2) to have a Eurorack sequencer (like the Varigate 4+) control note data sent to the Volca via MIDI for complex, evolving voltages.

**Result:**  
Advanced stereo imaging, multilayered bass, or even generative patterns, integrating Volca’s character into modular voicing.

---

## 5. _Triggering Modular Actions from Volca Playback_

**Idea:**  
Leverage Volca’s sequencer playback to trigger modular events.

**How:**  
- Run Volca SYNC OUT to a gate/logic processor (e.g., Doepfer A-166 Dual Logic) to generate gates or triggers that can ping function generators (Make Noise Maths, Mutable Stages).
- Use these events to launch envelopes, sequencers, or Euclidean rhythm generators, turning Volca rhythm into modular patch control.

**Result:**  
Dynamic live sets where Volca pattern changes reorder your modular rhythms and textures in real time.

---

## 6. _Volca Into Utility Modules for External MIDI Control_

**Idea:**  
Use Volca as a CV or MIDI master clock device—thanks to its MIDI IN port, you can synchronize modular and external gear.

**How:**  
- Use a MIDI-to-CV module to let a hardware DAW or modular sequencer control Volca Bass.
- Conversely, use the Volca as a clock master for modular performance using MIDI Thru devices.

**Result:**  
Jamming or composing with everything in clocked harmony—sequenced melodic basslines on Volca, complex rhythms and textures from the modular world.

---

## 7. _Layer with Inspire Polyphony Using Multiple Volcas and Modular_

**Idea:**  
Use multiple Volca units and layer their outputs via a Eurorack stereo mixer or quad VCA (e.g., Intellijel Quad VCA, Befaco Hexmix), mixing processed and dry signals.

**How:**  
- Sync multiple Volca Bass/Keys/Drums using SYNC IN/OUT.
- Run their outputs into the modular for live mixing/effects insertion, and route LFOs/envelopes for dynamic control.

**Result:**  
Deep, multi-layered sounds—Volca voices as evolving submixes, spilling into the modular universe for performance.

---

## Bonus: **Recommended Modules for Experimentation**
- **Clock Dividers and Logic:** 4ms RCD, Doepfer A-160/A-166
- **Audio Interfaces:** Befaco Instrument Interface, Intellijel Audio Interface II
- **Filter/waveshaper:** Bastl Timber, Dan & Dan DSQ-1, Tiptop Fold Processor
- **Envelope Followers:** Mutable Instruments Ears, Doepfer A-119
- **VCAs and Stereo Mixers:** Intellijel Quad VCA, Befaco Hexmix
- **Effects:** Erica Synths Fusionbox, Make Noise Mimeophon, Strymon Magneto
- **MIDI-to-CV:** Mutable Yarns, Expert Sleepers FH-2, Arturia Keystep Pro (outside rack)

---

With these ideas, the Volca Bass becomes more than just a groovebox—it can function as a powerful, patchable engine within your modular ecosystem.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)