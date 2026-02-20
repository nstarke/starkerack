# Qu-Bit — Cascade

- [Manual PDF](../../manuals/Getting_Started_Cascade.pdf)

---

[**Download the Qu-Bit Cascade Manual (PDF)**](https://www.qubitelectronix.com/_files/ugd/1d8f27_cc2fd52d2bf04c5a929df18ca9c82ca8.pdf)

---

# Creative Patch Ideas for Qu-Bit Cascade: Distorted Percussion, Basslines & Atmospheric Pads

The **Qu-Bit Cascade** is a versatile Eurorack module offering envelope generation, VCA/LPG behavior, ratcheting, internal sound sources, compression, and more, perfect for experimental sound design. Let's break down possibilities for three specific sound design goals:

---

## 1. **Distorted Percussive Sounds**

**Key Tools:**  
- Internal hi-hat, kick, and noise sources  
- Ratcheting AD envelope  
- Fast/slow envelopes & shape modulation  
- Compressor with virtual sidechain  
- 'Invert' and 'Offset' controls for further shaping

**Patch Ideas:**  
- **Layered Percussives:** Patch the internal hi-hat or noise source into the VCA. Use the Ratcheting AD mode with repeats set high (e.g. 4–12x@fast) to create rapid-fire percussive weirdness. Push 'curve' toward exponential for snappy attacks/distorted artifacts.
- **Envelope Sidechain Crunch:** Feed external drums or harsh sources into ‘VCA In’, and set the mode to COMPRESSOR. Use extreme 'ratio' and low 'threshold'; fast attack/decay makes for harsh, aggressively ducked textures (crunchy, sidechain-like distortion).
- **Audio-Rate Envelope Mod:** Patch an LFO or pitched oscillator into the envelope's 'trigger' input set to high speed (audio rate). This can "AM" the envelope, blurring the percussive shape and producing digital distortion artifacts.
- **Envelope Inversion:** Try 'invert' mode to flip your envelope. Nonlinearities in the envelope can cause asymmetric distortion (especially if level is maxed, or with added offset).
- **Hot Output:** Crank the 'level' and 'offset' unnecessarily high, then saturate external analog filters or wavefolders for extra heat.

---

## 2. **Crazy Basslines (e.g. Dubstep/DnB)**

**Key Tools:**  
- Internal sine for sub-bass  
- Fast, snappy envelopes  
- Looping mode for LFO-like shapes  
- Envelope Follower for audio-reactive movement  
- VCA for dynamic amplitude modulation

**Patch Ideas:**  
- **Wobble Bass:** Use the sine tone internal source, patch it to the VCA. Use ASR or AD mode, set envelope to loop (high repeat, infinite at knob end) for LFO-like modulation. Send envelope out to modulate filter cutoff externally (for formant sweeps). Changing ‘curve’ and ‘decay’ = morphing LFO shapes.
- **Envelope-Followed Bass:** Feed a drum loop into VCA In, set Cascade to Envelope Follower. Envelope out now tracks the amplitude of the drum and can *modulate oscillator FM, filter cutoff, or VCA for reactive, "talking" basslines*.
- **Double Ratcheting Glide:** Set repeats high, enable ratcheting, so each trigger gives a stuttering, machinegun bass note (great in DnB). Add glide by patching envelope output as a pitch CV to an external VCO.
- **AM/FM Bass:** Patch a sequencer to trigger, sync repeats to the clock, and tweak envelope times to create rhythmic, almost FM-like bass patterns. Try sending both envelope out and VCA out to a mixer for layered, harmonically rich bass.
- **Compressor Mayhem:** Use the compressor with sine or noise; extreme settings squash the audio, clipping and distorting for aggressive movement and dirty subs.

---

## 3. **Haunting Atmospheric Pad Sounds**

**Key Tools:**  
- Internal white noise + sine  
- ADSR/ASR mode for long evolving envelopes  
- Gentle gravity (Amplitude+Time Gravity in Edit Functions)  
- Use Level/Offset for higher dynamic range  
- VCA in for stereo/parallel processing (feed external drones in)

**Patch Ideas:**  
- **Multi-stage Pad Swells:** In ADSR or ASR mode, set long attack/decay/release. Mix noise + sine (or external drones) into VCA in; trigger long gates/envelopes from a slow clock/LFO for huge echos or "clouds."
- **Gravity Curves for Evolving Textures:** In Edit Functions, enable Amplitude and Time Gravity. Envelope times and intensity will dynamically respond to input, creating pads that morph over time (naturalistic rise/fall, never quite the same twice).
- **Dreamy Gated Pads:** Gate out in EOD or EOA mode patched into external effects or VCAs — gates now correspond to envelope phases for dynamic layering. Manipulate sustain with offset/level for ghostly, shimmering fades.
- **Pad Distortion/Aliasing:** Lower the envelope time to minimum, crank repeats (infinite), and mix in some internal hi-hat or external audio for strange, grainy artifacts. Layer this on top of slower pads for lo-fi grit.
- **Sidechain Swells:** Use internal compressor with virtual sidechain for classic “ducked pad under kick” effect. Adjust ratio and threshold for dramatic "pumping" pads.

---

## Further Exploration

- **External Modulation:** Use external CV in (to VCA, envelope time, level, offset) for even more unpredictable shifting.  
- **Edit Functions:** Hold Shift and experiment with gravity/gate behaviors for performance-ready variations on the fly.

---

**More details and patches:**  
[https://www.qubitelectronix.com/shop/cascade](https://www.qubitelectronix.com/shop/cascade)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)