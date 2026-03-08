# Doepfer — A-138B

- [Manual PDF](../../manuals/A138_man.pdf)

---

[Manual PDF](#)

# Doepfer A-138 Mixer: using it for melodic patching

The attached manual is for the **Doepfer A-138 Mixer** only, so I can explain how **this module** contributes to creating melodic material in a Eurorack system, and how it works **with other melodic modules** like sequencers, quantizers, oscillators, envelopes, LFOs, and filters.

## What the A-138 does

The **A-138** is a **4-channel mixer** with:

- **4 inputs**, each with its own level control
- **1 master output level**
- two versions:
  - **A-138a**: **linear** pots, best for **control voltages (CV)**
  - **A-138b**: **logarithmic** pots, best for **audio**

It can mix:

- **audio signals**
- **control voltages**
- or a combination in utility contexts

There is also an **offset function on Input 1** on later versions:
- if nothing is plugged into input 1, knob 1 can generate:
  - **positive offset** (~0 to +5V), or
  - **negative offset** (~0 to -5V)
- this is set with an internal **JP4 jumper**

That offset feature is especially useful for melody building.

---

## Best role in melodic patching

The A-138 is **not itself a sound source or sequencer**, but it is very powerful as a **melodic utility**. It helps create melodies by letting you:

- combine multiple pitch-related CV sources
- add transposition offsets
- blend slow and fast modulation into pitch
- create variation in filter cutoff tied to melody
- mix several audio voices into one musical line or layered phrase

For melodic work, the most important version is usually:

## Use the **A-138a** for melodic CV

Because the **A-138a** has **linear potentiometers**, it is the better choice for:

- pitch CV mixing
- transposition
- combining sequencer + keyboard + modulation
- blending envelopes/LFOs/random with melodic control

The **A-138b** is better when mixing final audio from voices.

---

# How it can be used with other modules to create melodic components

## 1. Transposing a sequence

A classic melodic use is to mix:

- a **sequencer pitch CV**
- with a **keyboard CV**, **precision voltage**, or **offset**

### Patch idea
- Sequencer pitch CV → **A-138 input 2**
- Offset or keyboard CV → **A-138 input 1**
- A-138 output → **VCO 1V/oct input**
- Sequencer gate → envelope/VCA as normal

### Result
You can shift the whole melody up or down.

### Why this is musical
This gives you:

- key changes
- phrase transposition
- verse/chorus movement
- manual melodic variation during performance

### Extra tip
If your A-138 has the **offset jumper enabled**, and nothing is plugged into input 1, then **knob 1 becomes a transpose control**. That makes the mixer into a simple performance transposer.

---

## 2. Combining sequencer + vibrato + envelope pitch movement

You can layer several pitch influences into one melodic line.

### Patch idea
- Main pitch sequence CV → **input 1**
- Slow LFO → **input 2**
- Envelope → **input 3**
- Random stepped CV (lightly attenuated) → **input 4**
- A-138 output → **VCO pitch input**

### Result
The oscillator receives a sum of:

- the base melody
- subtle vibrato
- pitch envelope attack movement
- a little random instability

### Musical use
This is great for:

- expressive lead lines
- acid-style plucks
- animated basslines
- “humanized” melodies

### Important note
Pitch inputs are sensitive, so keep modulation amounts small unless you want large interval jumps.

---

## 3. Creating harmonic intervals from one melody source

If you have multiple oscillators, the A-138 can help build related melodic voices.

### Patch idea
- Sequence CV multed to:
  - VCO 1 directly
  - A-138 input 2
- Offset voltage into A-138 input 1
- A-138 output → VCO 2 pitch

### Result
- **VCO 1** plays the root melody
- **VCO 2** plays the same melody transposed by the offset

This creates:

- thirds
- fifths
- octaves
- drones against a moving melody

If your offset is manually set, you can perform harmonic movement live.

---

## 4. Mixing control voltages for filter melody-tracking

Melodic character is often not just pitch, but also how the **filter follows the note pattern**.

### Patch idea
- Keyboard/sequencer pitch CV → **input 1**
- Envelope CV → **input 2**
- LFO → **input 3**
- A-138 output → **VCF cutoff CV input**

### Result
The filter opens according to a blend of:

- note position
- envelope articulation
- slow movement

### Musical effect
This can make a melody feel:

- brighter on higher notes
- more expressive per note
- alive over time

This is especially useful for:

- basslines
- leads
- plucked melodic patches
- Berlin-school style sequences

The manual explicitly mentions mixing CVs for controlling something like a **VCF** from several sources.

---

## 5. Using the A-138b to layer melodic voices in audio

If you have multiple melodic voices, the **A-138b** is useful at the audio stage.

### Patch idea
- VCO/voice 1 audio → input 1
- VCO/voice 2 audio → input 2
- Sub oscillator or noise layer → input 3
- Another voice/delay return → input 4
- A-138 output → filter, VCA, or external mixer

### Result
You can create:

- layered lead sounds
- intervals and dyads
- thicker unison lines
- simple chord-like stacks

Because the A-138b uses **logarithmic pots**, it feels more natural for balancing audio levels.

---

## 6. Building a controlled melodic modulation bus

One of the most useful musical applications is treating the A-138 as a **CV mixer for one destination**.

For example, for a lead voice:

### Into the mixer
- sequencer row
- keyboard pressure / aftertouch
- LFO
- envelope

### Out to one destination
- oscillator pitch
- filter cutoff
- wavefolder depth
- FM amount

### Result
You get a single “melodic behavior” bus made from several influences.

This is powerful because melodies in modular are often not just notes, but **interactions between pitch, timbre, and articulation**.

---

## 7. Adding a manual phrase offset

If the jumper is set for the offset on input 1, and no cable is inserted there, knob 1 becomes a simple manual voltage source.

### Uses for melody
You can use this to:

- transpose a sequence
- shift filter cutoff for a new section
- move a melody into a different register
- bias an LFO or envelope mix before it hits pitch

This is one of the most performance-friendly uses of the A-138.

---

# Example melodic patch recipes

## Patch 1: Simple transposable melody

### Modules involved
- sequencer
- A-138a
- quantizer if needed
- VCO
- envelope
- VCA

### Patch
- Sequencer CV → A-138 input 2
- A-138 output → quantizer input
- Quantizer output → VCO 1V/oct
- Gate → envelope → VCA
- Audio voice → output
- Use input 1 offset knob as transpose

### Why it works
The quantizer keeps the mixed voltage musical, while the A-138 gives you manual transposition.

---

## Patch 2: Evolving lead

### Modules involved
- sequencer
- LFO
- envelope
- A-138a
- VCO
- VCF
- VCA

### Patch
- Sequencer pitch CV → A-138 input 1
- Slow LFO → A-138 input 2
- Envelope (small amount) → A-138 input 3
- A-138 output → VCO pitch

Optionally:
- Mult sequencer CV and envelope into another A-138 or other mixer for VCF cutoff

### Musical result
A lead that has:
- stable melody
- light movement
- per-note inflection

---

## Patch 3: Two-oscillator harmony line

### Modules involved
- sequencer
- A-138a
- two VCOs
- mixer/audio path

### Patch
- Sequencer CV multed:
  - directly to VCO 1
  - to A-138 input 2
- Offset into A-138 input 1
- A-138 output → VCO 2

### Musical result
- oscillator 1 = melody
- oscillator 2 = harmony above or below

Then mix both oscillators with:
- **A-138b** for audio, if available

---

## Patch 4: Melody-controlled timbre

### Modules involved
- sequencer
- A-138a
- envelope
- LFO
- filter

### Patch
- Sequencer CV → A-138 input 1
- Envelope → input 2
- LFO → input 3
- A-138 output → VCF CV input

### Result
The timbre follows the contour of the melody, helping even simple note patterns sound more musical.

---

# Practical advice

## For pitch CV, be careful
The A-138 is a general mixer, not necessarily a precision adder. That means:

- it is very useful for creative melodic CV mixing
- but for **exact interval transposition over many octaves**, a dedicated precision adder may be more accurate

Still, for many musical patches it works very well.

## A-138a vs A-138b
Choose based on task:

- **A-138a**
  - pitch CV
  - filter CV
  - envelope/LFO mixing
  - transposition duties

- **A-138b**
  - mixing oscillator audio
  - blending final melodic voices
  - audio submixing before external output

## The output attenuator is useful
Unlike many basic modular mixers, the A-138 has a **master output attenuator**, so it can:

- tame hot modular levels
- feed external gear more safely
- control overall level of a melodic submix

---

# Bottom line

The **Doepfer A-138** is best thought of as a **melodic utility hub**.

It helps create melodic components by allowing you to:

- mix pitch CV sources
- transpose sequences
- add expressive modulation to notes
- combine multiple melodic control signals
- shape filter movement tied to melody
- layer multiple audio voices into one musical part

If you have the **A-138a**, it is especially useful for **building and varying melodies** through CV combination. If you have the **A-138b**, it is excellent for **summing melodic audio voices** into a final line or layered part.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)