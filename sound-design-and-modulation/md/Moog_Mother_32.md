# Moog — Mother 32

- [Manual PDF](../../manuals/Mother_32_Manual.pdf)

---

[**Moog Mother-32 User Manual (PDF)**](https://cdn.moogmusic.com/sites/default/files/2016-04/Mother-32_Manual_v3_0.pdf)

---

# Modulation Strategies for Mother-32: Distorted Percussion, Crazy Basslines, & Haunting Pads

Drawing on the Moog Mother-32’s versatile semi-modular design and extensive patchbay, here's how you can employ CV modulation and creative patching to push the Mother-32 into unique territory including hard, digital-sounding percussion, extreme bass, and ethereal drones. 

## 1. **Distorted, Percussive Sounds**

### Kick/Drum Snares
- **Noise as an Oscillator**: Use the Noise output, patch it into the EXT AUDIO input. Now, the MIX control can blend between VCO waveform and Noise. Dial up the resonance on the filter for snappy, punchy attacks.
- **Short Envelope & Accent**: Use fast ATTACK/DECAY settings on the EG for sharp transients. Accent steps using the sequencer for added aggression.
- **VCF Self-Oscillation**: In Low Pass mode, with RESONANCE maxed, route KB CV to VCF CUTOFF and patch VCF OUT back to EXT AUDIO—this lets the filter become a sine oscillator, great for "clicks" and tuned percussion.
- **Tuning Modulation**: Use the LFO, set to Square, to VCO MOD IN; choose extreme (audio rate) modulation for gritty, biting timbres. Or patch LFO SQUARE/TRI into the VCF CUTOFF IN for fast filter "flicks."
- **External Feedback**: Patch VCF OUT into EXT AUDIO with MIX at max. This creates feedback/distortion, especially wild if you modulate MIX CV IN with audio-rate LFO or EG for clangorous, trashy drum tones.

#### Example Patch (Metallic Snare)
- [Manual Reference, p.53](https://cdn.moogmusic.com/sites/default/files/2016-04/Mother-32_Manual_v3_0.pdf#page=53)
    - Patch: VCF OUT → EXT AUDIO (for metallic ring), add NOISE via MIX; FAST Envelope. Try modulating VCA CV with an LFO or Envelope for gated, crushed effects.

---

## 2. **Crazy Basslines (Dubstep/DnB Style)**

### Aggressive, Moving Bass
- **FM & PWM**: Patch LFO SQUARE or external audio-rate signal to VCO LIN FM IN for growling, harsh frequency modulation. For signature bass wobbles, clock-sync the LFO TRIANGLE to modulate VCF CUTOFF IN.
- **VCO Pulse Width Mod**: Use the internal or external LFO to modulate VCO MOD IN (destination: PULSE WIDTH). At audio rates, this creates nasty, phasey textures.
- **Filter Overdrive and Modulation**:
    - Max RESONANCE, modulate VCF CUTOFF with Envelope (VCF MOD SOURCE: EG), set MOD AMOUNT high.
    - For rhythmic filter movement and dirty "tearing" sounds, ratchet sequencer steps (see Ratchet in manual), so the EG triggers the filter with rapid, repeating pulses.
- **Sequencer Tricks**: Program ratchets, ties and slide/glide between bass notes. Use Accent for occasional filter or VCA boosts—assign high ACCENT steps to push the VCA and Cutoff for variable drive.
- **Audio-Rate Feedback**: Patch VCO PULSE or SAW into EXT AUDIO for full, harmonically-rich parallel oscillators. Combine with internal VCO for FM-style metallic grit.

#### Example Patch (8-Bit Percussion or Filter Kick)
- Use step-skewed filter (RESONANT HIGH PASS) and Ratchet on key pattern steps, heavily modulate GLIDE and GATE LENGTH per-step for unruly, stuttering basses.

---

## 3. **Haunting Pads and Atmospheres**

### Drone & Texture Design
- **Swell Envelope**: Slow-attack and long-decay with EG (SUSTAIN ON) gives evolving, pad-like contours.
- **Filter Modulation**: Use LFO TRIANGLE (slow rate) patched to VCF CUTOFF IN. For more randomness, use the Assign output set to "STEP RANDOM" or "MIDI CC" and patch to VCF or MIX CV IN.
- **External Audio**: Feed field recordings or distant textures into EXT AUDIO IN, blend with internal NOISE and VCO using the MIX control (use slow VC MIX modulation for evolving blends).
- **Multiple Modulation Sources**: Use the VC MIX as a CV blender (mix LFO TRIANGLE and EG OUT), then patch to VCF CUTOFF or VCO MOD for richer, less-predictable modulation.
- **Feedback & Reverb**: Patch VCF OUT into EXT AUDIO and carefully modulate MIX CV IN with slow, gently varying LFO, simulating resonant, feedbacky reverb/diffusion.
- **Subtle PWM or FM**: Use a slow LFO to modulate Pulse Width if using PULSE waveform. Subtle FM can impart complexity without harshness at slower rates.

#### Example Patch (Drone)
- VCA ON (for continuous sound), slow LFO TRI → VCF CUTOFF and MIX CV. Fade in NOISE, turn up filter resonance. Optionally, defeat internal keyboard triggering for pure ambient soundbed.

---

## 4. **General Creative Mod Tips**

- **Self-Patching**: Many points (e.g., KB, EG, LFO outputs) can be patched to multiple inputs at once using the MULT for unison or composite modulation.
- **Assign Output**: In Setup Mode, configure the Assign output for "Step Random," "Step Ramp," or "MIDI CC" to produce wild, non-repeating modulations for filter, pitch, VCA, or MIX.
- **External Modulation**: Use outside modules—distortion, wavefolders, bitcrushers, or more aggressive LFOs/sequencers—to drive Mother-32 CV inputs for even greater sonic instability.

---

> For further reference and example patch diagrams, refer directly to the [Mother-32 manual PDF](https://cdn.moogmusic.com/sites/default/files/2016-04/Mother-32_Manual_v3_0.pdf) (especially p.53–55 for drum and bass preset sheets).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)