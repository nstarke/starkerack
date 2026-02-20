# Nervous Squirrel — Conway's Game

- [Manual PDF](../../manuals/Nervous Squirrel - Conway's Game.pdf)

---

[**Conway's Game Module Manual (PDF scan)**](#)  
*(Link to the attached manual PDF is not available for direct linking, but manual images are above for reference)*

---

# Creative Patching & Sound Design with Conway’s Game Eurorack Module

The **Conway’s Game** Eurorack module is a cellular automaton-based pattern generator, using the Game of Life algorithm to drive 64 individual trigger/gate outputs. It also functions as a MIDI-to-trigger converter. Below, you’ll find tips and patch ideas to maximize its creative potential for *distorted percussion*, *crazy basslines*, and *atmospheric pads*.

---

## 1. Distorted Percussive Sounds

### **Patch Concept**
- **Randomized Rhythms:** Use the outgoing 64 triggers/gates as a source of unpredictable, evolving patterns for percussive modules.

### **How To Patch**
- Patch several *outputs* from the Conway module to various drum modules (kick, snare, hats, metallic/noise sources).
- To add chaos, use the **external clock input**—try running fast clocks or even audio-rate clocks (as recommended, >270Hz “starts getting weird”).
- Switch between *TRIGGERS* for sharp percussive hits, and *GATES* for longer noise bursts or pseudo-loops.

### **Distortion & Character**
- Send drum signals through distortion/wavefolding modules after triggering to achieve crunchy, glitchy, or industrial sounds.
- Modulate the clock frequency dynamically with a fast LFO or envelope, creating continuously evolving trigger densities and syncopation.

---

## 2. Crazy Basslines (Dubstep/Drum & Bass)

### **Patch Concept**
- Use the module as a sequencer for a bass synth voice, but with chaotic, algorithmic patterns.

### **How To Patch**
- Patch one or two Conway outputs to a *bass VCO’s* gate/trigger input or through a sequential switch for “random access” bass notes.
- Use *MIDI mode* and send specific MIDI notes from a DAW or MIDI keyboard to directly trigger bass hits in conjunction with other voices.
- **Clock at audio rates** or modulate clock tempo with a stepped random voltage for “wonky” bass glitches.

### **Bass Enhancement**
- Send the triggered envelopes to modulate filter cutoff/resonance, wavefolder amount, or FM index on your bass synth for deep, growling, or squelchy effects.
- Use multiple Conway outputs to trigger side-chained comp/LFO resets or retriggered distortion/envelope followers for high-energy movement.

---

## 3. Haunting Atmospheric Pads

### **Patch Concept**
- Use the Conway outputs as “polyphonic” gates for a set of ambient/texture VCOs or sample players.

### **How To Patch**
- Connect several Conway gates to envelopes controlling the amplitudes of multiple oscillators or sample players loaded with eerie textures.
- Use long gates instead of short triggers (set module mode to *GATES*) for sustained, layered pads that phase in and out with the evolving automata patterns.
- The 8x8 grid can create clusters and waves of “living” sound, perfect for generative, haunting soundscapes.

### **Pad Atmosphere Enhancement**
- Use a slow LFO or random CV to occasionally hit the **RESET** input, re-populating the automaton for a continual evolution.
- Rout triggered sources through granular, shimmer, or spectral effect modules to build even more ethereal textures.

---

## Extra Modulation Tips

- The **external clock input** is your key to wild modulation: Feed everything from audio-rate oscillators to slow S&H voltages to completely warp the pattern generator’s speed and therefore the rhythm and feel of your output triggers/gates.
- Use the **TRIGGER/GATE switch** and **MIDI/LIFE mode toggle** to change the interaction style on the fly—play Conway’s Game algorithmically, then switch to MIDI input for more controlled madness.

---

> Check more about Conway’s Game and get creative!  
[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)