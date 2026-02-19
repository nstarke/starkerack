# Noise Engineering — Sec Ruina

- [Manual PDF](../../manuals/Seca Ruina - Noise Engineering Documentation.pdf)

---

[Seca Ruina Manual (PDF)](https://manuals.noiseengineering.us/sr/)

---

# Using Seca Ruina for Hyper-Complex Percussion in Eurorack

## Module Recap

**Type:** Multiband Distortion / VCA  
**Function:** Splits audio input into 3 bands (Low/Mid/High), distorts each individually, allows CV control per band or globally, features individual outs and sum out, onboard VCA with bypass.  
**CV Range:** 0 to 5V for all CV inputs

---

## Generating Densely Rhythmic, Hyper-Complex Percussion

**Seca Ruina** is a distortion-effect module rather than a voice. Its extreme bandsplitting and per-band drive capabilities make it ideal for reshaping, mangling, and rhythmically modulating percussion sounds and sequences. Here’s how to manipulate it for punchy, unique, and percussive results:

### 1. **Preparing the Input**
- **Input Material:** Send drum loops, percussion samples, or rapid-fire synthesized percussion hits to the Audio In. Melodic complex patterns or even noise bursts work great.
- **Source Variety:** Use polyrhythmic triggers/sequences to generate percussive sound sources feeding Seca Ruina.

### 2. **Splitting & Driving with Polyrhythms**
- **Polyrhythmic CV Modulation:**
  - Patch different clock divisions or Euclidean/polyrhythmic gates from a sequencer (e.g., Pam’s New Workout, Euclidean Circles) to the CV inputs (Low, Mid, High). Each band can be dynamically overdriven according to a unique rhythm.
  - **Example:** A 3-step pattern for low, 5-step for mid, and 7-step for high. Each band pulses/distorts in a distinct rhythmic cycle, creating interlocking beats.

- **Global Rhythmic VCA:**
  - Patch a complex envelope, LFO, or stepped random pattern with odd time signature to the “All” CV input. This rhythmically gates/distorts all bands simultaneously, or layers above the per-band modulations.

### 3. **Complex Patterns via Per-Band Outputs**
- **Individual Outs:**
  - Route each band’s output to different effects (filters, delays, comb filters, ring mods) and re-combine in a mixer or matrix mixer. This enhances separation and punch, letting you shape distinct polyrhythmic layers before summing.
  - Post-process outs with further amplitude or CV rhythm modulation. 

- **Sum Out:**
  - Process the summed output for a cohesive but dense percussive result—adjust the drive knobs to give each band a tailored distortion character.

### 4. **Patch Tricks for Maximum Impact**
- **Dynamic Range via VCA:**
  - Flip between heavily distorted and clean sounds using dynamic or sequenced modulation of the VCA (Sum CV). Use accent tracks or random gates for unexpected percussive punches.
- **Transient Design:**
  - Feed short envelope attacks or triggers to any CV input for pseudo-transient shaping. Each band can “snap” in at different times for ultra-complex grooves.
- **Audio-Rate CV:**
  - Try feeding audio-rate signals to the band CVs (e.g., fast LFOs or oscillators in complex polyrhythmic relation) for brutal audio-rate amplitude/distortion modulation — adds chaotic percussive harmonics.

### 5. **Advanced Sequencing & Performative Control**
- **Manual Performance:**
  - Ride the band drive knobs live for accent and fill effects in complex drum passages.
- **Preset Switching:**
  - If you have a sequencer with preset CV outs, flip between different polyrhythmic drive CV patterns over time.

---

## Example Patch 

**Goal:** Dense, evolving beat cutting through with distinct, morphing textures.

1. **Drum Loop (polyrhythmic pattern)** → Seca Ruina Audio In  
2. **CV Generator 1 (5/8 time LFO or random sequence)** → Low CV  
3. **CV Generator 2 (7/16 time Euclidean)** → Mid CV  
4. **CV Generator 3 (3/4 stepped voltage sequence)** → High CV  
5. Tweak drive knobs for flavor  
6. Patch **Low Out** → Envelope Follower → Sidechain synth bass  
7. **Sum Out** → Mixer/Master for dense final output

> Layer and process each band differently for stunning complexity and independence.

---

**Manual PDF:** [Seca Ruina Manual](https://manuals.noiseengineering.us/sr/)

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)