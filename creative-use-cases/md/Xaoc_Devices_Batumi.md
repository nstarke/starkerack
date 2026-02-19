# Xaoc Devices — Batumi

- [Manual PDF](../../manuals/xaoc_batumi2_poti2_manual.pdf)

---

[Download the Xaoc Batumi II + Poti II Manual PDF](https://xaocdevices.com/manuals/xaoc_batumi2_and_poti2_manual.pdf)

# Creative Patch Ideas for Xaoc Batumi II + Poti II

The Xaoc Batumi II, especially with the Poti II expander, is a *deeply* creative, performance-friendly, and modulation-focused quad LFO with optional audio-range VCO abilities. Below are patch strategies, module interactions, and creative workflows that harness its full potential in your Eurorack setup.

---

## Modular Pairings and Patch Recipes

### 1. **Envelope & Sequencer Animation**
**Pair With:** Make Noise Maths, Intellijel Quadrax, ALM Pam's New Workout, Mutable Instruments Stages (as step sequencer).
- **Patch:** Use Batumi II’s quadrature, divided, or multiplied modes to create phased or related LFOs. Send each to modulate amplitude, decay, or stage length of different envelope generators. Now your envelopes evolve over time or create polyrhythmic modulation.
- **Creative Use:** Animate the speed of envelopes for generative, non-repeating modulation. Batumi II’s random outputs (stepped/smooth) into sequencer CV inputs for melodic motion or rhythmic gating.

### 2. **Complex VCO Cross Modulation**
**Pair With:** Mutable Instruments Plaits, Make Noise DPO, Tiptop Z3000.
- **Patch:** Switch Batumi II into audio rate (Free Mode, with 1V/oct tracking), use two channels as VCOs. Patch one out to modulate the FM input of a traditional analog oscillator, and vice versa.
- **Creative Use:** Exploit exact phase control and resets for experimental FM/PM synthesis. Use phase or wave switching modulation via Poti II for evolving timbres.

### 3. **VCAs and Animated Effects**
**Pair With:** Mutable Veils, Intellijel Quad VCA, Befaco A*B+C, FX modules like Strymon Magneto.
- **Patch:** Use Batumi II’s assignable waves to modulate four channels of a quad VCA. Send diverse modulation to volume, filter cutoff, dry/wet mix, delay repeats, etc.
- **Creative Use:** Animate multiple FX parameters for immersive, spatial textures. Poti II’s individual attenuation keeps the mix subtle or intense.

### 4. **Rhythmic Clock Division/Multi-Layered Euclidean Patterns**
**Pair With:** 4ms Quad Clock Distributor, ALM Pamela’s Pro Workout, Mutable Grids, Malekko Varigate, Tempi.
- **Patch:** Use Divide or Multiply mode—sync Batumi II to a master clock and use divided/multiplied outputs as clock/gate sources for logic or trigger modules.
- **Creative Use:** Generate interrelated patterns for auxiliary percussion, modulation, or switching FX paths. Patch Batumi II’s random stepped output to a logic/counter for wild generative rhythms.

### 5. **Modulated Wavetable CV Generator**
**Pair With:** Mutable Instruments Rings, Tiptop Z-DSP (or any wavetable oscillator).
- **Patch:** Assign unique waveforms per channel, shape-modulate with CV through Poti II, and use these as evolving CV sources for a wavetable oscillator’s morph or position input.
- **Creative Use:** Animate audio timbres or filter curves with simultaneous, CV-morphing shapes. Modulate the shape change rate with Batumi’s own CV inputs.

### 6. **Self-Patching Feedback Networks**
- **Patch:** Use Batumi II’s outputs to modulate its own frequency, phase, or ratio CV inputs. Employ Poti II to adjust depth/attenuation per channel.
- **Creative Use:** Create chaotic modulation, strange cyclic patterns, or even pseudo-random voltage sequences. Experiment with resetting/syncing in different modes for unpredictable modulation.

### 7. **Quad Panning or Spatial Modulation**
**Pair With:** Happy Nerding PanMix / Joranalogue Mix 3 / Make Noise X-Pan.
- **Patch:** Batumi’s LFOs go to pan/CV inputs of a quad panner. Shape and offset each output via Poti II.
- **Creative Use:** Envelop soundscapes in evolving, 3D movement across a stereo or multi-channel field.

### 8. **Animated Quad Sample & Hold**
**Pair With:** Doepfer A-148, Mutable Kinks, Random*Source S&H, Erica Synths Black S&H.
- **Patch:** Route Batumi’s stepped random outs to multiple sample & hold modules clocked differently or at rates derived from Batumi itself.
- **Creative Use:** Generate four parallel, oddly correlated random voltages for evolving modulation or melodies.

### 9. **Multi-Layered Polyphonic or Paraphonic Modulation**
**Pair With:** Polyphonic synth voices (Doepfer A-111-4 Quad VCO, Endorphin.es Godspeed, Mutable Instruments Polyend).
- **Patch:** Use Batumi II’s VCOs each tuned/tracked to a separate voice. Assign independent shapes, CV modulate them, or use global phase/frequency relationships for coordinated timbral evolutions.

### 10. **Interactive Performance Macros**
**Pair With:** ALM Boss Bow Two, Ritual Electronics Miasma, expressive controllers.
- **Patch:** Use reset/sync inputs with triggers/gates from performance controllers or logic for live phase changes, switching between rhythmic and free modulation on the fly.
- **Creative Use:** Live polyrhythmic morphing, macro modulation, or staged texture evolution—Poti II lets you jump between preset wave shapes or depths per channel on demand.

---

## Bonus "Otherworldly" Combos

- **Spectral Shaping:** Batumi’s random outs into morph/tilt EQ or spectral processors (Verbos Bark Filter for zoned spectral animation).
- **Video Synthesis:** Batumi II acts as a precise control voltage generator for video synthesis, using phase/division to spin, warp, or cycle through video domains (LZX Industries systems).
- **Trigger-based Chopping:** Use Batumi’s divide outputs for rhythmic amplitude chopping, crossfading, or rapid-fire gating.

---

**Pro Tips:**
- Exploit separate shape assignment and attenuation per channel for ultra-fine control—think of Batumi II/Poti II as a ‘control voltage designer showcase.’
- Use Batumi as a clock *source* for logic or sequential switch modules for meta-sequencing (i.e., using LFOs to clock or flip sequencer stages).
- Patch Batumi’s phase mode into a quad filter bank’s cutoff for swirling, rotating filter animation.

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)