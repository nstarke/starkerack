# WMD SSF — Chimera

- [Manual PDF](../../manuals/Manual_v1.2.pdf)

---

[WMD Chimera Manual (PDF)](https://wmdevices.com/pages/chimera-manual)

---

# Creative Ways To Use The WMD Chimera  
*Metallic Percussion Synthesizer — Eurorack Patch Ideas & Tips*

The WMD Chimera is a unique percussion module capable of shimmering, metallic timbres and evolving granular textures. Its blend of dense digital grittiness and physical modeling opens up a variety of patching options within your Eurorack system. Here are some creative uses and patch recipes:

---

## 1. **Dynamic Drum Textures**

### **Recipe: Chimera as Main Percussion Source**
- **Trigger**: Use a trigger sequencer such as the ALM Pamela’s New Workout, Mutable Instruments Grids, or any Euclidean trigger generator to fire the Chimera.
- **Accent**: Patch an accent or velocity output from an expressive controller (like Intellijel Tetrapad, or a velocity-sensitive MIDI-to-CV module) to the ACCENT input to produce dynamic emphasis within your patterns.
- **Choke**: For hi-hat style staccato, patch a closed-hat trigger or another rhythmic burst to the CHOKE input, simulating classic open/closed hat behavior.

---

## 2. **Granular Drones & Atmospheric Beds**

### **Recipe: Infinite Textural Wash**
- **Decay & Feel**: Set DECAY high and use the final (free oscillation) FEEL mode for constantly morphing sound beds.
- **Pitch CV**: Modulate PITCH by routing a slow random LFO (like from Make Noise Maths or Mutable Instruments Tides) into the PITCH input.
- **Surface CV**: Use an envelope follower from an external signal (like contact mic or field recorder input via Mutable Instruments Ears or Make Noise Mimeophon’s ENV OUT) to sweep the SURFACE parameter, creating responsive “live” surfaces.
- **FX**: Add comb filtering and modulate FX AMT with another slow LFO or stepped random for ever-evolving metallic drones.

---

## 3. **Polyrhythmic & Algorithmic Grooves**

### **Recipe: Algorithmic Rhythm Machine**
- **Trigger**: Patch two or more clock sources (e.g., 7/8 vs. 8/8) to TRIG and ACCENT via logic modules (such as Mutable Instruments Branches or Doepfer A-166) for swingy, unpredictable patterns.
- **VCA**: Use a CV grid sequencer (e.g., Malekko Voltage Block or Tiptop Z8000) to modulate the VCA input, creating accentuated or ghost notes with evolving volume patterns.

---

## 4. **Metallic Melodic Lines**

### **Recipe: Sequenced Metal**
- **Pitch Sequence**: Use a sequencer like Make Noise René or Intellijel Metropolis to sequence melodic lines via the PITCH input.
- **Envelope Modulation**: Send snappy envelopes (Maths, Zadar, Quadra, etc.) to the DECAY or SURFACE parameters for morphing articulation on each note.
- **FX AMT CV**: Sequence or randomly modulate FX AMT with stepped voltages from a random source (e.g., Mutable Instruments Marbles or Wogglebug) for chromatic, laser-like effects.

---

## 5. **Layered Percussion in Drum Bus**

### **Recipe: Hybrid Drum Kit**
- **Parallel Drum Channels**: Mix the Chimera with classic analog kick/snare modules (like Tiptop Audio BD808, SD909) and sample players (like 2hp Play or Erica Drum Sample) for layered and complex percussion sounds.
- **Just A Splash**: Use the Chimera as an occasional layer triggered via logic (XOR, AND gates) when both your kick and snare fire together, creating “special moment” metallic bursts in your mix.

---

## 6. **Audio Rate Modulation & Processing**

### **Recipe: Audio-Rate CV Madness**
- **Audio Rate Modulation**: Patch the output of another oscillator (e.g., Dixie II+, STO) into the FX AMT or PITCH CV input for FM-like metallic mayhem.
- **External FX**: Route Chimera’s OUT into granular or spectral processors (Mutable Instruments Clouds, Make Noise Mimeophon, Expert Sleepers Disting in spectral mode) for further wash and glitch processing.

---

## Module Type Recommendations

- **Random/CV Generators**: Mutable Instruments Marbles, Wogglebug, Turing Machine
- **Sequencers**: Make Noise René, Intellijel Metropolis, Malekko Voltage Block
- **LFOs/Envelopes**: Make Noise Maths, XAOC Zadar, Intellijel Quadra
- **Logic & Utility**: Mutable Instruments Branches, Doepfer A-166, Erica Synths Pico Logic
- **Mixers/VCAs**: Intellijel Quad VCA, Mutable Instruments Veils
- **FX**: Mutable Instruments Clouds, Strymon Magneto, Make Noise Mimeophon
- **Controllers**: Tetrapad, MIDI-to-CV/Velocity modules

---

Explore these patches and ideas to unlock the full potential of the WMD Chimera in your rack!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)