# Moog — Subharmonicon

- [Manual PDF](../../manuals/Subharmonicon_Manual.pdf)

---

[Moog Subharmonicon User Manual PDF](https://www.moogmusic.com/sites/default/files/2020-05/M2200_Subharmonicon_UM_WEB.pdf)

---

## Using Moog Subharmonicon for Hyper-Complex Percussion & Polyrhythmic Sequences

The **Moog Subharmonicon** is an analog polyrhythmic semi-modular synthesizer, exceptionally suited for rhythmic and percussive complexity thanks to its unique sequencer, polyrhythm, and subharmonic oscillator architecture. Let’s break down how you, as a Eurorack user, can harness its power for maximal rhythmic density and percussive punch.

---

### Core Features for Rhythmic Complexity

**1. Four Integer-Based Rhythm Generators**  
- Each divides the master clock by an integer (1–16); assignments are highly flexible.  
- Any combination of rhythm generators can trigger either/both sequencers.
- Mix multiple divisions (e.g., 3, 5, 7, 11, 13) for intricate, non-repeating polyrhythms.

**2. Two 4-Step Sequencers (Per VCO group/voice)**  
- Each sequencer independently controls pitch or subharmonic divisor assignments, or both.  
- Steps can be set to micro/macro-tuning ranges–great for pitched percussion!  
- Use with Quantize OFF for microtonal/atonal percussion, or ON for striking melodic clanging rhythms.

**3. Subharmonic Undertone Oscillators**  
- Two per VCO: allows each step, via sequencers, to shift both main pitch and subharmonic divisors.  
- This yields metallic, bell-ish, or “prepared percussion” timbres with shifting, stacked undertones.

**4. Full Patchbay Integration**  
- 32 patch points: CV/gate sequencers, clock in/out, triggers, EGs, VCO modulation, etc.
- Patch to and from other Eurorack modules for clock manipulation, external envelope shaping, further modulation, and audio/CV mangling.
- Patch SEQ 1/2 CLK outputs, or even TRIGGER outputs, for polyrhythmic trigger streams—perfect for drum voices or modulation.

---

### Techniques for Dense, Percussive, and Unique Patterns

#### **Polyrhythmic Generative Patching**
- Assign each rhythm generator to different sequencers, and stack multiple rhythm triggers onto one sequencer.
- Use uneven rhythm divisions (e.g., Rhythm 1 = 3, Rhythm 2 = 4, Rhythm 3 = 5, Rhythm 4 = 7) and combine them, then reset the sequence to bring things back into phase.
- Use the RESET and PLAY patch points to externally retrigger or stutter sequences from an external controller for maximal complexity.

#### **Percussive Voice Sculpting**
- Use sawtooth wave for snappy, brassy percussion; square with PWM modulated by sub-osc outputs (patchbay) for woody or bell-like clangs.
- Crank mixer levels to hit the Moog filter for added distortion, emphasizing punches and transient bite.
- Use the VCF’s EG amount bi-directionally: apply both positive and negative envelopes for unique attack/decay behavior, or to generate “reverse” percussive sweeps by using negative amounts.
- Patch in external envelopes or function generators (from Maths, Batumi, Zadar, etc.) to VCA/VCF inputs for custom punch/envelope shapes.

#### **Pattern Complexity & Microtiming**
- Patch the SEQ 1 CLK out to external modules (e.g. clock dividers or logic) and feed those back in via the Rhythm Generator CV ins for clock-logic feedback and emergent patterns.
- Modulate the Rhythm Generator CV ins with random sources, LFOs, or even another sequencer for constantly shifting, non-repeating drum patterns.
- Clock Subharmonicon from external sources with non-4/4 PPQN divisions for off-grid “broken” time signatures.
- Use the filter’s resonance at self-oscillation, and modulate pitch with sequencers for percussive, tomb-like hits, FM clangs, or accidental glass/bottle sounds.

#### **Layering & Polyphony**
- Use both VCO sections and their associated subharmonics to create layered percussion: “kick” from one, “snare” from subharmonics, etc.
- Cross-patch SEQ 1 output to VCO 2 or vice versa for “cross-sequencing”—one sequence modulates pitch/subharmonic assignments of the other.
- Patch VCO outputs or sub outputs as percussive audio-rate modulators into other modules for AM/FM percussion in your larger system.

---

### Making It Stand Out in a Mix

- Use sharp, short EGs and plenty of filter resonance for snap, but play with long attack for “swelling” percussion layers.
- Add external effects via the patchbay (VCAs, distortion, waveshapers).
- Mult the TRIGGER out to fire other percussion modules, layering polyrhythmic patterns for density using a single shared clock.

---

### Further Reading

- [Moog Subharmonicon User Manual PDF](https://www.moogmusic.com/sites/default/files/2020-05/M2200_Subharmonicon_UM_WEB.pdf)

---

### Example Patch Concepts

#### **Algorithmic Drum Cluster**
1. Patch all RHYTHM outputs in “odd” divisions to SEQ 1 (for kick) and SEQ 2 (for snare/perc), each with different rates.
2. Quantize sequences to 8-JI for pure intervals—increase step voltages randomly for microtiming.
3. Use patched VCA CV in from an external envelope for snappy transients.
4. Use subharmonic oscillators detuned for metallic “stacking.”

#### **Dense Trigger Grid**
- Patch SEQ CLK outs to a logic module (AND/OR/XOR) and feed results to TRIGGER ins on percussion voices or envelopes for ultra-dense, non-linear drum landscapes.

---

For deeper custom patching, inspect the complete [Moog Subharmonicon User Manual PDF](https://www.moogmusic.com/sites/default/files/2020-05/M2200_Subharmonicon_UM_WEB.pdf).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
