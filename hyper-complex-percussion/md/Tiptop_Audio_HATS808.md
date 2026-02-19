# Tiptop Audio — HATS808

- [Manual PDF](../../manuals/Tiptop_Audio_HATS808_ns.pdf)

---

[HATS808 Manual PDF](https://tiptopaudio.com/manuals/HATS808_manual.pdf)

---

# Using the Tiptop Audio HATS808 for Dense, Complex, and Hyper-Rhythmic Percussion in Eurorack

The Tiptop Audio HATS808 is a clone of the iconic TR-808 hi-hat voice, expanded for Eurorack with CV control and creative potential far beyond the original. If your aim is hyper-complex, densely layered percussive music—think extreme polyrhythms, polymeters, and intricate dynamic patterns—this module is a powerful building block.

Below, you’ll find advanced musical strategies and manipulation techniques to push the HATS808 deep into experimental rhythm realms:

---

## 1. Patch Foundations: Understanding the Voices

- **CH (Closed Hat) & OH (Open Hat)**: Both are available simultaneously. Use separate rhythmic triggers for maximum overlap and "choke" interplay.
- **Band-Pass OUT**: Feed this to additional filters, wave folders, or VCAs for radically new textures.
- **Resonance/Q Control**: Turn up for metallic, noisy, or even pitched tones. CV can radically animate the timbre.

---

## 2. Sequencing for Hyper-Complex Rhythms

- **Polyrhythms & Polymeters**:  
  - Connect distinct, unsynchronized gate sequencers to CH and OH, each running different step lengths (e.g., 7 against 5, or 13 against 16).
  - Patching two grids ensures the hats interact unpredictably, especially in how the choke circuit truncates OH decays.
- **Clock Skewing/Time Signature Tricks**:  
  - Sequence hats off odd divisions. Example: Clock CH with a /3 divider and OH with a /5 divider, both reset with different intervals.
  - Or, employ rotating or logic-based sequencers (Ornament & Crime, Euclidean modules, etc.) for evolving, skipping rhythms.

---

## 3. Sound Animation: Unique, Punchy Percussive Timbres

- **Dynamic Accent Control**:
  - Patch a fast LFO, stepped random, or complex envelope to the ACCENT IN. This means each hit varies in loudness and punch—far more dynamic than a static drum machine pattern.
  - Manual accent knob becomes a trim for fine-tuning groove feel.

- **Extreme Gain/Overdrive**:
  - Crank LEVEL and ACCENT for overloaded, harmonically rich hats.  
  - Take OUT into a wavefolder or analog distortion for industrial crunch.
  - Record both ‘hot’ and ‘soft’ takes; layer for thick, punchy hats.

---

## 4. Modulating Decay & Q for Textural Complexity

- **Animated Decay**:  
  - Patch stepped random CV or sequence to an external VCA that gates the input trigger, causing variable envelope lengths for a “live” drummer feel.
  - Use a slow LFO to modulate DEACY between short blips and washier hats.

- **Q/VC-Q for Morphing Sizzle**:
  - Sequence or randomize Q via the CV input (VC-Q) for each trigger. Fast modulation here generates metallic, comb-filtered, or “broken digital” hats.
  - Send audio-rate modulation (oscillator output) into VC-Q for wild FM crunch!

---

## 5. Advanced Choke Techniques

- **Creative Choke Interactions**:
  - Program CH hits to “interrupt” long OHs for intentionally glitchy, stuttery hat lines.
  - Disable choke with the PCB jumper for pure layered textures when needed.

---

## 6. Band-Pass Out as a Parallel Percussion Voice

- Send the Band-Pass OUT through another envelope/VCA/filter for a second, heavily processed “hat” to layer with the main CH/OH outs.
- Use this OUT as a percussive synth voice—mix back in for controlled chaos.

---

## 7. Feedback, Self-Patching, and Processing

- Mult the OUT or Band-Pass OUT back into your modular for feedback (through distorting preamps, filters, or LPGs).
- Use other percussion, radio noise, or field recordings as CV sources for VQ or Accent to add organic unpredictability.

---

### Extra Tips

- **Accent Trick**: Use stepped random triggers on the ACCENT input (rather than just gates)—some hats “pop” and some are soft, creating micro-grooves.
- **CV Animate Everything**: Modulate as many parameters as possible, ideally sequenced or with random sources.
- **Layering**: Stack several HATS808s (or one HATS808 plus digital hat voices) for hyper-complex hi-hat percussion beds.

---

*With creative clocking, accent modulation, aggressive filter resonance, and extreme gain/overdrive, the HATS808 can become a ferocious, living, and hyper-complex rhythm generator—perfect for pushing your Eurorack into new percussive territory.*

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)