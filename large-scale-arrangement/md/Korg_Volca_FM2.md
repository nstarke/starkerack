# Korg — Volca FM2

- [Manual PDF](../../manuals/volca-fm2_OM_EFGSCJ3.pdf)

---

[Download the Korg volca fm2 Manual PDF](https://www.korg.com/us/support/download/manual/0/897/4527/)

---

## How to Use the Korg volca fm2 in Eurorack Setups for Full-Length Songs

Turning modular jams and short loops into complete, evolving songs is a classic difficulty in Eurorack music production. The Korg volca fm2, though not a dedicated Eurorack module, offers unique tools for sequencing, sound manipulation, and integration with modular gear that can help bridge the gap between inspired loops and finished tracks. Here’s how you can maximize its potential in a modular system:

### 1. **Pattern Chaining and Section Creation**

**What volca fm2 offers:**
- 16 memory locations for sequence storage
- Chain function for consecutive playback of patterns

**How to use it:**
- Create short sequences (e.g. A: intro, B: main loop, C: fill, D: breakdown, etc.)
- Chain patterns (using the MEMORY + select buttons) to outline traditional song sections: intro, verse, chorus, bridge, etc.
- With precise timing and pattern design, you can form a full song structure controlled directly from the volca.

**In combination with other modules:**
- Use a sequential switch or clock divider/multiplier to create scene or section changes elsewhere in your rack in sync with the volca’s sequence chains.
- Trigger modulation changes, muting, or even preset changes on other modules as volca advances through sequences.

### 2. **External Clock and Synchronization**

**What volca fm2 offers:**
- SYNC IN/OUT (3.5mm jacks, compatible with Eurorack-level sync/trig with conversion cable)
- MIDI IN/OUT for tighter DAW or modular integration

**How to use it:**
- Use a master clock module or any modular clock source to drive the volca’s sequencer, making the entire rig play together.
- Conversely, if you’re writing on the volca first, use its SYNC OUT to advance gates, clocks, or triggers in your modular system to synchronize changes or modulations for different song sections.

**In combination with other modules:**
- Use clocked logic, switches, or matrix mixers to route rhythmic structure from the volca into triggering variations, fills, or scene changes in your rack.
- Send MIDI clock from your DAW to both the volca fm2 and a MIDI-to-CV module in your case for perfect tempo sync.

### 3. **Automation and Variation via Motion Sequencer**

**What volca fm2 offers:**
- Motion Sequencer for recording parameter automation to steps (modulation, filter, transpose, velocity)

**How to use it:**
- Use motion sequencing to vary timbre, filter cutoff, velocity, or pitch across steps, evolving patterns from simple loops to expressive sequences that “tell a story.”
- Automate transitions where chorus/verse use the same base pattern but with parameter shifts for energy and excitement.

**In combination with other modules:**
- Sample & Hold, slew limiters, or CV recorders in your modular rig can capture or add additional automation to CVs generated or synchronized with the volca.
- Use FX modules (delays, reverbs, granular) with CV-able parameters, having their modulation sequenced by clock divisions tied to the volca’s active steps or exports.

### 4. **Export/Import, Sound Design, and Evolving Timbres**

**What volca fm2 offers:**
- Easy saving/exporting of presets and sequences
- Full FM synthesis with 32 algorithms, per-operator editing

**How to use it:**
- Periodically change presets during performance via MIDI or program recall, shifting from clean bass to pads, sharp leads, or percussive FM noises in sync with section changes.
- Edit parameters on the fly: sweep algorithms, swap operators, or randomize parameters for breakdowns and buildups.

**In combination with other modules:**
- Voltage-controlled switches, MIDI Program Change via MIDI-to-CV, or manual macro control with a controller/sequencer in your rack can trigger these changes from the modular system.
- Use quantizers, envelope followers, or modular audio manglers to interact with the volca output, making each section’s timbre distinctly different.

### 5. **Utilizing the Sequencer as a Modulation Source**

- Use the volca’s sequencer’s clocked gates (seen as audio, envelope followers, or via MIDI notes) to trigger events in your rack for fills, mutes, or FX on downbeats or pattern changes.
- Use MIDI OUT on the volca to drive voices in your modular, layering external analog or digital voices with the volca’s own FM sounds for thicker arrangements.

### 6. **Live Manual Song Progression**

- Take advantage of the volca’s playability: switch sequences, mutate active steps, or hands-on knob-performs to “build” and “release” song sections in real time.
- This direct interaction translates well live, especially when paired with generative or probabilistic modules to supplement programmed structure.

---

## General Recipe for Song Form Using volca fm2 in Modular:

1. **Write basic patterns/sections** (16 slots).
2. **Chain patterns** to define song structure (intro, verse, chorus, break, outro).
3. **Sync** all gear via MIDI/SYNC.
4. **Automate** key parameters with motion sequences per section.
5. **Cue external events** in modular rack via gate/trigger/MIDI conversion for things like filter sweeps, FX, or drum fills when pattern changes.
6. **Evolve sounds** via CC/program changes, sound randomization, or layered voices.
7. **Perform manual changes**/play in real time for dynamics.

---

**For even more advanced processing, explore and script utilities using [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**