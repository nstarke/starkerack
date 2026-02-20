# Nervous Squirrel — Conway's Game

- [Manual PDF](../../manuals/Nervous Squirrel - Conway's Game.pdf)

---

[**Conway's Game Manual PDF**](attachment://Conways_Game.pdf)

---

# Eurorack Song Creation Strategies With Conway's Game (Nervous Squirrel)

Conway's Game is a highly original pattern generator and MIDI-to-trigger utility, utilizing the mathematics of Conway’s Game of Life. Here’s how you can leverage this tool for creating **full-length songs**—not just loops!—using the module in combination with others in your system.

## How Conway’s Game of Life Module Works, In Brief

- **Pattern Generator:** Generates 8x8 grids of living/dead cells on an LED array, influenced by the Game of Life rules.
- **Trigger Matrix:** Each of the 64 outputs corresponds to a cell, firing triggers or gates based on the simulation.
- **MIDI Mode:** Incoming MIDI notes (C2–E7) directly set output triggers, mapping music into modular voltage.
- **Clock Control:** Runs off internal 10 Hz clock or any external gate/LFO/audio signal for tempo.
- **Reset, Mode, and Trigger/Gate switches:** For resetting patterns, switching between GoL and MIDI, and output type.

---

## Creating Song Structure: Patch Recipes & Workflow Strategies

### 1. **Pattern Evolution as Arrangement**

**What to do:**  
Let the GoL simulation continuously evolve, generating new trigger/gate patterns as your “sequencer.”  
**How to advance sections:**  
- Use the **RESET** input/trigger to clear out and initialize new patterns—each reset can act as a song section change (verse, chorus, bridge).
- Or, let the GoL pattern run until it naturally reaches a stable state or loop, and reset automatically (as module supports).

**Patch example:**  
- Use the RESET from a footswitch, another sequencer, or a clock divider to force a “section change” at key moments in your song.

### 2. **Controlling Drums & Percussion With Life Patterns**

- Assign specific rows (or columns, or clusters) of outputs to drum voices.  
- E.g. Row 1 = Kick, Row 2 = Snare, Row 3 = Hi-Hat, etc.
- **Result:** Patterns morph and evolve—beats constantly change, then stabilize.

**For Song Development:**  
- Use the TRIG/GATE setting so that drums sound different as cells go on/off.
- Combine this with manual or automated resets to provide breakdowns, fills, or drops.

### 3. **Melodic and Bass Triggering**

- Patch triggers from the GoL grid to quantizers, then to oscillators or pitch CV inputs.
- Use several outputs together with logic (AND/OR) modules or sequential switches to steer “melody” voices for different sections.
- The MIDI mode can map keys or MIDI sequences directly to the output grid, perfect for “scored” variations for specific song parts.

### 4. **Song Section Cycling and Randomization**

- Use the **CLOCK IN** to radically vary how quickly patterns change:  
  - Slow clock = long, evolving sections (ambient, generative music).  
  - Fast clock = glitchy, busy textures.
- Modulate the clock rate via LFO, envelope, or random source to create dynamic buildups, transitions, or drops.
- Combine slow pattern sections with abrupt RESETs or clock bursts to transform your song energy.

### 5. **Routing for Song Complexity**

- Combine outputs via logic modules to create even more intricate song structures (e.g., only fire a certain voice if two specific cells are alive at the same time).
- Use matrix mixers to vary how much each GoL output influences other module parameters, letting you "fade" between song sections or instrument groups.

### 6. **Automation and Morphing**

- Automate RESETs and mode switches with sequencers or gate automation (e.g., at the end of every 8-bar cycle, force a new GoL pattern, or switch to MIDI mode for a bridge).

### 7. **Triggering FX and Modulation**

- Use GoL outputs to trigger sample-and-hold, envelope generators, or effect sends—different sections can introduce new textures or modulation behaviors.

---

## Practical Workflow Example

1. **Intro:** Start with a sparse initial pattern (manually initialize or use MIDI).
2. **Main Section:** Let GoL run, evolving triggers for drums and synth lines.
3. **Buildup:** Increase clock speed or introduce new voices/FX via GoL outputs.
4. **Drop:** Hit RESET at a key moment; let new, dense pattern take over.
5. **Breakdown:** Switch to MIDI mode for a hand-played or sequenced phrase.
6. **Outro:** Let GoL fade out naturally as cells die.

---

## Songflow Tips

- **Scene Management:** Use a switch or analog matrix to reroute outputs for each “scene” or song part.
- **Section Memory:** Record CV or audio outputs as stems, then sequence in your DAW or live with a looper for full tracks.
- **External Sync:** Sync GoL’s clock input to your main sequencer or DAW clock so transitions happen in time with your whole setup.

---

## Additional Inspiration

- **Multimodal Morphing:** Crossfade between GoL and MIDI modes during a song for dramatic composition changes.
- **Controlled Randomness:** Use GoL as an inspiration generator; resample stable patterns as regular “choruses” and evolving states as “verses” or “fills.”

---

> [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)