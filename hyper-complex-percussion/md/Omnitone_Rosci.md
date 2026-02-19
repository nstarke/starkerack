# Omnitone — Rosci

- [Manual PDF](../../manuals/Rosci-Manual.pdf)

---

[Rosci User Manual PDF](https://omnitone.ca/manuals/Rosci_Manual_Rev3.pdf)

---

# Making Hyper-Complex Percussion With Rosci (Eurorack)

The **Rosci** module, as described in the manual, is a highly flexible digital oscillator designed to excel at customized waveform generation. Its ability to morph between shapes, interpolate, and introduce nonlinearities makes it perfect for *unusual, percussive, and detailed rhythmic material*, especially when you combine it with external rhythmic modulation sources.

Below is a detailed strategy for achieving **densely rhythmic, polyrhythmic, and highly complex percussion sequences** using Rosci, along with tips for maximizing its uniqueness and punch.

---

## 1. Use Rosci As a Percussive Voice

### **Set Up Rosci as a Drum Voice:**

- **Mode**: Keep Rosci in VCO mode for metallic digital drums; flip to LFO mode for slow, generative CV percussive triggers.
- **Waveform Complexity**: Use the *Generate* and *Complexity* parameters to craft transient-rich, short, inharmonic wave shapes. Try 2-6 points for clicky, snappy percussive attacks; add harmonics for metallic noise.
- **Roundness and Formants**: Experiment with these to mimic physical, vocal, or organic drum-like timbres.
- **Detune**: Detune for percussive clashing overtones.

---

## 2. External Rhythmic Control for Polyrhythms

### **Triggering & Sequencing:**

- **Trigger Input**: Patch different trigger/gate streams (e.g., from Euclidean, polyrhythmic, or random step sequencers) into Rosci's trigger input.
    - Each distinct trigger pattern can activate Rosci at off-grid, overlapping rhythms for polyrhythms or odd time signatures.
- **V/OCT Input as Pattern Parameter**: Sequence Rosci with shared or independent melodic or non-traditional *pitch patterns* (e.g., microtonal, odd scales) for further rhythmic variation.

---

## 3. Modulate the Sound for Variation

Assuming you have several modulation sources (LFOs, random generators, sequencers):

- **CV Inputs**: Patch rhythmic CV sources into Complexity, Harmonics, Formants, and Detune.  
    - E.g., send clock-divided or probability-skipping gates into Harmonics/Complexity for per-step timbral changes that sync or desync with Rosci’s triggers.
- **Envelope & Random**: Patch fast, percussive envelopes or stepped random voltages (e.g., sample-and-hold based on polyrhythmic triggers) to Roundness or Formants for morphing attacks/sustains.
- **Morphing & Interpolation**: Switch interpolation methods mid-sequence for jumps between sharp and smooth transitions—emphasize punchy vs. clicky textures.

---

## 4. Patch Ideas for Complex Rhythms

- **Multi-Trigger Input**: Combine several gate patterns with a logic module (OR, XOR) to drive Rosci's trigger input for interlaced, complex rhythms.
- **FM/AM**: Use an audio-rate VCO or fast envelope to modulate the pitch (V/OCT) input for “FM drum” or clangorous bell sounds, or modulate parameters for constantly changing attacks.
- **Manual Play**: Tap out triggers live for fills, then automate them for evolving patterns.

---

## 5. Unique Percussive Effects

- **CV-Controlled Switching:** Use a sequencer to rhythmically switch/interpolate Rosci's parameters in extreme ways, turning each trigger into a seemingly new drum/click sound.
- **Formant Compression:** Set Formants and Harmonics to extremes for "vocal percussion"—Kabuki or robotic-sounding hits.
- **Max Detune:** Sweep Detune with random or sneaky slow LFOs to create moving, phasey percussive ripples.

---

## 6. Combine With Effects

- **Resample**: Route Rosci to a granular or delay module and re-trigger with polyrhythmic gates.
- **Ring Mod/Distortion**: Feed output into analog ring modulation or distortion for raw, accentuated texture.

---

# Summary Table

| Feature      | Rhythmic / Percussive Application           |
|--------------|---------------------------------------------|
| Generate     | Make new per-hit waveforms on triggers      |
| Complexity   | Morph between attack types                  |
| Roundness    | Control punch/snap versus mellow            |
| Harmonics    | Shift metallic/woody/raspy content          |
| Formants     | Vowelly, vocal timpani                      |
| Detune       | Adds movement; detune for metallic clangs   |
| V/OCT        | Sequence for melodic or FM drum sounds      |
| Output       | Use as audio or trigger for next module     |

---
**Tips**:  
- Use different, unsynchronized modulation clocks for each parameter control.
- Feed Rosci’s output to a VCA controlled by rhythmic envelopes for even more articulation.
- Resample or layer Rosci with other drum modules for hyper-complex grooves.

---

[Rosci User Manual PDF](https://omnitone.ca/manuals/Rosci_Manual_Rev3.pdf)  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)