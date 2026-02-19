# Centreville — PlusMix

- [Manual PDF](../../manuals/PlusMix _ centrevillage.pdf)

---

[Download PlusMix Manual PDF](https://centrevillage.net/products/PlusMix.html)

---

# Creative Rhythmic Uses for PlusMix Utility Mixer Switch in Eurorack Percussion Patching

The **PlusMix** is a gate-controlled unity mixer, ideal for high-precision CV or audio mixing, and can be dynamically controlled via gates and polarity switches. Its architecture gives you powerful tools for sculpting percussive, polyrhythmic, or complex modular rhythmic music.

## Key Features Relevant to Rhythmic Complexity

- 3 audio/CV inputs (**PLS1, PLS2, BASE**), 1 mix output (**MIX**).
- 2 gate inputs (**SW1, SW2**) and 2 gate-polarity switches (**SW1PL, SW2PL**).
- **PLS1** and **PLS2** inputs are selectively mixed, per gate and polarity status.
- **BASE** always mixes through.
- Can be used as manual switch or gate-automated for rhythmically dynamic processes.
- DC Coupled — suitable for both audio and CV.

---

## Techniques for Complex Rhythmic and Percussive Music

### 1. **Dynamic Patterned CV Mixing for Polyrhythms**

Route multiple sequencer CVs (possibly from polyrhythmic sources, e.g., a 7-step and 5-step sequence) into **PLS1** and **PLS2**. Use gate/trigger patterns from your rhythm/clock modules (e.g., Euclidean sequencers, clock div/mults, logic processors) patched to **SW1** and **SW2**.  
**Result**: Only at specific beat coincidences do one or both patterns merge to the output. Complex, evolving melodics or modulation.

**Example Patch:**
- **PLS1:** 5-step modulation CV, clock-divided.
- **PLS2:** 7-step modulation CV.
- **SW1:** Main clock triggers.
- **SW2:** Swung/divided clock or logic OR from other percussive triggers.

This propagates polyrhythms to any CV destination (oscillator pitch for tuned percussion, filter cutoff, etc.).

---

### 2. **Percussive Audio Layer Gating**

Feed **PLS1/2** with audio-rate percussive sources (e.g., different digital noise bursts, metallic FM hits). Gates to **SW1/SW2** select which layer is present, with polarity switches (SW1PL/SW2PL) providing instant inversion/mute.

**Result**: Rapid, switchable layering of drum hits, claps, glitches—unique composite percussion sounds that change at intricate rhythmic intervals.

---

### 3. **Probabilistic/Conditional Percussion Hits**

Insert a logic or probability gate module before **SW1/SW2**. Now, percussion layers or modulation get mixed in only on rare, non-regular triggers, producing unpredictable fills and accents.

**Example**:  
- **Probability gate** on **SW2**.  
- Odd step triggers on **SW1**.
- Two contrasting percussion voices, switched as dictated by the gates.

---

### 4. **Morphing Manual Switch for Live Performance**

Use when unpatched (SW1 & SW2 normals engage), and flip polarity switches for instant, punch-in/out percussion changes; perfect for rimshot/hat/snare switching on stage.

---

### 5. **Precision Pitch CV Remixer for Drum Melodies**

Because PlusMix is high-precision, send pitch CVs to PLS1/PLS2/BASE and merge them rhythmically to oscillators tuned for percussive synth drums. This creates drumlines with evolving, rhythmically changing tunings—think Aphex Twin/IDM drum edits.

---

### 6. **Nested Syncopation with Clock-Linked Gates**

Feed in pulse trains from different clock-divisions (e.g., 3/16, 7/16, 13/16) to SW1/SW2, with percussion CV/audio routed accordingly. Utilize the gate polarity switches to invert or phase-offset layers, exploiting the normalization to create cross-rhythm accents as the clocks "breathe" together.

---

## Tips to Maximize Punch & Uniqueness

- Mix envelopes or accent CVs that open VCAs downstream, creating dynamic, talking percussion.
- Switch between different effects sends (distortion, delay, bitcrush) under gate control.
- Use BASE for the main pulse and gate-mix in noisy or metallic layers for "ghost" hits.
- Chain several PlusMix modules for even more combinatorial rhythmic complexity.

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**