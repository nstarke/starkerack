# Intellijel — Metropolix

- [Manual PDF](../../manuals/metropolix_manual_v1.4_2022.04.04.pdf)

---

[Metropolix Manual PDF (Firmware 1.4)](https://intellijel.com/downloads/manuals/metropolix_manual_v1.4.pdf)

---

# How to Create Full-Length Songs with Intellijel Metropolix

The **Intellijel Metropolix** is not just a step sequencer—it’s a deeply performative, compositional instrument, designed to generate, modulate, and structure evolving sequences. To move beyond cool grooves and into “full songs”, you need ways to introduce **variation**, **structure**, and **performability**. Here’s an analysis of strategies, techniques, and creative workflows using the Metropolix in combination with other Eurorack modules.

---

## Core Features for Song Creation

**Metropolix** includes:

- **Two independent, deeply modifiable pitch/gate tracks** (TRK 1 & 2)
- **Eight simultaneous MOD lanes** for internal/external modulation of virtually any parameter (think: automation lanes)
- **64 presets & 8 chainable preset banks** for “scene” or section switching
- **Extensive randomization, probability, accumulation (transposition), and ratcheting**
- **CV/AUX inputs & CTRL knobs**—modulate parameters live or from other modules
- **MIDI I/O (USB)** for clocking, sync, and DAW interaction
- **Loopy mode** for live improvisation, fills, and on-the-fly rearrangement

---

## Techniques for Building Full-Length Arrangements

### 1. **Preset Chaining: Sections and Song Forms**

**Preset Chains** allow you to structure a full set or song from 64 sequence/preset “scenes” (Intro, Verse, Chorus, Bridge, Fills, etc.).

- **Design each section** as its own preset (melodic material, rhythm, modulation, mutes).
- **Chain them together** in the Preset Chain screen: select bank/color, slot, how many times it repeats, and which tracks or MOD lanes are muted for each section.
- **Automate evolutions**—for example: “Verse 1” is sparse, “Verse 2” brings in MOD lane-driven variations, “Chorus” changes track lengths or swing.
- **Instant/multibar transitions**: Use ‘Total Pulses’ or ‘Queue Pulses’ in global setup so transitions happen after a musical amount of bars, ensuring smooth phrase changes.

> **TIP:** Think of Preset Chains as a non-linear DAW timeline—sections are linked, repeated, and can have their own muting, length, and arrangement logic.

---

### 2. **Song Variation via Modulation & Automation**

Most step-sequencers loop—the Metropolix becomes a song machine by using:

- **MOD Lanes**: assign to parameters like “root”, “order”, “length”, “slide”, “swing”, or external CV/gate outputs.
    - Evolve melodies by modulating scales, roots, or slide amounts per section.
    - Drastically alter grooves by crossfading between play orders or skipped steps.

- **AUX Inputs**: use LFOs, envelopes, a MIDI controller, or external modulation sources to:
    - Animate chord changes (assign a MOD lane, CTRL knob, or AUX input to “Scale (User)” or “Root”)
    - Create evolving bass lines/melodies by modulating “Pitch Pre”, “Pitch Post”, or “Accumulate”
    - Control fill triggers or mutes (assign to “Mute”, “Skip Invert”, or Loopy/Reset)
- **CTRL Knobs**: as performance macros—assign to modulate musical “scene” parameters, i.e., fade from straight rhythm to swung, change sequence lengths, invert play orders, etc.

> **Combine**: Use a function generator/envelope to open up filter cutoff, *and* turn up Metropolix “Gate Length” for a break, then snap both back for the drop!

---

### 3. **Live Improvisation: Loopy, Stage Player, and Performance Macros**

- **Loopy Mode**: Instantly “punch in” to a sub-loop, useful for breakdowns, fills, or live variations—repetition glues sections or provides surprise. Use 2-finger loopy for snare rolls or repeat phrases.
- **Stage Player**: Trigger individual steps as notes—use as manual fills, drum triggers, or soundboard during a jam.

---

### 4. **Randomization, Probability, and Generative Structure**

- **Per-stage Randomization** (ALT + AUX X/Y): Introduce subtle to radical variations in pitch, ratchet, gate type, probability, etc.
- **Probability**: Humanize or thin out sequences; assign probability to drum steps for swingy, “not-quite-the-same” patterns.
- **Accumulator/Transposition**: Diatonically transpose sequences automatically over time—mimic classic 303 and Berlin school sequences that “spiral upwards/downwards”.

---

### 5. **Integration with Other Eurorack Modules**

- **CV Clock & Reset**:
    - Use external clock for tight sync (DAW/Drum machine) or internal clock for hands-on jamming.
    - Insert clock dividers/multipliers upstream or downstream for polyrhythm/polymeter.

- **Envelope Followers/Gate Processors**:
    - Use logic (AND/OR/XOR), sequential switches, or gate mutes to route, combine, or remix Metropolix outputs for greater complexity.
    - Use switch modules to toggle voices, process triggers from MOD lanes or stage gates to switch basslines, melodies, or percussion on the fly.

- **Effects & VCAs**:
    - Automate or perform transitions/reverb/delay/fx on mix elements by assigning Metropolix outputs or MOD lanes (with gate or voltage CV) to FX parameters or mixer VCAs for dramatic effect.

- **Complex Voices, Filters, & Drum Modules**:
    - Route Track 1 and 2 as melody/bass, assign MOD lane (or even CV lanes as gates) to drum triggers or timbral modulation.

- **MIDI/DAW**:
    - Record pattern and preset transitions as MIDI notes or CC into your DAW, use DAW to sequence “meta” events.
    - Program external synths with MIDI output per track for hybrid setups; combine Metropolix generative structure with polished studio sound.

---

### 6. **Performance Strategy Examples**

- **“Mute Automation”**: Use preset chains or MOD lane automation to gradually build up/layer tracks for verse/chorus/bridge breakdowns.
- **“Scale/Chord Progression”**: Set up a mod lane to selection of custom scales/user banks; modulate with an LFO, envelope, or sequence for chord progressions and key changes.
- **“Polyrhythmic Evolution”**: Use different clock dividers and sequence lengths for each track/MOD lane; results in constantly shifting interplay.
- **“Live Remix”**: Randomize or morph certain step parameters via AUX Y or X in “ALT” mode for spontaneous, unrepeatable versions of your song.
- **“CTRL Knob DJ Moves”**: Assign one knob to “track swap,” “skip invert,” or “swing” for dramatic, drop-like moments or live breakbeats.

---

## Final Recommendations

- **Design Themes per Preset/Section:** Think of each Preset as a “scene” in the song.
- **Choreograph Macro Changes:** Use Preset Chaining for structure, MOD lanes for micro-automation, and CTRL/CV for live gestures.
- **Integrate Other Modules:** Use clocking, logic, CV processing, and effects for mixing/mastering-quality dynamics and transitions.
- **Perform and Record:** Use Metropolix as the live brains in a studio or on stage—capture its outputs directly or the MIDI for later multitracking.

With these capabilities, **Metropolix can drive a set that evolves, develops, and grooves as well as any computer DAW-based sequencer—each performance, even with the same presets, can be unique.**

---

## Further Reading

- [Metropolix Manual PDF (Firmware 1.4)](https://intellijel.com/downloads/manuals/metropolix_manual_v1.4.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)