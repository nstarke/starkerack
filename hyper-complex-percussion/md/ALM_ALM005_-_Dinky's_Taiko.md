# ALM — ALM005 - Dinky's Taiko

- [Manual PDF](../../manuals/alm005-manual.pdf)

---

[ALM-005 ‘Dinky’s Taiko’ Operation Manual PDF](https://www.busycircuits.com/docs/alm005-dinkys-taiko-manual.pdf)

---

## Using ALM-005 'Dinky’s Taiko' for Hyper-Complex, Densely Rhythmic Percussion

**Dinky’s Taiko** is a powerful, versatile digital percussion voice—the module's design and control layout offer many opportunities for advanced rhythm generation, punchy sounds, and evolving complexity. Let’s break down how to creatively exploit its features for polyrhythms, odd time signatures, and complex percussive textures.

### Key Sonic Manipulation Strategies

#### 1. **Trigger, Accent, Choke Inputs: Advanced Rhythm and Dynamics**
- **Multiple Gate/Trigger Sources:** Use different clock dividers/multipliers (e.g., Pamela’s Workout, Temps Utile, etc.) to send independent and polyrhythmic triggers to the main, accent, and choke inputs.
  - *Example:* Main trigger receives a 5-step sequence clock, accent receives a 3-step, choke gets a 7-step for cross/accented rhythms.
- **Accent for Dynamic Emphasis:** Program accent triggers for velocity/volume swings, or micro-rhythmic accents per beat or subdivided over a bar, to introduce organic feel or stuttering effects.
- **Choke for Stuttering/Stops:** Use choke triggers in fast polyrhythm or burst patterns to abruptly cut the tail of each sound, introducing complex gates/stutters.

#### 2. **Voltage Control for Morphing Patterns**
All key parameters take both knob and control voltage (CV) input:
- **Use CV Sequencing:** Modulate Spectrum, Release, Freq Start, Freq End, Speed, and Wave via step sequencers or LFOs clocked to different subdivisions/polyrhythms.
  - *Example:* Use a voltage block or similar CV sequencer in an odd pattern to shift noise and oscillator pitches every trigger, giving evolving, never-repeating hits.
- **Accentuate Polyrhythms:** Modulate Release or Mix with polyrhythmic LFOs for alternate bursts of noise/oscillator blends, changing tonality mid-pattern.

#### 3. **Mix and Output Section for Sonic Impact**
- **EQ (Tilt):** Automate via knob or CV for sweeps between bass-heavy and treble clicks, either per hit or morphing over a bar/groove.
- **Mix (Noise vs Osc):** Crossfade between digital noise and pitched elements using step-cv sources for variation within patterns (e.g., every 5th hit is pure noise).
- **Wave Selection:** Parameter lock or sequence the wave table per step to unlock glitched, FM, or snare-like percs in a single pattern.
- **HOT Output:** Use the “hot” (±10V) output to aggressively drive further (VCAs, wavefolders, or clipping) downstream for extra punch.

#### 4. **Make Use of Snapshot Behavior**
- When triggered, all parameters are “snapshotted”: automate fast parameter changes with synchronized, differently-phased steppers or random CV bursts.

#### 5. **Patch Tips for Complexity**
- **Layer Multiple Dinky’s Taiko or Other Percussion Voices:** Each voice on a separate clock division for overall polyrhythmic texture.
- **Percussive "Choke Networks":** Use the Choke output from rhythm module A to trigger Choke on Dinky’s Taiko when you want rhythmic “sidechaining” between voices.
- **Patterned CVs:** If using a matrix sequencer, assign different destinations to different polyrhythmic channels for ever-evolving movement.
- **Randomized Breaks:** Occasional random voltages on Wave/Release for fills or glitch moments within a defined structure.

### Sample Complex Patch Tree

- **Pamela’s Pro Workout (Master Clock):**  
  - Ch1: Main trigger (6/8)
  - Ch2: Accent (7/16)
  - Ch3: Choke (5/8 or Euclidean pattern)

- **CV Sequencer:**  
  - Out1: Modulates Freq Start (stepped, odd-length sequence)
  - Out2: Modulates Mix (random gates)
  - Out3: Modulates Wave (patterned morphing per beat)

- **Result:**  
  - Ever-shifting, evolving percussion, punchy with accents, chopped by choke, with spectra that slide and leap.

---

**For More Details:**  
- [ALM-005 ‘Dinky’s Taiko’ Operation Manual PDF](https://www.busycircuits.com/docs/alm005-dinkys-taiko-manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)