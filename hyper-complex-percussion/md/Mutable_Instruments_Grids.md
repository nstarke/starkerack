# Mutable Instruments — Grids

- [Manual PDF](../../manuals/Manual - Mutable Instruments Grids Documentation.pdf)

---

[Mutable Instruments Grids Official Manual (PDF)](https://mutable-instruments.net/modules/grids/manual.pdf)

---

# Advanced Guide: Generating Dense, Hyper-Complex Percussion with Mutable Instruments Grids

Mutable Instruments Grids isn't just a generative rhythm box—it's a morphing, data-driven percussion brain designed to go way beyond standard "groovebox" duty. Here we'll detail power-user techniques for creating dense, intricate, polyrhythmic, and truly hyper-rhythmic sequences, perfect for advanced eurorack percussion architectures.

---

## Super Dense & Complex Rhythms: Key Concepts

**1. Master the Map Interpolation:**  
- Use both the **X (Map X)** and **Y (Map Y)** coordinates to explore spaces between genre-derived rhythm clusters.  
- Slowly modulate these with looping or random CV (e.g., from LFOs, sequencers, chaotic sources) to glide between straight, swung, and complex patterns without losing groove.
- Morph the map during performance—this results in smoothly evolving variations that remain musically useful.

**2. Fill Parameters for Hyper Activity:**  
- Crank **E1, E2, E3 (FILL)** towards max for each channel to increase note density.  
- Assign random or complex stepped CV to these FILL controls for on-the-fly, unpredictable 'density bursts.' The result is frantic, IDM-like drum fills and breakdowns.
- For *hyper-complexity*, sequence or modulate all three FILLs differently. This makes kick, snare, and hats clash in unpredictable, non-linear ways—ripe for polyrhythm.

**3. Inject Chaos (Controlled Randomness):**  
- The **CHAOS** control adds random hits like rolls and ghost notes.  
- Assign an LFO or smooth random CV here for dynamic, living patterns.  
- In *swing* mode, CHAOS morphs into a groove controller—highly useful for unnatural off-grid jitter.

**4. Use CV for Everything:**  
- All prime Grids parameters (X, Y, CHAOS, FILL1/2/3) are CV-controllable (0-5V).  
- Try sample-and-hold, stepped random generators (e.g. Turing Machine), or evolving LFOs for shifting, unpredictable rhythms.
- Clocked step sequencers can control map or fill values for planned polyrhythmic evolution.

**5. Clock Division & Polyrhythm:**  
- Use odd/even, uneven, or modulated external clocks (especially when pairing with sequencer modules).
- Grids supports various clock resolutions: 4, 8, and 24 ppqn. Lower resolutions create quantized, jagged patterns—great for “wrong” feels.
- Try clocking Grids with one tempo, but run non-matching sequencers (e.g., a 5-step or 7-step melodic sequencer) against it for polyrhythmic, cross-beat magic.
- In **Euclidean sequencer mode**, set different cycle lengths (C1, C2, C3) per channel for classic additive polyrhythm. Modulate these cycle lengths with CV for generative polyrhythms.

**6. Accent and Gate Tricks:**  
- ACCENT outs highlight structural points; use these to trigger additional percussion, modulate effects, or clock further modules.
- Switch TRIG to GATE mode for long percussive envelopes; great with LPGs or VCAs for organic clacks and snaps.

**7. Use with Unconventional Sound Sources:**  
- Instead of classic drums, trigger noise, metallic resonators, or granular synth voices.
- Send triggers to envelope generators controlling everything from distortion to filter cutoff for unique percussive synth lines.

---

## Unique, Punchy, Percussive Tips

- Pair Grids with analog stompboxes (e.g., compressors, distortion) following its trigger-outs to create body and edge.
- Mult the trig/acc outputs: One to a drum voice, one to clock a rhythmic modulation (tempo-synced LFO for filter FM).
- Randomize swing in real time: Switch **CHAOS** to swing, then sweep the amount during performance.
- Invert or process CV controlling FILL for reverse or stuttering effects—use with a slew/lag processor for gliding fills.

---

## Example Patch: Ultimate Polyrhythmic Grid

1. **Set Grids to Euclidean Sequencer Mode** (see manual).  
2. Set each channel's cycle length to a different prime number (e.g., C1=5, C2=7, C3=11).
3. Modulate each FILL input with different slow random LFOs.  
4. Patch triggers to drum voices—experiment with atypical sources (resonators, LPGs, granular synths).
5. CV-control Map X/Y with random voltages to interpolate between different rhythm genres.
6. Use ACCENTS to clock a voltage sequencer modulating reverb/delay time for spot FX on important hits.
7. Clock Grids with irregular pulses from another module for extra time signature weirdness.

---

**Manual Download:** [Mutable Instruments Grids Official Manual (PDF)](https://mutable-instruments.net/modules/grids/manual.pdf)

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**