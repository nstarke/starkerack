# 2hp — Comb

- [Manual PDF](../../manuals/Comb_Manual.pdf)

---

[**Download the Comb 2hp Manual (PDF)**](#)  
*(Replace "#" with actual manual link as needed.)*

---

# Creative Modulation Guide for the 2hp Comb Eurorack Module

The 2hp Comb is a powerful, compact IIR peaking comb filter. With its cutoff frequency, resonance (capable of self-oscillation), feedback dampening, and abundant CV control, it offers a vast palette for sound design. Below, I've highlighted strategies to harness those features for unique **distorted percussive sounds**, **aggressive basslines**, and **haunting pads**. Each approach focuses on creative use of the module’s parameters and CV inputs.

---

## Module CV Points & Controls

- **FREQ CV Input:** Controls cutoff/delay time (`±5V`)
- **RES CV Input:** Controls resonance/feedback (`±5V`)
- **DAMP CV Input:** Controls feedback path dampening (`±5V`)

---

## 1. Distorted Percussive Sounds

**Goal:** Create sharply attacked, metallic or shredded drum hits and glitch artifacts.

**Patch Ideas:**

- **Source:** Route clicks, short envelopes, or white noise bursts to **IN**.
- **FREQ Control:** Use a fast, snappy envelope or even trigger pulses via the **FREQ CV In** to sweep the cutoff at audio rate. This will cause intense, sometimes metallic transients—ideal for aggressive percussive timbres.
- **RES Control:** Crank the **RES** knob high (or modulate it with a steep envelope) so the comb filter teeters into self-oscillation when percussive signals hit. This adds harmonic clang (like hitting a metal plate).
- **DAMP:** Use a sharp envelope in **DAMP CV In** to briefly *open* the damp (fully clockwise) on attack, then *close* it (counterclockwise) to darken the decay. This creates “pingy” or splattering decay tails.
- **Add Feedback:** Turn up **RES** and use the **DAMP** control to push feedback into self-oscillation right as a percussive sound hits, then clamp it down to avoid runaway.

**Advanced:** Modulate all three parameters (Freq, Res, Damp) simultaneously with different envelopes or stepped random voltages to create evolving, unpredictable percussion.

---

## 2. Crazy Basslines (Dubstep/DnB Style)

**Goal:** Ridiculously resonant, growling, “torn” basses with moving peaks and synthetic character.

**Patch Ideas:**

- **Source:** Feed in a simple sub-oscillator (triangle, saw, or pulse) or dirty noise.
- **FREQ CV:** Use an LFO or sequencer track to modulate FREQ rapidly. Fast LFOs (audio-rate modulation) can create vowel-like, formant shifting growls.
- **RES:** Set high for squealing, overtone-rich peaks. Try modulating **RES** with a square or stepped random voltage to make the resonance jump or “chirp.”
- **DAMP:** Animate DAMP with an LFO or envelope inversely to resonance—e.g., when resonance goes up, damp opens, then vice versa. This keeps the sound moving and lively without overpowering feedback.
- **Self-Oscillation:** Push feedback to self-oscillation and modulate **FREQ** with envelopes or pitch CV. The result is a “re-triggered,” morphing resonator that can breathe and snarl—classic for neuro/DnB reese basses and dubstep growls.

**Tips:** For even more movement, mult a sequencer or random source to several CV inputs so all parameters move in complex, interrelated ways.

---

## 3. Haunting Atmospheric Pads

**Goal:** Ethereal, otherworldly washes with fluttering harmonics and evolving textures.

**Patch Ideas:**

- **Source:** Feed in sustained drones, chordal samples, or even slow granular textures.
- **FREQ:** Slowly modulate FREQ with a slow LFO or random smooth voltage (e.g., Turing Machine, Wogglebug). This adds subtly moving harmonic notches and peaks for evolving character.
- **RES:** Set to medium for gentle resonances. Use a secondary slow LFO to drift RES for swelling/receding harmonic emphasis—think of wind, breath, or shifting pitches in a cave.
- **DAMP:** Modulate DAMP gently around the mid-point with long, irregular envelopes or smooth random signals. The resulting brightness/darkness fluctuation brings morphing timbral shifts, akin to environmental motion.
- **Serial Processing:** Chain the Comb after a reverb or before a shimmer reverb to amplify the ghostly spatial effect.

**Performance Tip:** Use manual tweaking of all three knobs during a performance; slight, coordinated changes in FREQ, RES, and DAMP can lead a pad from serene to ominous to radiant with minimal patch changes.

---

## Final Notes

**General Tips:**
- Use audio-rate signals in CV inputs for wild FM-style effects.
- Combine with wavefolders, distortions, or bitcrushers for harsher sound design.
- Add subtle modulation for organic-sounding textures, or harsh stepped voltage for destruction.

**Summary:**  
The 2hp Comb excels as a timbre-warping creative tool. Its full CV control means you can sculpt audio far more dynamically than with fixed filters—use it for impact, movement, and atmosphere.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)