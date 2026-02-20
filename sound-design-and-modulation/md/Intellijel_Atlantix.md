# Intellijel — Atlantix

- [Manual PDF](../../manuals/atlantix_manual_2024.09.12.pdf)

---

[Download the Intellijel Atlantix Manual (PDF)](attachment:Atlantix_Manual_2024.09.12.pdf)

---

# Modulating the Intellijel Atlantix for Unique, Interesting Sounds

Below are tailored patching/modulation strategies for three styles: **distorted percussive sounds**, **crazy basslines (dubstep/drum & bass)**, and **haunting pads and atmospheres**. Each approach is based on details and creative routings described in the [Intellijel Atlantix Manual](attachment:Atlantix_Manual_2024.09.12.pdf).

---

## 1. Distorted Percussive Sounds

**Characteristics:** Fast attacks, clicky envelopes, overdrive, heavy filter resonance, sync, ring-mod, glitchy S&H, and use of noise.

### Patch Ideas & Modulation Strategies

- **Envelope for Percussive Shapes:**  
  - Use the [ENVELOPE RATE] switch to `FAST`.
  - Set `ATTACK` and `RELEASE` sliders low for very fast transient.
  - In ENV/GATE mode, try both for snappy/organ-like contours.
- **VCA Distortion:**
  - Engage the [DRIVE] switch in either `SYM` (symmetrical) or `ASYM` (asymmetrical) positions for clipping; `ASYM` sounds raw and glitchy.
- **Filter Excitation/Resonance:**
  - High [Q] setting on VCF for ringing/peaky attack.
  - Modulate [VCF cutoff] with both envelope (hardwired) and/or S&H from MOD section for random filtering effects.
  - Try **inverted** ENV polarity for aggressive "sucking" percussive attacks.
- **Oscillator Hard Sync:**
  - Set VCO A [SYNC TYPE] to `HARD` for classic punchy transients.
  - Sync VCO A to VCO B (use GATE or VCO B SAW as source).
- **Noise + S&H for Snap:**
  - In the MIXER, ride the [NOISE] slider.
  - Patch [NOISE OUT] from MOD section to modulate VCF cutoff or PWM for glitch.
  - S&H: Modulate VCO A’s frequency or VCA level with stepped/random voltages for digital-glitch percussion.
- **Ring Mod for Metal/Noise:**
  - Use ATLX expander's RING MOD output (sum/difference of two VCOs or VCO + noise).
  - Patch this back into the VCA or directly to output.
- **Pulse Width/Amplitude Tricks:**
  - Modulate VCO A PWM deeply for clicky, silenced pulses (100% pulse width kills oscillator).
- **AUX Routing for Parallel Processing:**
  - AUX 2 set to `VCA` position for layering external/processed sounds.

**Bonus Patch:**  
- Patch ENV INVERTED ([5.E]) to VCA LEVEL IN [5.C] for unusual dynamic response (transient ducking).

---

## 2. Crazy Basslines (Dubstep, DnB)

**Characteristics:** Aggressive filter movement, FM growls, sync, metallic/talking timbres, harmonically rich bass, stepped/chaotic modulation.

### Patch Ideas & Modulation Strategies

- **FM Bass Growl:**
  - Set VCO A FM 1 to `TZFM` mode (`AC` for pitch tracking, `DC` for wild modulations).
  - Use VCO B in audio-rate, patch its output to VCO A FM 1 IN or FM 2 IN.
  - Modulate FM INDEX slider with envelope or S&H for movement.
- **VCF Movement:**
  - Run envelope and MOD Y into both FM 1/2 of VCF; invert polarity for "wub-wub" effects.
  - Patch S&H OUT to one of VCF FM inputs for stepped/random wobbles.
  - Ride the [Q] slider for “scream” effects; high resonance, maybe self-oscillating.
- **Pulse/Sync Tricks:**
  - Sync VCO A to VCO B and detune for aggressive harmonics.
  - Modulate pulse width deeply (envelope, MOD X/Y, S&H, noise).
- **Parallel Processing / Sub Layer:**
  - Use SUB oscillator set to `-2` for deep bass foundation.
  - Send part of the sound post-filter (AUX 2 to VCA), and use another version pre-filter (main mix), for clean sub + distorted top.
- **Distortion/Drive:**
  - Use VCA DRIVE in `ASYM` for extra filth.
- **VCO B as LFO:**
  - Modulate VCF or VCO A FM for slow/fast rhythmic bass movement.
- **MOD Source Cross-Patching:**
  - MOD X: Use VCO B Square/Saw or S&H as FM input to VCO A.
  - MOD Y: Use NOISE or S&H as filter modulation for randomness.
- **Use of S&H / T&H:**
  - Switch to T&H for looser, drifting “talking” bass modulation; S&H for clean stepped changes.

**Bonus Patch:**  
- Patch audio from ATLX outputs (SAW, TRI, PULSE) through VCA, modulate amplitude with MOD X/Y or ENV for timbral bass shaping.

---

## 3. Haunting Pads & Atmospheric Sounds

**Characteristics:** Long evolving envelopes, smooth modulation, lush timbres, slow movement, stereo/parallel layers, shimmer, phase, subtle randomization.

### Patch Ideas & Modulation Strategies

- **Slow Envelopes:**
  - Set [ENVELOPE RATE] to `SLOW`.
  - Use long ATTACK and RELEASE for evolving textures.
- **VCF:**
  - Use BP (bandpass) or PHZ modes with modest [Q] for airy/washed pads.
  - Modulate filter cutoff with slow LFO (VCO B in LFO mode), or MOD X/Y set to Sine/Triangle.
  - Slight randomization: modulate ENV amount with S&H at low rate, or noise at low amplitude.
- **Oscillator FM & Sync:**
  - Soft sync for organic instability; modulate FM at slow rates for subtle shimmer.
  - Set VCO B as LFO and patch to VCO A FM for subtle drifting pitch/timbre changes.
- **Parallel Harmonics/Aux Layers:**
  - Mix in TRI, SINE, or noise at low levels in MIXER section.
  - Use AUX 2 routed to VCA for an ethereal layer bypassing the filter.
- **Pulse Width Animation:**
  - Modulate VCO A PWM with slow LFO, envelope, or S&H for gentle undulating movement.
- **VCF/Phaser:**
  - Switch to PHZ mode for phasey, haunting textures.
  - Sweep filter cutoff (manual or CV) for moving notches.
- **Self-Patching Feedback:**
  - Patch filtered output (ATLX BP/PHZ OUT) to external delay/reverb, return to AUX 1/2 for feedback.
- **S&H for Subtle Unpredictability:**
  - At slow rate, use S&H OUT to gently modulate mixer levels or VCA envelope level.

**Bonus Patch:**  
- Use MOD X and MOD Y both set to LFOs with phase offset (one SINE, one TRIANGLE) to crossfade/filter and FM for stereo/animated pad-like morphs.

---

## Additional Tips

- **Utilize MOD X/Y Unipolar/Bipolar/Polarity switches** for nuanced control over modulation destinations.
- **Leverage ATLX Expander** for dedicated outputs, easy parallel/processing, or external re-injection.
- For all patches: experiment with cutting normalled signals and repatching for self-patching feedback and unique cross-modulation.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)