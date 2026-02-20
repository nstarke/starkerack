# Schlappi Engineering — 100 Grit

- [Manual PDF](../../manuals/100_GRIT_MANUAL_20190826.pdf)

---

[Schlappi Engineering 100 Grit Manual PDF](https://schlappiengineering.com/wp-content/uploads/2020/03/100GRITMANUAL.pdf)

---

# Creating Full-Length Songs with the Schlappi Engineering 100 Grit

The **Schlappi Engineering 100 Grit** is a unique distortion/filter/VCA module with interactive touchpoints and extensive internal feedback. While it excels at wild timbral transformation and audio-rate chaos, it can become a real asset for **composing and performing full-length songs in a Eurorack environment** if approached with intention and strategy. Below, I’ll break down techniques and patch ideas for sculpting a song’s structure, evolution, and dynamic range utilizing the 100 Grit in combination with other modules.

---

## 1. Dynamic Timbre and Song Structure

**A. Scene Transitions and Variation**

The 100 Grit’s extensive feedback normalization and touchpoint interactivity make it ideal for transforming a simple sound source (bassline, drums, lead, drone) into dramatically different timbres across a song.

- **Intro:** Use the filter section for subtle coloration; keep gain and resonance low for a clean, evolving sound.
- **Build-up:** Gradually modulate the resonance and/or add touchpoint manipulation for increasing intensity and harmonic interest.
- **Climax/Drop:** Flip the x100 GAIN switch, increase the distortion, and create aggressive resonance feedback for explosive energy.
- **Breakdown:** Reduce gain, sweep filter cutoff low, or use external CV to pull back energy, transitioning seamlessly to a quieter section.

**Automate these transitions via external sequencers, envelope generators, LFOs, or manual touchpoint performance.**

---

## 2. Live Interaction and Performance

**A. Touchpoints as Performance Macros**

The eight brass touchpoints act as macro controllers—grab, tap or connect pairs to introduce sudden timbral shifts or rhythmic artifacts. Combine this with **preset voltage recall** (via sequential switches or voltage-addressed attenuators) for moving between song sections.

- Sequence or randomly trigger alligator clips/patch cables to bridge points for “composed” chaos at specific moments.
- Use touchplates for live improvisation (think fills/breaks or textural flourishes in real time).

---

## 3. Integration with Other Utilities

**A. Voltage-Controlled Song Evolution**

- **Sequencer or Sample & Hold:** Modulate GAIN CV, RES CV, or Frequency input to have sections with very distinct sound palettes triggered according to song sections.
- **Clocked LFOs/Function Generators:** Slowly ramp filter cutoff or distortion level up and down through automation, dramatizing song contours.
- **VCAs/Envelopes:** Sidechain or duck the 100 Grit’s OUT or DIST output using envelopes from your drum section for “pumping” or breathing mixes.

**B. Audio Routing**

- Process drum buses, chords, basses, or even vocals through 100 Grit for sound “scenes.”
- Parallel process: Dry signal + 100 Grit DIST out, mixed via a crossfader or matrix mixer. Morph between clean and dirty sounds during the track.

---

## 4. Song Architectures

**A. Create Multi-Part Compositions**

- **Song Sections:** Arrange your song so that the 100 Grit is only in the signal path during certain sections (verse, chorus, bridge). Use sequential switches or VCAs controlled by your song’s sequencer/controller.
- **Motif Variation:** Send the same melodic or rhythmic material through 100 Grit in different ways per section—clean sequence becomes distorted sequence, filter sweeps punctuate transitions, etc.

**B. Generative or Evolving Patches**

- Utilize the feedback normalizations and touchpoint patching to slowly shift the system over time, so the patch naturally “composes itself” across a track’s runtime.
- Algorithmic sequencers or complex modulation sources (eg, Turing Machine, Marbles) can influence 100 Grit parameters, introducing non-repetitive evolution.

---

## 5. Patch Example: Evolving Groove

```text
1. Bassline and Drums → Mixer → 100 Grit IN 1
2. Melody or Texture → 100 Grit IN 2
3. Drums Sidechain Out → Envelope Follower → GAIN CV (for dynamic ducking)
4. Slow LFO → Frequency CV (subtle evolving tone color)
5. Song Section CV (from sequencer or manual trigger) toggles x100 GAIN switch via solenoid or mutable utilities.
6. Crossfade between OUT (cleaner) and DIST (wilder) for tension/release.
7. FX return: Touchpoints voltage-patched by sequencer for fills/breaks every 8 bars.
```

---

## 6. Additional Tips

- **Preset Management:** While Eurorack isn’t easily “presettable,” you can patch up the 100 Grit in multiple parallel chains and switch between them with a matrix mixer or switching module to recall distinct song sections.
- **Event Macros:** Pre-plan and score touchpoint manipulations as part of your song arrangement, treating them like instrument solos or drum fills.
- **Vocal or Sample Processing:** The 100 Grit’s distinct distortion/character can make for striking “chorus” effects or breakdown moments when applied to vocals or speech snippets.

---

## Final Thoughts

The 100 Grit thrives as both a timbral chameleon and a chaos generator. Its real power for SONGWRITING lies in using its dynamic routings (feedback normalizations), voltage-controlled parameters, and touchpoint performability to transform repeating modular loops into fully realized, ever-evolving musical compositions. With careful planning, modulation routing, and performance gestures, you can push your Eurorack system far beyond "loop mode" and into the realm of storytelling, drama, and dynamic, full-length songs.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)