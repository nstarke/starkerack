# Instruo — Tona

- [Manual PDF](../../manuals/Tona-Manual-A5.pdf)

---

[**Instruō tòna Oscillator User Manual (PDF)**](https://www.instruomodular.com/wp-content/uploads/2022/08/tona_web.pdf)

---

# Using the Instruō tòna to Create Full Length Eurorack Songs

The Instruō tòna is a versatile analog voltage-controlled oscillator (VCO) with built-in wavefolding, classic east/west coast waveforms, robust frequency modulation (FM), and sync options. While many modular patches excel at short riffs, building those into evolving, full-length tracks is a creative challenge. Below are strategies using the tòna—often in combination with other modules—to help you construct rich, structured songs.

---

## General Song Structure in Modular

To create full-length songs, you need:

- Evolving timbres
- Dynamic musical phrases and variation
- Transitions between sections
- Arrangement tools (mute/unmute, fade-ins/outs, pattern changes)
- Rhythmic and melodic variation

Below are practical tips focused on the tòna:

---

### 1. **The Tòna as a Theme Engine**

Use the tòna's precision tracking for melodies, basslines, or leads. Connect a sequencer for the fundamental theme of your song.

**Tip:**  
*Patch the tòna’s Triangle or Sine output for basslines, reserving the Wavefold output for leads or evolving pads.*

#### **Evolving Melodies:**
- Modulate the tòna’s 1V/Oct with multiple sequencers or switch modules to alternate between verses/choruses.
- Use quantizers or precision adders downstream to transpose or vary the melody across song sections.

---

### 2. **Dynamic Timbre Shaping with Wavefolding**

The built-in wavefolder invites morphing timbres, a powerful technique for musical development.

#### **Automated Timbre Morphing:**
- Sequence the Wavefold CV input using slow LFOs, stepped random (sample & hold), or a modulation sequencer.
- Use an envelope (triggered only in certain song sections) to open up wavefolding, creating contrast between verse/chorus or intro/build/drop.

#### **Scenes:**
- Use a sequential switch to swap between tòna waveform outputs for different parts of your arrangement (e.g., Sine for verses, Folded for choruses).

---

### 3. **FM and Sync for Texture Variation**

Introduce FM or hard sync for foreground moments or transitions.

#### **Sectional Texture:**
- Assign an LFO, other VCO, or looping envelope to the Linear FM input.
- Fade in FM modulation with a VCA controlled by a slow envelope to "open up" the sound, perfect for breakdowns or to announce a new section.

#### **Sync Moves:**
- During song transitions, use a trigger sequencer or manual gate button to re-sync tòna, disrupting or re-aligning rhythmic or melodic content.

---

### 4. **Song Arrangement with Modulation Routing**

**Voltage-Controlled Routing**:
- Employ matrix mixers, sequential switches, or addressable VCAs to switch tòna outputs, modulation destinations, or mix levels.
- Use trigger sequencers to automate section changes, mutes, or filter/VCA states for verse/chorus/bridge structure.

#### **Dynamic Muting:**
- Use VCAs to control tòna’s audio and modulation paths, muting or adding voices per section.

---

### 5. **Integration with Percussion and Effects**

Let tòna form harmonic, melodic, or atonal textures and use other modules for drums. Cross-modulate tòna with percussion sources for industrial/experimental breakdowns.

#### **FX Automation:**
- Patch tòna into delays, reverbs, wave shapers, or granular effects.
- Use sequenced or random modulation to vary effect parameters throughout the track.

---

### 6. **"Performance Macro" for Live Automation**

**Manual Song Arrangement:**
- Assign performance macros (grouped attenuators, mix controls, or big knobs/faders) to control tòna’s waveform mix, fold amount, and pitch transpose for each song section.

**Automated Song Structure:**
- Use a voltage-addressed preset manager, like the Xaoc Zadar's preset sequencing, to recall configurations of modulation depths, wavefolder settings, and crossfades at different song parts.

---

## Sample Song Flow Using Tòna

1. **Intro**:  
   - Slow, filtered Sine or Triangle from tòna with opening wavefold for evolving pad.
2. **Verse**:  
   - Add sequenced melody (via 1V/Oct), minimal FM, subtle wavefold.
3. **Chorus/Drop**:  
   - Switch tòna output to Wavefold, ramp up FM and resonance, open VCAs and FX sends.
4. **Breakdown**:  
   - Cut audio out except for FM noise from tòna, high modulation and sync, heavy effects.
5. **Build-Up/Outro**:  
   - Gradually bring back main sequence; change wavefold position, automate through scenes.
6. **End**:  
   - Fade tòna’s output via VCA or switch to a simpler waveform.

---

## Putting It All Together

Achieving full-length song structure in Eurorack is about deliberate modulation, dynamic routing, and rich transitions. The Instruō tòna’s multiple outputs, wavefolding, and FM capabilities make it a powerful centerpiece for any evolving patch. Use sequencers, switches, VCAs, and envelopes to create meaningful sections, automate changes, and keep the listener engaged throughout your performance.

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**