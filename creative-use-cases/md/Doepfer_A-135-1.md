# Doepfer — A-135-1

- [Manual PDF](../../manuals/A135_man.pdf)

---

[**Download the Doepfer A-135 VC-Mixer Manual (PDF)**](https://doepfer.de/a100man/A135_man.pdf)

---

# Creative Patch Ideas for Doepfer A-135 VC-Mixer

The Doepfer A-135 is a four-channel voltage-controlled mixer, each channel equipped with its own VCA under linear CV control, plus per-channel gain and CV amount. Here are some creative ways to use it with other Eurorack modules, taking full advantage of its structure and flexibility:

---

## 1. **Animated Quad Panning Mixer**

- **Modules Needed:**  
  - A-135 VC-Mixer  
  - 4x Audio Sources (Oscillators, Sample Players)  
  - Quad LFO (e.g., Doepfer A-143-3 or Batumi)  
  - Output Module

- **Patch Idea:**  
  - Patch four different audio sources into the four A-135 Audio Ins.
  - Use each channel’s CV input for modulation from a separate output from the Quad LFO.  
  - Tweak each LFO’s speed and waveform.  
  - Result: The four audio sources fade in and out rhythmically. Sum output to stereo/mono for randomized, evolving textures.

---

## 2. **Quad Envelope-Controlled Mixing for Morphing Sounds**

- **Modules Needed:**  
  - A-135 VC-Mixer  
  - 4x Envelope Generators (e.g., Doepfer A-140)  
  - 4x Sound Sources (or filters with different characteristics)

- **Patch Idea:**  
  - Run four different timbres into the A-135 inputs.
  - Each envelope generator controls one VCA via ext. CV.
  - Trigger all envelopes together to morph through different sources with complex amplitude shapes.
  - Pro Tip: Try different envelope speeds/shapes or retriggering methods for dynamic timbre transitions.

---

## 3. **MIDI-Controlled Mixer (Performance Morph Mixer)**

- **Modules Needed:**  
  - A-135 VC-Mixer  
  - MIDI-to-CV interface (e.g., Doepfer A-190-4)
  - MIDI controller or sequencer

- **Patch Idea:**  
  - Map MIDI control changes (mod wheel, aftertouch, etc.) to the A-135’s CV ins via the MIDI-to-CV's multiple outputs.
  - Assign each CC to a different channel’s VCA.  
  - Perform dynamic mixing, muting, or morphing from a MIDI keyboard or controller.

---

## 4. **CV-Controlled Drum Mixer with Randomization**

- **Modules Needed:**  
  - A-135 VC-Mixer  
  - Drum Modules or Samplers  
  - Random CV/Noise Source (e.g., Doepfer A-118, Wogglebug)  
  - Clock Divider (e.g., Doepfer A-160)

- **Patch Idea:**  
  - Patch drum hits into inputs.  
  - Send random stepped CVs (sample/hold or quantized random) to the channel CVs.
  - Use a clock divider to trigger fresh random CV values.
  - Output: Unpredictable, constantly remixing drum patterns or textures. Tweak random CV depth and gain for subtle to extreme mixes.

---

## 5. **Stereo Morphing or Crossfader**

- **Modules Needed:**  
  - A-135 VC-Mixer  
  - Doepfer A-144 Morph Controller  
  - 2x or 4x Oscillators/Audio Sources  
  - Dual Outputs (for stereo)

- **Patch Idea:**  
  - Use the A-144 to generate four related CVs from one knob/CV input—patch these into the four channel CVs.
  - Connect different sounds to the mixer inputs.
  - The A-144’s morph control will smoothly fade/morph through the four inputs, creating a single-knob or single-CV “morph” across timbres. Use for stereo morphs, evolving pads, or scene crossfading.

---

## 6. **Ring Modulation/LFO Audio-Rate AM**

- **Modules Needed:**  
  - A-135 VC-Mixer  
  - 4x Sound Sources (or noise/sample players)  
  - 4x Audio-rate Modulators (Oscillators or fast LFOs)

- **Patch Idea:**  
  - Patch your audio sources to inputs, and use other oscillators running at audio rate as CV sources.
  - This effectively does amplitude modulation/ring modulation on each input—great for metallic, clangorous, or FM-like effects.
  - Try mixing regular CV and audio-rate CV for even more complex modulation.

---

## 7. **DAW-like Automation via Sequencer**

- **Modules Needed:**  
  - A-135 VC-Mixer  
  - CV Sequencer (e.g., Doepfer A-155, Make Noise Pressure Points)
  - Several audio sources

- **Patch Idea:**  
  - Send different channels of your sequencer to the mixer’s channel CV ins.
  - Automate fades and levels for each channel, creating sequenced mixdowns, rhythmic muting, or doppler fade effects.

---

## Generic Suggestions

- Experiment with using *external signals* as CV inputs (audio for sideband effects, gate/triggers for rhythmic switching).
- Stack VCAs for feedback mixing or nonlinear summing (try patching the A-135’s output through more VCAs!).
- Use the A-135 as a VCA bank for quadraphonic or surround setups.

---

## References

- [Doepfer A-135 VC-Mixer User Manual (PDF)](https://doepfer.de/a100man/A135_man.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)