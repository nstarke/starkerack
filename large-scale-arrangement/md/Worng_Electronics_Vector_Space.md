# Worng Electronics — Vector Space

- [Manual PDF](../../manuals/Vector Space Manual v1.00.pdf)

---

[WORNG Electronics Vector Space User Manual (PDF)](https://www.worng.com.au/manuals/WORNG_Electronics_Vector_Space_Manual.pdf)

---

# WORNG Electronics Vector Space: Turning Modular Patches Into Full-Length Songs

## Overview

The WORNG Electronics Vector Space is a highly creative, purely analog module that expands three modulation sources into seventeen uniquely interrelated outputs. While its core function is modulation mixing, its depth allows for powerful control over generative structures, evolving textures, and structural changes — the very ingredients often missing in patches that don’t make it past looping grooves.

Below, you'll find ideas and strategies to unlock the Vector Space as a composition tool for *song-length structure* in a modular context. Each method pairs Vector Space's deep modulation possibilities with Eurorack staples (sequencers, VCAs, modulation sources, utility modules, etc.).

---

## 1. **Generative Arrangement Automation**

**Problem:** Patches are often static loops, repeating indefinitely.

**Solution:** Use Vector Space to distribute related, but unique, modulations to create evolving changes across your voices and effects.

### How-To:
- **Input:** Three slow-changing sources—LFOs, stepped voltages, envelope followers (via audio from a performance or field recording), or random sources.
- **Outputs:** Assign separate Cube, Plane, and Sphere outs to parameters like:
  - VCA levels (volume-fading or muting elements)
  - Filter cutoffs (dynamic brightness)
  - FX sends/returns (delay/reverb morphs)
  - Sequencer step lengths, quantizer scales, envelope times
- **Result:** Each output drives a different part of your system, causing coordinated, but distinct, variation. Slow transitions or sudden jumps introduce new sections or disrupt repetition—creating intro, verse, chorus, and bridge-like movement.

---

## 2. **Modulation Feedback for Structural Evolution**

**Problem:** Unchanging modulation leads to repetitive structures.

**Solution:** Patch some Vector Space outputs back to modulate the modulators. For example, modulate an LFO’s speed with a Plane out, or a random source’s probability/shape. This instigates slow, self-generating evolution that can:
- Build or dissolve complexity
- Gradually morph between rhythmic feels or tonalities
- Move towards or away from intensity (good for build-ups/breakdowns)

---

## 3. **Multi-Part Song Generation (Counterpoint, Harmony, Variation)**

**Problem:** All parts of a patch move in lockstep, no inter-melodic interaction.

**Solution:** Use the Plane outs’ “three-alike, three-unique” logic to create lines that periodically converge and diverge. Patch three sequenced voltages to the inputs; send multiple Plane outs through quantizers to different voices. Harmonies and unisons will form and dissolve in a pseudo-musical way—great for arrangements that “breathe.”

---

## 4. **Automated Mixing & Spatial Movement**

- Fade drum, bass, lead, and FX returns in/out with different Cube/Plane outs routed to VCAs.
- Create stereo/quad spatialization by mapping joystick/Vector Space outs to panning VCAs. Use Sphere/UnSphere outs for centralization and outward movement—cinematically introduce/retract elements in a performance.
- Use offsets (switches) live to reorganize the modulation and “scene switch,” like moving to a new section.

---

## 5. **Sequencer Manipulation & Structural Mutation**

Close song sections with major parameter shifts:
- Use Sphere or Plane outs to clock a sequencer, switch playback direction, or transpose patterns.
- Mask/enable whole sequences with VCA switching via unique outs for pseudo-“mute/solo” automation.
- Mutate effects order or patchbay routing using the unique relationships of outs.

---

## 6. **Timbral & Rhythmic Transitions**

- Vector Space can morph between several oscillator timbres, shifting the “center” of your patch to signal a new section (chorus, verse, breakdown) without abrupt patch changes.
- Use audio-rate modulation on one input and slow control on another to hybridize “textural” changes and “song-structural” changes — e.g., morph from bass to lead or percussion textures smoothly, mapped to the progression of a performance.

---

## 7. **Event-Driven Changes & Performer Interaction**

- Map physical controllers (joysticks, foot controllers, gates from manual buttons, or distant touch sensors) into the Vector Space for interactive scene changes and dynamic transitions.
- Use Vector Space outputs to simultaneously control lighting, visuals, or external MIDI-equipped gear for multimedia “song” progression.

---

## 8. **Combining with Other Modules**

- **Random/Chaos Modules:** Seed chaos into your modulation for non-repeating sections.
- **Logic Modules:** Extract triggers/gates from changing mod outputs for new section launches.
- **Sequential Switches:** Use Vector Space outs to select new voices, effects chains, or clock divisions.
- **Loopers/Samplers:** Drive sample position or layer selection for structure.

---

## Practical Song-Progression Patch Example

1. **Inputs:** Slow LFO, random stepped voltage, joystick (for live influence).
2. **Outputs:**  
   - **Cube Out:** Fade between two drum layers.
   - **Plane Out:** Modulate a shift-register sequencer's clock rate (generating new melodic fragments).
   - **UnSphere:** Control macro filter cutoff—intro is smooth, intensity rises mid-song, then softens for outro.
   - **NegSphere:** Mutes bassline at certain voltage thresholds (“drop out” sections).
   - **Extra:** Any output to a quantizer/voice for melodic counter-line.

Patch this, record your session long-form, and you get a patch that *itself transforms* over time—no two runs the same, but always with a sense of movement, narrative, and resolution.

---

Remember: Vector Space provides coordinated, yet non-identical, control voltages. By letting the module handle “macro-variation,” you can focus on the overall sound and performance. You don’t need to repatch between songs—just change modulation sources, or flip a switch, and a new arrangement emerges.

Go forth and write full-length, modular songs!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)