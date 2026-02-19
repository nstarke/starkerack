# Intellijel — Atlx

- [Manual PDF](../../manuals/Atlx - intellijel.pdf)

---

[Atlantix Expander (Atlx) Manual PDF](https://intellijel.com/downloads/manuals/Atlantix_Expander_Manual_2024.09.12.pdf)

---

## Using the **Atlx** (Atlantix Expander) for Dense, Hyper-Complex Percussion & Rhythmic Patching

The **Atlx** is an expander for the Intellijel **Atlantix** dual oscillator/subtractive synth voice, primarily adding 16 extra jacks including independent waveform and filter outs, and a built-in ring modulator. While not a dedicated rhythm generator or trigger sequencer, **the Atlx and Atlantix combo can be pushed into advanced percussive territory with creative patching**:

---

### 1. **Patch Individual Waveforms for Percussive Layering**

- **Dedicated outs** for both A and B oscillators (Sine, Triangle, Saw, Square w/PWM on A, Sub Square on A) allow you to:
    - Patch each waveform to different VCAs/Filters for separate dynamic envelope control.
    - Layer multiple rapid VCO “clicks” and “thumps” as drum-voice elements (e.g., Triangle for kick, Square for snare body).
    - **Complex Percussion Tip:** Cross-patch envelopes and LFOs to VCO pitch or pulse width for FM "snap" or transients.

### 2. **Advanced Filtering for Sculpting Rhythmic Timbres**

- **Filter outs** (Lowpass, Highpass, Bandpass, Phazor):
    - Send different waveforms to different filter outputs; sequence or randomly switch between them for morphing drum timbres.
    - Stack filter outputs into VCAs with independent envelopes for layered, shifting percussion.
    - Automate the routing of filters for dynamic patterning, even mid-pattern, for polyrhythmic timbral changes.

### 3. **Ring Modulator Magic**

- The on-board **ring modulator (RING Out)** can be fed oscillator A and B (X and Y IN) or *anything* in your rack:
    - Ring mod is classic for metallic, clangorous sounds (think hi-hats, cymbals).
    - Modulate one oscillator at audio or LFO rates, or try audio input plus LFO for moving/chaotic metallic percussion.
    - Even send rhythmic CV or clock bursts into one input for AM/rhythmic gating effects.

### 4. **Polyrhythmic/Complex Sequencing**

- **Not a sequencer itself, but the expander makes the Atlantix voice* far more patchable:**
    - Use external sequencers with per-step outputs controlling oscillator pitch, filter cutoff, VCA amplitude, or PWM for evolving, unpredictable percussion.
    - Self-patch outputs back into modulation inputs (example: Sub osc out to filter CV, or filter out to FM in) for chaotic, complex patterns that “play themselves.”
    - Patch envelopes or LFOs clocked/divided/multiplied by odd intervals for polyrhythmic modulations (e.g., trig env A at 4, env B at 7).
  
### 5. **Punchiness and Uniqueness**

- Use the **VCA drive circuit** in Atlantix for analog saturation on percussive hits—punchier kicks, claps, or snares.
- Modulate oscillator sync, filter resonance, or ring mod X/Y inputs with rhythmic pulses or random gates for “glitch” or “granular” percussion.
- Highly parameterize envelopes for snappy, clicky, or long decaying drum elements.
- Experiment with patching sub-oscillator, ring mod, or phazored outputs into effects or external resonators for more attack or “body.”

---

## Example Patch: Polyrhythmic Layered Drum Sequence

1. **Osc A Triangle** → VCA 1 (envelope from sequencer channel 1, 5/8 pattern) → Filter Lowpass out.
2. **Osc B Square** → VCA 2 (envelope from sequencer channel 2, 7/8 pattern) → Filter Bandpass out.
3. **Sub Square A** → VCA 3 (quick decay envelope, 3-step rotating clock) → Ring Mod Y input.
4. **Ring Mod Out** → additional VCA (snappy envelope; use this as "hi-hat" or clave).
5. **Mix filter outs** for composite percussion, multi-VCA mixing, or pan each to a different FX channel for maximum dynamism.

**Pro Tip:** Modulate oscillator pitch, filter cutoff, or PWM at audio rates from other rhythmic modules to create unpredictable, “broken” beats.

---

*The Atlx unlocks Atlantix for multi-layered, hybrid drum voices with tight, patchable integration. It excels with creative modulation, layering, and self-patching—invaluable for complex polyrhythmic music!*

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)