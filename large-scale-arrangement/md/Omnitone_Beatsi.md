# Omnitone — Beatsi

- [Manual PDF](../../manuals/Beatsi_Information_Package.pdf)

---

[Download the Beatsi Manual PDF](attachment:Beatsi-Information-Package.pdf)

---

# Using Beatsi to Build Full Length Eurorack Songs

Transitioning from powerful modular patterns to full-length, evolving songs is a challenge every Eurorack artist faces. The Beatsi module, with its digital modular drum synthesis, versatile CV assignments, and performance-oriented design, can be your core rhythmic tool. Below you'll find approaches and creative strategies for integrating Beatsi into dynamic, song-length structures, working together with other modules.

---

## Core Features for Song Structure

- **Three Kits, Seamless Morphing:** Acoustic, lo-fi, and alien kits offer a palette for evolving your drum sound over time. Timbres can be morphed, allowing gradual changes in energy and style.
- **Deep CV Modulation:** Every parameter (timbre, pitch, decay, level) for every drum voice is assignable to CV1/CV2, enabling complex, synchronized changes from sequencers, LFOs, or random generators.
- **Fast State Saving:** Performance tweaks and muting are saved automatically—useful for live improvisation or composing without interruption.

---

## Techniques for Writing Full Length Songs

### 1. **Section Development with Kits and Timbral Morphing**
- **Automate Kit Switching:** Use CV modulation or manual parameter changes to move from one kit (e.g., acoustic/intro) to another (alien/climax) over the course of a track.
    - Example: Start your song on the orange kit, transition to the blue for a breakdown, and launch into green for a final chorus/drop.
- **Morph Timbres with CV:** Assign an LFO or slow envelope to timbre, pitch, or decay parameters to create evolving drum atmospheres or smoothly transition between sections.

### 2. **Dynamic Rhythmic Evolution**
- **Variation via CV:** Assign sequencer tracks, random voltage sources (e.g., Wogglebug), or manual controllers to Beatsi’s parameters for dynamic, living rhythms.
- **Accent and Fill Programming:** Use external sequential switches or trigger sequencers to selectively re-route triggers, muting and unmuting kit pieces, simulating classic "fill" behavior at the end of phrases.

### 3. **Song Arrangement with Mutes and Triggers**
- **Manual Performance Muting:** Quickly mute/unmute drum voices by pressing parameter and value knobs, introducing breakdowns or drops.
- **Trigger Programming:** Feed Beatsi with complex trigger patterns from Euclidean sequencers, clock dividers, or burst modules to shift between regular grooves and complex fills/breaks.

### 4. **Integrating with Melodic and Harmonic Elements**
- **Synchronized Modulation:** Use the same CV source (e.g., a global envelope or LFO synced to your master clock) for timbral changes on Beatsi and filter cutoffs or oscillator tuning elsewhere in your system. This ties your drum evolution to melodic or harmonic content.
- **Polyrhythms and Polytempo:** Use multiple clock sources/trigger patterns to make your drums interlock with non-drum modular voices in complex, ever-evolving ways.

### 5. **Automated Transitions and "Scenes"**
- **Preset State Saving via Manual Automation:** While Beatsi doesn’t offer preset recall, its "wait 5 seconds" auto-save means you can manually evolve settings between scenes, then transition smoothly with other modules similarly set up.
- **CV Scene Morphing:** Patch a voltage "preset manager" (like Malekko Voltage Block, VPME T43, or SSSR Labs Matrixarchate) to send different fixed or evolving voltages to Beatsi’s CV inputs, instantly shifting the drum sound in sync with other changes in your patch.

---

## Example Full Song Workflow

1. **Intro:** Beatsi kicks and hats only, orange kit, long decay, sparse triggers from a simple sequencer.
2. **Build:** Morph to blue kit while modulating snare decay and pitch with envelopes/LFOs. Add in tom and crash pieces, open up using more complex trigger patterns from burst generators.
3. **Drop/Chorus:** Green kit, quick decay, heavy modulation on crash and hats, triggers from main sequencer plus manual fills, melodies and basslines open up in sync.
4. **Breakdown:** Drop out kick and hats using muting, morph to blue kit. Decay down trigger activity in external sequencers and slow envelope to reduce energy.
5. **Finale:** Bring all kit pieces back in, morph through timbres, automate return to orange kit for a cohesive outro.

---

## Bonus Tips

- **CV Randomization:** Occasional random CV to Beatsi’s parameters, especially timbre and decay, can add "human" feel and unpredictability.
- **Performance Control:** Use tactile controllers (like Mutable Instruments Pressure Points, Planar, or Tetrapad) for instant live changes.
- **Combine with Samplers:** Layer Beatsi’s synthetic drums with sample-based drums using an external sampler (like Erica Sample Drum) for depth and complexity.

---

By leveraging Beatsi’s deep CV integration, kit morphing, and clever parameter assignments, you’ll unlock evolving drum parts that grow, breathe, and transform to create full, expressive modular songs.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)