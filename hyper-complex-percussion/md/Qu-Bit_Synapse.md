# Qu-Bit — Synapse

- [Manual PDF](../../manuals/Synapse.pdf)

---

[Qu-Bit Synapse Manual (PDF)](https://cdn.shopify.com/s/files/1/0660/7545/files/Synapse_Manual.pdf)

---

# Using Qu-Bit Synapse for Densely Rhythmic and Hyper-Complex Percussion Sequences

The Qu-Bit **Synapse** is an advanced crossfading switch/router module—not a direct sound generator or effect, but a powerful utility for generating rhythmic complexity and timbral changes by dynamically routing, crossfading, and mixing any audio or CV. Its features make it uniquely suited to experimental, polyrhythmic, and sequenced percussion, transforming simple sources into a dense, hyper-detailed rhythmic tapestry. Here’s how you can exploit it for advanced, unique percussive results:

---

## Key Rhythm-Generating Features

### 1. **Dynamic Crossfade Sequencing (“Morphing” Percussive Sounds)**
- **Crossfade Between Sources:** Patch multiple percussion or synth voices (think classic drum modules, noise bursts, metallic hits, or even clicky waveforms) into the A/B inputs. Use the crossfade knobs, or (better yet) CV, to morph between them.
- **Automated Crossfade with Internal or External CV/LFOs:** Modulate the crossfade positions at audio, sub-audio, or clocked rates. Internal LFOs can be used per-channel—these can move crossfades rhythmically or at audio rate for AM-like effects.

*Tip*: Modulate crossfades using clock-divided or polyrhythmic trigger sources for shifting, stuttering, morphing percussion hits.

### 2. **Complex Sequential and Random Switching**
- **Terminal Functionality and Advance/Scatter Controls:**
  - Route outputs polyrhythmically or pseudo-randomly by clocking the `Advance` and `Scatter` inputs with complex rhythm sources.
  - “Shuffle” or rotate the output connections on every trigger to create shifting or unpredictable percussion arrangements.
  - Use the randomizing or advancing functionalities to create sudden, lively variations.

*Tip*: Use different, related rhythm sources (Euclidean triggers, clock multipliers/dividers with polyrhythms, etc.) to clock the switch functions, generating non-repeating but tightly rhythmic patterns.

### 3. **Memory Snapshots for Sections/Glitch-Style Switching**
- **Store & Morph Between States:** Save up to eight crossfade/route states as “memory snapshots”. Sequence between memory states in time with your composition (by CV or manually), allowing for instant, rhythmic pattern changes or wild glitch fills.
- **Randomize Memory for Evolutive Patterns:** Use the memory randomization function to periodically inject random crossfade/routing states into a pattern.
- **Recall for ‘Section’ Transitions:** Use memory to jump between percussive ‘sections’ (e.g., main groove, fill, breakdown).

### 4. **Internal LFO Polyrhythms**
- **Assign internal LFOs to crossfade channels.** Set different phase relationships (especially "Cascading" or "Phase Offset" modes)—these phase offsets can create natural polyrhythms when LFOs modulate different crossfade positions, resulting in shifting, phase-shifted, or compound patterns.

*Tip*: Let LFOs modulate crossfades between noise and tonal percussion at different phase offsets to create “rolling” or “turning” polyrhythmic textures.

---

## Techniques for Hyper-Complex Percussive Patches

### A. **Patch Recipe: Polyrhythmic Switch and Morph**
1. **Inputs:** 
   - Load 4 distinctly different percussive voices or audio-rate bursts into each A and B input.
2. **Crossfade CV:**
   - Use internal LFOs in phase-offset or cascading mode for each channel.
   - Alternatively, sequence crossfade CVs from a polyrhythmic, multi-track trigger sequencer.
3. **Routing:**
   - Use Advance and Scatter inputs, clocked by different clocks (e.g. 3 against 4, or other polyrhythms).
   - Route sum outputs to a shared bus/mixer; or split outputs to individual FX or processing.
4. **Memory:**
   - Program several “states”: e.g., all snares to output 1, all hats to 2, random blends to 3/4. Back-and-forth through memories creates instant variation.
5. **Inertia:**
   - Add a bit of inertia/slew for moving “slide” between crossfade/routing states, for a syncopated, “dragged” feel.

### B. **Punch, Uniqueness, and Percussive Edge**
- **Utilize Linear/Constant Loudness Modes:** Switch to constant loudness for punchier transitions between voices/samples—good for kick/snare/hard-edged effects.
- **DC Offset for CV Drum Triggers:** Enable the per-channel +5V DC offsets to generate stored modulation voltages or to trigger drum modules directly from Synapse outputs in sequence.
- **Click-Less vs Clicky Switching:** For extreme glitch-cuts, disable click-less switching: hard, abrupt transitions can be percussive; for smooth morphs, use click-less mode.

---

## Additional Creative Applications
- **Send different clock sources (divided/multiplied) to Advance and Scatter to force rhythmic “accidents” and emergent grooves.**
- **Randomize memory or LFOs during live performance to “fracture” a repeating groove into experimental fill territory.**
- **Sum Outputs for Layered Complexity:** Use 1+2 and 3+4 sums to fuse complex layers—send to different FX for chaos, then blend for even denser percussion beds.
- **Use as a Voltage “Rhythm Programmer”:** The module’s stored voltages and DC-offset mode can sequence other modules or modulate percussion synths in odd patterns.

---

## Sound/FX Uniqueness
Even though Synapse is not a voice or effect, it can radically alter the context, groove, and impact of percussive sounds. Inserting the Synapse between sources and the mixer or FX can make “safe” or repetitive rhythms explode into new domain—shattered, morphing, spatially redistributed, and re-contextualized.

---

## Reference

- [Qu-Bit Synapse Manual (PDF)](https://cdn.shopify.com/s/files/1/0660/7545/files/Synapse_Manual.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
