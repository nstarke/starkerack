# 2hp — Turing Machine

- [Manual PDF](../../manuals/TM_Manual.pdf)

---

[2hp TM (Turing Machine) Manual PDF](https://2hp.com/manuals/tm.pdf)

---

## Using the 2hp TM for Complex, Hyper-Rhythmic Percussion Sequences

As a Eurorack musician, the 2hp TM ("Turing Machine") is a powerhouse for generating controlled randomness and evolving patterns ideal for constructing hyper-dense, ever-changing rhythmic and percussive sequences. Here’s how you can leverage its functions for polyrhythms, complex time signatures, and frenetic percussion:

### 1. **Patch as a Rhythmic Voltage Generator**
- **Trigger Patterns:**  
  Patch various clock or trigger sources with *different divisions/multiplications* into the **TRIG** input. This allows you to use standard clocks, polyrhythmic triggers (e.g. 5/7/11-step clocks), or Euclidean sequencers. Each trigger advances the sequence, making the output patterns non-repetitive and rhythmically rich.

### 2. **Introduce Polyrhythms**
- **Multiple TM Modules:**  
  Chain or parallel multiple TM modules, each clocked at different rates. Route their outputs to modulate drum module parameters or to pitch inputs on digital percussion voices. Layering different polyrhythmic streams creates extremely nuanced textures.
- **Varying STEPS Length:**  
  Modulate the **STEPS** CV input dynamically with LFOs or stepped random voltages to create evolving, shifting loop lengths—resulting in emergent, interlocking rhythms.

### 3. **Composing With Complex & Odd Time Signatures**
- Use the **STEPS** control to dial in odd sequence lengths (e.g., 3, 5, 13 steps, etc.).  
- Each trigger events loops over that length, meaning you can have multiple TM outputs running at unique lengths and polyrhythms, especially powerful for non-4/4 time feel.

### 4. **Deriving Percussive Voices**
While TM itself is not a sound source or effect, it is a *CV generator*. However:
- **Percussion Sound Modulation:**  
  Use TM’s **OUT** to modulate:
  - Percussive voice pitch (making metallic, "bouncing ball", melodic percussion)
  - Decay or timbre/meta-parameters on drum modules, for dynamic hits
  - Filter cutoff on effects for rhythmic sweeps
- **Amplitude Dynamic:**  
  Harness TM’s **AMP** control to scale the range of modulation impacting other modules—punchy, short bursts or full-scale, wild swings.
- **Quantization:**  
  Patch TM’s OUT through a quantizer for melodic or semi-melodic percussion. Use microtonal scales or odd intervals for gnarlier rhythms.

### 5. **Making Patterns Unique, Punchy, and Percussive**
- **PROB Control:**  
  Set **PROB** high for new values every trigger (chaos!) or low for repeating patterns.  
  Modulate PROB with CV to rhythmically alternate between evolving and locked-in patterns.
- **Dynamic Range:**  
  Use fast modulated **AMP** for sharp accents; patch an envelope/VCA after percussion voices, triggered in sync, to accentuate or gate TM’s effect.
- **Trig Conditions:**  
  Patch multed clocks, logic or switching modules, or burst generators for more erratic, reactive rhythmic changes.

### 6. **Creating Dense, Shifting Complexity**
- Use Sample & Hold modules with the TM’s output for even greater unpredictability.
- Run the same TM output to multiple destinations, each with different response curves.
- Cross-patch with other generative modules (e.g., use a TM to select trigger patterns for another sequencer, or modulate TM’s PROB/AMP with random sources driven by other rhythmic events).

---

By leveraging the TM’s probability-based output, dynamic step length, and variety of control voltage inputs, you can construct highly complex, polyrhythmic, generative rhythm sections that constantly evolve yet can also lock into grid-tight, precision patterns when needed.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)