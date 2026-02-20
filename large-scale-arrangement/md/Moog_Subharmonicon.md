# Moog — Subharmonicon

- [Manual PDF](../../manuals/Subharmonicon_Manual.pdf)

---

[Moog Subharmonicon Manual PDF](https://www.moogmusic.com/sites/default/files/2020-05/Subharmonicon%20Manual%20052320.pdf)

---

# Making Full-Length Songs With Eurorack & the Moog Subharmonicon

The Moog Subharmonicon is a polyrhythmic, semi-modular analog synthesizer and sequencing platform, immensely powerful not just for composing loops, but for building performative, full-length pieces in a modular context. The following analysis highlights strategies, patch ideas, and compositional workflows for turning your Subharmonicon (along with other Eurorack modules) into a dynamic, performable “song-making” centerpiece.

---

## The Challenge: From Loop to Song

In modular synthesis, creating outstanding short patterns is straightforward, but dynamic arrangements, transitions, and song-like structures require careful planning or creative patching. Songwriting on modular is about evolving patterns over time, introducing variation, making transitions, and controlling sections—possibly by blending control voltages, logic, external sequencer control, or even hands-on performance.

### The Subharmonicon’s Strengths

- **Polyrhythmic Generators:** Multiple rhythm generators and sequence assignment (including polyrhythmic clocking).
- **Rich Sequencer Assignment:** Flexible assignment of sequencers to oscillators and subharmonics.
- **Analog and MIDI I/O:** DAW sync, external triggering, or internal clocking.
- **Extensive Patchbay:** Deep integration with Euro and other semi-modular synths (inputs/outputs for rhythm, sequence, triggers, envelopes).
- **Performable Controls:** Real-time hands-on tweaks (reset, next, envelope holding, sequence assignment toggles).

---

## Strategies to Build Full-Length Songs

### 1. **Song Structure via Polyrhythm & Sequence Assignment**
- **Vary Rhythm Generator Assignments:** Instantly change the 'feel' and length of a groove by reassigning rhythm clocks to sequencers during a performance. At key transition points, switch the polyrhythm sources, e.g., go from a simple clock to a dense polyrhythm for a "chorus" feel.
- **Transpose Sequences on the Fly:** Use external CV or MIDI (or another sequencer) to slowly move your sequence's key/root note over time—great for bridges or introducing new sections.

### 2. **Modular Control and Stage Transitions**
- **External Sequencer as Conductor:** Use a master (or companion) sequencer (like Pamela’s NEW Workout, Hermod, or even MIDI from a DAW) to control:
  - Clock/reset input for Subharmonicon.
  - Sequence/scale transposition via VCO 1/VCO 2 CV input.
  - Envelope, VCA, or VCF parameters for section-based timbral changes.
- **Manual Performance:** Use the EG, PLAY, RESET, and STEP buttons as live "scene" changes (e.g., holding EG for drones, using NEXT for step transitions, etc).

### 3. **Evolving Textures & Morphing Sections**
- **Patch External Modulation:** Use slow LFOs, Random modules, or stepped voltages (from modules like Maths, Batumi, Ornament & Crime, Tides):
  - Modulate Subharmonicon's mixer levels, filter cutoff, subharmonic ratios, or assign these modulations to different song sections with muted/unmuted CV inputs.
- **Audio-CV Cross-patching:** Patch envelope outputs and sub-oscillator outputs into other modules’ parameters, such as VCAs, filters, or effects.

### 4. **Arrangement with Muting, Mixing, and Layering**
- **External Mixer for Section Control:** Route individual VCO outputs (via patchbay) to a sequential switch, voltage-controlled mixer, or performance mute module. Crossfade/mute in different voices/subs for each section.
- **Separate Voices for Layers:** Use the patchbay to split out VCOs, Subs, or EGs to external signal paths—send to different FX or mix channels.

### 5. **Syncing and Integrating Other Sound Sources**
- **Drums/Percussion via DFAM:** Clock a DFAM or other drum module with a rhythmic output (CLOCK/TRIGGER/SEQ CLK) from Subharmonicon—sync drum breaks or big moments.
- **Mother-32 Integration:** Use Mother-32 for bass or lead, clocked by Subharmonicon for tight integration.

### 6. **MIDI and DAW Arrangement**
- **MIDI Clock Input:** Use a DAW or hardware MIDI sequencer as master clock, controlling when Subharmonicon’s sequencer starts, stops, resets, or reconfigures for song sections.
- **MIDI CC Morphs:** Automate filter cutoff, EG times, and oscillator frequency with MIDI CC sweeps to sculpt different song parts.

---

## Example Performance Song Structure Using Subharmonicon

| Song Part        | Control/Technique                                              |
|------------------|---------------------------------------------------------------|
| Intro            | Manual knob fade-in, subtle polyrhythm, single sequencer      |
| Verse            | Assign more rhythm generators, open up filter, add sub voices |
| Build/Breakdown  | Hold EG for drones, shift polyrhythm, modulate VCO freq w/ LFO|
| Chorus           | All rhythm generators, mixer full, bright filter resonance    |
| Bridge           | Reset both sequencers, switch clock source, transpose key     |
| Outro            | Gradually mute subs, close filter, decrease external FX send  |

---

## Combinatorial Patch Techniques

- Use [Matrix Mixers](https://www.doepfer.de/a138m.htm) to blend rhythmic or melodic outputs for evolving CV motion.
- Crosspatch envelope outputs to modulate external drum modules or effects (e.g. Lexicon PCM or modular reverbs for big moments).
- Patch Subharmonicon’s SEQ 1/2 out to quantizers or analog shift registers for generative melodies/harmony.
- Use logic modules (OR/XOR/AND) to create ever-changing trigger/gate combinations for dynamic song sections.

---

## Further Reading and Utilities

- [Subharmonicon Templated Patch Sheets (pdf, moogmusic.com)](https://www.moogmusic.com/sites/default/files/2020-05/Subharmonicon%20Manual%20052320.pdf)

---

## Conclusion

**Don’t be afraid to “play” the Subharmonicon as a live instrument:** changing assignments, polyrhythm divisions, patch routings, and muting voices for interactive, performative songwriting. Combine its unique sequencing, polyrhythm, and subharmonic structure with the rest of your rack for full-length modular compositions.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)