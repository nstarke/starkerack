# Tiptop Audio — TOMS909

- [Manual PDF](../../manuals/Tiptop_Audio_TOMS909_ns.pdf)

---

[Download the TOMS909 Manual (PDF)](https://tiptopaudio.com/manuals/TIPTOPAUDIO_TOMS909_MANUAL.pdf)

---

# Using the Tiptop Audio TOMS909 for Dense, Hyper-Complex Percussive Sequences

The Tiptop Audio TOMS909 is a powerful dedicated tom drum voice module, inspired by the Roland TR-909, but enhanced for the modular world. It offers the punch, clarity, and dynamic range of classic analog toms, while also enabling creative manipulation through voltage control and modular patching—perfect for experimental, densely rhythmic, and hyper-complex percussion.

Below are advanced strategies and patch tips to maximize its potential in polyrhythmic, odd-time, and deeply layered rhythm music:

---

## 1. **Layering and Polyphony**

- **Multichannel Out:** Each tom (Low, Mid, High) has its own output. Patch each tom to a dedicated mixer channel for independent stereo placement, panning, and further effects.
- **Mixed Out:** Use the MIX OUT for quick summed toms—great for creating a monolithic, thick percussive layer.

## 2. **Complex Triggering and Polyrhythms**

- **Separate Gating:** Utilize independent gate sequencer channels for each tom. Trigger each with different step lengths or clock divisions for natural polyrhythms.  
  - *Example*:  
    - LOW: 6-step sequence  
    - MID: 5-step sequence  
    - HIGH: 7-step sequence  
  This produces shifting, endlessly evolving cycles.
- **Trigger Riot / Advanced Sequencers:** Pair with trigger sequencers like the Tiptop Trigger Riot, or other complex Eurorack gate/trigger sources, to define intricate, asymmetrical patterns (see manual’s Riot patch).

## 3. **Dynamic Accent for Groove and Emphasis**

- **Accent Per Voice:** Uniquely, TOMS909 allows independent accent triggering per tom drum.  
  - **Patch Suggestions:**  
    - Use separate accent triggers, timed differently from main gates.  
    - Sequence accents to emphasize offbeats or unexpected step locations for more organic & 'human' feel.
  - **CV Accent:** Automate accent intensity/level for micro-dynamic changes.

## 4. **Time Signature and Pattern Manipulation**

- **Non-Standard Divisions:** Assign toms to gate sequencers running at different clocks (e.g., one at 4/4, one at 7/8, one at 5/16) to generate composite odd-time signatures and polymetric interaction.
- **Step Skipping & Rotations:** Use sequencers with pattern rotation, skipped steps, or probability for evolving rhythmic diversity.

## 5. **Advanced Sound Shaping (Timbrality & Punch)**

- **Voltage Control over Tune:**  
  - Patch LFOs, stepped sequencers, or function generators to VC-TUNE inputs for each drum.
  - Audio-rate modulation from other VCOs (like Tiptop’s Z3000) to VC-TUNE creates FM-style metallic overtones and radical timbral shifts—especially interesting for glitchy, noisy, or futuristic percussion.
- **Decay Per Drum:** Modulate decay times per tom to create tight, frenetic fills or long, droning tom pulses for dramatic effect.
- **Accent as a Gain Tool:** The Accent knob acts as a fine control for output gain—subtly compress or exaggerate dynamics in the mix.

## 6. **Further Modular Integration**

- **CV Over Decay/Tune:**  
  - Patching sequencers/envelopes into VC-TUNE enables per-step pitch variation, making toms sound alive and unpredictable in a groove.
- **External FX:** Use stereo delays (Z-DSP PingPong etc.), reverb, or even bitcrushers and distortion for energy and width.

## 7. **Example Hyper-Complex Patch (Conceptual):**

```
Low Tom: Triggered by a 5-step gate sequencer, VC-TUNE modulated by a slow LFO.
Mid Tom: Triggered by a 7-step gate sequencer, Accent CV from a random S&H, Decay modulated by an envelope following another percussion voice.
High Tom: Triggered by a 9-step gate sequence, VC-TUNE FM’d by a Z3000 VCO, accent manually played (with a pad or controller).
All Out: Indiv. outs sent through panning, stereo delay, and reverb for width/space.
```

- As steps and accents overlap, a complex web of interlocking rhythms emerges, with shifting pitch/tone and dynamic, percussive power.

## 8. **Performance Tips**

- Manually tweak TUNE and DECAY for dramatic fills and live variation.
- Repatch accent triggers during performance for extreme changes in groove dynamics.
- Use external random/sample&hold sources for evolving, pseudo-generative patterning.

---

**For further inspiration and advanced patch examples, always reference the official manual: [TOMS909 Manual (PDF)](https://tiptopaudio.com/manuals/TIPTOPAUDIO_TOMS909_MANUAL.pdf)**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)