# 2hp — Euclid

- [Manual PDF](../../manuals/2hp_Euclid.pdf)

---

[Manual PDF](#)

# Using 2hp Euclid to Create Melodic Components

The attached manual is for the **2hp Euclid**, a **Euclidean trigger pattern generator**. By itself, Euclid does **not generate pitch CV** or audio, but it is extremely useful for creating **melodic structure** when paired with other Eurorack modules such as:

- sequencers
- quantizers
- sample & hold
- shift registers
- clock dividers
- switches
- envelopes
- oscillators
- sequential switches
- logic modules

## What Euclid Does

Euclid creates a rhythm by distributing a chosen number of active steps across a pattern length.

Core controls:

- **Trig Input**: advances the pattern one step
- **Reset Input**: resets the pattern to step 1
- **Length**: pattern length from 1–16 steps
- **Steps**: number of active hits distributed across the length
- **Offset**: rotates the pattern
- **Output**: sends a **+5V, 6ms trigger** on active steps

So musically, Euclid is best thought of as a **musical trigger mask** or **rhythmic phrase generator**.

---

# How Euclid Contributes to Melody

Since melody is usually a combination of:

- **pitch selection**
- **note timing**
- **phrase structure**
- **accent and repetition**

Euclid mainly helps with:

1. **when notes happen**
2. **which notes are allowed through**
3. **how a phrase repeats and rotates**
4. **creating asymmetry and cyclical melodic motion**

That makes it excellent for melodic work, even though it is not itself a pitch sequencer.

---

# Patch Ideas for Melodic Use

## 1. Triggering a Pitch Source Rhythmicly

### Patch
- Clock → **Euclid TRIG**
- Euclid **OUT** → envelope generator trigger input
- Pitch sequencer or quantized CV → oscillator 1V/oct
- Envelope → VCA → oscillator audio

### Result
Euclid determines **which steps produce notes**. Your pitch source can be a traditional sequencer, and Euclid adds a Euclidean rhythm on top.

### Why it works
A plain 8-step pitch sequence can sound much more musical when only selected notes are articulated.  
For example:

- Length = 8
- Steps = 3

This creates a sparse 3-note articulation pattern over your 8-note pitch loop, often resulting in phrases that feel more alive than straight 8ths.

---

## 2. Advancing a Sequencer Only on Euclidean Pulses

### Patch
- Master clock → Euclid TRIG
- Euclid OUT → clock/advance input of a pitch sequencer
- Sequencer CV out → quantizer or oscillator
- Euclid OUT or master clock → envelope trigger depending on desired behavior

### Result
Instead of every clock pulse advancing the melody, the sequencer only moves on Euclidean hits.

### Musical effect
This creates melodies with:
- irregular spacing
- repeated notes between advances
- cyclic phrase lengths

If the sound is gated every master step but the sequencer advances only on Euclidean triggers, the same pitch may repeat before moving on. This is great for **hook-like motifs**.

---

## 3. Sampling Random Voltage Into Melodic Notes

### Patch
- Random CV source → sample and hold input
- Euclid OUT → sample and hold trigger
- Sample and hold output → quantizer
- Quantizer → oscillator 1V/oct
- Euclid OUT → envelope trigger

### Result
Euclid determines when a new pitch is chosen.

### Why it is melodic
Because the random voltage is only sampled on Euclidean hits, the melody becomes rhythmically coherent instead of constantly changing. The quantizer turns it into usable notes.

### Tip
Use:
- **Length = 5, Steps = 2** for sparse motifs
- **Length = 8, Steps = 5** for denser melodic movement
- adjust **Offset** to shift where the phrase starts without changing the note pool

---

## 4. Euclid as a Gatekeeper for a Quantized Sequence

### Patch
- Sequencer CV → quantizer → oscillator
- Clock → sequencer clock input
- Same clock → Euclid TRIG
- Euclid OUT → VCA envelope trigger

### Result
The pitch sequence runs continuously, but only some notes are heard.

### Why this is useful
This is one of the easiest ways to turn a basic sequence into a more sophisticated melodic phrase.  
Euclid acts like a **compositional editor**, deciding which notes are spoken and which are implied.

This can create:
- syncopation
- recurring motifs
- phrase holes
- pseudo-polyrhythms

---

## 5. Using Offset as Melodic Phrase Rotation

The **Offset** control rotates the Euclidean pattern.

### Melodic use
If Euclid is triggering:
- envelopes,
- sample and hold,
- sequencer advances,
- or note changes,

then Offset changes **where the accents or note events fall** in relation to the pitch material.

### Example
Suppose your pitch sequencer loops through:
C - D - E - G - A - G - E - D

If Euclid is set to:
- Length = 8
- Steps = 3

Then changing Offset may articulate:
- C, G, E
or
- D, A, D
or
- E, G, C

So Offset becomes a very playable **phrase rotation tool**.

---

## 6. Creating Polymetric Melodies

Euclid supports pattern lengths from **1 to 16** steps.

### Patch idea
- Main pitch sequencer running 8 steps
- Euclid set to 5, 7, or 9 steps
- Euclid OUT triggers envelope or sequencer advance

### Result
Because the rhythmic cycle and pitch cycle are different lengths, the melodic phrasing shifts over time.

### Musical outcome
This is excellent for:
- generative melodies
- minimalist patterns
- evolving arpeggios
- IDM-style shifting phrases

For example:
- pitch sequence = 8 steps
- Euclid rhythm = 5 steps with 2 or 3 hits

The note emphasis will drift against the pitch loop, producing long non-repeating structures.

---

## 7. Driving a Sequential Switch for Melodic Variation

### Patch
- Several CV sources into a sequential switch:
  - sequencer row A
  - sequencer row B
  - random voltage
  - fixed interval voltage
- Euclid OUT → switch advance
- Switch output → quantizer → oscillator

### Result
Euclid controls when the melodic source changes.

### Why this is powerful
Now Euclid is not just timing notes, but structuring **which melodic generator is active**. This can create:
- phrase A / phrase B alternation
- fills
- motivic changes
- controlled randomness

---

## 8. Triggering Envelope Shapes for Melodic Expression

Melody is not only pitch. It is also articulation.

### Patch
- Euclid OUT → envelope trigger
- Envelope controls:
  - VCA amplitude
  - filter cutoff
  - wavefolder depth
  - FM index

### Result
Each Euclidean hit becomes a melodic articulation event.

### Use case
Even with a static pitch drone or slow CV movement, Euclid can create the perception of melody through repeated dynamic accents and timbral shaping.

This is especially effective with:
- low-pass gates
- plucky envelopes
- resonant filters
- per-step timbre modulation

---

## 9. Using CV Over Length and Steps for Evolving Melodies

Euclid has CV inputs for:

- **Length CV**: 0V to +5V
- **Steps CV**: 0V to +5V

The incoming CV is added to the knob position.

### Melodic application
If you patch slow modulation into these inputs:
- LFO
- random stepped voltage
- another sequencer row
- pressure or joystick CV

the melodic rhythm will evolve over time.

### Example
- Slow triangle LFO → Steps CV
- Length manually set to 8
- Steps moving between 2 and 6

This causes the density of note events to breathe over time, making melodies feel less loop-bound.

### Important musical effect
As note density changes, the same pitch source can feel like:
- sparse motif
- arpeggio
- burst
- ostinato

---

## 10. Using Reset for Predictable Phrase Starts

The **Reset input** forces the pattern back to its first step.

### Why this matters for melody
If you want melodic phrases to align with bar lines or section changes, send a reset pulse every:
- 4 bars
- 8 beats
- phrase boundary
- transport start

### Benefit
Without reset, long Euclidean interactions can drift freely. That is great for generative music, but reset gives you:
- repeatable hooks
- song-form alignment
- stable downbeats

A useful compromise is to let Euclid drift for a while, then periodically reset it for structural clarity.

---

# Best Melodic Pairings for Euclid

## Euclid + Quantizer
A classic pairing for making random or semi-random CV melodic.

Euclid decides:
- when a new note happens

Quantizer decides:
- what scale note it becomes

---

## Euclid + Pitch Sequencer
Excellent for phrase masking, syncopation, and note selection.

Euclid decides:
- which sequencer notes are articulated
- when the sequencer advances

---

## Euclid + Sample & Hold
Great for generative melody.

Euclid decides:
- when a voltage is captured
- how often pitch changes

---

## Euclid + Sequential Switch
Great for melodic arrangement and variation.

Euclid decides:
- when to move between phrase sources

---

## Euclid + Logic / Clock Divider
Useful for more advanced melodic rhythms.

You can combine Euclid with:
- AND logic for note coincidence
- OR logic for denser note generation
- XOR logic for unexpected phrase shapes
- divided clocks for slower melodic layers

---

# Practical Melodic Patch Recipes

## Recipe 1: Euclidean Arpeggio
- Clock → Euclid TRIG
- Euclid OUT → arpeggiator advance or sequencer advance
- Arp/sequencer CV → quantizer → oscillator
- Euclid OUT → envelope

Try:
- Length = 8
- Steps = 5
- Offset adjusted by hand during performance

This gives a flowing but asymmetrical arpeggio.

---

## Recipe 2: Generative Lead Line
- Noise/random source → sample & hold input
- Euclid OUT → sample & hold trigger
- Sample & hold → quantizer in minor scale
- Quantizer out → oscillator 1V/oct
- Euclid OUT → envelope → VCA

Try:
- Length = 7
- Steps = 3

This produces a sparse, musical lead line with repeating cyclic logic.

---

## Recipe 3: Syncopated Bassline
- 8-step sequencer CV → oscillator
- Main clock → sequencer
- Same clock → Euclid TRIG
- Euclid OUT → VCA envelope trigger

Try:
- Length = 8
- Steps = 3 or 5

The bass pitches stay familiar, but Euclid creates syncopation and groove.

---

## Recipe 4: Rotating Motif
- Pitch sequencer running a fixed melody
- Euclid OUT → envelope trigger
- Manually turn **Offset** during playback

This creates phrase rotation without changing pitch order.

A very performance-friendly technique.

---

## Recipe 5: Evolving Melodic Density
- Slow CV source → Steps CV
- Another slow CV source or manual setting → Length CV
- Euclid OUT → sample and hold trigger and envelope trigger

This makes a melody generator that gradually changes how busy it is.

---

# Performance Suggestions

## Use Offset as your main live control
Offset is especially musical because it preserves the core pattern but shifts emphasis. It is ideal for:
- fills
- transitions
- melodic call-and-response
- variation without chaos

## Modulate Steps for tension
Lower Steps:
- sparse
- minimal
- more space

Higher Steps:
- active
- urgent
- more notes

## Change Length for phrase feel
Short lengths:
- repetitive
- hook-like
- dance-friendly

Longer lengths:
- evolving
- less predictable
- generative

## Reset on section changes
Use reset when moving from verse to chorus or when bringing in a new harmonic sequence.

---

# Limitations to Keep in Mind

Based on the manual:

- Euclid outputs **triggers only**, not gates of variable length
- Output trigger is **+5V, 6ms pulse**
- It does **not produce pitch CV**
- It does **not store note values**
- It does **not quantize**

So for melody, it must be paired with other modules that generate or process pitch.

---

# Summary

The **2hp Euclid** is not a melodic source by itself, but it is a very effective **melodic rhythm engine**. It helps create melody by controlling:

- when notes happen
- when pitch changes happen
- how phrases rotate
- how rhythmic density evolves
- how melodic cycles interact with pitch cycles

It works especially well with:

- pitch sequencers
- quantizers
- sample & hold
- random voltage
- switches
- envelopes

If you want melodies that feel:
- cyclical
- organic
- syncopated
- generative
- minimalist
- polymetric

then Euclid is an excellent utility for building them.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)