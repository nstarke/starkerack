# Make Noise — MultiMod

- [Manual PDF](../../manuals/multimod-manual.pdf)

---

[**Download the Make Noise MultiMod Manual (PDF)**](https://makenoisemusic.com/manuals/MakeNoise_MultiMod_Manual.pdf)

---

# Using the Make Noise MultiMod to Create Full-Length Eurorack Songs

## Overview

The Make Noise MultiMod is a breakthrough modulation processor that can transform a single control signal into multiple, independently phase-, speed-, and shape-varied versions. This offers powerful possibilities for orchestrating evolving, non-repetitive, and dynamic song structures in a eurorack modular system. Consider it a modulation brain: it lets you send out variations on a single idea to many destinations, synchronizing or unsynchronizing elements across your entire patch.

In this guide, we’ll explore how to use MultiMod to **move beyond loops** and **build full-length, evolving songs** by leveraging its unique capabilities. We’ll include patch ideas and integration tips for crafting intros, builds, breakdowns, drops, and outros—all with hands-on, organic variation.

---

## Song Structure in Eurorack: The Challenge

- It’s easy to make a repeating loop (beat, melody, bassline) in eurorack.
- The challenge is creating variation, progression, and "song-ness": **sections**, **evolving energy**, **drama**, and **resolution**.

**MultiMod** excels at orchestrating multi-part, evolving variation from a single modulation or clock source.

---

## Concepts for Full-Length Songs with MultiMod

### 1. **Macro Modulation: Global Section Changes**

#### **Technique: Scene Switching with Hold, Time, and Shape**

- Use the **Hold** function to lock the current modulated states, then re-engage to unleash a new modulation pass, essentially acting as a "scene switch" or "drop."
- Automate or manually morph the **Time** and **Shape** parameters at specific song moments to globally alter the modulation curves feeding your patch.
    - Example: Short **Time** values = tight, fast sections. Wind it longer for breakdowns or intros.
- **Shape** can morph output modulation from snappy to smooth or random, causing major section changes.

#### **Patch Example**
- MultiMod OUTs → CV inputs of attenuators controlling filter cutoff, VCA, oscillator shape, effect sends.
- Use an external gate or performance button to engage **Hold**—this "freezes" a section.
- Between sections, hit **Reset** to realign everything on a musical boundary.

### 2. **Layered Groove and Melodic Expansion**

#### **Technique: Phase and Spread for Polyrhythms & Counterpoint**

- **Spread** introduces increasing/decreasing speed deviations per channel—spread your groove.
    - Channel 1 drums (straight), channels 3/5 percussion (offset/accelerated for fills).
    - Channel 8 sends to melodic modulation source (phase-shifted arpeggio, etc.).
- **Phase** offers micro-movement—a handful of melodic or rhythmic lines with intentional drift, returning to sync at Resets.

#### **Patch Example**
- MultiMod OUTs → Several EGs or VCO pitch CVs, each creating overlapping, polyrhythmic parts.
- Adjust **Spread** for fills/accents to gradually arise apart from the main loop.
- Periodically reset phase for structural endpoints (end of section, drop, etc.).

### 3. **Generative Automation: Slow Macro-Evolution**

#### **Technique: Self-Generating Textures & Section Splits**

- With the internal LFO, Shape, Phase, and Spread, MultiMod can output slowly shifting CVs for drone, pad, or evolving melodic content.
- Change Shape mid-song for a dramatic "movement" (e.g., ramp to random shape—orderly to chaos).
- Use **Time** for very slow modulations across several minutes (intros, breakdowns, outros).

#### **Patch Example**
- MultiMod OUTs all multed to multiple VCF or VCO modules with slightly different offset/attenuation.
- Morph through **Shape** options to transition between song atmospheres.

### 4. **Cueing and Arrangement with External Sequencers or Performers**

- Use a master clock to both **Tempo In** and synchronize sequencers/drum machines.
- Use **Channel Index Out** as a "section detector" to trigger events/scene changes elsewhere in your patch (great for transitioning energy, cueing FX or arrangement changes).

---

## Putting It All Together: Performance & Arrangement Tips

- **Automate MultiMod Controls:** Use CV sources (sequencer lanes, random, joystick, pedal) to morph **Time, Phase, Spread, Shape** across a performance, building and releasing tension.
- **Synced Section Transitions:** Patch clock/gate streams to **Hold** and **Reset** for quantized scene changes.
- **Feed MultiMod with Dynamic CV:** Any manual modulation (fader, pressure, touch) into MultiMod gets "broadcast" as 8 related but non-identical gestures, yielding energetic, never-exactly-repeating phrases.
- **Patch Diversity:** Send different MultiMod OUTs to melodic, rhythmic, and textural destinations—one signal controls all, but each part shifts in its own way.
- **Variation Through Limitation:** By feeding one source into MultiMod, the unity makes the output feel like a cohesive "song" rather than disparate random events.

---

## Example Song Progression

1. **Intro:** Slow Time, minimal Spread, smooth Shape. Patch LFO mode to ambient parts.
2. **Verse:** Advance Time and Spread, start introducing rhythmic/tonal modulation, maybe step Shape.
3. **Chorus/Drop:** Open Spread wide, faster Time, dramatic Shape (square/pingpong/random). Engage Hold, Reset on downbeat for big impact.
4. **Breakdown:** Reduce Spread back, revert Shape to Sine, extremely slow Time for soundscape.
5. **Outro:** Fade Time to zero, Shape to random, let sounds drift to silence, then hit Hold.

---

## MultiMod Integrations: Useful Companion Modules

- **Sequential Switches:** For repatching MultiMod OUTs to different downstream modules per section.
- **Voltage Controlled Switches:** Use Channel Index to automate routing.
- **Attenuverter/Mixer Banks:** To sum and carefully adjust MultiMod outs for melodic modulation.
- **CV Recorders/Loopers:** To capture and recall MultiMod performances across song parts.
- **Clock Dividers/Multipliers/Logic:** For even more complex timing sections when using external clocks.

---

## Conclusion

The **Make Noise MultiMod** unlocks song-length, multi-section modular performances by:
- Turning any modulation into eight ever-evolving streams
- Giving you phase, speed, and shape control over entire arrangements
- Allowing hands-on and automated movement through song sections

It’s not just a utility—it's a powerful engine for macro-level musical storytelling in your eurorack system.

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)