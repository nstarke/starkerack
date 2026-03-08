# Centreville — PlusMix

- [Manual PDF](../../manuals/PlusMix _ centrevillage.pdf)

---

[Manual / Product Page PDF Source](https://centrevillage.net/products/PlusMix.html)

# centrevillage PlusMix — melodic use analysis

The attached manual describes **PlusMix**, a **2HP unity mixer with gate-controlled switching**.  
It is small, but very useful for building **melodic variation, transposition, phrase selection, and pitch recombination** in a Eurorack system.

## What the module does

### Inputs and outputs
- **Inputs**
  - `BASE`
  - `PLS1`
  - `PLS2`
  - `SW1` gate input
  - `SW2` gate input
- **Output**
  - `MIX`

### Core behavior
- `BASE` is **always present** at the output.
- `PLS1` is added to the mix only when its gate logic condition is true.
- `PLS2` is added to the mix only when its gate logic condition is true.

### Gate logic
Each switched layer has:
- a gate input (`SW1`, `SW2`)
- a polarity switch (`SW1PL`, `SW2PL`)

A `PLS` signal is mixed when:
- the corresponding gate is **HIGH** and the polarity switch is set to **H**, or
- the corresponding gate is **LOW** and the polarity switch is set to **L**

So each added signal can be made active on:
- gate high
- or gate low

### Normalization
- `SW1` is normalized to **+5V**
- `SW2` is normalized to **SW1**

This means:
- with nothing patched to `SW1` or `SW2`, the polarity switches act like **manual on/off selectors**
- with a gate patched only to `SW1`, both `PLS1` and `PLS2` can follow that gate unless `SW2` is separately patched

---

## Why this is musically important for melody

Because PlusMix is a **precision CV mixer**, it is especially useful for **pitch CV**.  
That means you can combine voltages representing notes, intervals, or transpositions without the slop that would make melodies go out of tune.

In practice, that makes PlusMix great for:

- **adding intervals to a base melody**
- **switching transpositions in and out**
- **creating A/B melodic variants**
- **building call-and-response phrases**
- **adding octave jumps conditionally**
- **making rhythmic melodic accents from gates**
- **recombining multiple pitch sources into one melodic line**

---

## Best melodic roles for PlusMix

## 1. Conditional transposition mixer
Use `BASE` for your main pitch sequence, and use `PLS1`/`PLS2` for interval offsets.

Example:
- `BASE` = main sequencer pitch
- `PLS1` = +1V octave transpose
- `PLS2` = +0.583V approximate perfect fifth if your source can generate exact interval CV
- `MIX` → oscillator 1V/oct

Then use gates into `SW1` and `SW2` to decide when those intervals are added.

Result:
- melody plays normally sometimes
- jumps up an octave on selected steps
- adds another interval on other steps
- can combine both for larger jumps

This is one of the most direct ways to create **melodic contour variation** from a static sequence.

---

## 2. Phrase variation from gate patterns
Feed the same melodic base into `BASE`, then patch offset voltages or alternate melodic fragments into `PLS1` and `PLS2`.

Example:
- `BASE` = 8-step sequence
- `PLS1` = small offset, like +2 semitones
- `PLS2` = another offset, like -3 semitones
- `SW1` = gate pattern from a trigger sequencer
- `SW2` = slower gate or clock division

Result:
- certain notes are pushed upward
- certain notes are pulled downward
- repeated patterns become evolving phrases

This creates **motivic development** without needing a second full sequencer.

---

## 3. Manual performance transposer
Because of the normalization, if no gates are patched:
- `SW1PL` and `SW2PL` become manual enable/disable switches for `PLS1` and `PLS2`

Example:
- `BASE` = running melody
- `PLS1` = +12 semitones
- `PLS2` = +7 semitones

Now the two switches become immediate performance controls:
- enable octave
- enable fifth
- enable both for a larger harmonic lift

This is excellent for:
- live arrangement
- moving between verse/chorus
- introducing fills
- changing melodic register on the fly

---

## 4. Gate-defined note accents
Use a rhythmic gate source to add pitch only on selected steps.

Example:
- `BASE` = root note sequence
- `PLS1` = +2 semitones
- `SW1` = snare-related trigger pattern or Euclidean rhythm

Result:
- the melody “leans” into accented notes only when the gate is present

This is useful for:
- syncopated hooks
- acid-style step accents
- dynamic lead lines with repeating structure

---

## 5. Recombining quantized pitch sources
PlusMix can combine several pre-shaped CV sources into one line.

Example:
- `BASE` = slow quantized melody
- `PLS1` = stepped random voltages scaled to chord tones
- `PLS2` = manual offset from a precision adder, keyboard, or fixed voltage source

Use gate inputs to bring these layers in and out.

Result:
- one coherent melodic output with controlled variation
- a hybrid between sequencing and performance patching

---

# How to use it with other modules to build melodic components

The manual only covers PlusMix, but in a normal Eurorack melodic patch it pairs especially well with the following module types:

## With a sequencer
Use the sequencer as the main pitch source.

Patch:
- sequencer pitch → `BASE`
- fixed voltage / second sequencer row / transpose CV → `PLS1`
- another offset or phrase row → `PLS2`
- sequencer gates / trigger track → `SW1`, `SW2`
- `MIX` → quantizer or directly to oscillator

Musical result:
- one sequence becomes multiple melodic variants
- you can derive several phrases from one pitch lane

If exact tuning matters, it is often best to:
- either feed quantized offsets into PlusMix
- or send `MIX` into a **quantizer** afterward

---

## With a quantizer
This is one of the strongest pairings.

Patch:
- melodic CV and interval offsets into `BASE/PLS1/PLS2`
- `MIX` → quantizer → oscillator

Why:
- PlusMix creates combinations of voltages
- the quantizer snaps the result to a scale

Musical result:
- controlled melodic branching
- gate-switched note changes that remain in key
- easy creation of arpeggio-like and modal patterns

This setup turns PlusMix into a kind of **melody decision matrix**.

---

## With clock dividers or logic modules
Since the `PLS` inputs are controlled by gates, any module producing related rhythms can drive melodic structure.

Patch:
- divided clock to `SW1`
- inverted or offset rhythm to `SW2`

Result:
- one transposition happens every 2 bars
- another happens every offbeat or every fourth note
- melody develops in longer cycles

This is very effective for:
- generative melodies
- evolving minimalism
- polyrhythmic transposition

---

## With sequential switches or gate sequencers
A gate sequencer can decide exactly which notes get altered.

Patch:
- gate sequencer channels → `SW1`, `SW2`
- offsets at `PLS1`, `PLS2`

Result:
- deterministic melodic editing on a per-step basis
- very efficient for creating:
  - passing tones
  - octave pickups
  - phrase-end lifts
  - recurring motifs

---

## With envelopes and VCAs in parallel
Use PlusMix for pitch variation while related gates also trigger articulation changes.

Example:
- `SW1` gate adds +12 semitones to pitch
- same gate also opens a brighter VCA/filter envelope

Result:
- when melody jumps, timbre also changes
- leads sound more intentional and expressive

That is a strong compositional trick: **pitch accents aligned with timbral accents**.

---

## With sample & hold or random voltage
Patch a stable melody into `BASE` and use random or semi-random voltages as occasional additions.

Patch:
- `BASE` = core melody
- `PLS1` = sample & hold voltage attenuated to a small interval range
- `SW1` = sparse random gate

Result:
- occasional melodic decorations
- controlled unpredictability
- very useful for ambient, IDM, and generative patches

For tonal music, a quantizer after `MIX` is especially recommended.

---

# Practical melodic patch ideas

## Patch 1: Two-level transposing lead
**Goal:** create a lead that changes shape over time.

Patch:
- sequencer pitch → `BASE`
- fixed +1V → `PLS1`
- fixed +0.167V or +0.333V style interval source → `PLS2`
- slower gate pattern → `SW1`
- faster accent gate → `SW2`
- `MIX` → quantizer → oscillator

What happens:
- the base melody is always present
- some notes jump an octave
- others are nudged into another interval
- some notes combine both offsets

Use:
- techno leads
- modular arpeggios
- melodic electro sequences

---

## Patch 2: Verse/chorus melody switcher
**Goal:** create structural change from one melodic line.

Patch:
- main melody CV → `BASE`
- chorus transpose amount → `PLS1`
- ending phrase lift → `PLS2`
- manual or arranged gate → `SW1`
- phrase-end gate → `SW2`

What happens:
- verse plays dry
- chorus activates a transposition layer
- phrase endings gain an extra lift

This works very well in live performance because the module is immediate and compact.

---

## Patch 3: Generative melodic mutation
**Goal:** one melody that evolves without losing identity.

Patch:
- quantized sequencer → `BASE`
- random stepped CV, attenuated → `PLS1`
- fixed interval → `PLS2`
- Euclidean rhythm → `SW1`
- clock divider → `SW2`
- `MIX` → quantizer → oscillator

What happens:
- most notes follow the original melody
- some are altered by random decoration
- some receive predictable structural transposition
- the line stays coherent but never static

---

## Patch 4: Manual harmonic lift for live sets
**Goal:** hands-on melodic arrangement.

Patch:
- sequence → `BASE`
- +7 semitone equivalent CV → `PLS1`
- +12 semitone CV → `PLS2`
- leave `SW1` and `SW2` unpatched
- use `SW1PL` and `SW2PL` manually

What happens:
- switch 1 adds harmonic lift
- switch 2 adds octave lift
- both together create a stronger section change

This is simple but highly playable.

---

# Strengths of the module for melody

## Very compact
At **2HP**, it adds melodic decision-making without eating valuable space.

## Good for pitch CV
The manual specifically notes **high-precision CV mixing**, which is critical for melodic use.

## Gate-controlled variation
Instead of just mixing everything all the time, you can make melodic additions happen only on chosen steps.

## Manual + patch programmable
It works both as:
- a hands-on performance tool
- and a fully patch-controlled melodic utility

---

# Limitations to keep in mind

## It is a unity mixer, not an attenuating mixer
The manual describes it as a **unity mixer**, so the incoming levels are summed as given.  
That means interval sizes must already be correct before entering `PLS1` or `PLS2`.

If you want exact semitone intervals, use:
- precision voltage sources
- quantized pitch rows
- precision offset generators
- or a quantizer after the mix

## Only two switchable add layers
You get:
- one always-on base
- two conditional additions

That is powerful, but still intentionally simple.

## No built-in quantization
For melodic tonal work, a quantizer after the output may be the best companion.

---

# Bottom line

**PlusMix is a small but extremely musical utility for pitch-CV composition.**  
Its best melodic use is to take a stable pitch line at `BASE` and then use `PLS1` and `PLS2` as **conditional interval or phrase additions**, controlled by gates.

Used with sequencers, quantizers, gate sequencers, logic, and fixed-voltage sources, it can create:

- transposed note accents
- alternate phrase shapes
- octave jumps
- evolving generative melodies
- manual arrangement changes
- precise pitch remixing

In a melodic Eurorack patch, think of it as a **gate-addressed pitch recombiner**:  
a way to turn one melody into several related melodies without losing coherence.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)