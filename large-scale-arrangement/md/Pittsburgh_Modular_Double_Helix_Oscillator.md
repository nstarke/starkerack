# Pittsburgh Modular — Double Helix Oscillator

- [Manual PDF](../../manuals/Lifeforms Double Helix Oscillator - Pittsburgh Modular Synthesizers.pdf)

---

[Download the Lifeforms Double Helix Oscillator Manual (PDF)](https://pittsburghmodular.com/documents/Pittsburgh_Modular_Lifeforms_Double_Helix_Manual.pdf)

---

# Using the Pittsburgh Modular **Double Helix Oscillator** to Build Full Length Songs in Eurorack

When crafting full-length, structured tracks on a modular system, moving beyond simple loops (beats, melodies, and bass lines) to arrangements that evolve over time is the main challenge. The **Double Helix Oscillator** is a highly flexible dual-oscillator module with complex internal signal paths, modulation routing, and analog signal shaping options. Here’s how you can harness it as the core tonal and timbral source in full Eurorack compositions.

---

## Key Features That Support Song-Length Structure

### 1. **Dual Oscillators = Multiple Voices**
- **Primary and Secondary Oscillators** each offer wide-range (LFO to audio), multiple waveforms, and FM options.
- You can patch them as:
    - **Melody and Bass** (separate transposition, tracking from two sequencers)
    - **Melody and Drone/Pad**
    - **Stacked for Chord Intervals or Complex Modulation**

### 2. **Advanced Contour/Wave Shaping and Dynamic Impulse Gate**
- The internal **wavefolder** and **low pass gate** add analog rich timbre that’s highly modulatable.
- The contour’s **“striking” behavior** (Impulse Input) is ideal for percussive, plucked, or pseudo-acoustic sounds—excellent for dynamic song sections and transitions.

### 3. **Flexible Internal (and External) Modulation**
- Built-in LFO, noise, and steppable random voltages.
- **Voltage Controlled Routers** allow dynamic re-routing of modulation—crucial for creating evolving textures or automated changes between song sections.

---

## Approaches for Creating Full-Length Songs

Below are some strategies for leveraging the Double Helix in a full composition:

### **A. Song Structure Through Sequencer and Modulation**

1. **Multi-Part Sequencing**
    - Use an external sequencer (e.g., BeatStep Pro, Eloquencer, or MIDI-to-CV interface) to track melodies on one oscillator and bass or counter-melody on the other.
    - Consider **cross-modulation** for movement between voices, or tune them to musically related intervals.

2. **Section Variations via Modulation Matrix**
    - Assign external CV sources (slow LFOs, stepped random, or envelope generators) to the modulation matrix’s **A/B inputs**.
    - Use external sequential switches or manual control to change what’s routed where (e.g., changing the source for FM or wavefolder depth between verse and chorus).

3. **Dynamic Tonality/Timbral Transitions**
    - Automate the **Dynamics** and **Timbre** parameters using CV—dedicate a channel on your sequencer to send gate/envelope CV to these inputs, evolving the sound over time.
    - Exploit wavefolder “opening” for brighter chorus, “closing” for mellow verse.

### **B. Performative Manual Control**

1. **Performance Macros**
    - Map key performance controls (Dynamics, Timbre, FM Amount) to large, reach-friendly knobs to sweep or “play” the tone during a set.
    - Combine manual tweaks with voltage-controlled matrix switching for active arrangement participation.

2. **Ping/Impulse for Unique Transitions**
    - Use the Impulse input to generate “event” sounds—transitions, fills, or drops by pinging the low pass gate at strategic points in your arrangement.

### **C. Layering and Sample Re-Use**

1. **Layer Outputs**
    - The multiple simultaneous outputs per oscillator (Sine, Saw, Blade, Sub, etc.) allow you to layer and re-patch or sample/loop distinct voices—useful for live overdubbing or building up arrangement density.

2. **Sampling and Resampling**
    - Use a sampler or looper module to capture interesting patterns and have them reappear or morph later in the song (think "A-B-A-C-A" structures). The Double Helix’s analog richness lends well to creative resampling.

### **D. Creating Arrangement “Scenes” using Switching**

- Using sequential switches, manual matrix switching, or voltage-controlled switch/logic modules (like the Doepfer A-150 or Erica Synths Sequential Switch), you can reroute oscillator outputs and modulation to different destinations for different song sections.
    - E.g., In “Verse”, Oscillator 1 -> filter -> LPG, Oscillator 2 FM’s Oscillator 1; in “Chorus”, flip routing so Osc 2 is audio, Osc 1 becomes LFO modulator, etc.

### **E. External Integration**

- Sync/clock your modular rig to DAW/Drum Machine for tight structural changes.
- Use external modules for effects (delay, reverb, distortion) and automation via CV, expanding the sonic palette.

---

## Example Patch Ideas for Full-Length Track Movement

- **Intro/Verse:** Slow, evolving pads from the Primary Oscillator’s Blade or Sine output. Low Dynamics and Timbre; modulation routed to subtle FM.
- **Chorus:** Open up the Dynamics and Timbre, patch aggressive wavefolded output. Add Sub oscillator for weight. Route sequencer gates to Impulse for percussive stabs.
- **Bridge/Break:** Use Secondary Oscillator as an LFO/modulator for chaotic FM, while using noise/random CV for timbral disruption.
- **Outro:** Decay into airy noise, ramp down filter/LPG, reduce modulation.

---

## Combination Module Suggestions

- **Sequencer**: for patterns, melodies, and automation (e.g., Winter Modular Eloquencer, Intellijel Metropolix).
- **Envelope/LFO Generators**: for evolving CV (e.g., Maths, Zadar).
- **Sequential Switch**: for scene switching/routing changes (e.g., Doepfer A-151).
- **Sampler/Looper**: for resample-repeat structures (e.g., Morphagene, Squid Salmple).
- **Utilities**: VCA, logic, attenuators, mults for patch flexibility.

---

## Final Words

**The Double Helix Oscillator’s** deep sound shaping, performance-oriented modulation matrix, and ability to serve as multiple voices make it an effective hub for modular song-building. With careful patching, scene management, and performance or sequencer-driven automation, it can be the nucleus of dynamic, evolving, and truly “song-like” modular performances.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)