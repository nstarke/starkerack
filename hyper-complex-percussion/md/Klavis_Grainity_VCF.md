# Klavis — Grainity VCF

- [Manual PDF](../../manuals/Klavis_-_Grainity_User_Manual.pdf)

---

[**Klavis Grainity User Manual (PDF)**](https://www.klavis.com/all-products/grainity/grainity_user_manual_revA.pdf)

---

# Techniques for Hyper Complex, Densely Rhythmic Percussion with Klavis Grainity

The **Klavis Grainity** excels not only as a character-driven filter or effect, but as a tool for wild, complex rhythmic synthesis, especially when paired with Eurorack modulators, sequencers, and unconventional signal paths. Here's how you can exploit its architecture for polyrhythmic, percussive, and intricate patterns:

## 1. **Exploit the Granular VCF Cycling with External Triggers**

- **Percussive Input + External Triggers**: Route drum sounds, glitch samples, or noisy sources to Grainity's main input. Take clock, trigger, or gate patterns (from logic modules, sequencers, or polyrhythmic sources) into the **Detect** input. This decouples the rhythmic filter cycling from the audio input.
  - **Recipes:**
    - Use complex polyrhythmic gate streams (e.g., Euclidean, rotating clocks, or prime divisions) into Detect for variety.
    - Map two or more sequencers at different lengths (say, 5 and 7 steps) to produce interlocking rhythmic filter cycles.
- **Unique Effect**: Instead of regular cycling, Grainity advances filter structure steps every time the trigger/clock hits—great for granular stutter and unpredictable accenting.

## 2. **Layer Rhythms with the Division Parameter**

- The **Div** setting on the granular side multiplies the length of each step, making the filter "hang" on a structure stage for 2, 3, 4, up to 128 cycles.
  - **Modulate Div** with CV (again possibly from a stepped random, or a different modulator running in an odd-length loop) to vary subdivision lengths, breeding more complexity.
- Division CV tied to a stepped LFO or pattern sequencer further scrambles and syncopates the rhythm.

## 3. **Create Polyrhythm Through Chained Detect Inputs**

- Send one rhythmically complex voice (e.g., a bursty gate) to Detect and a totally unrelated percussive stream/audio to Main Input. The two will overlay, generating unique rhythmic filter gates and timbral "pulses."
- Intermodulation emerges especially if the two rhythms aren't simply related—excellent for off-grid, shifting patterns.

## 4. **Structure and Randomness for Pattern Mutation**

- **Structure Selector**: Using longer or odd-number length filter structures (3, 5, 7, 8-steps, especially from the Structure table), you introduce subharmonics, flips, and accent positions that don’t fit standard 4/4 grids. Each structure's step is essentially a "rhythmic accent" point.
- **Random Structures**: At the end of the list (shown with 'rX'), select algorithmically random step orders, making the rhythmically filtered output less predictable but musically complex.

## 5. **Phasing, Flanging, and "Percussive Movement" with Phase/Track**

- CV modulation of the Φ/Frq (Phase/Frequency) parameter (by a slow or stepped random generator) turns static patterns into morphing, flanging, and phasing rhythms.
- Use the **Track** mode to quantize filter cycling to musical intervals, creating layers of rhythmic ratios over your audio.
- For unison effects that vary with each hit/cycle, use phase-shift CV with irregular LFOs—great for chorus/flanger-enhanced percussion, injecting life and swing.

## 6. **Self-Oscillation for Filter-Voiced Percussion**

- On extreme resonance (self-oscillation), Grainity’s multimode and granular VCFs can act as tuned drum voices. Use V/Oct or FM with fast pitch envelopes or stepped CV for percussive, Zaps, or "pinged filter" sounds—with the granular section repeatedly cycling the core at strange rates.

## 7. **Mixing and Polarity Inversion for Texture and Impact**

- **Mix** output balances between the clean MultiMode filter and the wilder Granular filter. Automate via Mix CV: Realtime fade between two flavors of the same percussion or flip phase for punch-enhancing "thwacks" at pattern accents.
- Invert polarity (long press Type/inv button) to introduce phase cancellation tricks—sometimes creating sharp, cut-up staccato effects.

## 8. **Patch Ideas**

### A: **Polyrhythmic Percussion Bus**
- Drums or noise burst—> Main In  
- Two the clock/gate sources of prime length—> Mix (with one going to Detect)  
- Sequencer with polyrhythmic length—> Structure CV  
- Stepped random or LFO—> Div CV  
- Outputs: Take G.VCF and/or Mix to FX or direct to speakers.

### B: **Granular Filter Sequencer**
- Feed complex percussion loop to Main In.  
- Route a probabilistic trigger/gate pattern (from a burst generator or skipping clock divider) into Detect.  
- Manually or CV-sequence Structure for unpredictable filter patterns.  
- Modulate Phase/Frq and resonance for extra motion.

---

**For more creative patching and inspiration, refer to the full [Klavis Grainity User Manual PDF](https://www.klavis.com/all-products/grainity/grainity_user_manual_revA.pdf).**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
