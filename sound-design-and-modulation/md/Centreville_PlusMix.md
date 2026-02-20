# Centreville — PlusMix

- [Manual PDF](../../manuals/PlusMix _ centrevillage.pdf)

---

[PlusMix Manual (PDF)](https://centrevillage.net/products/PlusMix.html)

---

# Creative Modulation Ideas for PlusMix  
*(centrevillage PlusMix – Unity Mixer with Gate Controlled Switch)*

The **PlusMix** is a utility module that goes beyond standard mixing—its gate-controlled inputs and polarity switches allow for expressive dynamic modulation of your CV and audio paths. Below are creative ways to exploit these features to produce **distorted percussive sounds**, **complex dubstep/drum & bass basslines**, and **haunting pads**.

---

## Module Recap
- **Inputs:**  
  - `PLS1`, `PLS2`, `BASE` (audio or CV)
- **Outputs:**  
  - `MIX`
- **Gate Inputs:**  
  - `SW1`, `SW2`
- **Gate Polarity Switches:**  
  - `SW1PL`, `SW2PL`
- **Mix Logic:**  
  - `BASE` is always mixed.
  - `PLS1`/`PLS2` are mixed when their gate input + polarity status match ("H" + High or "L" + Low).

---

## **1. Distorted Percussive Sounds**

**Goal:** Use dynamic switching and fast gates to “punch in” signals and create rhythmic, choppy, or burst-driven percussive textures.  
**Approach:**  
- **Patch a noise source** or a short audio burst to `BASE` (always present).
- **Patch a high-gain drum oscillator** or complex waveform to `PLS1` and/or `PLS2`.
- Use a fast envelope (e.g., AD or AHR) or trigger sequencer to gate `SW1` and/or `SW2`.
- Set `SW1PL` and/or `SW2PL` to "H" for normal gate behavior (active on high), or "L" for inverted for more off-beat, glitchy gating.
- **Result:**  
  - Incoming drums or bursts are sharply mixed in for the length of the gates, producing clicks/cuts/rhythmic percussive hits layered atop your noise.
  - Add distortion (from another module) post-mix for extra saturation.

**Variation:**  
Randomize gate lengths with a random gate/trigger generator for unpredictable percussion.

---

## **2. Dubstep / DnB Bassline Madness**

**Goal:** Complex, switchable, morphing bass textures with sharp, modulated movement.  
**Approach:**  
- **Route two different bass synth voices** (e.g., filtered saw from one oscillator, FM bass from another) to `PLS1` and `PLS2`.
- **Patch a steady sub oscillator** to `BASE`.
- Use rhythmic or LFO-modulated gates (sync’d to your beat) into `SW1` and `SW2` to chop/flick between your morphing voices.
- **Manually flip** `SW1PL` or automate with a clock divider that provides high/low gate changes for extra syncopation or swing.
- Use complex LFOs or random stepped voltages to modulate gates for always-evolving bassline timbres.

**Advanced:**
- Insert audio-rate gates (from a noisy oscillator or burst generator) for glitchy, digital-grit effects.
- Run the output through a wavefolder or saturation module for extra edge.

---

## **3. Haunting Atmospheric Pads**

**Goal:** Slowly evolving, dark, layered textures using slow gating and polarity inversion for subtle, spectral blends.  
**Approach:**  
- **Send evolving drones or harmonically rich wavetable oscillators** to `PLS1` and `PLS2`.
- A steady pad base (filtered noise, choir sample, sine) to `BASE`.
- **Slow LFOs** (sine, triangle) or shift registers sequence gentle, long gates to `SW1` and `SW2`.
- Use `SW1PL` and `SW2PL` as manual “mix-in” switches for live performance blending.
- Try cross-fading LFO shapes (sometimes manually, sometimes routed from external modulation—e.g., a joystick or envelope follower).
- **Result:**  
  - Layers move in/out with smooth or ghostly abruptness. Inverted polarity means sometimes the pad will “hollow out” as other layers come in, creating cavernous, spectral spaces.
- Can be used on control voltages (CV) for pitch or filter modulation for moving harmonic “clouds.”

---

## **Additional Tips**

- **Precision mixing** means you can patch pitch CV through for creative multi-sequenced lines, switching between separate arpeggiators or sequencer patterns on the fly.
- The gate-normalization (SW1 to 5V, SW2 to SW1) means even with nothing patched, you have manual control—useful in live improvisation.

---

**For more module ideas, code, and tools:**  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)