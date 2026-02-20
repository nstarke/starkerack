# Qu-Bit — Chord

- [Manual PDF](../../manuals/QB_Chord.pdf)

---

[Chord v2 Manual (PDF)](https://manuals.qubitelectronix.com/chord/Chord_v2_Manual_v2.01.pdf)

---

# Using the Qu-Bit Chord v2 for Full-Length Eurorack Songs

The **Qu-Bit Chord v2** module is not just a polyphonic oscillator, but a transformative tool for arrangement, harmonic development, and live performance in Eurorack modular systems. Below, I’ll outline strategies, patch ideas, and workflow enhancements to help you progress from interesting sketches to full-length modular tracks using the Chord v2 as a centerpiece.

---

## Overview – Why Chord v2 is Special

Most Eurorack modules focus on monophonic lines or simple layering. Chord v2, however, provides:

- **Polyphony:** Four voices, fully independent or harmonized.
- **Chord/Voicing/Quality Modes:** Enabling dynamic harmonic shifts (maj, min, 7th, etc.).
- **Waveform Diversity:** Analog, FM, organ, chiptune, or even user-loaded wavetables.
- **Sequencing & Modulation:** Each voice can be externally sequenced or collectively modulated.
- **Custom Chords/Wavetables:** Highly customizable with SD card support.

---

## Strategies for Songwriting & Arrangement

### 1. **Dynamic Harmonic Progression**

- **Technique:** Automate or sequence the **Quality** and **Voicing** CV inputs.
    - **Result:** Song sections can shift from major, minor, sus, diminished, to extended or custom harmonies.
    - **Pro Tip:** Use a voltage sequencer (e.g., Make Noise Pressure Points, Intellijel Metropolis) or step LFO to modulate chord type in real time for verse/chorus contrast.
- **Performance:** Manually switch presets or activate custom chords stored on the SD card for live jams.

### 2. **Voice Independence for Song Structure**

- **Free Poly Mode:** All four voices can be sequenced independently.
    - **Use Case:** 
        - Voice 1 → Bass (Root Output)
        - Voice 2 → Lead or pad (Third Output)
        - Voice 3 → Countermelody (Fifth Output)
        - Voice 4 → Accent/melody or rhythm (Seventh Output)
    - **Tip:** Use separate sequencers or channels of MIDI-to-CV. You can mute/unmute voices over time for breakdowns/builds.
- **Melody Mode:** Sequence a melody over a steady chord bed, using the Lead input to drive the seventh output.

### 3. **Textural and Timbral Variation**

- **Automation:** 
    - CV the **Waveform** and **Bank** parameters for movement between pure/warm/digital/lo-fi sounds. 
    - This allows you to define different song sections by timbral change alone.
- **SD Card Custom Wavetables:** Load unique wavetables for different “tracks” or song palettes.
- **CV Control with LFOs/Random:** Modulate waveform/bank with slow LFOs for evolving ambient tracks.

### 4. **Mix Automation and Section Transitions**

- **Triad Feature:** Toggle to remove the seventh from the mix output for cleaner, more focused sections (e.g., verses), then add it back for chorus density.
- **Manual Mutes:** Run the various outputs to a quad VCA or manual muting module (e.g., Befaco Muxlicer). Fade or mute individual voices for arranging peaks, drops, and transitions.

### 5. **Multi-Part Song Construction**

- **Sample & Hold or Sequential Switches:**
    - Use a S&H or gate sequencer to shift quantized root notes, chord types, or voicings as “scene” changes.
    - This can automate verse-chorus-bridge movement when synced to your master clock.
- **Scene Memory via Custom Chords:** Store unique chord forms on the SD card for instant recall.

### 6. **Integration with Drums, Percussion, & FX**

- **Rhythmic Modulation:** Use envelope followers or triggers from percussion modules to modulate Chord v2 parameters (FM, Quality, etc.), tying harmony to rhythm.
- **FX Chains:** Send Chord v2 outputs through different effects chains (delay/reverb for pads, distortion for leads, phaser on melodies), and use VCAs to bring effects in and out per section.

### 7. **Using LFO Mode for Modulator Tracks**

- Enable **LFO_MODE** via config.txt to turn outputs into synchronized or harmonically related LFOs.
- Modulate filter cutoffs, delay times, or other parameters elsewhere in your rack to achieve complex, evolving arrangements tied to the harmonic base.

---

## Example Patch Workflows

### Live Ambient Song (Evolving Harmonic Drone)

1. Set Harm to Major or Minor, automate Quality for chord progression.
2. CV-modulate waveform/bank with slow, out-of-sync LFOs.
3. Use all four outputs routed to a quad reverb or panning VCAs for spatial movement.
4. Manually switch to user chords or banks for “movement” between verses and chorus.

### Beat-driven Track with Song Structure

1. Root output → Bass voice, Fifth → Lead synth, Third and Seventh → pad/texture voices.
2. Drum triggers sent to sequential switches to change quality/voicing per 16 bars.
3. Use Triad toggle and VCA mutes for breakdowns/drops.
4. Sequence Lead output independently for melody sections using external sequencer.

---

## Final Advice

- **Pre-plan song “scenes” (verse, chorus, bridge) using custom chords or user wavetables.**
- **Use CV-mapping to tie harmonic change to other musical events (gates, triggers, or modulation).**
- **Leverage modularity: let the Chord v2 handle harmonic and timbral evolution, freeing up other voices for rhythm, bass, or melodic improvisation.**
- **Record multi-track and arrange in a DAW, or automate modular performance tools for live arrangement.**

---

### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)