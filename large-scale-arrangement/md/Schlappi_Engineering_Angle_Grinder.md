# Schlappi Engineering — Angle Grinder

- [Manual PDF](../../manuals/angle_grinder_manual_20181022.pdf)

---

[**Schlappi Engineering Angle Grinder Manual (PDF)**](https://schlappiengineering.com/AngleGrinderManual.pdf)

---

# Using the Schlappi Engineering Angle Grinder to Create Full-Length Songs in Eurorack

The **Angle Grinder** is a deep multi-functional module, serving as a **quadrature sine wave VCO**, **state variable filter**, and a unique **waveshaping/wavefolding processor**. While it excels at classic duties like basslines, leads, drones, and metallic textures, its flexible routing and voltage control open up many strategies for building evolving, dynamic, and full-length arrangements in your Eurorack system.

Below are detailed suggestions on using the Angle Grinder, in combination with other modules, to move beyond simple patterns and create complete musical journeys.

---

## Key Features for Song Construction

- **Oscillator & Filter Duality**: Switch dynamically between oscillator and filter modes within a patch.
- **Four Phase-Related Outputs**: Use quadrature (0°, 90°, 180°, 270°) sine phases for stereo, quad-panning, or inter-modulation.
- **Voltage Controlled Grind**: Morph and automate wavefolding intensity throughout a track.
- **FM/Sync Capabilities**: Complex, evolving timbres via internal/external modulation and sync.
- **Audio & CV Processing**: Angle Grinder is both a sound source and audio/CV processor.
- **External Input/Inject**: Use as a core filter or effect, bringing in sequenced/melodic material from other modules.

---

## Strategies for Composing Full-Length Songs

### 1. **Macro Song Structure via Modulation**
- **Automate Major Transitions**:  
  Use timed voltage sources (CV sequencers, function generators, manual control, or workflow-oriented sequencers like **Intellijel Metropolix**, **Malekko Voltage Block**, or **Endorphines AUTOPILOT**) to move between oscillator and filter modes by modulating the **GRIND -> SPIN** and **DAMPING** controls over the arc of a performance, morphing from pure tones to filtered noise/waveshaping over time.
- **Automated Timbre Evolution**:  
  Sequence or randomly modulate the **GRIND SLIDERS** and their associated CV inputs. Remap these modulations to different song sections (e.g., verse: subtle, chorus: aggressive, bridge: metallic/noisy).

### 2. **Polyphony & Interlocking Patterns via Quadrature Outputs**
- **Polyphonic/Fake-Polyphonic Arrangements**:  
  Use the four phase outputs as separate voices:  
  - Envelope generators (e.g., **ALM Pamela’s New Workout**, **Make Noise Maths**) can trigger separate events based on these outputs.
  - Route each phase to different chains—one for a lead, another processed for bass or pads, the third to a wavefolder, and the fourth for modulation.
- **Quad Panning/Spatialization**:  
  Pan each phase to different outputs via **VCAs** and a quad panner (e.g., **Doepfer A-134-1** or using a matrix mixer) to spatially animate your mix.

### 3. **Song Section Morphing with Patch Programming**
- **Exploit Filter Modes**:  
  Morph between VCO, LPF, BPF, and HPF outputs to change textural roles. With the right switching or manual control, you can smoothly transition sections (think ambient intro -> acid bassline -> metallic breakdown).
- **Inject External Audio for Sectional Change**:  
  Use the **INJECT** input to process entirely different melodic or percussive voices, bringing dramatic texture changes (i.e., live sampling or buffer-based melodies routed through Angle Grinder for a “drop”/fill/bridge).

### 4. **Synchronize Sections with FM & Sync**
- **Use FM1/FM2 for Rhythm & Tonality**:  
  Sequence FM depth to sync with your drum patterns, accentuate transitions, or create risers/noise swells during fills using connected modulator oscillators synced to your clock/dividers.

### 5. **Automation & Morphing – Maximize Voltage Control**
- **Scene-Based Automation**:  
  Combine with **preset managers** (e.g., **Voltage Block**, **Hermod**, **Vector Sequencer**) for programmable control of all CV-able parameters—let you jump or morph between entire parameter sets at key song points.
- **Use with Compare/Logic Modules**:  
  Trigger changes using CV comparators/logic (e.g., **Mutable Instruments Kinks**), e.g., flip filter mode, GRIND level, or inject, only when all voices hit a certain volume or section cue.

---

## Example Song Flow Using Angle Grinder

1. **Intro Section**: 
    - *LFO Mode*: Use Angle Grinder as a quadrature LFO for quad panning/slow undulating drones feeding reverb.
    - *Transition*: Raise **GRIND -> SPIN**, and automate via sequencer to morph into oscillator mode.
2. **Main Groove/Verse**: 
    - *Audio-Rate Oscillation*: Use as the main bass or lead. FM/AM inputs with clocks/rhythmic CV for evolving lines.
    - *Melody/Countermelody*: Use multiple quadrature outputs for melodic/rhythmic interlocking parts, routed to wavefolders or VCA envelopes triggered by sequencer.
3. **Breakdown/Bridge**:
    - *Filter Mode*: Inject external drum/bass, process with non-linear filtering and slider automation for mangled breakdown textures.
    - *Noise/Soundscapes*: Push DAMPING and GRIND to extremes for metallic sound, drone, and noise washes.
4. **Chorus/Drop**:
    - *Full Automation*: Swell sliders with sequencer automation, switch back to oscillation, and envelop-sync for “drop” impact.
5. **Outro**:
    - *Fade Out*: Use quadrature outs for stereo pads, automate DAMPING out to silence, or close all sliders for a gentle return to ambient.
  
---

## Module Pairings to Enhance Song Creation

- **Sequencers/Controllers**: Voltage Block, Hermod, Rene, Five12 Vector, or any controller for scene programming.
- **VCAs/Matrix Mixers**: Animate Quadrature out levels (e.g., Doepfer A-135-2, Dnipro Dot).
- **Clock/Logic/Divider Modules**: Pam’s New Workout, Acid Rain Maestro.
- **Random/Probabilistic Modulators**: Mutable Marbles, Wogglebug.
- **Effect Processors**: Clouds, Magneto, Data Bender for textural change and transitions.
- **Performance Mixers**: For smooth stereo panning/level control.
- **Switches/Sequential Switches**: To re-route Angle Grinder outs for dramatic song structure changes.

---

## Takeaways

**Angle Grinder** is much more than a tone generator—by liberally exploiting its voltage control, phase-related outputs, dual oscillator/filter identity, and growling grind section, you can infuse your compositions with **rich timbral transitions**, **structural contrasts**, **automated morphing**, and **spatial movement** across full-length songs.

**Approach your patch as a series of dynamic scenes rather than a static groove, and let Angle Grinder’s flexibility drive dramatic compositional shifts.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)