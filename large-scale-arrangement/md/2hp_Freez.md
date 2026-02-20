# 2hp — Freez

- [Manual PDF](../../manuals/Freez_Manual.pdf)

---

[**Download the Freez Manual (PDF)**](sandbox:/mnt/data/Freez_Manual.pdf)

---

# Using the 2hp Freez to Craft Eurorack Full-Length Songs

## Introduction

The **2hp Freez** is a voltage-controlled locked looper and audio buffer/mangler module, capable of freezing, looping, mangling, and decimating incoming audio. It excels at turning short moments into continuously evolving audio, from beat repeats to granular glitches. While building strong loops is the heart of modular, the challenge is often **song structure**—evolving your sound beyond a loop or groove, introducing variation, breakdowns, and evolving textures over time.

Below are creative ways to use the **Freez**—especially in combination with other modules—to help sculpt a **full-length, evolving song** from your modular system.

---

## 1. **Layering and Re-sampling for Transitions**

**Technique**: Route sections of your patch (e.g., melodic phrases, basslines, or even percussion) into Freez at key moments. Use the **FREEZ** button or CV triggers to capture musical phrases or one-shot textures.

- **Transitions**: Freeze a melody, then mangle it with the **SIZE** and **S. RATE** controls, introducing bitcrushing/glitch effects for breakdowns, fills, or bridge sections.
- **Layering**: Duplicate your main loop; process one layer with Freez (chopped, reversed, decimated) for alternate “song sections” (verse/chorus).
- **Variation**: Use a sequencer or random CV triggers to capture/freeze at different places—every 16 or 32 bars—creating evolving motifs.

## 2. **Dynamic Song Structure Using CV Control**

**Technique**: Utilize **CV control** over **Size** and **S. Rate**. Modulate these with envelopes, LFOs, or sequencers synced to your song’s progression.

- **Verse/Chorus/Bridge**: Automate buffer size/sample rate for each song part. Example: larger buffer for chorus, smaller for verses, lo-fi grain for breakdowns.
- **Automation**: Sequence the **TRIG** input from your drum machine or sequencer to introduce/punctuate fills and transitions on the fly.
- **Timbral Evolution**: Slowly morph **Size** and **S. Rate** over time for evolving textures across the song, rather than static looping.

## 3. **Real-Time Sample Manipulation for Live Arrangement**

**Technique**: Use the **momentary/latching** mode toggle for performative capture and release.

- **Live Jams**: Momentarily freeze audio sections live and manipulate them for fills, breakdowns, or dramatic stops (e.g., momentarily freeze before song drop).
- **Latching**: Use for hands-free long sections—freeze a part for a verse, then unfreeze for chorus.
- **Trigger Input**: Automate these changes using CV or gates from your performance sequencer or DAW.

## 4. **Beat Repeat and Glitch Processing for Breakdown Sections**

**Technique**: Use the **lowest buffer size and sample rates** to create granular stuttering, beat repeats, and bit-crushed textures.

- **Breakdown/Build Up**: Suddenly reduce buffer/sample rate during breakdowns to fragment sound—great for electronic genres.
- **FX Sections**: Route only drums, or just vocals/instruments for glitch transitions or build tension before the next section.

## 5. **Complex Song Arrangements through Parallel Processing**

**Technique**: Use Freez in **parallel with dry audio**, switching/morphing between the two for A/B sections, using a VCA or mixer.

- **A/B Song Parts**: Alternate between dry signal and mangled, frozen audio for verses/choruses.
- **Evolving Pads/Textural Layers**: Loop ambient wash or granular pads captured by Freez, layered under changing melodies above.

---

## **Suggested Combinational Modules**

- **Sequencers**: Automate freeze, size, and sample-rate changes (Pamela’s New Workout, Hermod, Voltage Block).
- **Random/Probability Generators**: Use for unpredictable freeze events and textural variety (e.g., MI Marbles, Turing Machine).
- **Switches and VCAs**: Crossfade or switch between dry/processed signals, enabling quick song structure changes.
- **Additional Loopers/Delays**: Route Freez into other buffer-based FX for deeply layered songs.
- **Effect Modules**: Pair with reverb/delay/distortion after Freez for even richer transitions.

---

## **Example Routing for a Full-Length Song**

```text
Drums ───┬──────────────> Mixer ──> Out
         │
         └──> Freez (beat freeze/glitch) ──> FX ──┘

Bass  ─────────────> Mixer ──┤

Melody ──┬────> Freez (phrase capture) ──┘
         └────> Mixer (blend live/mangled)
```
- Use sequencer or LFO to trigger Freez for each song part.
- Use CV to morph SIZE/S. RATE per section.
- Crossfade between dry/mangled for structure.

---

## Conclusion

The 2hp **Freez** is a powerful weapon for moving past modular “loop lock,” enabling dynamic arrangement, live performance, and deep textural evolution—core to making modular songs that breathe and progress.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
