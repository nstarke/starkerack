# Xaoc Devices — Batumi

- [Manual PDF](../../manuals/xaoc_batumi2_poti2_manual.pdf)

---

[**Xaoc Devices Batumi II + Poti II Official Manual** (PDF)](https://xaocdevices.com/manuals/xaoc_batumi_ii_manual_ENG.pdf)  
*(Based on the images provided and referencing the official documentation)*

---

# Using Batumi II for Hyper-Complex Percussive & Rhythmic Eurorack Patches

Xaoc Devices **Batumi II** is an extremely powerful and flexible tool for generating and modulating complex rhythms and polyrhythms. While not a sound source on its own, its LFOs—capable of running into audio rates and tracking 1V/oct—make it an expansive modulation hub for percussion and rhythm-based eurorack systems. Adding the **Poti II** expander multiplies the creative possibilities.

Below are strategies to leverage Batumi II for intricate rhythmic and percussive music:

---

## 1. **Polyrhythmic Clock Generation**

- **Divide Mode:**  
  - Set channel A to your base clock (e.g., 120 BPM / 2 Hz).
  - Use channels B, C, and D in **divide mode** to output subdivisions like /3, /5, /8, etc (non-standard, polyrhythmic ratios).
  - Patch Batumi II’s **RECT outputs** into percussive voice trigger/gate inputs.  
- **Mult Mode:**  
  - Conversely, assign B, C, D to **multiply** A's rate, creating complex interlocked rhythms (e.g., channel A = quarter notes, B = eighths, C = dotted eighths).
- **Creative resets:**  
  - Periodically reset channels independently via external triggers for evolving, phase-shifting patterns.

---

## 2. **Complex Time Signatures & Pattern Evolution**

- **Phase Mode:**  
  - Lock all LFOs to A’s frequency.  
  - Use the PHASE sliders (and CVs for modulation) on B, C, D to set non-orthogonal phase angles (e.g., B at 90°, C at 150°, D at 270°). This causes outputs to trigger at mathematically interesting offsets within A’s cycle.
  - Use phase-modulated RECT or “asgn” (assignable) outputs to clock different drum modules or envelopes.
  - Add random or CV sequencing to phase sliders to mutate polyrhythms.
- **Random Waves:**  
  - Assign stepped or smooth random waveforms to one or more outputs. Use the resulting (sample & hold-esque) rhythms to trigger or modulate percussion for “non-repeating” beats.

---

## 3. **Creating Unique, Punchy & Percussive Modulations**

- **Audio-Rate LFOs:**  
  - Crank Batumi II into audio range and use its outputs as oscillators to feed drum voices’ pitch or timbral parameters for metallic or FM percussion.
- **Wave Morphing (with Poti II):**  
  - Use Poti II CV inputs to morph the assigned waveform (asgn) or to perform wavefolding on sine outputs (great for snappy, clangorous percussive CV).
  - Modulate the RECT output’s pulse width per channel for punchy, variable-width triggers—essential for dynamic “swingy” clocks or velocity-mapped gates.
- **Attenuation:**  
  - With Poti II, carefully attenuate outgoing CV to sculpt the intensity of envelopes, filter sweeps, or FM amounts for percussive voices.

---

## 4. **Advanced Techniques for Hyper-Complexity**

- **Stacking/Combining Outputs:**  
  - Mix or logic-OR multiple RECT outputs (via OR combiner/module) to generate unpredictable composite trigger streams—ideal for glitch/noise hi-hats or fills.
- **Tempo Sync & Tap Tempo:**  
  - In “Sync” mode, lock complex polyrhythms to an external clock, DAW, or modular sequence so that your hyper-rhythmic patterns always follow master tempo but mutate per your slider/CV settings.
- **Evolving Mutations:**
  - Use slow random or phase-shifted LFOs to modulate percussion processing parameters (e.g., VCA, filter, distortion, effects sends for each percussion module).

---

## 5. **Example Patch Ideas**

**Polyrhythmic Drum Sequencer:**
- Channel A RECT: Kick drum trigger (1:1)
- Channel B RECT (Divide by 3): Snare drum trigger (for a 4:3 polyrhythm)
- Channel C RECT (Divide by 5): Hi-hat or rimshot trigger
- Channel D stepped random: Percussion sample trigger for “aleatoric” sequence

**Evolving Percussive Groove:**
- Channel A: Master clock (triggers all others)
- Channels B, C: Phase mode, sliders modulated by slow LFOs/random
- RECT outputs to drum triggers
- SINE/ASGN outputs to modulate drum decay/filter envelopes

**Glitch Generator:**
- Stack all four RECT outputs into a logic OR (use a logic module)
- Use the combined “hyper-fast” clock for glitchy percussion or a stuttering effect

---

### **More Tips:**
- Combine Batumi II outputs with step sequencer gates for even more complex, humanized rhythms.
- Patch rectified (RECT) outputs into slew/lag processors for variable-length envelope triggers.
- Use Batumi II as a source of polyphonic cycling envelopes to modulate distortion or reverb parameters in sync with your percussion.

---

## **Batumi II is not a sound source, but a rhythm architect. Think of it as four modular “heartbeat brains” that can phase, multiply, divide, randomize, and pulse your system into unprecedented rhythmic territories.**

---

**Manual PDF:**  
[https://xaocdevices.com/manuals/xaoc_batumi_ii_manual_ENG.pdf](https://xaocdevices.com/manuals/xaoc_batumi_ii_manual_ENG.pdf)  
**More resources/tools:**  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)