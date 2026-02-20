# Mutable Instruments — Braids

- [Manual PDF](../../manuals/Manual - Mutable Instruments Braids Documentation.pdf)

---

[**Mutable Instruments Braids Manual (PDF Download)**](https://mutable-instruments.net/archive/manuals/manual_braids_v1.8.pdf)

---

# Using Mutable Instruments Braids to Make Full-Length Eurorack Songs

Mutable Instruments Braids is a digital macro-oscillator with a huge sonic palette, lending itself to everything from simple mono synth basses to experimental soundscapes and drum hits. While it's easy to use Braids for a great loop, taking it from the "cool 16-step groove" to a dynamic, evolving song is the true challenge in modular. Here’s how to leverage Braids, plus a handful of other modules, to construct complete tracks.

## 1. **Braids as Your All-Purpose Voice**

**Braids covers an immense territory:**

- Percussive sounds (kick, snare, cymbal, drum, bell, pluck, noise, etc.)
- Lead and bass synths (classic analog, wavetable, FM, additive, formant/vowel, ring mod, waveshaping)
- Ambient textures and FX (granular, digital noise, drone, speech, QPSK, etc.)

**Why does this matter?**
You can actually use just Braids as nearly every "instrument" within your song structure simply by automating its model selection, CV controls, and patching its output in different ways.

---

## 2. **From Loops to Songs: Eurorack Arranging Techniques**

Here are concrete musical/patching techniques, paired with Braids features, for arranging a full-length song:

### A. **Automate Braids’ Sound and Role in Your Track**
- **Model Selection (META Mode):** Use the META mode so that CV into the FM jack scrolls through oscillator models. Use sequencers, LFOs with steps, or even manual control to shift Braids from, say, bass wavetables, to a pluck or drum sound, to granular/wind at different sections.
- **TIMBRE & COLOR Automation:** Patch envelopes, CV sequencers, or random/generative LFOs into these inputs to morph sound texture and modulate instrument characteristics within a phrase or section.

### B. **Layer Multiple Roles With Switches/Utilities**
- Use a sequential switch or manual switch to route Braids’ output, or a set of different CVs into its controls, to play different musical roles at different times (lead/bass/drum/textures).
- With mults/buffered mults, you can duplicate your pitch CV and envelope signals to send to Braids as it morphs roles.
- Sample & Hold + random modulation using sources like Mutable Marbles or Wogglebug keeps transitions interesting and organic.

### C. **Song Sections: Manual and Automated Structural Change**
- **Manual:** Move between Braids’ models by hand in performance, or fade between Braids, other oscillators, and voices using a crossfader module or mixer with mutes, to create song structure (verse, chorus, bridge).
- **Automated:** Use gate sequencers or clock dividers/multiplier modules to change what Braids is doing every 4, 8, or 16 bars: for example, trigger physical models with TRIG for hits, then switch to wave-based synthesis for melody.

### D. **Percussion Sequencing With Braids**
- Use a trigger/gate sequencer (or drum machine outputs) to excite Braids’ physical models (PLUK, BOWD, KICK, etc.).
- Use a second Braids instance (or another VCO for counterpoint) for melodic duties—consider sample-and-hold or quantized random for evolving melodies over time.

### E. **Building Evolving Arrangements**
- **Envelopes to Parameters:** Use a modulation matrix or lots of basic EGs/LFOs to automate TIMBRE, COLOR, FM for subtle or radical vibes.
- **Quantizer Integration:** Braids has a built-in quantizer. Use it for harmonically stable progressions, or disable for experimental.
- **Dynamic Range with Internal Envelope:** Use Braids' AD envelope generator to modulate output VCA and sound parameters, creating attack/decay and dynamic variation within notes or phrases.

### F. **Utilizing Effects and External Processing**
- Send Braids through filters, delays, reverbs, distortion, or granular processors as part of the performance/arrangement chain.
- Use mute switches, VCAs, or sequential switches for dropouts, breakdowns, and transitions.

### G. **Recording and Overdubs**
- Record individual Braids parts (bass, percussion, lead, FX) in sequence to a DAW or looper for multi-tracking, so you can focus on one musical element at a time.
- Use voltage-addressed switches or a matrix mixer for layering and re-arranging Braids' output live.

---

## 3. **Sample Arrangement Structure** *(all with a single Braids + utilities)*

| Song Section      | Example Braids Role                     | Control/Modulation         | Additional Modules                |
|-------------------|-----------------------------------------|----------------------------|-----------------------------------|
| Intro             | Granular noise or bell, text scroll     | CLOU/PRTC models, meta     | Clocked random/LFO                |
| Verse             | Subtractive synth lead, snare hits      | ZLPF/ZBPF/DRUM models      | Envelope to Color/Filters         |
| Chorus            | FM lead + KICK, thick wavetable bass    | FM, WMAP, KICK models      | Fast gates, envelope to VCA       |
| Bridge            | Swarm/supersaw, vowel drones            | /|/|/|/| and VOWL models   | S/H for pitch, slow LFO to Color  |
| Breakdown         | Granular reverb, resonant drums         | CLOU, BELL, DRUM           | FX send, sequencer to CV          |
| Outro             | Filtered noise, random melodic hits     | NOIS, WLIN models          | Random trig, quantizer            |


---

## 4. **Tips for Song-Structure and Storytelling**
- **Contrast:** Don't be afraid to go from thin/simple sound (one Braids) to multi-layered (Braids + FX + drum models), and back.
- **Surprise:** Automate model switches and parameters to create unexpected sound morphs, even within a section.
- **Performance:** Use Braids' click encoder and CV control to dynamically change roles in live sets—riff on your sequence and twist the sound as the story unfolds.

---

## 5. **Companion Modules to Consider**

- **Sequencers:** Eloquencer, Metropolix, Rene, or a simple trigger sequencer (for gates/triggers).
- **Utility:** Switches (e.g. Doepfer A-151), VCAs, attenuverters (Maths, MI Shades).
- **Random/Envelope:** Mutable Marbles, Pam's New Workout, Batumi, Zadar, Maths.
- **FX:** Clouds, Magneto, Mimeophon, or any multi-effect pedal/rack.

---

Braids’ flexibility, when combined with strategic control over its models, parameters, and external processing/sequencing, lets you create songs with true beginning, middle, and end—with evolving timbres, dynamic sections, and organic change.

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)