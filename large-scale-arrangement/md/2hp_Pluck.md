# 2hp — Pluck

- [Manual PDF](../../manuals/2hp_Pluck.pdf)

---

[**2hp Pluck Official Manual (PDF)**](https://2hp.com/products/Pluck-Manual.pdf)

---

# Creating Full-Length Eurorack Songs with the 2hp Pluck Module

The **2hp Pluck** is a highly compact, yet versatile, physical modeling string synthesizer based on the Karplus-Strong algorithm. Its expressive controls over **damp**, **decay**, and **pitch**, coupled with four-voice polyphony, make it an intriguing melodic and textural element in a eurorack system.

Below, you'll find strategies, patch ideas, and workflows to help bridge the gap from *great riffs* to *song-length compositions* using the Pluck—often in combination with other modules—to fully realize arrangement, structure, and evolution over time.

---

## Overview: What Pluck Brings to the Table

- **Polyphonic Plucked String Synthesis:** Melodies, chords, or evolving harmonic beds
- **Voltage Control:** Dynamic timbral changes via CV
- **Expressive Decay/Damp Controls:** Lets you move from tight, percussive pops to shimmering, evolving tones

---

## Strategies for Song-Length Composition

### 1. **Separating Song Sections (Intro, Verse, Chorus, Bridge, Outro)**

**Technique:** Modulate Pluck’s parameters per section  
**How-To:**
- Use a sequencer (like Arturia Keystep Pro, Five12 Vector, or a Eurorack sequencer) to send different patterns or melodies to Pluck for each song part.
- Pair with a programmable CV source (e.g., Mutable Instruments Marbles, Intellijel Planar, Make Noise Maths as CV scene memory) to automate changes in **DAMP**, **DECAY**, and/or **PITCH** knob positions per song part.
- **Result:** The same Pluck voice morphs to play different melodic patterns and timbres in each section.

### 2. **Dynamic Arrangement with Polyphony and Triggers**

**Technique:** Use the 4-voice polyphony for harmony and movement  
**How-To:**
- Send chord sequences using a polyphonic sequencer (e.g. Polyend Poly, Hermod, or several monophonic triggers in creative polyphony).
- For single melodic lines, layer overlapping melodies to create movement (e.g., arpeggios, layered harmonics).
- Use a sequential switch or trigger sequencer (like Pamela's Pro Workout or Mutable Branches) to selectively fire voices, simulating new phrases/sections.
- **Result:** Expanding melodies into harmonies and back—a musical evolution across the composition.

### 3. **Automated Timbre and Texture Changes**

**Technique:** Evolve the sound’s character over time  
**How-To:**
- Use LFOs, envelopes, or automation lanes to modulate **Damp** and **Decay** CV inputs. For instance, open the sound up for the chorus and tighten it for the verse.
- Feed random or stepped modulation (from S&H modules or random generators like Wogglebug or Marbles) to **Damp** and **Decay** for subtle or drastic evolutions.
- Animate the **Pitch** knob or V/Oct input for vibrato, slides, or atonal/experimental transitions.
- **Result:** The “instrument” comes alive, feeling less loop-based and more performed/windowed in time.

### 4. **Sample, Loop, and Remix**

**Technique:** Record Pluck’s output as part of a larger composition and reuse  
**How-To:**
- Multitrack Pluck’s lines into a DAW (Ableton Live, Logic, etc.), then slice, rearrange, or process the audio. 
- In-rack sampling (using an Erica Sample Drum, Mutable Instruments Clouds, or similar) captures licks, chord stabs, or motifs to be triggered later as structural anchors or fill material.
- **Result:** Freed of ‘live only’ constraints, allows for verse/chorus contrasts, breaks, or motif returns.

### 5. **Integration with Percussion, Bass, and Lead**

**Technique:** “Orchestrate” with other voices  
**How-To:**
- Sync Pluck’s triggers with drum machines/triggers for tight, percussive lines.
- Pair with a classic subtractive synth VCO/VCF/EQ for bass or lead, reserving Pluck for harmonics or counter-melodies.
- Use a performance mixer (like Erica Black Mixer, Befaco Hexmix) or VCAs to fade in/out Pluck—creating verse/chorus delineation.
- **Result:** Each section has distinct instrumentation changes, strengthening arrangement.

---

## Example Patch: Arranged Song with Pluck

- **Sequencer:** Sends melody/chord CV + trigger to Pluck (Pattern A for verse, Pattern B for chorus, Pattern C for bridge, etc.)
- **LFO/Envelope/Random:** CVs to **DAMP**/**DECAY** per song section
- **Drum Machine:** Syncs patterns via master clock/reset
- **Performance Mixer:** Handles fading, muting, and returning of Pluck’s signal
- **Reverb/Delay Effects:** Adds space around Pluck, evolving from dry (verse) to lush (chorus)
- **Sampler or Loop Pedal:** Captures lines for later playback in new contexts

---

## Pro Tips for Songwriting

- **Plan Structure:** Sketch out arrangement goals before patching. Knowing when Pluck should be featured vs. supportive helps guide modulation choices.
- **Performance Automation:** Use hands or performance CV controls for evolving knobs live—often more dynamic than static settings.
- **Layering:** Mult with an effect send—use different reverbs or delays to accentuate transitions.
- **MIDI Integration:** Consider a MIDI-to-CV module for easier DAW control or recording.

---

### Additional Resources  
- [2hp Pluck Official Manual (PDF)](https://2hp.com/products/Pluck-Manual.pdf)

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)