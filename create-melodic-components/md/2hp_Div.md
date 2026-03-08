# 2hp — Div

- [Manual PDF](../../manuals/Div_Manual.pdf)

---

[Manual PDF](#)

## Using the 2hp Div to Create Melodic Components

The **2hp Div** is a **dual clock divider/multiplier**. On its own, it does **not generate pitch CV**, quantized notes, or melodies directly. What it *does* do extremely well is create the **timing structure** that melodic material can ride on. In a Eurorack patch, that makes it a powerful **melody rhythm engine**.

Because both channels derive from the same input clock but can run at different multiplied/divided rates, Div is especially useful for:

- creating **independent rhythmic streams**
- generating **polyrhythmic note triggers**
- driving **sequencers, quantizers, sample-and-holds, and envelopes**
- making one melodic line feel related to another while still being rhythmically distinct

---

## What the module does

From the manual:

- **1 clock input**
- **2 independent outputs**
- Each output can be set to:
  - divide the clock by: **/16, /8, /7, /6, /5, /4, /3, /2**
  - pass the original clock
  - multiply by: **×2, ×3, ×4, ×5, ×6, ×7, ×8, ×16**
- Each channel has:
  - a **RATE knob**
  - a **RATE CV input** (0–5V)
  - an LED showing output activity

This means a single master pulse can become two related but different pulse streams.

---

## Best role in a melodic patch

Think of **Div** as the module that determines **when notes happen**, not **what notes happen**.

To create melody, pair Div with modules such as:

- **step sequencers**
- **quantizers**
- **sample & hold**
- **Turing machine / random CV source**
- **envelope generators**
- **logic modules**
- **switches**
- **sequential switches**
- **oscillators and VCAs**

---

## How it contributes to melody

### 1. Clocking a pitch sequencer at different rates
Patch:
- master clock → **Div IN**
- **OUT 1** → sequencer clock
- sequencer CV → quantizer → oscillator 1V/oct

Result:
- The RATE 1 setting determines how quickly the sequence advances.
- At slower divisions, you get sparse, deliberate melodic movement.
- At multiplications, the sequence becomes more active and ornamented.

This is one of the simplest ways to reshape a melody without changing its notes.

---

### 2. Creating two related melodic voices
Patch:
- master clock → **Div IN**
- **OUT 1** → sequencer A clock
- **OUT 2** → sequencer B clock
- sequencer A CV → oscillator A
- sequencer B CV → oscillator B

Result:
- Both voices are locked to the same source clock, so they feel connected.
- But because each output can have a different divide/multiply ratio, the two melodies unfold at different rhythmic densities.

Example:
- OUT 1 = **/2**
- OUT 2 = **×3**

This gives one slower, grounding phrase and one busy, animated counter-line.

---

### 3. Driving a sample & hold for generative melodies
Patch:
- random CV source → sample & hold input
- master clock → **Div IN**
- **OUT 1** → sample & hold trigger
- sample & hold output → quantizer → oscillator

Result:
- Div controls how often a new note is sampled.
- Change RATE 1 to make the melody update slowly or rapidly.
- CV over RATE 1 can make the melodic rhythm evolve over time.

This is especially effective for generative or ambient patches.

---

### 4. Creating melodic accents and variation
Patch:
- master clock → **Div IN**
- **OUT 1** → sequencer clock
- **OUT 2** → envelope trigger or VCA accent trigger

Result:
- One output advances notes.
- The other adds accents at a different rhythmic interval.

Example:
- OUT 1 = original clock
- OUT 2 = /4

Now every fourth note may be louder, brighter, or longer, which gives the melody phrasing and structure.

---

### 5. Using multiplication for ratchets and fast ornamentation
Clock multiplication is especially useful melodically.

Patch:
- main sequence clock → **Div IN**
- **OUT 1** = normal or slower sequencer advance
- **OUT 2** = multiplied trigger stream to envelope/VCA, burst input, or switch

Result:
- The melody can have fast repeated notes or subdivisions while the underlying harmonic movement remains slower.
- This creates:
  - ratchets
  - trills
  - repeated note fills
  - arpeggiated embellishments

Example:
- sequencer advances at **/2**
- envelope retriggers at **×4**

This can turn one step of pitch into a cluster of repeated articulated notes.

---

### 6. Dynamic melodic rhythm via CV control
Each channel has a **0–5V CV input** for rate control.

Patch:
- slow LFO / random stepped CV / sequencer row → **RATE 1 CV**
- master clock → **IN**
- **OUT 1** → melodic sequencer or sample & hold trigger

Result:
- The rhythm controlling your melody changes over time.
- This can create:
  - phrase expansion/contraction
  - unpredictable note density
  - evolving generative structures

Important musical effect:
- The *pitch source* can remain stable while the *rhythmic trigger pattern* becomes animated.

This often sounds more musical than randomizing pitch alone.

---

## Practical melodic patch ideas

## Patch 1: Slow melody + fast ornament voice
**Goal:** one main melodic line and one decorative high voice

Patch:
- master clock → Div IN
- OUT 1 set to **/2** → sequencer clock
- sequencer CV → quantizer → VCO 1
- OUT 2 set to **×4** → trigger input of envelope for VCO 2
- same pitch CV multed to VCO 2, or use a second sequencer

What happens:
- Voice 1 plays a measured melody
- Voice 2 plays rapid subdivisions, making the patch feel alive
- If VCO 2 is tuned an octave up, it becomes a nice melodic shimmer

---

## Patch 2: Polymetric counterpoint
**Goal:** two melodies that phase against each other

Patch:
- master clock → Div IN
- OUT 1 = **/5** → sequencer A
- OUT 2 = **/7** → sequencer B
- both sequencers → separate quantizers/oscillators or a shared scale

What happens:
- Because 5 and 7 cycle differently, the melodies interlock in a long repeating pattern
- Great for minimalist, generative, or Berlin-school style music

---

## Patch 3: Quantized random melody with evolving note density
**Goal:** controlled random melodic line

Patch:
- noise/random stepped CV → sample & hold input
- Div IN ← master clock
- OUT 1 → sample & hold trigger
- sample & hold output → quantizer → oscillator
- slow LFO → RATE 1 CV

What happens:
- New pitches are sampled at changing rhythmic intervals
- The melody remains tonal if quantized
- Very strong for ambient, experimental, and generative patches

---

## Patch 4: Phrase and accent separation
**Goal:** make a sequence feel musical and phrased

Patch:
- OUT 1 = original clock → sequencer clock
- OUT 2 = **/4** or **/8** → envelope controlling filter cutoff or VCA boost

What happens:
- The main melody proceeds steadily
- Every 4th or 8th trigger adds emphasis
- This creates bar-like structure from a simple repeating line

---

## Patch 5: Clocked switch for melodic rearrangement
If you have a sequential switch:

Patch:
- master clock → Div IN
- OUT 1 → main sequencer clock
- OUT 2 → sequential switch advance
- multiple pitch CV sources into switch
- switch output → quantizer → oscillator

What happens:
- One rhythm advances notes
- The other rhythm chooses which melodic source is active
- Very effective for creating evolving phrases from simple material

---

## Musical strengths of this module

### Tight related timing
Since both outputs come from one input clock, they stay musically related. This is ideal for layered melodic systems where you want complexity without total chaos.

### Easy creation of rhythmic contrast
The divide/multiply options let you move between:
- sparse notes
- normal pulse
- rapid subdivisions

That’s exactly the kind of contrast that makes melodies feel expressive.

### Excellent for generative patches
A lot of generative melody comes from combining:
- one pitch source
- one trigger source
- variation in timing

Div gives you that timing variation in a compact format.

---

## Limitations to keep in mind

Based on the manual, Div is **not**:

- a pitch sequencer
- a quantizer
- a melodic CV generator
- a logic module
- a probability trigger source
- a reset-based phrase manager

So by itself it won’t produce “notes.” It needs companion modules for that.

Its melodic usefulness comes from controlling the **rhythmic architecture** around note generation.

---

## Best pairings for melodic use

Div works especially well with:

- **quantizers** for tonal melodic output
- **sample & hold** for random note generation
- **sequencers** for defined melodic phrases
- **switches** for phrase variation
- **envelopes and VCAs** for articulation
- **logic** for more complex trigger combinations
- **LFOs/random CV** into RATE CV for evolving rhythms

---

## Summary

The **2hp Div** is best thought of as a **melodic timing processor**. It helps create melody by:

- clocking sequencers at different speeds
- triggering sample & hold for note generation
- creating counter-rhythmic melodic voices
- producing accents and phrasing
- generating fast subdivisions for ratchets and ornamentation
- modulating note density through RATE CV

If you combine it with even a basic sequencer or quantized random source, it becomes a very strong tool for building melodies that feel **alive, structured, and rhythmically rich**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)