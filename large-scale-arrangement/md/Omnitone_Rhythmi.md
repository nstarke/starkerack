# Omnitone — Rhythmi

- [Manual PDF](../../manuals/Rhythmi_Information_Package.pdf)

---

[PDF: Rhythmi Information Package Manual](attachment:file.pdf)

---

# Using Rhythmi to Create Full Length Eurorack Songs

The **Rhythmi** Eurorack drum sequencer is designed not just for generating engaging drum patterns, but for evolving those patterns live, enabling dynamic changes throughout a performance or recording. If you often “hit a wall” turning an impressive loop into a full track, Rhythmi’s hands-on and CV-modulatable parameters provide creative solutions to keep your music moving and transforming. Below are techniques and patch strategies for integrating Rhythmi into extended, song-length modular compositions.

---

## Song Arrangement Concepts Using Rhythmi

### 1. **Evolving and Transforming Patterns**
- **Evolve Parameter:** Use the Evolve encoder or CV modulation to morph drum patterns during the track. Start with your Root Rhythm for the intro/verse, and introduce evolution for choruses, bridges, or fills. Automate the Evolve parameter using sequencers or LFOs for short fills or transitions.
- **Pattern Randomization:** Short-press the Evolve encoder (or send CV > 75%) at section changes for fresh rhythmic content. Return to the Root Rhythm for recurring motifs or to “reset” the groove post-drop.

### 2. **Macro Arrangement Control**
- **Energy Control:** Assign Energy to automation for building energy over time. Low settings = basic groove (verse/intro), mid-range ramps up fills and density (pre-chorus/bridge), max triggers Crash (drop/chorus, transitions) and fully energizes the kit.
- **Length Parameter:** Dynamically change loop length to shift between tight, repetitive sections (4–8 steps) and more open, evolving ones (16–32 steps). Short lengths can be breaks/hip-hop; long lengths yield electroacoustic fills or “breakbeat” flavor.

### 3. **Swing & Syncopation**
- **Real-Time Groove Changes:** Use Swing modulation for groove subtlety—straight sections (0% swing) for tension, then increase swing to “loosen up” at drops or breakdowns. Syncopation control on individual drums lets you periodically switch from rigid to laid-back feels.

---

## Integrating Rhythmi With Other Modules

### 1. **Song Structure Automation**

**Sequencers/Controllers:**  
- **Voltage Sequencer:** Sequence CV to Evolve, Energy, Length, and Swing to automate song sections.
- **Manual Controllers:** Use faders (e.g., Frap Tools FALISTRI, Make Noise Maths) to fade sections in/out, manipulate groove in real time.
- **Preset/VCA Recall:** Use modules like Mutable Instruments Frames or Make Noise Morphagene to recall specific rhythmic settings for different song sections.

### 2. **Global System Events**

**Crash Output as Section Change Signal:**  
- Mult the Crash output to envelopes, sequential switches, or logic modules to:
  - Trigger fills, resets, or changes in bass/melodic sequences.
  - Clock scene changes in effect modules (e.g., send Reverb/Delay to max at drop).
  - Reset or “jump” sequencer patterns on major transitions.

### 3. **Dynamic Drum Kit Sound Design**

**CV-to-Tom Output:**  
- Patch the TOM CV out to drum synth VCOs, additional percussion, or even melodic voices for tom-driven fills that track the module’s phrasing.

**HI-HAT Output (Gated):**  
- Use logic or slew limiters downstream to morph between tight closed hats and long open ones, responding to musical density.

### 4. **Layering and Parallel Processing**

- Pair Rhythmi with other sequencers (e.g., Mutable Grids, Euclidean Circles) to crossfade or blend between organic and surgical drum parts throughout the song.
- Use rhythmic outputs as modulation sources for synths, VCAs, effects, or sample playback, tying all musical elements to the evolving drum core.

---

## Example Full Song Workflow

1. **Intro:**  
   - **Minimal Energy + Low Evolve, Long Loop:** Sparse basic groove, few hits, max anticipation.
2. **Verse:**  
   - **Increase Density/Length Slightly, Introduce Swing:** Groove fills out, more syncopation, hats open up.
3. **Pre-Chorus:**  
   - **Raise Energy (More Toms, Early Fill), Increase Evolve, Shorten Loop for Tension**.
4. **Chorus/Drop:**  
   - **Max Energy (Crash triggers), High Swing, Fully Evolved Patterns**. Use Crash to cue melodic and FX changes.
5. **Bridge/Breakdown:**  
   - **Lower Energy and Evolve, Change Base Pattern, Add Randomization**.
6. **Outro:**  
   - **Reduce Length, Density, and Swing to fade out**. Optionally randomize or “reset” to Root Rhythm.

---

## Patch Tips and Collaborations

- **Pair with Generative Sequence Modules** for evolving bass/melody.
- **Use Clock Output** from Rhythmi to drive synchronized sequencers, arpeggiators, or LFOs.
- **Record Automation Moves** with external CV recorders for repeatable live jams or composed works.

---

For maximal creative potential, design and automate macro changes (energy, evolve) alongside classic step sequencing and performance controls. Rhythmi’s design philosophy excels at breaking the “8-bar loop trap” common in modular systems, pushing your live and composed tracks to full song forms.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)