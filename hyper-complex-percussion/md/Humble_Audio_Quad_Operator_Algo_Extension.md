# Humble Audio — Quad Operator Algo Extension

- [Manual PDF](../../manuals/Quad Operator Manual.pdf)

---

[Quad Operator Manual PDF](https://www.dropbox.com/paper/doc/print/JsIQoU7GbeAboEJku9ZgE?print=true)

# Using the Humble Audio Quad Operator for Dense Rhythmic / Hyper-Complex Percussion

The Quad Operator is not a drum module in the traditional sense, but it is *very* well-suited to building intricate percussion systems because it gives you:

- 4 operators with independent outputs
- lock/free behavior per operator
- audio-rate FM and self-FM
- variable waveshapes
- reset input for phase re-triggering
- LFO mode for complex modulation generation
- gain CV per operator, which acts like a per-operator VCA for both output and modulation depth
- an FM routing matrix
- optional Algo expander for storing and morphing modulation networks

That means you can treat it as:

- a **4-voice percussion oscillator bank**
- a **complex modulator source**
- a **cross-modulating drum core**
- a **rhythmic FM network** whose timbre changes per hit, per bar, or per phrase

## The key idea

For dense, polyrhythmic percussion, think of each operator as one of these:

- kick body
- metallic hit / bell partial
- snare tone
- tom
- click/transient source
- modulation-only operator
- sub-audio rhythm modulator in LFO mode
- external audio-rate mod source return via AR FM

The trick is to combine:

1. **independent trigger/gate-derived gain CV animation**
2. **different operator tunings or ratios**
3. **selective FM routing via the modulation matrix**
4. **phase resetting**
5. **lock vs free states**
6. **algorithm changes with the Algo expander**

This is how you get percussion that feels structured but still unstable and alive.

---

# What matters most from the manual for percussion

## 1. Independent outputs per operator

This is huge. You do **not** need to mix everything internally as one FM voice. Instead:

- patch **Op 1–4** to separate VCAs, LPGs, filters, wavefolders, or envelope-controlled channels
- sequence each output independently
- create layered percussion where one operator is the body, one is the snap, one is metallic noise, one is ghost motion

This is the easiest route to dense drum programming.

---

## 2. Gain CV acts like a built-in VCA and modulation animator

From the manual:

> Gain CV affects both output level and how intensely the operator modulates other operators via its modulation sends.

This is probably the most important performance/composition feature for percussion.

That means if you send a trigger-derived envelope to an operator’s **Gain CV**:

- the operator becomes audible only during the hit
- its FM influence on other operators also appears only during the hit

So each percussion event can dynamically reshape the rest of the network.

In practice:

- a hit on Operator 3 can briefly become audible
- *and* during that same instant it can also modulate Operators 1, 2, and 4
- this creates transient-dependent timbre shifts and interlocking drum behaviors

This is where “hyper complex” starts happening.

---

## 3. Lock vs Free state

## Lock state
Use for:

- harmonic percussion
- tuned toms
- resonant kick bodies
- classic FM clangs that remain musically related

Ratios are integer relationships to master pitch. This helps preserve coherence.

## Free state
Use for:

- noisy metallic percussion
- inharmonic hats
- unstable sidebands
- dissonant clicks
- unrelated per-operator pitches

In free state, each operator behaves as an independent oscillator, and the Ratio control becomes coarse tuning with 1V/oct via Ratio CV.

For complicated percussion systems, a strong strategy is:

- keep one or two operators in **lock** for the “pitched skeleton”
- set one or two operators to **free** for “chaotic metal/noise/transient layers”

This gives you rhythmic complexity without total sonic collapse.

---

## 4. Reset CV

The manual notes Reset resets all operator phase.

This is incredibly useful for percussion because phase reset creates repeatable attacks. If you drive Reset from your rhythmic system:

- every trigger can create a more consistent transient
- or every larger phrase can realign the whole FM network
- or irregular resets can create structured instability

Good uses:

- send your master downbeat trigger to **Reset**
- send a phrase reset every 5, 7, or 9 steps
- use a logic-derived reset from combined clocks to periodically re-synchronize complex modulations

That gives polyrhythmic movement that still “lands” on key beats.

---

## 5. LFO mode

The whole module can run in LFO mode, creating phase-locked complex modulation signals.

This makes the Quad Operator usable as a **rhythmic modulation engine**, not just a sound source.

You can use LFO mode to generate:

- interlocked CVs for external VCAs
- evolving modulation for drum filters
- rhythmic shape animation
- periodic but complex control voltages

One especially strong workflow is to alternate between:

- **VCO mode** for audio percussion voices
- **LFO mode** for generating synchronized modulation phrases that animate other drum modules

If you have a second voice for actual sound generation, Quad Operator in LFO mode can become the “rhythm brain.”

---

# Best patching concepts for complicated percussion

# 1. Four-lane polyrhythmic percussion voice

Use each operator as a separate percussion lane.

Suggested setup:

- **Op 1**: low sine/triangle in lock state = kick/tom body
- **Op 2**: higher ratio, light FM = snare tone or woodblock
- **Op 3**: free state, square/saw, high tuning = hats/clicks
- **Op 4**: free or locked high ratio with self-FM = metallic accent layer

Patch each output through its own VCA or LPG.
Use different trigger streams/envelopes for each Gain CV or downstream VCA.

Example rhythmic divisions:

- Op 1 on 5-step cycle
- Op 2 on 7-step cycle
- Op 3 on 11-step cycle
- Op 4 on 13-step cycle

This immediately creates a dense rotating percussion grid.

### Why it works
Even before FM interaction, the independent outputs and different rhythmic lengths produce polymeter. Once cross-modulation is added, each hit also changes the others.

---

# 2. “Transient modulator” patch

Use one operator mostly as a modulator rather than a voice.

Example:

- **Op 1** = audible kick/tom core
- **Op 2** = audible snare/clang
- **Op 3** = mostly silent transient modulator
- **Op 4** = metallic/noise accent

Set:

- Op 3 gain low or externally muted
- Turn up Op 3’s modulation sends to Op 1, 2, and 4
- Trigger Op 3’s Gain CV with a dense Euclidean rhythm

Now Op 3 only “exists” on certain hits, and when it does, it sharply distorts the other operators’ spectra. This creates:

- ratcheted accents
- pseudo-flams
- timbral ghost notes
- unstable transient bursts

This is excellent for advanced percussion lines.

---

# 3. Self-FM percussion for metallic hits

The matrix allows an operator to modulate itself.

For hats, zaps, metallic pings, and digital hand percussion:

- use a higher ratio or free-tuned operator
- set wave shape toward square or saw
- add moderate self-modulation
- use short envelope bursts into Gain CV
- optionally reset phase per trigger

This produces sharp, shifting percussive spectra.

For more control:

- keep the operator in lock if you want repeatable harmonic clang
- switch to free if you want brittle inharmonic metal

---

# 4. Feedback-style AR FM patch

The manual specifically mentions using the **AR FM** input for feedback patches with lock mode operators.

Try:

- patch an operator output, or a processed copy of one, into **AR FM**
- use the **AR FM Gain** and **Mod 1–4** sends to distribute that external audio-rate modulation
- animate AR FM Gain CV with rhythm

This creates a fifth modulation source that can be:

- burst on selected accents
- routed unequally to all four operators
- used to inject external drum layers or noise

Very strong sources for AR FM:

- filtered noise
- a wavefolder output
- a distorted copy of one Quad Operator voice
- another oscillator
- a resonant pinged filter
- a cymbal/noise module

This is one of the best ways to push the module into aggressive percussion territory.

---

# 5. Phrase-level FM algorithm switching with the Algo expander

The Algo expander stores modulation send knob positions and crossfades between them.

For percussion, this means you can treat saved algorithms like **drum scene states**.

For example:

- **Algo A** = sparse, mostly clean tones
- **Algo B** = dense cross-modulation and self-FM
- **Algo C** = metallic chaos / feedback-heavy routing
- **Live** = improvised state

Use this musically:

- A for verse
- B for chorus
- C for fills or breakdown transitions
- crossfade between A and B over 8 or 16 bars
- punch to C on every 4th phrase for a fill

This is one of the most powerful composition tools on the module because rhythm is not just timing; it’s also *density over time*.

---

# How to approach polyrhythms and complex time signatures

## A. Separate trigger lengths per operator

The most straightforward method:

- Operator 1 envelope every 4 steps
- Operator 2 envelope every 5 steps
- Operator 3 envelope every 7 steps
- Operator 4 envelope every 9 or 11 steps

Keep one common clock but use different sequencer lengths or clock divisions/multiplications.

Because operators can also modulate each other, the resulting pattern is not just layered—it is *interdependent*.

---

## B. Different reset cycles

Send **Reset** not on every hit, but on a larger structural rhythm, such as:

- every 16 steps
- every 15 steps against a 16-step bar
- every 3 bars
- from a logic condition, e.g. only when two clocks coincide

This creates repeating but long-form phase structures.

For instance:

- drums trigger on 5, 7, 11, 13 step cycles
- module reset every 16 pulses
- algorithm crossfade every 32 pulses

Now the patch has multiple temporal scales.

---

## C. Use lock state as the meter anchor, free state as the disruption layer

A nice musical arrangement is:

- Op 1 and Op 2 locked, tuned musically
- Op 3 and Op 4 free, less stable, higher or lower frequencies

Then sequence:

- Op 1 and 2 on regular or semi-regular pulse structures
- Op 3 and 4 on prime-length rhythms or burst generators

This gives the listener something to hold onto while still hearing extreme rhythmic complexity.

---

## D. Trigger gain CV instead of muting outputs only

Because Gain CV changes both loudness and FM contribution, triggering Gain CV creates more interesting rhythmic interaction than simply opening a final VCA.

That means:
- a hit is not just “sound on”
- it is “sound on + modulation topology changed”

This is ideal for intricate drum systems.

---

# Practical patch recipes

# Patch 1: Polyrhythmic FM Drum Quartet

## Goal
Four interlocking percussion lanes with evolving timbre.

## Setup
- VCO mode
- Op 1: lock, low ratio, sine
- Op 2: lock, medium ratio, sine/triangle
- Op 3: free, high tuning, square-ish
- Op 4: free, very high or mid-high tuning, saw-ish

## Matrix
- Op 2 -> Op 1 a little
- Op 3 -> Op 2 medium
- Op 4 -> Op 3 a little
- Op 4 self-FM medium
- minimal or no modulation to Op 1 at first

## Rhythms
- Gain CV 1: 4-step kick rhythm
- Gain CV 2: 5-step rhythm
- Gain CV 3: 7-step rhythm
- Gain CV 4: 11-step sparse accents

## Extras
- Reset every 16 or 20 master pulses
- slowly modulate shape CV on Op 3 and 4
- use external VCAs for final articulation if needed

## Result
A rotating constellation of kick/tom/hat/metal sounds with repeating long-cycle interactions.

---

# Patch 2: Complex snare and hat generator

## Goal
One operator as snare body, one as noisy overtone source, one as click, one as metallic wash.

## Setup
- Op 1: lock, ratio near 1, sine/triangle = drum body
- Op 2: lock, higher ratio = overtone snap
- Op 3: free, high pitch, square = click
- Op 4: free, self-FM, saw = metallic/noise element

## Matrix
- Op 2 -> Op 1 moderate
- Op 3 -> Op 1 small
- Op 4 -> Op 1 and Op 2 moderate
- Op 4 self-FM moderate/high

## Rhythm
- Op 1 gain envelope on backbeats or displaced accents
- Op 3 tiny short envelopes on denser pulse train
- Op 4 irregular Euclidean rhythm
- occasionally reset phase on major beats

## Result
Snare-like events whose transient structure differs every time depending on which auxiliary operators fire.

---

# Patch 3: Phase-locked pseudo-ratchets

## Goal
Create extremely fast-feeling internal subdivisions without needing explicit ratchet programming.

## Setup
- Use short envelopes into Gain CV
- Patch Reset with a dense but selective trigger stream
- Use one high-frequency operator to modulate a lower one only on some hits

## Method
- Op 3 in free state at high frequency
- Op 3 -> Op 1 strong
- Envelope Op 3 Gain CV with bursts
- Trigger Reset on the first pulse of each burst group

## Result
The attack of Op 1 changes in a way that reads like ratcheting, buzzing subdivisions, or clustered strikes.

---

# Patch 4: AR FM as external percussion injector

## Goal
Inject another rhythmic layer into the Quad Operator network.

## Setup
- Patch a noise source, cymbal voice, or another oscillator into AR FM
- Adjust AR FM gain to avoid clipping
- Use AR FM Mod 1–4 to send different amounts to each operator
- Sequence Gain AR FM with a different rhythm than the operators

## Rhythm ideas
- AR FM active every 3 beats in 4/4
- or on a 9-step Euclidean pattern against a 16-step drum phrase
- or only in fills

## Result
The entire percussion network blooms into harsher, more complex spectra only on selected accents.

---

# Patch 5: Algorithm morphing for fills and sectional form

## Goal
Use the Algo expander as rhythmic arrangement control.

## Save states
- **A**: low modulation, punchy, clear
- **B**: medium inter-operator FM, more snares/toms
- **C**: high self-FM and cross-mod, metallic chaos

## Performance method
- Crossfade A -> B over a long phrase
- Snap to C for fill
- Return to A or Live
- Double-tap Live if you want the panel to take over again

## Result
Your pattern complexity evolves at the network level, not just through note programming.

---

# Strategies for unusual meters

If you want 7/8, 11/8, 13/16, or layered metric structures:

## Use one operator as the “meter narrator”
For example:
- Op 1 marks the main pulse or downbeat relationship
- keep it relatively stable, low modulation, lock state

## Use others as cycle offsets
For example in 7/8:
- Op 2 accents every 3
- Op 3 accents every 4
- Op 4 runs a 5-step cycle against the bar

Or in 11:
- Op 1 follows 3+3+3+2
- Op 2 follows 4+4+3
- Op 3 follows 5+6
- Op 4 follows an independent 7-cycle over two bars

The Quad Operator excels when rhythmic layers are not merely separate events, but modulation sources for one another.

---

# Sound design tips for percussion on this module

## For kicks / toms
- lock state
- low ratio
- sine or triangle
- very little modulation
- short punch envelope externally
- add slight FM only for attack click

## For snares
- one operator as body
- another higher ratio operator modulating it briefly
- add free-state operator for noise/edge
- use square/saw carefully

## For hats / metallics
- free state often works better
- high pitch
- self-FM
- square/saw shapes
- short gain bursts
- irregular reset for changing transients

## For clicks / digital percussion
- high pitch
- square-ish waves
- short envelopes
- strong modulation depth in tiny windows

## For tuned mallet / bell percussion
- lock state
- integer ratios
- start with sines
- use moderate FM
- reset for consistent attack

---

# Important “musical sanity” advice from the manual

The manual explicitly says this module can quickly get noisy and dissonant. For harmonic results they recommend:

- VCO mode
- all operators in lock state
- all detune at noon
- all shape knobs fully CCW to sine
- all modulation sends fully CCW initially

For percussion, that’s also a great starting point.

Then add complexity in this order:

1. get the rhythm structure working first
2. tune operators
3. add one modulation route at a time
4. add self-FM
5. move one operator to free state
6. introduce AR FM
7. use reset creatively
8. save/morph algorithms

If you go too fast, everything becomes hash.

---

# Best workflow for hyper-complex percussion

## Stage 1: Build a stable skeleton
- Op 1 and 2 in lock
- low modulation
- clear rhythms

## Stage 2: Add rotational complexity
- Op 3 and 4 on independent cycle lengths
- free state for one of them

## Stage 3: Make hits affect each other
- use Gain CV envelopes, not just final VCAs
- route modulation from transient operators into body operators

## Stage 4: Add macro-form
- periodic reset
- algorithm morphing with Algo
- AR FM brought in only in fills/phrases

## Stage 5: Performance control
Map external modulation or manual gestures to:
- Gain CV bursts
- Shape CV
- AR FM Gain CV
- Algo crossfade

That gives you micro-rhythm, meso-rhythm, and phrase-level structure all at once.

---

# A very strong full-system patch concept

## “Prime cycle percussion engine”
- Op 1: kick/tom body, 5-step pattern
- Op 2: snare/wood hit, 7-step pattern
- Op 3: hat/click, 11-step pattern
- Op 4: metallic accent, 13-step pattern
- Reset: every 16 or 32 clocks
- AR FM: external noise burst on 9-step pattern
- Algo crossfade: move from A to B over 64 clocks, switch to C for fills

This yields:
- local rhythmic density
- long-cycle emergent repetition
- recurring but non-obvious accents
- timbral mutation tied to rhythm instead of layered on top of it

That is exactly the kind of patch architecture that supports densely rhythmic, hyper-complex percussion music.

---

# Final advice

The Quad Operator is best understood not as “one FM voice,” but as a **networked percussion ecosystem**.

If your goal is complex rhythm:

- use the independent outputs
- think in separate cycle lengths
- use Gain CV as rhythmic modulation control
- mix lock and free states
- exploit Reset for structural alignment
- use AR FM as a chaos injection point
- use the Algo expander for section changes and fill states

If you want, I can also give you:

1. a **10-patch cookbook** specifically for IDM/broken beat percussion on Quad Operator  
2. a **clocking and logic plan** for polyrhythms with this module  
3. a **starter patch sheet** showing exact operator roles and modulation matrix settings

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)