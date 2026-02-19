# Erica Synths — Black Multi Mode VCF

- [Manual PDF](../../manuals/black_multimode_vcf_manual_web.pdf)

---

[**Erica Synths Black Multimode VCF Manual (PDF)**](https://www.ericasynths.lv/media/Black_Multimode_VCF_manual_1.pdf)

---

# Creative Patch Ideas: Erica Synths Black Multimode VCF

The Erica Synths Black Multimode VCF is a flexible and characterful filter module, featuring simultaneous HP/BP/LP outputs, voltage control for cutoff and resonance, and a unique germanium diode overdrive on the input. Here are some creative ways to exploit its features in your Eurorack system, both with specific module suggestions and general module types.

---

## 1. **Three-Way Parallel Processing**

**Idea:** Split your sound source (oscillator, sampler, etc.) and patch it to the VCF input, then process its HP, BP, and LP outputs separately.

- **Mix & Morph:** Send the three outputs to a mixer module (e.g. Intellijel Triatt, Mutable Instruments Shades). Manually blend them for evolving timbres or use VCAs with envelopes/LFOs for automated morphing.
- **Processing Chains:** Route LP to a reverb, BP to a phaser, and HP to a distortion. Then recombine for a rich, dynamic texture.

---

## 2. **Voltage-Controlled Overdrive & Dynamic Harmonics**

**Idea:** Use the input drive/level knob with external signal amplitude modulation.

- **Sidechain CV:** Patch an envelope follower (e.g. Mutable Instruments Ears or Befaco Envelope Follower) from a drum or vocal source into the VCF audio input or drive CV if available. The harder your source hits, the more overdrive is applied, resulting in dynamic saturation.
- **Dynamic Patching:** Run a sequencer or random CV into the drive CV (via CV mixer/attenuverter) for evolving overdrive character.

---

## 3. **Self-Oscillating Madness & FM**

**Idea:** Tap into the VCF's self-oscillation as a sine(ish) wave oscillator at high resonance.

- **V/oct Tracking:** Use precise CV sources or sequencers to control the cutoff, effectively "playing" the filter as a tonal voice.
- **Filter FM:** Use a second oscillator or complex LFO patched to the cutoff CV input to explore filter FM. Try audio-rate signals for metallic or percussive sounds.

---

## 4. **Complex CV Animation**

**Idea:** With CV control over both cutoff and resonance, use different modulation sources for each.

- **Dual-LFO Animation:** Run two LFOs at different rates into the cutoff and resonance CV ins. Attenuvert their depth for gentle evolving or wild, chaotic sweeps.
- **Envelope Control:** Patch a snappy envelope to the resonance CV for filter "pings" or squelchy attacks while a slower envelope or LFO changes cutoff.

---

## 5. **Stereo Effects Creator**

**Idea:** Exploit the multiple outputs to generate stereo or spatial effects.

- **Dual-Channel Processing:** Send LP out to left and HP out to right channel in your final out/mixer/panorama. Animate cutoff with a cycling CV for a moving spectral stereo image.
- **BP Pan Sweep:** Use a stereo mixer with CV panning (e.g. Happy Nerding PanMix) and move the BP output dynamically between speakers.

---

## 6. **Feedback Patch for Chaos & Textures**

**Idea:** Create feedback loops by routing one filter output (e.g., HP or BP) back into the audio input with attenuation and/or effects in between.

- **Feedback Control:** Use a VCA or attenuator to tame the amount of feedback. Insert delay, reverb, or even another filter in the feedback path for dubby, metallic or drone textures.

---

## 7. **Play with Overvoltage-Resistant Inputs**

Given that all I/O is protected, don't be afraid to patch CV or audio-rate signals creatively, even in ways that may not be "traditional".

- **Audio-Rate CV:** Patch an audio oscillator into the resonance CV for wild, gritty modulations.
- **Logic Gates/Sequencer:** Try sequencing resonance or cutoff with random gates/triggers for glitchy or rhythmic filter movements.

---

## 8. **Specific Module Pairings**

- **Oscillators:** Mutable Instruments Plaits, Make Noise STO, or Erica Synths’ Black VCO for diverse source timbres.
- **Modulators:** [ALM Busy Circuits Pamela’s New Workout](https://busycircuits.com/alm017/) for complex, synced modulation, or Xaoc Devices Batumi for quad LFO duties.
- **Mixers & Morphers:** Intellijel Planar2 for joystick-controlled live morphing of filter outputs, or St. Modular Morph for voltage-controlled crossfading.
- **Envelope Generators:** Maths, Zadar, or Erica Synths Black EG for advanced envelope control.
- **VCAs/Attenuverters:** Mutable Instruments Veils or Befaco A*B+C to shape your CVs and audio flow.

---

**Links:**

- [Erica Synths Black Multimode VCF Manual (PDF)](https://www.ericasynths.lv/media/Black_Multimode_VCF_manual_1.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)