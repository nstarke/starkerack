# Altered State Machines — Eris

- [Manual PDF](../../manuals/Eris _ Altered State Machines.pdf)

---

**[Eris 4x4 Matrix Mixer Manual (PDF)](https://alteredstatemachines.net/eris)**

---

# Creative Modulation With Eris 4x4 Matrix Mixer

The Eris 4x4 Matrix Mixer is a powerful tool for constructing complex signal routing, feedback, distortion, and modulation schemes. With DC-coupled inputs/outputs and per-signal gain up to 4x, you can use it to sculpt both audio and CV in unique ways. Here’s how to exploit its features for various advanced sound design goals:

---

## 1. Distorted Percussive Sounds

**Goal:** Achieve aggressive drum hits and glitchy textures through distortion, feedback, and dynamic routing.

### Techniques:
- **Overdrive Inputs:** Send drum or percussive audio into one input and crank its corresponding pot above unity (up to 4x) to clip the signal internally, creating distortion.
- **Feedback Patch:** Patch an output back into an unused input via an effects pedal or module (e.g., distortion or wavefolder), then send that return to additional outputs. Increasing the gain will intensify distortion and feedback.
- **Aux Mute as Transient Generator:** Use the vactrol-based soft mute on the auxiliary input/output as a clickless on/off gate. Send a drum sound or noise burst to the aux input, manually or with a gate, for percussive gating or muted bursts.
- **Resonant Feedback:** Route an output through a filter/resonator, returning to an input to create metallic or self-oscillating percussive attacks when struck with short envelopes.

### Example Patch:
1. Drum module → Eris Input 1 (set Gain to 3x–4x)
2. Output 1 → distortion pedal / wavefolder → Eris Input 2
3. Output 2 → Eris Input 3
4. Use aux input with soft mute for gating a noise or snare burst.

---

## 2. Aggressive Basslines (Dubstep/Drum & Bass)

**Goal:** Generate thick, punchy, modulated basslines with movement and edge.

### Techniques:
- **Layered Oscillators:** Patch multiple oscillators (saw, square, sub) to Eris inputs, use pots to balance or overdrive layers for a fat, harmonically rich sound.
- **Feedback Modulation:** Send one output through a filter or wavefolder, then back to an Eris input—use the gain to push into self-oscillation or heavy saturation.
- **Dynamic Waveshaping:** Modulate input gains with CV (if your version supports it, or use external VCAs pre-Eris) to create dynamically shifting distortion and timbral changes.
- **Aux Channel Crunch:** Send the main bass out of Output 1, then route processed effect returns into aux input. Use the mute to animate (chop) sections of the bassline for rhythmic interest.

### Example Patch:
1. Oscillator 1 (saw) → Input 1, Oscillator 2 (square/sub) → Input 2
2. Outputs 1 & 2 to filter/modules → return to Inputs 3 & 4 (feedback)
3. Filtered Output 3 to aux input → aux output as processed bass
4. Experiment with different gain settings for loud, saturated growls or wobbles.

---

## 3. Haunting Atmospheric Pads

**Goal:** Construct complex, evolving soundscapes and pads that morph in tone and space.

### Techniques:
- **CV Matrix Routing:** Feed multiple slow LFOs or envelopes to Eris inputs and use outputs to simultaneously modulate cutoff, pan, reverb amount, etc., across several modules—use the matrix functionality for rich, cross-modulated modulation.
- **Blend Environmental Layers:** Mix samples, drones, and granular textures into inputs. Use matrix mixing to crossfade and spatially split layers to different effects chains (reverb, delay, shimmer).
- **Feedback for Etherial Tones:** Output a reverb FX return into an input for feedback pads that slowly self-oscillate and evolve. Adjust gain for subtle shimmer to howling drones.
- **Soft Muted Swells:** Use the aux input & mute to bring in textural layers gradually and clicklessly, ideal for spooky fade-ins and fade-outs.

### Example Patch:
1. LFO 1–4 → Inputs 1–4; Outputs route to mod destinations (filter, FX, panning, etc.)
2. Drones/textures → Inputs 1–2; outputs to granular, reverb, delay → return to Inputs 3–4 for feedback.
3. Send reverb return into aux input, use the mute switch for gentle rising/falling atmospheres.

---

## Pro Tips

- **Patching for Surprise:** Experiment with patching audio to CV or CV to audio paths to find unexpected rhythms or distortions.
- **Gain Staging:** The high headroom lets you experiment safely—but keep levels in check to avoid accidentally overloading downstream equipment.
- **Matrix Modulation:** Use Eris as a CV modulation matrix, with outputs routed to modulate VCA, VCF, VCO, or FX parameters, for extremely complex morphing patches.

---

### [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)