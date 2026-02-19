# Moog — Mother 32

- [Manual PDF](../../manuals/Mother_32_Manual.pdf)

---

[Download the Moog Mother-32 Manual PDF](https://www.moogmusic.com/sites/default/files/2017-07/Mother32_Manual_v2.1.pdf)

---

# Using the Moog Mother-32 for Hyper-Complex, Densely Rhythmic Percussion Sequences

As a eurorack modular musician, the Moog Mother-32 is a powerful semi-modular analog synthesizer voice, with deep potential for rhythmic exploration—including polyrhythms, non-standard time signatures, and heavily modulated percussion. Here’s how you can weaponize its capabilities for your musical pursuit:

## **Sequencer: Building Complicated Patterns**

- **Patterns up to 32 Steps:** Use the built-in sequencer to store up to 64 patterns, each with up to 32 steps. This enables long and intricate sequences, ideal for odd or evolving time signatures.
- **Ratcheting:** The Mother-32 sequencer allows 1-4 ratchets per step. Use these for rapid-fire "rolls" or fills on single hits—a core tool for dense, glitchy percussion.
    - *Set per-step ratchets*: SHIFT + twist the GLIDE knob during step input in KB or Step mode.
- **Ties, Rests, and Accents:** Each step can be a note, tie, rest, or accented hit. Layering accents and playing with rests and ties lets you break up the rhythm for syncopated, non-4/4 grooves.
- **Rotating/Offsetting Patterns:** In Step mode, rotating steps shifts your rhythmic downbeat—great for polymetric feels, or to offset one pattern against another.
- **Swing:** Apply negative or positive swing to push/pull timing on off-beats and on-beats. Extreme values can totally reshape groove.

## **Patch Bay: Polyrhythms & Modulation**

- **Patch In External Clocks:** Use the TEMPO input to slave the sequencer to odd division clock sources (e.g., 5/8, 7/8, etc.), or clock from divided/multiplied pulses for polyrhythmic layers.
- **Sequencer Clock/Divide Outs:** The ASSIGN output can be set (via Setup Mode) to output different clock divisions (step, clock/2, clock/4, etc.). Use these as triggers/envelope sources for other modules, or to clock LFOs or sample/hold modules for evolving percussion.
- **Advanced Modulation:** Route LFOs (or external CV) to VCF Cutoff, VCO Pitch, VCA CV, or even to the sequencer tempo for time warping/rhythm morphing FX.
- **Randomness:** In Setup Mode, assign ASSIGN output to Step Random—use this to trigger random modulation or sample/hold CV for unpredictable percussion hits.

## **Designing Percussion: Unique, Punchy, and Distinct**

- **Mother-32 as a Drum Voice:** 
    - Fast DECAY, no SUSTAIN, and snappy ATTACK for classic percussive envelopes.
    - Use PULSE wave and modulate PULSE WIDTH for “clap”/“snare” character.
    - Noise + VCF for snares, hi-hats, shakers (patch NOISE to EXT AUDIO and blend in MIX).
    - RESONANCE self-oscillation = Sine source: Kick drums, toms (VCF as oscillator! See manual tips).
- **Harmonic complexity:** Use audio-rate LFO (over 20Hz) into VCO mod input for FM percussion with metallic/inharmonic tones.
- **VCF Tricks:** Patch VCF OUT back into EXT AUDIO (with MIX at max) in HIGH-PASS mode for biting, feedback-heavy percussion.
- **Glide & Legato:** Use ties and glide for sliding, 808-cowbell/water-droplet style percussion. Glide per-step, modulate glide amount via CV for evolving groove.

## **Patch Examples for Complex Percussion:**

- **Polyrhythms:** Patch clock dividers/multis to feed different external clocks to Mother-32s, each running a different pattern length.
- **Randomized Percussion:** Assign ASSIGN output to Step Random, patch to VCF cutoff or VCO FM for continually morphing percussion timbres.
- **Layering:** Use VC MIX or Mult to layer internal and external sources; for example, stack Mother-32 percussive plucks with external Eurorack percussion voices, synced but running different step lengths.

## **Suggestions for Further Complexity:**
- **Eurorack Integration:** Break Mother-32 out of its case, and use in a modular system. Let external modules (logic, probability gates, Euclidean sequencers, etc.) interact with the patchbay for even more rhythmic intricacy.
- **MIDI Interplay:** Use incoming MIDI clock (odd meters, triplets) or MIDI note data for triggering/overlaying on top of internal sequences.

---

## **Pro Tips**

- **Live Tweaking:** During playback, use LIVE ACCENT, LIVE MUTE, and LIVE RATCHET (by holding SHIFT and relevant controls/buttons) to dynamically reshape your rhythm in performance.
- **Preset-Based Drum Kits:** Use or design custom presets (see manual patch sheet) for different percussive sounds. Rapidly switch patterns/presets for structured, song-like rhythmic arrangement.

---

### [Download the Official Moog Mother-32 Manual PDF](https://www.moogmusic.com/sites/default/files/2017-07/Mother32_Manual_v2.1.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)