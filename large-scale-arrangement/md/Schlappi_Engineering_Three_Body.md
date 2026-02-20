# Schlappi Engineering — Three Body

- [Manual PDF](../../manuals/three_body_manual_01302023a.pdf)

---

[**Three Body Manual (Schlappi Engineering) – PDF Download**](https://schlappiengineering.com/manuals/threebody_manual.pdf)

---

# Using Schlappi Engineering Three Body For Full-Length Songs in Eurorack

## Overview

The **Schlappi Engineering Three Body** module is a highly flexible phase, frequency, and ratio FM engine with three digitally-linked oscillators and deep modulation possibilities. While Eurorack excels at improvisational sound, bass, and lead creation, using a powerful tool like Three Body to architect a coherent, dynamic, full-length track requires strategizing control, structure, and musical evolution.

Below, I provide creative workflows, patch ideas, and modular combinations to help bridge the gap between "cool patch" and **songwriting** with Three Body at the center of your system.

---

## 1. **Polyphonic and Harmonic Frameworks**

### **Use Three Body as a Chord Engine or Drone Bank**
- **Patch Approach:**
  - Set each oscillator to different but musically related ratio modes (e.g., root, third, fifth, or pedal bass + intervals). Use the RATIO and SYNC features for easy tuning.
  - Modulate ratios rhythmically using sequenced CV, envelopes, or LFOs tied to your song’s sections (verse/chorus contrast, modulation for mood, etc.).
- **Result:** 
  - Build evolving chord beds, shifting drones, or sustained harmonic fields behind leads or vocals through the song.

### **Stereo Spread and Movement**
- Route center oscillator's Sine/Cosine or Saw/Cosaw to stereo channels with dynamically modulated phase offsets for animated, wide stereo pads.
- Automate pan or crossfade between outputs using VCAs under sequencer or manual control.

---

## 2. **Melodic and Bass Material**

### **Complex FM & Phase Mod Bass/Leads**
- Use one oscillator in FREE HIGH as the main voice; route other oscillators as FM/phase modulators.
- Sequence V/OCT of the main oscillator from your sequencer or quantizer. Use step-modulation or evolving LFOs to alter FM indices/timbre for "verse/chorus" variation or evolving sections.

### **Song Section Variation**
- **Breakdown:** Use deep FM/PM indices to create noise or percussion textures for breakdown & riser sections.
- **Drop/Chorus:** Dial indices back to reveal clear bass/melodic content; flip oscillator states for brighter timbres or harmonic progression.

---

## 3. **Rhythmic & Percussive Elements**

### **Polyrhythmic Oscillator FM**
- Clock or trigger external rhythms into the SYNC input of one oscillator.
- Patch differing rhythms into the outer oscillators in ratio mode for shifting polyrhythms and FM clangorous percussive effects.
- Use sequential switches or clock dividers/multipliers to create macro song progressions (e.g., verse/chorus A/B using different oscillator sync sources).

### **FM/PM for Clicks, Blips, and Snares**
- Exploit through-zero FM and sharp phase modulation for percussive, metallic, or noise-based hits—excellent for "abstract drums" and fills.

---

## 4. **Macro Song Control & Automation**

### **Preset Morphing**
- Use voltage-controlled switches or matrix mixers to route modulation and change each oscillator’s mode/state per section.
- Scene-based control: For dramatic structure changes, switch oscillator modes with gate/button control (manual or via external sequencer) to jump between setups (e.g., from drone to melody+percussion).

### **Envelope and Sequencer Integration**
- Use multi-stage function generators or complex LFOs (like Maths) to automate fade-ins, evolving FM indexes, or stereo width across song sections.

### **Feedback, Cross-Modulation, and Chaos**
- Deploy feedback/cross-phase modulation under controlled conditions for rising tension, climactic drops, noise sweeps or breakdowns. Fade in chaos for transitions, then return to order.

---

## 5. **Tips for Full Song Structure**

- **Song Transitions:** Use the module’s SYNC and ratio tracking to lock to external clock/LFOs—allowing those clocks to evolve over time (riser, tempo-change, breakdowns).
- **Automation:** Pair with keyframe sequencers (like Malekko Voltage Block, Frap Tools USTA) for parameter animated changes per section.
- **Performance:** Use manual or footswitches to switch phase direction, index depths, stereo configurations, or oscillator tracking for live arrangement.
- **Mixing Considerations:** Use VCAs (for gate/velocity), filters (for subtractive contrast), and stereo mixing for evolving textures and dynamic range.

---

## 6. **Putting it Together: Example Song Structure**

1. **Intro:** Slow drone with gradual stereo phase sweep (long LFO on phase CV), subtle evolving FM texture.
2. **Verse:** Main melody in oscillator 1, driven by external sequencer; supporting oscillator in ratio mode for harmony.
3. **Chorus:** High index FM/PM swept in for brash timbre; all three oscillators harmonized; phase modulation increases stereo spread.
4. **Breakdown:** Oscillators cross-modulated, deep FM index for noisy/abstract textures; percussive elements.
5. **Outro:** Fade back to one oscillator, slow stereo phase offset, index back to zero for a clean, pure tone.

---

## **Module Combinations for Compositional Control**

- **Sequencers (Korg SQ-1, Make Noise René, Eloquencer):** for main melodies, mod index automation.
- **Envelope Generators/VCAs** for dynamic timbral control.
- **Switching Modules (Doepfer A-151, Mutable Branches):** for macro section switching.
- **Matrix Mixers (Doepfer A-138m, Erica Synths Matrix Mixer):** for easy re-routing modulation sources and oscillator cross-modulation per section.
- **Stereo Mixers & Effects (Mordax Data, FX Aid):** to capture, process, and automate stereo out for space/finalizing.

---

By thinking of the Three Body as three “voices” interactively tied together in timbre, harmony, and rhythm, and by **sequencing both its pitch and modulation states** in tandem with your compositional sections, it becomes a dynamic instrument for full-album-scale musical narratives, not just a wild FM drone box.

---
**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**
