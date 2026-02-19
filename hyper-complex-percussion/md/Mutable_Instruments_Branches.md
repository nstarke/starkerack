# Mutable Instruments — Branches

- [Manual PDF](../../manuals/branches_quickstart.pdf)

---

[Branches Manual PDF](https://mutable-instruments.net/modules/branches/manual.pdf)

---

## Using Mutable Instruments Branches for Complex Percussion and Polyrhythms in Eurorack

The **Mutable Instruments Branches** is a dual Bernoulli gate—basically a probabilistic trigger router. It's not a voice or an effect, but a gate/trigger utility that introduces randomness or switching logic into rhythmic signal flows. This makes it an incredibly powerful tool for creating dynamic, densely-layered, and ever-evolving percussion or rhythmic sequences, perfect for polyrhythms, odd time signatures, and generative patterns.

Here’s how you can leverage Branches in the quest for **hyper-complex rhythmic results**:

---

### 1. **Generating Polyrhythms with Branches**

#### **Application:**
- **Feed two different rhythmic triggers** (for instance, from a clock divider and a sequencer) into the two INs of Branches (or just one IN, letting the internal normalized routing do the rest).
- **Use the Probability knob or CV input** to alter how incoming triggers are routed — one output could go on to fire a kick, the other a snare, for example.
- By **modulating probability with an LFO or stepped random voltage**, you can dynamically change the polyrhythmic structure over time.

#### **Result:**
- As triggers are probabilistically switched or split, you achieve unexpected but musical re-distribution of events, ideal for layering contrasting time signatures and evolving rhythmic interplay between percussion elements.

---

### 2. **Complex Time Signatures & Algorithmic Patterns**

#### **Application:**
- **Feed a simple clock or trigger train** (say, 16th notes).
- Use **toggle mode**: Now, Branches doesn’t just route the trigger at random, but can “flip-flop” between outputs based on probability. This can create complex, semi-algorithmic pulses and pseudo-random pattern lengths.
- Sequence the **Probability knob via CV** from a sequencer or a stepped random source to change patterning on a per-step basis, injecting controlled chaos into time signatures.

#### **Result:**
- Shifting between semi-deterministic and random pathing results in phasing, unexpected accents, or shifting downbeats—core ingredients for dense, jazzy, or IDM-like percussion.

---

### 3. **Hyper-Complex Percussion Patterns**

#### **Application:**
- **Daisy-chain both sections:** Connect OUT A of section 1 to IN of section 2 for nested coin-flips, creating cascading branching structures akin to probability trees.
- **Route each output to different percussion modules** or samplers (e.g., OUT A to a hi-hat, OUT B to a rimshot, and so on).
- **Use Latch mode:** A hit will keep an output high (+5V) until the next trigger swaps to the other output. This can be used to gate a complex percussion voice, holding it open for irregular durations—excellent for glitchy or stuttering fills.

#### **Result:**
- This introduces both micro-variation (which drum hits when) and macro-structure (which voices may temporarily dominate the pattern), maximizing rhythmic interest.

---

### 4. **Creative Modulation/Extensions**

- **Mult the output(s) of Branches** into effects, envelopes, or other modulators that shape percussion timbre (filter cutoff, wavefolder CV, etc.) for per-hit variance.
- **Patch Branches at the end of a clock division chain:** Use it to redirect triggers from heavily divided clocks to accent or “ghost” percussive elements, or to generate fills that aren’t on a fixed schedule.

---

### **Patch Inspiration Example**

```markdown
- Clock/funky sequencer → Branches IN 1
- Probability CV → Stepped random voltage or a slow LFO
- OUT A → Trigger input of main hi-hat
- OUT B → Trigger input of woodblock
- Branches IN 2 left unpatched (uses internal normalization)
- Use Toggle and Latch modes to evolve the pattern over time
- Mix OUTs through a VCA/waveshaper for extra randomness in texture
```

---

#### **TIP:**  
Pairing Branches with a voltage-addressed switch or sequential switch can further route its probabilistic triggers to *even more* voices, breaking out of “just two-way” patterning!

---

For full details and patch examples:  
[Branches Manual PDF](https://mutable-instruments.net/modules/branches/manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)