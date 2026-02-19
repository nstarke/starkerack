# Black Noise — Cosmos

- [Manual PDF](../../manuals/BLACK-NOISE_COSMOS_User-Manual_V1.pdf)

---

[**COSMOS User Manual PDF**](https://blacknoisemodular.com/download/manual-cosmos.pdf)

---

# Using COSMOS for Hyper-Complex Percussion and Dense Rhythmic Eurorack Sequences

The **Black Noise COSMOS** is not just a utility or logic module—it's an interactive analog computer for your rack, capable of extreme rhythmic complexity and uniquely punchy, percussive sound sculpting. Here are concrete strategies to leverage its vast feature set to craft machine-like rhythms, dense polyrhythms, and intricate percussion textures:

---

## 1. **Complex Polyrhythmic Gate/Groove Creation**

#### **Randomized & Probabilistic Rhythms**
- **Random Gates Patch (Manual pg 35):**
  - Use a master clock or gate source as **X IN**.
  - Feed a random Sample & Hold output (sampled noise, etc.) into **Y IN** via an offset generator like GOMA.
  - Take XOR, AND, OR and their inverted counterparts for multiple rhythmic streams based on the random CV, producing controlled probabilistic beats.
  - Modulate the offset for shifting probabilities in real-time—making some rhythms appear/disappear or probability-controlled drum triggers.

#### **Rhythm Multiplication and Swing**
- **Clock Multiplier with Swing (pg 36) & Trigger Multiplier with Delay (pg 37):**
  - Use a steady pulse or trigger in **X IN**.
  - Mix the OR and NOR trigger outputs for double, swung clocks—great for tuplets, 3-against-2, or non-standard time signatures.
  - Patch the swing/delay control to a CV source; automate groove and shift accents for evolving rhythmic feel.

#### **Analog Logic as Sequence Modifiers**
- Use MIN/AND, MAX/OR, XOR, XNOR, and their inverted gates with clock-divided or shifted pulses to blend and mutate polyrhythms.
- Example: Combine two clocks at different rates (e.g., 5:4) and run them through COSMOS to extract all logic combinations. Patch these outputs to drum module triggers or envelopes for polymetric drum lines.

---

## 2. **Percussive Voice Processing & Unique Timbral Tricks**

#### **Clamping VCA & Ring Mod (pg 21-22)**
- **Punchy/Distorted Transients:**
  - Run drum or percussion sounds through COSMOS’ **inv. TZ CLIP** output for analog saturation and percussive wave-warping.
  - Modulate the “clamp amount” with fast-moving envelopes or stepped random, mimicking analog transient shaper or accent.

#### **Rhythmic Modifier (Gated/Chopped Audio)**
- **Use logical gates (AND, NOR, XOR, etc.) with rhythmic CVs or random gates to create cut-up, chopped, or stuttered effect on percussive loops or drum voices.**
- Modulate gate patterns at audio rates for glitchy textures.

#### **Real-Time Rhythmic Modulators**
- Use the touch pads for performative modulation—create fills or mutes by hand, contributing real-time interaction to dense, generative percussion.

---

## 3. **Advanced Pattern Generation & Processing**

#### **Window Comparator & Comparator Logic (pg 19-20)**
- Take polygonal LFOs or sequencer CVs into input X; set windows or thresholds using Y (possibly another LFO, random wave, or offset).
- Outputs give gated accents only within certain CV “windows”—perfect for emphasis or probabilistic accents within patterns.

#### **Envelope Combiner (pg 33)**
- Combine multiple envelopes for double/triple-sided drum hits (e.g., clap, snare flam) or shape otherwise binary rhythm into expressive, dynamic percussion.
- MIN and MAX outputs give you two contrasting percussive envelopes to route to VCAs or filters.

---

## 4. **Unusual Voices for Percussion—Kosmische Drums**

#### **Oscillator Self-Patched (pg 24)**
- Feed XNOR gate to X IN for an audio-rate square. Shape with envelopes or waveshapers for futuristic percussive tones.
- Use slew limiters, offsets, and VCA after for pitch sweep and decay (808-esque behavior).

#### **Wave Shaping: Shattering Kicks/Snares**
- Use full-wave/half-wave rectification, comparator with fast-moving CV, or harmonic wave shaper (pg 28) for highly unnatural, metallic, or thunderous percussive sounds.
- Patch audio to X, CV accents to Y, and extract multiple transformed outputs for parallel processing.

---

## 5. **Cross-Patch for Highly Modular Structures**

- Use feedback, self-patching, or send COSMOS outputs to further logic processors, clock-randomizers, or analog sequences for webs of intermodulated rhythmic logic.
- Couple complex COSMOS outputs to trigger sampler modules, percussion synths, or modulation destinations for morphing electro-mechanical grooves.

---

### **Tips for Extreme Percussion Use:**
- **Patch all outputs:** Even rarely used gates (NAND/XNOR, etc.) can result in surprising, off-grid emphasis.
- **Feedback:** Insert short delay, slew or distortion in feedback patching for unstable rhythmic flurries.
- **Overlay CV-Controlled Pattern Mutation:** Use CV control (GOMA, offsets) to swing, bias, or randomize logic dynamically throughout your set.

---

_The COSMOS is a playground for algorithmic, analog rhythm and percussion programming. Explore multi-level logic, self-patching, and interactive touch for rhythmic structures impossible with mere step sequencing._

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)