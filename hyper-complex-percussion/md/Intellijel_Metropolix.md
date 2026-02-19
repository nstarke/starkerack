# Intellijel — Metropolix

- [Manual PDF](../../manuals/metropolix_manual_v1.4_2022.04.04.pdf)

---

[**Intellijel Metropolix Manual (PDF)**](https://intellijel.com/downloads/manuals/metropolix/Metropolix-Manual-1.4.0.pdf)

---

# Making Dense, Complex Rhythms & Percussion with Metropolix

The **Intellijel Metropolix** is not a voice or effect, but a hyper-flexible, hands-on, performance sequencer. While it excels at melodic and harmonic applications, it’s also a secret weapon for *dense, hyper-complex percussion sequencing* and wild polyrhythms, particularly when pushed beyond "melody sequencing" into the gates, modulation lanes, and probability systems.

Below are approaches and creative techniques for generating the kinds of percussion complexity you’re after—think ever-twisting hats, polymetric kick/snare arrangements, and grid-melting percussive patterns.

---

## Key Metropolix Features for Rhythm Complexity

- **Per-Stage Pulse Count (PULSE COUNT switches):** Set the number of clock pulses each stage persists, per stage. Use odd/even numbers for polyrhythms.
- **Per-Stage Gate Type:** Each stage can be a HOLD, MULTIPLE, SINGLE, or REST—customizing the gate pattern drastically on a stage-level.
- **Two Note Tracks + 8 MOD Lanes:** Layer multiple polyrhythmic tracks and clock-divided MOD lanes for more complexity.
- **Playback Order/Direction (ORDER):** Use Linear, Jump, Odd/Even, Shuffle, Random, Pendulum, Converge, Diverge, and other orders for pattern mutation.
- **Ratchets:** Per-stage bursts of gates for fast rolls, digital "fills", broken rhythms.
- **Clock Division/Multiplication (DIV):** Per-track clock division for polymetric layering.
- **Probability (PROB):** Per-stage chance of gates firing, for evolving/dense or sparse rhythms.
- **Skip (SKIP):** "Mute" or "drop out" steps instantly, per stage.
- **Manual and Mod Lanes CV sequencing:** Send CVs to percussion module parameters or even trigger sequencing on drum synths.
- **Preset Chaining:** Build song-like macro-structures with variations and transitions.

---

## Practical Steps & Eurorack Patch Methods

### 1. **Polyrhythms and Polymetric Sequences**

- **Pulse Count per Stage:**  
  Assign prime/odd numbers to different stages (e.g. 3, 5, 7, mixed with 2, 4) on Track 1 and Track 2 to immediately create rhythm cycles that drift in/out of phase.
  - *Example:* Set Track 1 to 5 pulses, Track 2 to 7 pulses. Use each to trigger different voices or percussive elements.

- **Track Clock Division (DIV):**  
  Assign different clock divisions to Track 1 and Track 2. E.g. Track 1 = /3, Track 2 = /5.  
  - Send their gate outputs to percussion voices (kick, snare, hats—that's three rhythmic layers out of sync).

### 2. **Complicated Gate Patterns & Sequence Shapes**

- **Random, Shuffle, Jump Orders:**  
  In the ORDER menu, use "Random" or "Shuffle" for generative (non-repeating, chaotic) patterns, or use other non-linear playback orders to build unpredictability.

- **Skip, Probability, and Ratchets:**  
  - "Edit+SKIP" to drop out hits for shuffle/funk/dub-type grooves.
  - "Edit+PROB" to set chance-per-stage for further rhythmic mutation—setting some triggers to 70%, some to 30%, etc.
  - "Edit+RATCH" to add bursts or retrigs (for rolls or glitch-cuts).

### 3. **More Voices: Using MOD Lanes for Percussion**

- **MOD Lanes as Multi-Track Trigger Sequencers:**  
  Assign MOD Lanes to OUT A/OUT B set to GATE toggle mode (see `Assigning a MOD Lane to an OUT Jack`). Patch these to trig inputs of additional percussion voices (clap, rim, sample module, synth percs).
  - Each MOD Lane can have its own ORDER, LEN, and DIV—polyrhythms galore.
  - Stagger MOD Lane lengths and divisions for never-repeating / slow-evolving grids.

- **MOD Lanes as CV Modulators:**  
  Use lanes to modulate pitch, decay, or timbre parameters of drum modules/digital/hybrid percussion.  
  - *Tip:* If your drum module is sensitive to CV, use the MOD Lane’s `Ramp`/`Step` transitions for continuously morphing percussive timbres.

### 4. **Preset Chaining & One-Shot/Variation Patterns**

- **Build Preset Chains** for song sections or dramatic transitions.
- Chaining can be used to alternate between different time signatures, polyrhythmic schemes, or "fill" oriented presets every N cycles.

### 5. **External Manipulation & Self-Modulation**

- **AUX Inputs:**  
  Feed random/synced/chaotic CVs or gates into the X, Y, Z jacks. Assign them to control Probability, Pulse Count, Play Order, pattern Mutation, or even Reset.
  - This is killer for live reactivity or external modulation from other sequencers/LFOs.

- **CTRL Knobs:**  
  Assign to swing, stages, order, clock division, or probability for macro-level rhythmic morphs in a live or improvised context.

- **Self-Modulation:**  
  Assign MOD or AUX to modulate track clock div, swing, or probability, so the grid is forever changing.

### 6. **Sequencing Complex Drum Channels**

- **Metropolix as Brain for a Drum Rack:**  
  Route TRK 1 GATE OUT, TRK 2 GATE OUT, and MOD LANES (set as GATE, sent via OUT A/B) to drum modules, even combining as AND/OR triggers or layering.
- **Use probability and ratchets in percussive voices:**  
  Percussion voices often benefit from randomization, glitch, and dense trigger bursts.

---

## Bonus Tips for Unique, Punchy, Percussive Results

- **Use Swing (per-track):** Crank it for drunken or unquantized grooves.
- **Ratcheting (gate stretching ON/OFF):** Create different microtiming feels for every drum sound.
- **Stage Offset/LEN Tricks:** For "shifting" polyrhythms.
- **Preset Morphing on the Fly:** Use latching/preset loading (with queue or pulse delay) to launch fills and variations live with tight sync.

---

## Example Eurorack Percussion Patch Flow

```
TRK 1 GATE OUT -> Kick voice trig
TRK 2 GATE OUT -> Snare voice trig
OUT A (MOD Lane 1 GATE) -> Hi-Hat (clock-divided)
OUT B (MOD Lane 2 CV) -> Mod CV to percussion sample slot or decay
AUX IN -> Probability, RATCH, or Order (external chaos!)
```

---

### References

- [Full Metropolix Manual (PDF)](https://intellijel.com/downloads/manuals/metropolix/Metropolix-Manual-1.4.0.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

#### Want more patches or ideas? Let me know your goals or the rest of your system and I can give patch-specific strategies for your drum modules or external effects.