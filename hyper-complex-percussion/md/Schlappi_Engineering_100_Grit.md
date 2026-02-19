# Schlappi Engineering — 100 Grit

- [Manual PDF](../../manuals/100_GRIT_MANUAL_20190826.pdf)

---

[**Schlappi Engineering 100 Grit Manual PDF**](https://schlappiengineering.com/wp-content/uploads/2020/04/Schlappi-Engineering-100-Grit-Manual-2020.pdf)

---

# Creating Densely Rhythmic, Hyper-Complex Percussion with the 100 Grit

The **Schlappi Engineering 100 Grit** is a touch-controlled distortion, filter, and VCA, designed not just for classic timbral shaping but also for unruly, generative chaos—ideal for experimental, polyrhythmic percussion. Here’s how to harness its features for deeply complex rhythmic music:

---

## 1. Understanding 100 Grit's Percussive Power

- **Role:** The 100 Grit can be both a voice (self-oscillating, noise-generating, feedback) and a distortion/filter/effect for drums and percussion.
- **Features for Percussion:**
  - Harsh, punchy distortion and feedback.
  - Voltage-controlled VCA and filter for shaping dynamics and tone.
  - Touch points and internal feedback paths enable performable and pseudo-random variations.
  - Able to self-oscillate and/or turn into a noise source, useful for percussion voices.

---

## 2. Patch Ideas for Densely Rhythmic Patterns

### **A. Self-Oscillating Percussive Voice**

1. **Setup for Self-Oscillation:**
   - No external input, or patch a trigger into an input (e.g., audio-rate trigger for physical modeling).
   - Set **RES** to just at or above self-oscillation (see Calibration in the manual).
   - Turn up **GAIN** to drive the output.
   - Use **DIST OUT** for a noisy, metallic drum voice.

2. **Triggering and Modulation (Complex Rhythms):**
   - Use external, polyrhythmic gate/trigger sources (from Euclidean sequencers, clock dividers, or anything generating different time signatures) to modulate **FM1**, **FM2**, **GAIN CV**, or **RES CV**.
   - Each CV input can affect timbre and articulation. Polyrhythmic modulation of the VCA and resonance can create intricate, crossfading accents.

3. **Performance:**  
   - Use the **Touch Points** to "play" fills, rolls, and randomizations.
   - Touch multiple points with conductors for stochastic changes in feedback, amplitude, and filter frequency.
   - For emergent, complex rhythms, patch irregular trigger sources into the touch points as well.

### **B. Processing Percussive Material**

1. **Insert Percussion Sample(s):**
   - Patch drum machine, chopped breakbeats, or complex triggered noise into **IN 1/IN 2**.
   - Use input distortion for transient shaping and high attack.

2. **Rhythmic Modulation:**
   - Modulate **GAIN CV** and **FM1/FM2** with different clocks/LFOs running at non-matching divisions (e.g., 5-step vs. 7-step, or tuplets).
   - Use sequencers outputting weird time signatures as CVs.
   - Short, percussive envelopes on **RES CV** for snappy, resonant filter sweeps.

3. **Hybrid Patching:**
   - Mix in sustained inputs with raw triggers into **IN 2** to layer tones (thuds, ticks) with the main audio.
   - Combine feedback paths (DIST out back into FM inputs) with clocked gates for unpredictable, rolling percussion layers.

### **C. Feedback Noise Machine (No Inputs)**
- Set up the "Noise Box" patch (IN1/IN2 up, GAIN up, x100 ON, no input).
- Play touch points or modulate inputs with polyrhythmic CVs/gates.
- Use the resulting output as percussion—metallic, bit-crushed, glitch, or raw.

---

## 3. Making It Unique, Punchy, and Hyper-Complex

**Tips:**

- Take advantage of the extremely wide gain/distortion range (use the x100 switch for extreme effect).
- Don't ignore subtle settings—gentle feedback and low resonance can yield drum machine–like clicks or woodblocks; extreme values yield more clangorous hits.
- Use touch points as interactive percussive fills and random layer triggers.
- Use the pole outputs and the two OUT types (OUT, DIST OUT) for parallel processing: e.g., layer clean and dirty percussion, route to different effect chains.
- Normalize unused CV/audio inputs to internal feedback paths for more internal variation.
- Patch complex, multi-stage envelopes (modulated at polyrhythmic rates) into GAIN CV or RES CV for accent cycling and groove complexity.

**Example:**
```
- External clock (e.g., 5/8 at 160bpm) -> trigger sequencer -> FM1
- Another clock (e.g., 7/8 at 160bpm) -> envelope generator -> GAIN CV
- Distorted snare input -> IN 1; percussive sine blip -> IN 2
- Touch points manually bridged during live performance for unpredictable 'glitch fills'
- Use 'DIST OUT' as main percussion feed, with 'OUT' for parallel, less-distorted thump
```

---

## 4. Takeaway

The 100 Grit is beyond a normal distortion or filter—it’s a playable, feedback instrument. Treat every modulation, input normalization, and touch point as a voice- or rhythm-altering parameter. Combine this with multi-clocked CVs, irregular envelopes, and interactive touch play for patterns no grid-based drum machine can sequence.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)