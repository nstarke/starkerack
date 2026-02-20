# Tiptop Audio — HATS808

- [Manual PDF](../../manuals/Tiptop_Audio_HATS808_ns.pdf)

---

[HATS808 Manual PDF](https://tiptopaudio.com/manuals/HATS808_manual.pdf)

---

# Using the Tiptop Audio HATS808 to Create Full Length Songs in Eurorack

The Tiptop Audio HATS808, as described in the [manual](https://tiptopaudio.com/manuals/HATS808_manual.pdf), is a faithful analog clone of the TR-808 hi-hat section with several creative enhancements for modular users. While most modular enthusiasts can quickly patch up an exciting beat, evolving that beat into a structured, full-length track is more challenging. The following analysis provides strategies to leverage the HATS808—and its unique features—in conjunction with other modules to compose dynamic, long-form electronic music.

---

## Key HATS808 Features for Song Creation

- **Independent Accent and Level Controls**: Allows for nuanced dynamic control, essential for arrangement and movement.
- **Choke Function**: Adds interactivity and organic variation between open and closed hi-hat patterns.
- **Voltage-Controlled Resonance (Q) & VC-Q Input**: Enables hands-off, evolving textures and timbral changes.
- **Enhanced Gain Stages**: Facilitates drive/distortion for energetic breaks or transitions.
- **Bandpass Output**: Offers a raw source for further processing—ideal for creative layering or custom percussion.

---

## Techniques for Song Structure & Progression

Below are patching and performance ideas, organized around typical song sections and transitions:

### 1. **Introduction/Breakdown**
- **Sparse Patterns**: Mute or reduce hi-hat triggers. Use low accent and level for a subtle, percussive texture.
- **Filtered Texture**: Patch the Bandpass OUT to a VCA controlled by a slow LFO or envelope for swelling hi-hat "wash" effects.
- **VC-Q Automation**: Modulate Q (via sequencer or envelope) for tonal sweeps, evolving the high-frequency content over time.

### 2. **Building Energy (Verse/Pre-Chorus)**
- **Accent Sequencing**: Use a trigger sequencer (e.g., Euclidean circuits or random gates) to selectively accent certain hi-hat hits, creating syncopated, dynamic lines.
- **Choke Transitions**: Exploit the choke circuit to tighten up the groove, especially when switching from open to more closed hi-hat patterns.
- **Resonance Animation**: Slowly increase the Q via manual control or sequencer CV to introduce metallic overtones, signaling a build in energy.

### 3. **Chorus/Drop – Maximizing Impact**
- **Hot Gain Settings**: Push both Level and Accent to max for aggressive, cutting hats in the mix.
- **Layered Processing**: Split the output—send main OH OUT to the mix and Bandpass OUT to parallel FX (phaser, distortion, etc.) for a multi-layered hi-hat stack.
- **Complex Modulation**: Patch a random or envelope-driven CV to VC-Q, creating "alive" hi-hats that change character every bar or phrase.

### 4. **Breakdown/Bridge**
- **Automated Silence**: Use a sequential switch or clock divider to rhythmically mute the HATS808, or modulate a VCA for manual stutter or gating effects.
- **Slow Choke Decay**: Disable the choke for long, washed-out open hats, or enable and experiment with envelope times for syncopated gating.

### 5. **Outro**
- **Decaying Brightness**: Gradually lower LEVEL and ACCENT, while automating a decrease in Q—softening the hats into the background.
- **Creative FX**: Process the Bandpass OUT with heavy reverb or delay for trailing, ghostly textures.

---

## Making Parts Evolve: Song Form Tactics

- **Scene Progression**: Use sequencers or manual switches to introduce new hat patterns for verse, chorus, and fills.
- **Dynamic Accents**: Change the accent pattern to differentiate sections—e.g., keep accents on every offbeat in the verse, then on every 4th in the chorus.
- **Manual Performance**: Use the front panel controls—LEVEL, ACCENT, Q—to "play" dynamics and timbre live, making the arrangement feel performed, not static.

### Example Patch: Evolving Hi-Hats Through a Song

```
Kick & Bass
|
|---> Drum Sequencer --> HATS808 OH & CH Triggers
|       |                |     |
|       |                |     +---> Accent (trigger sequencer or hand-played for manual dynamics)
|       |                |
|       |                +---> OH OUT (main hats to mixer)
|       |
|---> Bandpass OUT --> VCA --> FX Chain (modulated by an LFO for swelling transitions or breakdown FX)
|
VC-Q IN <-- Envelope or sequencer CV for evolving resonance
```

#### **Song Progression Suggestions**
- **Intro:** Minimal triggers, low accent/level, some Bandpass FX for atmosphere.
- **Verse:** Steady hat pattern, light accent modulation, Q slowly rising.
- **Chorus:** Increased accent, higher level, aggressive Q, Bandpass OUT layered and prominent.
- **Bridge:** Alternate hats pattern, creative choke use, dramatic Bandpass FX (reverb/delay throws).
- **Outro:** Gradually reduce LEVEL/Q, filter-drenched Bandpass tail.

---

## Additional Module Combos

- **Sequential Switch/Matrix Mixer:** For switching between hat patterns or processing paths mid-song.
- **Complex Envelope Generators:** To modulate VC-Q or Level for evolving, expressive performances.
- **Probability/Gate Skippers:** Inject musical variation into patterns for more organic grooves.
- **Random/Noise CV Sources:** For subtle, continuous movement in resonance/tone.

### Pro Tip
Combine the HATS808 with clock dividers/multipliers to create polyrhythms or breakbeat fills, reintroducing the main groove with sudden accent/Q increases for impact.

---

By treating the HATS808 not just as a static drum voice but as a dynamic, CV-modulated instrument, you unlock the ability to shape and evolve your rhythm section—taking a simple hi-hat pattern to a full, expressive song structure. Use manual tweaks, sequenced CV, and modulation sources to automate changes that replicate the arrangement techniques familiar from DAWs but with the organic, tactile feel that only modular can provide.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)