# Worng Electronics — Vector Space

- [Manual PDF](../../manuals/Vector Space Manual v1.00.pdf)

---

[WORNG Electronics Vector Space User Manual (PDF)](https://static1.squarespace.com/static/5947c99b3a04112670a75d50/t/5a9430329140b7f962468164/1519678771602/Vector+Space+user+manual.pdf)

---

# Advanced and Creative Uses for WORNG Electronics Vector Space

The Vector Space from WORNG Electronics is a powerful utility/modulation module that excels at both simple mixing and wild, high-dimensional CV mangling. After studying the manual, here are several creative ways to use it in a Eurorack system, ranging from beginner to advanced patching paradigms:

## 1. **Dynamic Modulation Source Hybridization**
**Recommended Modules:**
- 3 Different LFOs (classic: Doepfer A-145, Xaoc Batumi, DivKid Ochd)
- Envelopes (Intellijel Quadrax, Maths)
- Stepped Random Generators (S&H, Wogglebug, Mutable Marbles)

**Patch Idea:**  
Patch three LFOs (with different waveforms/rate syncs) into the i, j, and k inputs. Take the 17 outputs to various destinations: filter cutoff, VCO FM, wavefolder, LPGs, panning, VCAs. The result is modulations related but phase-shifted, inverted, and generally more organic than three basic LFOs.  
- **Tip:** Use S&H or stepped random waves for interesting stepped modulation “counterpoint”.

## 2. **Performance Macro-Morphing**
**Recommended Modules:**
- Joystick (Doepfer A-174, Planar2, Erica Synths Joystick 2)
- Preset Voltage Source (Mutable Frames, Voltage Block)

**Patch Idea:**  
Use a joystick to control two or three dimensions (i, j, k). Send Cube outputs to VCAs panning different sound sources, gesturally morphing your patch in stereo, quad, or even octal spatialization.  
- Map one axis to timbre (via wavefolder/waveshaper), another to spatialization (VCAs), and one more to send effects (reverb send, delay feedback, etc.).

## 3. **Cross-Modulation Feedback Networks**
**Recommended Modules:**
- VCAs (Intellijel Quad VCA, ALM Tangle Quartet)
- Envelope Generators (ADSR, Maths)
- Complex Oscillators (DPO, Cylonix/Shapeshifter, Instruō Cs-L)

**Patch Idea:**  
Send envelope or modulation outputs from your main voices into i, j, and k. Use some Plane or Sphere outputs to send back to modulate the shape, rise/fall, or FM input of those same EGs or oscillators. This “cross-feedback” network generates highly animated, self-adapting envelopes or timbres.  
- If using audio-rate modulation, Vector Space can act as a complex ringmodulator or vector amplitude transformer.

## 4. **Multidimensional CV Re-Mapping for Sequencers**
**Recommended Modules:**
- Sequencers (Metropolis, Rene, Stillson Hammer, Eloquencer)
- Quantizer (Qu-Bit Bloom, ADDAC207, Intellijel Scales)

**Patch Idea:**  
Take three related but different melodic sequences or stepped voltages to Vector Space inputs. Take unique outputs (such as Plane or Cube outs) to different quantizer channels, then to multiple oscillators. Create generative “counterpoint” between voices—sequences will interlock and drift apart automatically. Tweak input switches for huge variations.

## 5. **Vector-Based Audio Mangling**
**Recommended Modules:**
- Three related oscillators (Tiptop Z3000, Dixie II+, STOs, Bubblesound VCOs, etc.)
- Wavefolder (Serge, Timbre, Erica Fusion)
- Mixer

**Patch Idea:**  
Feed three audio signals or oscillators that are close in pitch (detuned but harmonically related) into i, j, k. Send the 17 outputs—each a unique phase/timbre combination—into mixers, panners, or effects, and blend for rich audio morphing, reminiscent of Vector Synthesis. Try modulation via a joystick or envelopes on one or more audio inputs for dynamic waveshaping.

## 6. **Rhythmic Complexity via Clock Modulation**
**Recommended Modules:**
- Trigger/Gate Generators (Pam’s New Workout, Euclidean Circles)
- Burst Generators (Random Rhythm, Zularic Repetitor)
- Logic/Clock Dividers (Doepfer A-160-2, Plog)

**Patch Idea:**  
Patch three different clocks or rhythmic triggers into Vector Space. Use Cube or Plane outputs as new gate streams to trigger envelopes, drum voices, or sequential switches. The differential/inverted combinations can create hocketing, Euclidean, or polyrhythmic effects only achievable by high-level logic modules, but with continuous CV hybridization.

## 7. **Multi-Parameter Macro-Control**
**Recommended Modules:**
- Any classic module with CV control
- Matrix Mixers (Doepfer A-138m, 4ms VCAM)

**Patch Idea:**  
Use envelopes, LFOs, or performance gestures to the Vector Space, and distribute its many outputs to parameters system-wide (filter cutoffs, oscillator FM, delay time, wavefolding, reverb send, stereo placement, etc.). Tune the mapping such that one gesture can affect dozens of patch points with intricate, natural-feeling relationships.

---

## Some Quick General Tips:

- **Unipolar vs. Bipolar:** Try switching the input ranges in realtime for performative voltage jumps.
- **Rectification:** The Plane and Sphere family outputs will “fold” negative voltages, great for doubling rates or unique CV shapes.
- **Audio-Rate Processing:** Vector Space is fully analog and can be used at audio rates—experiment with AM/ringmod/RM craziness.
- **Feedback Loops:** Patch outputs back to inputs for self-modulating, generative chaos.
- **MIDI Integration:** Use MIDI-to-CV converters (e.g., Expert Sleepers FH-2, Mutant Brain) to “play” the module from a DAW or controller for precise parameter morphing.
- **Effect Routing:** Use as a routing hub for multiple effect chains, especially with morphable sends/returns.

---

## Further Reading / Patching Inspiration

- [WORNG Electronics Vector Space User Manual (PDF)](https://static1.squarespace.com/static/5947c99b3a04112670a75d50/t/5a9430329140b7f962468164/1519678771602/Vector+Space+user+manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)