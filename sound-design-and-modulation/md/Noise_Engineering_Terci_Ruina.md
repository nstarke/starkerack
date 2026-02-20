# Noise Engineering — Terci Ruina

- [Manual PDF](../../manuals/Terci Ruina - Noise Engineering Documentation.pdf)

---

[**Terci Ruina Manual (PDF Link)**](https://manuals.noiseengineering.us/tr/)

---

# Creative Modulation with Terci Ruina (Noise Engineering)  
*For Distorted Percussion, Dubsteppy Basslines, and Haunting Pads*

The **Terci Ruina** is a triple-distortion 4HP Eurorack module, offering three distinct analog distortion circuits (FB, FF, FZ) in series or standalone, with a distinctly raw and chaotic character. Exploiting its modular patching and modulation potential can create wild, genre-pushing textures. Here’s how to get the most out of it for your sound design goals:

---

## 1. Creating Distorted Percussive Sounds

### Key Approaches:

- **Insert After a Percussion Source:** Route drum modules (analog or digital, e.g. BIA or samples) directly into the input of Terci Ruina.
- **Experiment with Input/Output Normalization:** By patching in and out between individual stages (FB, FF, FZ), you can reorder or isolate distortions for unique flavors.
- **CV Modulation:** Terci Ruina does not offer CV control over its distortion levels by default. To achieve dynamic, animated timbres:
    - **Use a VCA (pre-TR):** Modulate input amplitude with an envelope or LFO for amplitude-dependent distortion character.
    - **Place VCA (post-TR):** Use a short, snappy envelope to tame tails and create punchy, gated distortion.
- **Rhythmic Sidechaining:** If you want the distortion to "pump" in time with your drums, route the output through a VCA modulated by another track’s envelope/LFO.
- **Explore Filtering:** Pre- or post-filtering shapes which frequencies get distorted or amplified. E.g. a LPF before Terci Ruina means only low end gets heavy distortion—great for throbbing kicks.

### Patch Example:
1. Drum oscillator (e.g., BIA or analog kick/snare) → [VCA] (modulated by percussion envelope) → Terci Ruina IN 1
2. OUT 3 → [VCA or Env Follower] → Mixer
3. (Optional) Use output of OUT 1, 2, or 3 direct to mixer for parallel processing or layering.

---

## 2. Designing Aggressive Basslines (Dubstep, DnB)

### Key Approaches:

- **Distortion Stage Reordering:** Try routing through individual IN/OUTs to change saturation color (e.g., start with FZ fuzz, then FB, then FF). Each order yields different harmonics.
- **Envelope Shaping:** For dubstep wobble, send your bass voice through a filter with an envelope/LFO modulating cutoff and/or resonance, then into Terci Ruina.
- **Manual Performance:** Twist the TR knobs live to create evolving, expressive distortion sweeps. For more control, patch an external voltage-controlled attenuator (like an external VCA) in series.
- **Parallel Bass:** Blend clean and processed signals. Use a mixer to recombine for clarity with aggression.
- **Resonant Filtering:** Insert resonant LP or BP filter pre- or post-TR, modulated by fast LFO or envelope, for talking/wah timbres.

### Patch Example:
1. Bass oscillator (complex, wavetable, or saw) → [Filter, cutoff modulated by LFO/env] → Terci Ruina (try inputting into FZ or reordering stages)
2. OUT 3 → [VCA, envelope-controlled] → Sub-mixer
3. Clean signal parallel to processed signal for added punch.

---

## 3. Building Atmospheric, Haunting Pads

### Key Approaches:

- **Gentle/Glitchy Distortion:** Lower input gain into Terci Ruina, just barely hitting clipping. This keeps it textural, not overblown.
- **Modulating Input Dynamics:** Subtle modulation of input level with slow, looping envelopes to animate distortion movement over held pads.
- **Post-TR Effects:** Combine with reverb & delay after Terci Ruina for vast, eerie space. Ring mod or granular processing can add further complexity.
- **Dynamic Filtering:** Place VCF after TR, modulate cutoff with a very slow LFO for an evolving, spectral effect.
- **Multistage Patching:** Parallel process different voices through different TR sections, recombine, pan, and effect separately for width and movement.

### Patch Example:
1. Polyphonic pad voice (audio interface or oscillator cluster) → VCA (modulated by slow attack envelope or LFO) → Terci Ruina IN 1 or 2
2. OUT 3 → Stereo reverb → Delay → Filter (modulated by LFO or random CV) → Mixer

---

## Pro Tips:

- **Order Matters:** Try different ordering of the distortions by patching IN/OUT individually; FB → FF → FZ, or try FZ → FB → FF, etc.
- **Cleanup:** After extreme distortion, put a VCA or gate (Sinclastic Empulatrix, Sinc Bucina) at the end of chain to control excessive noise or feedback.
- **Live Play:** Even without CV, manual knob tweaks during live performance can yield dynamic, morphing character.

---

For complete details, refer to the [**official manual**](https://manuals.noiseengineering.us/tr/).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)