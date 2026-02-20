# 2hp — Euclid

- [Manual PDF](../../manuals/2hp_Euclid.pdf)

---

[2hp Euclid Manual PDF (official site)](https://2hp.com/wp-content/uploads/2hp-euclid-manual.pdf)

---

# Using the 2hp Euclid To Structure Full Length Eurorack Songs

The 2hp Euclid is a compact but versatile Euclidean rhythm generator for Eurorack modular systems, ideal for injecting evolving, musically-interesting rhythmic patterns into your patches. While it excels at creating immediate grooves, its real power—especially for full-length song structure—is in how you can use its features and CV inputs to create rhythmic variation, structure, and dynamic progression over time.

Below, I describe strategies for leveraging the Euclid module in the context of full-track composition, including how to interact with other modules to achieve song-length variety and development.

---

## Euclid Module Key Features Highlighted for Song Creation

- **Generates Euclidean rhythms (up to 16 steps, variable density)**
- **CV control over Steps and Length**
- **Offset control for phase shifting**
- **Reset and Trigger inputs for syncing**
- **6ms gate outputs for triggering other modules**

---

## Strategies to Build Full Tracks with Euclid

### 1. **Automate Rhythmic Variation Over Time**

- **Use CV to Morph Patterns:**  
  Sequence the **Length** and **Steps** parameters with slow LFOs, step sequencers (like a Doepfer A-155, or even a MIDI-to-CV interface running an automation track in your DAW), or programmable function generators (e.g. Make Noise Maths, Intellijel Quadrax).
    - **Example:**  
      - 16-step rhythms for the chorus, 8 in the verse.
      - Steps rising/falling to build or release energy.
- **CV-sequence the Offset:**  
  Shift the phase of your rhythm to subtly or abruptly alter groove placement across sections of your song.
    - Good for creating fills or song transitions.

### 2. **Macro Song Structure via Manual or Automated Control**

- **Reset Input:**  
  Use a master clock divider (e.g. 4ms QCD, Pamela’s Pro Workout) to reset the Euclid pattern at section boundaries (verse, chorus, breakdowns) to synchronize changes across your whole rack.
- **Length or Steps Jumps:**  
  Use a CV switch/sequential switch (e.g. Doepfer A-151) to switch between pre-programmed rhythm patterns at key moments in your track.

### 3. **Layer and Modulate Multiple Euclidean Patterns**

- **Polyrhythm/Polymeter:**  
  Run several rhythm modules, or multiple uses of the Euclid, each with different length/step settings, triggering different percussive voices (kick, snare, hats, synth stabs, etc.).  
- **Inter-module Cross-Influence:**  
  Use Euclid’s trigger output to clock S&H, sequential switches, sequential analog switches (for chord progressions, basslines, or FX changes) in sync with rhythm variations.

### 4. **Fill Creation and Breakdowns**

- **Modulate Steps/Length for Fills:**  
  Use CV or manual control to create quick fills—suddenly lowering the number of steps or steps at the end of a section.
- **Mute/Unmute with Switches or VCAs:**  
  Route Euclid’s output through a VCA or switch, muting the rhythm during breakdowns, or using gates/envelopes (triggered by song-structure logic modules such as Mutable Instruments Marbles, Erica Pico SEQ, or external MIDI).

### 5. **Drive Non-Drum Sounds for Evolving Texture**

- **Modulate Non-Percussive Elements:**  
  Send Euclid triggers to envelope generators controlling filter cutoff, wavefolder amount, or delay send levels for evolving pads, drones, or effect sounds.
- **Melodic Triggers:**  
  Use as a step input for pitch sequencers, advanced quantizers, or switch-based melodic routing, creating rhythmically complex melodic patterns.

---

## Practical Example Patch: Full Song Arrangement

```text
Clock source (Pamela's Pro Workout) → Euclid Trigger In
Pamela's pattern divider → Euclid Reset In (trigger at measure start/chorus change)
Pamela's CV out (random/automation) → Euclid Length CV In
Pamela's CV out (different lane) → Euclid Steps CV In

Euclid Out →
    1. Percussion voice (snare, hat, or rim - e.g. Mutable Peaks in drum mode)
    2. Envelope generator for synth stabs (trigger VCA or effect send)
    3. Clock input for sequential switch (changing basslines or FX)

Patch VCA for rhythmic mute/fade for breakdowns, outro, or song sections.
```

---

## Additional Techniques for Song-Length Structure

- **Record and Loop changes with CV recorders (e.g. WMD S.S.R., ALM Pamela’s Workout looped automation)**
- **Mute/unmute or swap between multiple Euclid setups with switches or logic modules**
- **Combine with MIDI-CV for DAW-synced macro control of patterns and transitions**  
- **Use Euclid triggers to set scene changes, sample triggers, or send cues to visual/lighting systems for live performance**

---

**The key to full-length song form with Euclid is leveraging CV, reset, and inter-module communications to automate rhythmic change, create variety, and sequence transitions at multiple levels—from pattern detail to entire track sections.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)