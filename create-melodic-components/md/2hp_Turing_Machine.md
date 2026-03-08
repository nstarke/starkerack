# 2hp — Turing Machine

- [Manual PDF](../../manuals/TM_Manual.pdf)

---

[Manual PDF](#)

# Using the 2hp TM to Create Melodic Material

The attached manual is for the **2hp TM**, a compact probabilistic random sequencer/CV generator. On its own, it does not quantize pitch, clock itself, or generate gates for note articulation beyond responding to an incoming trigger. But as a melodic utility in a Eurorack system, it can be very effective when paired with a **clock/trigger source**, **quantizer**, **VCO/voice**, and optionally **sample & hold, slew, logic, or modulation**.

## What the module does

The **TM** outputs a **0–5V random control voltage** at its **OUT** jack whenever it receives a trigger or gate at **TRIG**.

Its key idea is that it does not behave like pure chaos all the time. Instead, it stores a sequence of step voltages and uses a **probability control** to decide whether each step changes or remains the same as the sequence advances.

### Core controls
- **TRIG input**
  - Advances/generates on incoming trigger or gate
  - Threshold: **2.5V**
- **PROB knob + PROB CV**
  - Far left = **100% probability** of generating a new random voltage for the active step
  - Far right = **0% probability**, effectively locking the existing sequence
- **STEPS knob + STEPS CV**
  - Sequence length from **1 to 32 steps**
- **AMP knob**
  - Scales output range from **0V to 5V**
- **OUT**
  - Random/stored sequence CV output, **0–5V**

## Musical interpretation

This is best thought of as a **Turing Machine-style looping random melody source**:
- At high probability settings, the melody changes constantly.
- At low probability settings, the melody becomes increasingly repeatable.
- At 0% probability, it acts like a locked sequence.
- Changing **STEPS** changes phrase length.
- Changing **AMP** changes melodic range before quantization.

That makes it very useful for:
- generative melodies
- evolving basslines
- semi-repeating motifs
- controlled random transposition
- modulation of melodic parameters

---

# How to patch it for melody

## 1. Basic generative melody patch

### Patch
- **Clock/trigger source** → **TM TRIG**
- **TM OUT** → **quantizer IN**
- **quantizer OUT** → **VCO 1V/oct**
- Same clock or a related gate pattern → **envelope/gate input**
- Envelope → **VCA**
- VCO → **filter/VCA/audio chain**

### What happens
Each trigger advances the TM. The output voltage is quantized into musical notes, giving you a melody.

### Suggested settings
- **PROB** around 9–12 o’clock for evolving repetition
- **STEPS** around 5–8 for short melodic phrases
- **AMP** around 10–1 o’clock to keep pitch movement in a usable range

### Why it works
The quantizer turns the TM’s raw random voltages into scale tones. The TM’s probability memory gives the result more structure than pure sample-and-hold randomness.

---

## 2. Locked looping melody

### Patch
Same as above.

### Settings
- First, turn **PROB** left so new values are written often.
- Let it run until you hear a phrase you like.
- Then turn **PROB** fully right to **lock the sequence**.

### Result
You now have a repeating melodic loop with up to **32 steps**.

### Performance trick
Momentarily bring PROB left to let a few notes mutate, then return right. This gives subtle phrase evolution without losing the identity of the melody.

---

## 3. Controlled random bassline

### Patch
- Trigger sequencer / clock divider → **TM TRIG**
- **TM OUT** → quantizer set to minor pentatonic / minor scale
- Quantizer out → bass VCO
- Gate pattern → envelope → VCA

### Settings
- **STEPS**: 4–8
- **AMP**: low to medium
- **PROB**: low, around 1–3 o’clock if you want mostly stable looping with occasional mutation

### Result
Because the output range is reduced with **AMP**, the quantizer sees a narrower CV span, which often creates tighter melodic contours suitable for basslines.

---

## 4. Melodic phrases with variable length

### Patch
- Clock → **TM TRIG**
- Slow LFO / random CV / sequencer row → **STEPS CV**
- **TM OUT** → quantizer → voice pitch

### Result
The phrase length changes over time, causing the melodic cycle to shift.

### Musical use
This is great for:
- non-repeating ambient melodies
- phase-like pattern changes
- evolving techno arps

### Tip
Subtle modulation of **STEPS CV** tends to be more musical than wild jumps.

---

## 5. Varying predictability over time

### Patch
- Clock → **TM TRIG**
- Slow LFO, envelope, or another random source → **PROB CV**
- **TM OUT** → quantizer → oscillator pitch

### Result
The melody moves between:
- highly unstable / novel
- semi-repetitive
- fully locked

### Musical use
This is one of the strongest features of the module. You can automate tension and release:
- verses: lower probability, more repeatability
- transitions: higher probability, more mutation
- breakdowns: fully random
- choruses: locked phrase

---

# Best companion modules for melodic use

Since TM is only one module, the "used together" part really means how it works alongside other common Eurorack categories.

## 1. Quantizer
This is the most important partner.

TM outputs **continuous random CV from 0–5V**, not discrete musical notes. A quantizer converts that into a scale.

### Good uses
- Major/minor tonal melodies
- Pentatonic ambient lines
- Modal sequences
- Arpeggio-like note sets

### Tip
If the quantizer supports transposition, feed a second CV source into transpose for harmonic movement while TM handles note selection.

---

## 2. Clock / trigger source
TM needs external timing.

### Good trigger sources
- steady clock for regular melodies
- Euclidean trigger generator for asymmetrical note timing
- gate sequencer for rhythmic melody placement
- clock divider/multiplier for slower or faster melodic movement

### Tip
Changing the trigger rhythm changes the perceived sequence as much as changing the pitch data.

---

## 3. Oscillator or complete synth voice
Once quantized, TM can drive:
- a sine or triangle oscillator for simple melodies
- a wavetable VCO for animated lead lines
- a complex oscillator for experimental phrases
- a full voice module for compact patches

---

## 4. Envelope + VCA
TM does not produce note gates for articulation by itself beyond reacting to incoming triggers. So you usually pair the same trigger source, or a related rhythm source, with an envelope/VCA path.

### Patch logic
- trigger source branches:
  - one copy to **TM TRIG**
  - one copy to **envelope gate**
- TM controls pitch
- envelope controls note articulation

---

## 5. Slew limiter / glide
Placing a slew after the quantizer or before the oscillator can create:
- portamento
- gliding random melodies
- smooth ambient pitch transitions

Very effective for generative melodic textures.

---

## 6. Sample & hold / switch / sequential switch
These can further structure TM’s output.

### Ideas
- Sample the TM less often than it is clocked
- Alternate between TM and another sequencer
- Use a switch to route TM to different voices
- Create call-and-response melodies

---

## 7. Precision adder / offset
Since TM outputs 0–5V, you may want to control register.

### Uses
- transpose the melody up/down
- constrain the note center
- combine TM with another sequencer row
- create harmonic movement over a static TM phrase

---

# Practical melodic patch examples

## Patch A: Ambient generative lead
- Slow clock → **TM TRIG**
- **TM OUT** → quantizer set to Dorian
- Quantizer → VCO pitch
- Same clock → envelope
- Envelope → LPG/VCA
- Slow triangle LFO → **PROB CV**
- Slow random CV → **STEPS CV**

### Outcome
A self-evolving melody with recurring fragments and shifting phrase lengths.

---

## Patch B: Techno riff generator
- 16th-note trigger pattern → **TM TRIG**
- **TM OUT** → quantizer in minor scale
- Quantizer → acid-style VCO pitch
- Trigger pattern → short envelope → VCA/filter env
- **PROB** low enough to preserve groove
- **STEPS** at 8 or 16

### Outcome
A stable but mutable riff generator. Great for live performance by nudging PROB.

---

## Patch C: Bass + lead derived from one source
- Clock → **TM TRIG**
- **TM OUT** multed to:
  - quantizer 1 → bass oscillator
  - quantizer 2 or shifted copy → lead oscillator
- Use different trigger divisions for each envelope

### Outcome
Correlated melodic layers from the same evolving sequence.

---

## Patch D: TM as melodic modulation, not primary pitch
Instead of controlling oscillator pitch directly:
- **TM OUT** → quantizer → oscillator FM amount CV
- or **TM OUT** → filter cutoff CV
- or **TM OUT** → wavefolder symmetry

### Outcome
You preserve a fixed melody elsewhere while TM adds pseudo-melodic internal motion.

---

# Strengths of the TM for melody

## 1. Repeatability without rigidity
It sits between random source and sequencer.

## 2. Excellent for live improvisation
One knob move on **PROB** can move the patch from chaos to motif.

## 3. Compact
At **2hp**, it gives a lot of melodic utility in very little space.

## 4. Good phrase control
**STEPS** from **1–32** lets it do anything from drones to long evolving patterns.

## 5. Range control via AMP
This is deceptively useful. Lowering amplitude before quantization can keep melodies focused and musical.

---

# Limitations to keep in mind

## 1. No built-in quantizer
You will usually want an external quantizer for tonal melodies.

## 2. No internal clock
Needs external triggers.

## 3. No explicit reset input
This means phrase alignment with other sequencers may be less exact than with a traditional sequencer.

## 4. Output is unipolar 0–5V
Depending on your oscillator and quantizer, this can span a wide register. You may want attenuation, offset, or transposition management.

---

# Best workflow for composing melodic parts

A strong musical workflow with TM is:

1. **Clock it**
2. **Quantize it**
3. **Set a musical scale**
4. **Adjust AMP** for range
5. **Set STEPS** for phrase length
6. **Set PROB** for stability vs mutation
7. **Lock** the sequence when you find a phrase you like
8. Modulate **PROB CV** and **STEPS CV** slowly for long-term evolution

This makes TM especially strong for:
- ambient
- Berlin-school style generative sequencing
- minimal techno
- experimental tonal patches
- evolving soundtrack textures

---

# Summary

The **2hp TM** is best used as a **probabilistic CV melody source**. It becomes a powerful melodic tool when combined with:
- a **trigger/clock source**
- a **quantizer**
- a **voice or oscillator**
- and optionally **CV modulation, slew, switching, or transposition**

Its musical sweet spot is generating phrases that feel **alive, semi-repeatable, and gradually mutating**, rather than fully programmed or fully random.

If you want, I can also turn this into:
1. a **patch recipe list**,
2. a **beginner-friendly explanation**,
3. or a **“best companion modules” table**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)