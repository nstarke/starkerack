# Tubbutec — 6m0d6

- [Manual PDF](../../manuals/6m0d6-User-Manual-1.0.pdf)

---

[**6m0d6 by LPZW & Tubbutec User Manual (PDF)**](https://tubbutec.de/files/6m0d6_manual.pdf)

---

# Using the 6m0d6 Eurorack Drum Module to Create Full-Length Songs

## Overview

The [6m0d6](https://tubbutec.de/6m0d6/) is a highly flexible drum voice module inspired by the TR-606 but greatly expanded for Eurorack. With MIDI, CV control, multiple outputs, extensive sound-shaping, and dynamic response, the 6m0d6 serves as a powerful drum/percussion engine for modular compositions. However, the real artistry comes when you integrate its features to build not just loops, but song-length arrangements.

Below are strategies and patching ideas for using the 6m0d6—especially in combination with other Eurorack modules—to move from "great loop" to "full song".

---

## Main Approaches to Arranging with 6m0d6

### 1. **Section Building with Sequencer and Modulation**
- **Use Multiple Sequencer Patterns**: Pair the 6m0d6 with a Eurorack sequencer (e.g., Tubbutec 6equencer, Five12 Vector, or Hermod) to store and chain several drum patterns (A/B/C/Breakdown, etc.). Switch or morph patterns during performance or via CV automation to introduce variation.
- **Dynamic Accent CV and Modulation**: Take advantage of the dedicated Accent CV/gate and per-voice accenting for evolving drum dynamics. Use LFOs, random, or envelope generators to subtly (or aggressively) modulate the accent input, creating ‘loud/soft’ sections akin to verse/chorus.
  
### 2. **MIDI Control & External Automation**
- **MIDI Sequencing**: Send MIDI from a DAW or groovebox to trigger 6m0d6, drawing in song sections and automating parameters (e.g., snare decay for breakdowns, cymbal decay for build-ups) using MIDI CC messages.
- **Direct Metal Sound Performance**: Use the “Metal Sound” mode as a percussive synth voice, either for melodic bridges or synth breakdowns, with real-time or pre-programmed pitch and spread changes.

### 3. **Manual Control for Live Performance**
- **Mute/Solo via Outputs**: Use individual outs on the 6m0d6 with mixers/mutes (e.g., WMD Performance Mixer) to drop or bring in drum voices on the fly—classic for breakdowns, fills, and “drops”.
- **Hands-on Parameter Tweaks**: Morph drum tones (e.g., snare to bit-crushed, toms into subs, wild metal hats) by manipulating front panel knobs or assigning CV for automated sweeps. Plan knob turns for transitions between sections!

---

## Building Song Structure from Loops

Here's how to go from a 4-bar drum groove to a 4-minute track:

### **A. The Drum Skeleton**

- **Start Basic**: Program or sequence a base drum rhythm (kick, snare, hi-hat) for the core groove.
- **Output Routing**: Patch each drum to its own channel on your mixer or DAW for individual processing and arrangement control.

### **B. Sectional Variation**

1. **Drum Breaks / Fills**  
   - Use tricks like **changing the trigger length**, muting kicks or hats, and opening decay on snares/cymbals.
   - Metal/Cymbal voices can become melodic for intros or outros (“string synth” mode).

2. **Arrangement via MIDI/Sequencer**  
   - Preprogram verse, chorus, breakdown drum patterns.
   - Use MIDI CC to fade in metallic textures, reverb-like tom noise, or drive hats into distortion for climaxes.

3. **Modulation & Automation**
   - Patch a random voltage/LFO to accent amount or noise/metal parameters for evolving textures.
   - Cycle hat/cymbal swap for subtle rhythmic variation (toggle via gate sequencer or manual switch).

4. **CV-Controlled Transitions**
   - Patch envelope followers or dedicated scene-change LFOs to decay/time/metal spread for dramatic transitions.

5. **Mix Output for Arrangement**
   - Use the mixed output with additional FX (e.g., reverb, delay) controlled with a send/return mixer.
   - Pull elements out of the main mix (by plugging into individual outs) for “drop out” sections or build-ups.

---

## Example Patch: Creating a Song Structure

**Modules Used**:  
- 6m0d6 (drums/percussion),  
- Sequencer (e.g., 6equencer),  
- Modulation source (LFO/Random),  
- Performance Mixer,  
- Effects unit.

1. **Kick/Snare/Hi-hat sequenced for 32 steps, with variations every 8 steps.**
2. **LFO modulates snare decay and metallic spread for movement over time.**
3. **Accent CV receives stepped random for velocity/dynamics.**
4. **Manually switch CY.Pulse gate mode: intro with long cymbals → main groove with tight hits.**
5. **Bring in hats by patching individual out to a mixer channel.**
6. **Use MIDI to trigger melodic metal mode for bridge/break section.**

---

## Additional Creative Uses

- **Cymbal "Drone" or string-like textures** as ambient song sections.
- **Snare as a pseudo-melodic bit-crushed synth** for breakdowns.
- **Dynamic arrangement** via CV/audio-rate modulation of drum parameters.
- **Layered sound design** by processing individual outs with filters, distortion, or granular modules.

---

## Tips for Expanding Song Structures

- **Combine with other melodic modules:** route clock/modulation to melodic sequencers for synth lines that follow drum section changes.
- **Use sample/hold or random modules:** add non-repetitive fills or parameter changes that create “live” microswings and builds.
- **Transpose “metal” oscillators per section:** make the drum kit play “chords” or be tuned to the track's key for cohesion.

---

**[Read the official 6m0d6 manual PDF here](https://tubbutec.de/files/6m0d6_manual.pdf)**

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**