# Schlappi Engineering — Angle Grinder

- [Manual PDF](../../manuals/angle_grinder_manual_20181022.pdf)

---

[Download the Angle Grinder Manual PDF](https://static1.squarespace.com/static/5877376cd1758e13bbb0584f/t/5e6aa4d0a6dbf41964f112b2/1584006353939/AngleGrinder_MANUAL.pdf)

---

# Using Schlappi Engineering **Angle Grinder** For Eurorack Sound Design

**Angle Grinder** is a uniquely flexible quadrature oscillator and state variable filter with deep modulation possibilities. Its SPIN (oscillator/filter core) and GRIND (nonlinear waveshaper/comparator) sections enable a wealth of wild sonic territory. Here are creative modulation approaches to craft distorted percussion, gnarly basslines, and atmospheric pads.

---

## Core Modulation Possibilities

### 1. **FM1 / FM2 Inputs**
- **FM1**: Switchable between **linear** and **exponential** FM via jumper. Deep, audio-rate modulation here creates classic metallic or chaotic timbres.
- **FM2**: Exponential FM, great for aggressive pitch bends and bass growls.

### 2. **GRIND Sliders & CVs**
- Control the amplitude of phase-compared square waves subtracted from the input, allowing dynamic waveform mangling.
- CV (0–5V) modulates grind amount per phase; envelope or sequencer control here is key for percussive and bass movement.

### 3. **GRIND → SPIN / Damping**
- The **GRIND → SPIN** knob controls feedback from the waveshaper to the oscillator, morphing the overall behavior between pure oscillation and wild filter feedback.
- Modulating this parameter by CV (using a VCA + LFO/envelope) adds evolving distortion and self-oscillation artifacts.

### 4. **Inject and External Input**
- **INJECT** bypasses GRIND and can soft-sync the core, used with gates or audio for phase resets and extra punch.
- Regular INPUT takes in audio or CV to be wrangled by the GRIND comparators; try feeding percussion hits, FM modulator oscillators, or drones.

---

# Creative Sound Design Techniques

## A. **Distorted Percussive Sounds**

1. **Patch**
   - Leave Angle Grinder in LOW or HIGH range—try LOW for snappy modulation.
   - Patch gate, drum trigger, or envelope generator to one or more GRIND CV inputs to create shape/pulse-dependent distortion.
   - Use a drum sound or noise burst into INPUT (or INJECT for sharper sync).
   - Turn GRIND → SPIN knob up for feedback-driven distortion.

2. **Modulate**
   - **GRIND sliders**: Sequence or envelope-modulate individual sliders for evolving timbre with each drum hit.
   - **FM1/2 Inputs**: Patch percussion sound, audio-rate LFO, or random stepped CV to FM1 or FM2 for pitch artifacts; use exponential FM for wilder chaos.
   - **Damping**: Modulate with slow LFO for rhythmic shifting from tight hits to dirty resonance.

3. **Result:** 
   - You'll get squelchy, blown-out, bitcrushed percussive timbres—great for glitch, techno, and hard electro!

---

## B. **Dubstep/Drum & Bass Basses**

1. **Patch**
   - Set Angle Grinder as main VCO: Use V/OCT for pitch sequencing.
   - Crank GRIND → SPIN for aggressive feedback mixing.
   - Mult out 0° or 180° output to your main audio, and another phase output to modulate a filter or VCA downstream for stereo movement.
   - Mult envelope or LFO to both GRIND CV and FM2 for dynamic growl and movement.

2. **Modulate**
   - Send fast envelopes or wobbly LFOs to FM2 for pitch sweeps and growls.
   - Use clocked ramp or stepped random to GRIND slider CVs for formant-like bass movement.
   - Patch accent gates or kicks to INJECT for rhythmically resetting/syncing the oscillator — creates sync’d bass punches.

3. **Result:** 
   - Brutal, vowel-like or metallic basses loaded with movement (think classic "talking" bass).
   - Explode low-end with subharmonics by mixing both sine and GRIND outs.

---

## C. **Haunting Atmospheric Pads**

1. **Patch**
   - Set Angle Grinder to LOW range for LFO-speed quadrature outputs (modulate VCAs/panners downstream for enveloping stereo effects).
   - Patch drones or reverb-washed signals into INPUT; keep GRIND sliders low for subtle effect, or up for lo-fi color.
   - Use slow, unipolar LFOs on GRIND CVs to gently morph the waveshape.

2. **Modulate**
   - **FM1 (linear)**, with slow LFO/attenuated noise or even recorded sample waveform for organic drift and detune.
   - **GRIND → SPIN**: Slowly move manually or with a slow envelope to sweep between pure, filtered, and feedback-warped tones.
   - **Damping**: Animate with footsteps, envelope, or random for evolving resonance and shimmer.

3. **Result:** 
   - Four drifting, phase-shifted outputs (all phase-locked) allow for lush quadraphonic or moving stereo textures.
   - GRIND section adds brittle, spectral edges and eerie harmonic motion.

---

# Bonus Tips

- Use **ALL PASS** (phase shifted output) for unique layering and phasing effects.
- Feedback external audio (resample) through INPUT or INJECT for abrasive, self-modifying noise textures.
- The unlimited output headroom (up to 22Vpp!) lets you overdrive mixers and VCAs downstream for bonus saturation.

---

For more patching inspiration, check out the [Angle Grinder PDF Manual](https://static1.squarespace.com/static/5877376cd1758e13bbb0584f/t/5e6aa4d0a6dbf41964f112b2/1584006353939/AngleGrinder_MANUAL.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)