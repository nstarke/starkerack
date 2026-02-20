# Free Modular — Boost

- [Manual PDF](../../manuals/boost_manual.pdf)

---

[**Download the Boost Manual (PDF)**](https://nstarke.github.io/eurorack-processor/manuals/BOOST.pdf)

---

# Using the Boost Eurorack Module for Full-Length Song Creation

## Introduction

It’s common in Eurorack to get stuck on short loops—beats, basslines, and melodies that don’t evolve into a “song.” The Boost module is a deceptively simple analog tool that can be central to achieving movement, energy, and transitions throughout your performance. Below, I’ll outline creative ways to leverage Boost for song-length structure, dynamics, and transitions—especially in combination with typical Eurorack utilities.

---

## Key Features of Boost
- **26dB Gain / Gentle Distortion**: Adds punch, warmth, or aggression to any signal.
- **Tone Control**: Adjusts high frequency emphasis post-clipping—great for timbral shifts.
- **No CV Control**: Distortion amount can be modulated indirectly via pre-Boost VCAs/attenuators.

---

## Song-Length Techniques Using Boost

### 1. **Section Transitions (Verse/Chorus/Energy Changes)**
- **How:** Use a VCA or volume pedal before the Boost module. Automate CV to fade in more gain/distortion during choruses/big sections.
    - _Example Patch:_ Drum loop → VCA (CV from sequencer or LFO for transitions) → Boost
- **Result:** Huge, “lifted” sound on command. Pull back to clean for “verse,” and add Boost for “chorus” or “drop.”

### 2. **Dynamic Builds and Drops**
- **How:** Assign modulation sources (LFOs, envelopes, manual controls) to the VCA before Boost, increasing input gain as the song builds.
- **Tip:** Use the Tone knob to sweep from warm to bright as the build escalates.
- **Result:** Organic “tension and release” with both volume and timbral excitement.

### 3. **Automated Distortion for Drum Variation**
- **How:** Put percussion/bass through Boost, and automate the amount of distortion by sequencing VCA gain pre-Boost.
- **Result:** Create “gritty” sections, transition fills, breakdowns, or switch from clean to lo-fi/overdriven drums—without needing additional drum modules.

### 4. **Timbre and Texture Movement (Live Instrument Feels)**
- **How:** Use the Tone control as a performance control. Sweep it slowly during bridges, intros, or outros.
- **Result:** Keeps the same riff sounding fresh. Think of it like a subtle “filter sweep” but with harmonic overtones.

### 5. **Mix Bus Master Effect**
- **How:** Run your whole mix through Boost (be careful with gain!). Tame or hype the highs with Tone.
- **Pro Tip:** Patch a parallel dry/wet blend in a mixer for A/B-ing clarity versus saturation.
- **Result:** Live “mix bus glue” or excitement for the entire patch.

### 6. **Vocal/Speech FX for Narrative Flow**
- **How:** Use Boost to bring a vocal/voice sample forward for important sections by adding subtle drive and gain.
- **Result:** Gives spoken word, samples, or vocal chops a featured, punchy, modern feel.

---

## Combining Boost With Common Eurorack Modules

- **With VCAs/Sequencers:** Automate when and how “intense” a section feels, naturally building arrangement over time.
- **With Filters:** Post-Boost filtering can tame harshness or add movement. Modulate cutoff for ear-catching transitions.
- **With Modulators (LFOs, Envelopes):** Patch to VCAs or signal sources before Boost for living, breathing timbre changes.
- **With Delays/FX:** Distorted/boosted signals into reverb/delay are great for “exploding” breakdowns or spacey bridges.

---

## Patch Example: Song Structure Performance Rack

```plaintext
1. Percussion → VCA1 (sequenced gain) → Boost → Mixer
2. Bass → VCA2 (envelope modulated) → Boost → Mixer
3. Melodic synth → Filter → Boost → Mixer (Tone swept live)
4. Mixer → Reverb/Delay (FX)
5. Mixer Out → Final VCA (master volume/fade)
```

- **Transitions:** Use VCA1 & VCA2 CV sequences to automate “clean”/“overdriven” sections.
- **Improvisation:** Perform with the Boost’s Tone knob, or fade in more gain with external attenuators.
- **Full-Length Song:** Plan sequence variations, automating Boost involvement. Save “maxed” Boost settings for climaxes/outros.

---

## Summary

While Boost appears simple, its analog gain and tone sculpting can play a powerful role in moving from static loops to structured, exciting songs. Think of it as an expressive, performable glue module that bridges different sections and helps your modular “tell a story.”

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)