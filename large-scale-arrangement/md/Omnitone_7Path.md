# Omnitone — 7Path

- [Manual PDF](../../manuals/7Path - Ethernet Patch Cable Bridge - Omnitone.pdf)

---

[7Path - Ethernet Patch Cable Bridge PDF Manual](https://omnitone.ca/products/7path-connect-eurorack-cases-in-synth-jams-eurorack-module-to-connect-cases-no-long-patch-cables)

---

# Using the 7Path Ethernet Patch Cable Bridge to Create Full-Length Eurorack Songs

## Module Summary

**7Path** is a pair of passive Eurorack modules that let you connect up to 7 signals between two points (or two different cases) using just a single ethernet cable. This modular bridge is especially useful for reducing long, cluttered patch runs when expanding your system or for collaborative setups (e.g., live jams).

**Key Features:**
- Passes any type of Eurorack signal (CV, gate, audio) on any jack
- 1-to-1 jack mapping across modules
- Does not require power
- Up to 10ft with unshielded ethernet cable, longer with shielded

---

## Why the 7Path is Powerful for Song Structure

In Eurorack, one of the greatest challenges is moving from a loop/sequence to a **full-length song** with dynamic sections, variation, and transitions. The 7Path excels in situations where:
- You have **multiple cases** (or distant parts of a big case) and want to creatively exchange signals between "song sections"
- You want to **modularize control**, enabling quick and drastic re-patching during a set
- You want to introduce **variation and live performance elements** without rewiring between tracks

---

## Strategies for Full-Length Song Creation with 7Path

Here’s how to leverage this module, turning great loops into dynamic tracks:

### 1. **Section-Based System Design**
- **Divide your rack into two "sections":** Sequencer/structure and Sound Generation/FX.
- **Connect the sections via 7Path:** Use the bridge to pipe CVs/gates, modulation, triggers, or audio, effectively creating two subnetworks you can quickly re-map for different song parts.

**Example Patch:**
- Section A: Sequencer/clock/modulation sources
- Section B: Voices/drums/effects
- Use 7Path to send different triggers, melodies, modulations, or even audio to/from Section B when moving from verse to chorus.

### 2. **Live Section Switching**
- Swap which signals connect across the 7Path’s 7 channels during a performance:
    - e.g., send drums on channel 1 for verse, move a melody on channel 2 for chorus, or switch modulation paths for the “drop.”
- Use mute/attenuator modules before 7Path inputs to temporarily break or crossfade connections for breakdowns/builds.

### 3. **Collaborative and Physical Transitions**
- In large, multi-case jams or collaborative performances, 7Path lets you assign each player (or left/right case halves) unique "responsibilities," exchanging musical elements at set moments for smooth, performed transitions.

### 4. **Automation & Song Progression**
- **Patch Matrix Variant:** Use switches or sequential switches before the 7Path to programmatically control which signals are sent when, for morphing between song sections hands-free.
    - Example: Use a sequential switch to change which modulation or melody lane crosses cases as your song progresses.
- **Morphing and Layering:** Combine different signals (mixers/VCAs into 7Path) and automate their levels to blend/morph across “scenes” from one section to the next.

### 5. **Audio Routing for Variation**
- Send audio feeds (like drums or bass) from one case to another for unique FX processing just in choruses or breakdowns, then return them back via other 7Path channels during verses.
- Allows “one cable re-patch” of entire song sections’ audio flows for dynamic arrangement.

---

## Example Song Structure Patch

| Song Part    | 7Path #1   | 7Path #2   | 7Path #3   | 7Path #4   | 7Path #5   | 7Path #6   | 7Path #7   |
|--------------|------------|------------|------------|------------|------------|------------|------------|
| Intro        | Clock      | CV1        | Mod1       | -          | -          | -          | -          |
| Verse        | Drum trig  | Bassline   | Env gate   | FX CV      | -          | -          | -          |
| Chorus       | Lead CV    | Chord CV   | FX return  | Gate fill  | Drum FX    | Mod2       | Mod3       |

- Use external switches/mutes or sequencer automation to reroute signals in real time.

---

## Essential Patch Combinations

- **Mix with Matrix Switches:** Sequentially switch entire signal groups sent through the bridge for “scene” changes.
- **Combine with VCAs/Faders:** Fade in new song elements routed through the 7Path, creating build-ups or breakdowns.
- **Use for Send/Return FX Loops:** Send audio or CV through 7Path to remote FX cases or pedal loops, returning results via other channels.

---

## Final Tips

- Think of 7Path as a **modular "scene change" or group patcher**—ideal for organizing, routing, and quickly shifting complex patch systems over the course of a full-length song, all with a single cable swap.
- Experiment with what, not just audio but **modulation and CV signals**, you route—sometimes sending a clock, envelope, or random to a new destination can be the biggest change!

---

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**