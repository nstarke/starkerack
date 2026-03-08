# Kaona Instruments — Skippy

- [Manual PDF](../../manuals/Skippy_2-2_ENG.pdf)

---

[Skippy Manual PDF (Kaona)](https://www.kaona.fr)

# Kaona Skippy — creating melodic components in a Eurorack system

Skippy is fundamentally a **4-track gate/CV trigger sequencer** with unusual timing behavior: Euclidean rhythms, logarithmic/Gaussian spacing, matrix and non-matrix timing, per-track independence, and synchronized global behavior. On its own, it does **not appear to generate pitch CV** from the outputs described in this manual; it outputs **5V gates** on four channels, plus uses internal timing and external clock/reset behavior.

So, as a Eurorack musician, I’d treat Skippy as a **melodic structure generator**, not a pitch sequencer by itself. It excels at generating the rhythmic logic that makes melodies feel alive.

---

## What Skippy contributes to melody

Skippy can create melodic components by controlling:

- **when notes happen**
- **which notes are accented**
- **how often a voice changes pitch**
- **when multiple melodic layers interlock**
- **when a melody is regular vs humanized vs unstable**
- **how phrases realign over time**

That means Skippy is best paired with modules such as:

- **quantizers**
- **sample & hold / track & hold**
- **sequential switches**
- **CV sequencers**
- **precision adders**
- **envelope generators**
- **clockable random sources**
- **oscillators / voices**

---

## Important operational idea

Each of Skippy’s 4 tracks can be set independently with:

- BPM
- step count
- begin/end arc
- gate length
- probability
- chaos
- direction
- swing
- timing algorithm (Gauss, Euclid, Tiles, Polyr, Jazzy, etc.)
- spin
- pause/reset behavior

This means each track can act like a separate **phrase engine** for one aspect of melody.

For example:

- Track 1 = main note trigger
- Track 2 = pitch-change trigger
- Track 3 = accent trigger
- Track 4 = phrase reset / ornament trigger

That’s where Skippy becomes musically powerful.

---

# Best ways to use Skippy for melody

## 1. Triggering a pitch source

The most direct melodic use:

- Send one Skippy output to an **envelope + VCA/voice**
- Send another Skippy output to a **sample & hold**
- Feed the sample & hold from random CV, a slow sequencer, or a modulation source
- Quantize the sampled CV
- Send quantized CV to oscillator pitch

### Result
One Skippy track decides **when a note is heard**, and another decides **when the pitch changes**.

### Why this is musical
Because note articulation and pitch updates don’t have to happen at the same time. This creates:

- repeated notes
- held tones
- syncopation
- melodic motifs
- evolving ostinati

### Example
- Track 1: Euclidean 5/16 → triggers envelope
- Track 2: Tiles alternating sparse pattern → clocks sample & hold
- Random CV → quantizer → oscillator 1V/oct

This gives a melody where some notes repeat while others change.

---

## 2. Building a 4-part melodic architecture

Because Skippy has four synchronized but independent tracks, it naturally maps to four melodic jobs.

### Suggested assignment
- **Track 1:** main melody triggers
- **Track 2:** pitch change clock
- **Track 3:** transposition or accent events
- **Track 4:** phrase reset, ratchet substitute, or secondary voice

### Patch idea
- Track 1 → envelope for lead voice
- Track 2 → clock a sample & hold grabbing CV from a sequencer/random source
- Track 3 → trigger another S&H that samples a slower transposition voltage, then add via precision adder
- Track 4 → trigger second oscillator or harmonic layer

### Result
A melody with:
- changing note density
- changing pitches
- occasional transpositions
- layered countermelody

Skippy is especially good here because different step lengths and timing modes drift and re-align in long cycles.

---

## 3. Euclidean melody generation

Skippy’s **EUCLID** is ideal for melodic rhythm.

The manual says Euclidean distribution is calculated in real time and can be used with any chosen step count from 1 to 64, with the active pulses selected independently.

### Melodic use
Pair Euclid with pitch generation modules.

### Patch
- Track 1: Euclid 7/16 → note trigger
- Track 2: Euclid 3/16, spun a few steps → pitch update trigger
- Track 3: Euclid 2/16 → accent envelope or filter ping
- Track 4: Euclid 1/16 or 1/32 equivalent phrase marker → reset or transposition

### Musical effect
This gives you melodies where:
- some notes repeat
- some pitches update off the main beat
- accents appear in a separate Euclidean layer
- phrasing emerges from the overlap

This is excellent for:
- Berlin-school patterns
- minimalism
- polyrhythmic techno leads
- generative melodic percussion

---

## 4. Using GAUSS for non-linear melodic phrasing

Skippy’s **GAUSS** function is one of the most interesting for melody because it changes the spacing between steps logarithmically.

The manual notes that high values can create very long final intervals, even seconds or minutes.

### Melodic use
Use GAUSS not for drum timing, but for **phrase timing**:
- when pitch changes happen
- when transpositions occur
- when a sequence opens/closes
- when a second voice enters

### Patch
- Track 1: regular main trigger pattern
- Track 2: GAUSS → clocks a sample & hold for pitch changes
- Track 3: slow GAUSS → triggers transposition changes
- Track 4: regular accent or reset

### Result
Your melody has a stable pulse, but the pitch decisions feel organic and stretched.

### Best application
- ambient
- electroacoustic
- generative composition
- evolving arpeggios

Also, the manual specifically suggests **WAY ping-pong** can work well with GAUSS. For melody, that means the phrase can "breathe" forward and backward in time.

---

## 5. Using TILES to make repeating note/rest structures

**TILES** is a matrix function where a number of played steps alternates with silent steps.

This is very useful for melody because it creates predictable note/rest architectures.

### Patch
- Track 1: TILES → main envelope trigger
- Pitch source: quantized CV sequencer or S&H
- Track 2: regular trigger to advance pitch every step
- Track 3: accent trigger
- Track 4: occasional reset

### Result
The melody can advance continuously in pitch, but only some steps are articulated.

This creates:
- implied melodic syncopation
- rests
- off-beat motifs
- broken arpeggios

If Track 2 advances pitch more often than Track 1 articulates notes, you get "skipped" melody notes. If Track 1 fires more often than Track 2, you get repeated tones.

Both are musically useful.

---

## 6. Using POLYR for alternating melodic subdivisions

The manual describes **POLYR** as a non-matrix function where two tempos alternate, like 4/3, and Skippy recalculates total steps to maintain the alternation consistently.

### Melodic use
This is excellent for:
- alternating long/short phrase movement
- uneven melodic gait
- "breathing" sequences
- non-straight arpeggios

### Patch
- Track 1: POLYR for note triggers
- Track 2: steady pitch-change clock
- Track 3: slower Euclid for accents
- Track 4: occasional phrase transposition

### Result
The melody feels as if it is moving through alternating metrical spaces, even if the pitch source is simple.

This works great when the pitch source is:
- a 4- or 8-step CV sequencer
- a quantized random source
- a shift register melody
- a chord CV source sampled into single notes

---

## 7. Using JAZZY as a melodic gate slicer

**JAZZY** slices 32 steps into predefined groove patterns across styles like bossa, folk, funk, jazz.

This is extremely valuable for melody because groove often matters more than note choice.

### Patch
- Track 1: JAZZY pattern → note trigger
- Track 2: regular or sparse trigger → pitch updates
- Track 3: additional JAZZY or Euclid trigger → accent
- Track 4: secondary voice or call-and-response trigger

### Result
Even with a simple pitch source, the melody sounds stylized and intentional because the articulation pattern carries genre character.

### Best use
- jazzy lines
- broken chords
- syncopated bass melodies
- groovebox-style sequencing
- humanized hooks

Because JAZZY forces 32 steps, it also works well as a master phrasing layer against other shorter or longer cyclic events.

---

## 8. Probability and chaos for melodic variation

Skippy provides two strong variation tools:

- **PROBA**: probability of not triggering an otherwise scheduled step
- **CHAOS**: temporal random acceleration between steps

These are gold for melody.

### PROBA use
Use on:
- trigger stream for the main voice
- pitch update triggers
- accent triggers

### Effect
- missing notes
- variation in repeated motifs
- ghosted phrases
- less mechanical repetition

### CHAOS use
Use more carefully, especially on pitch update clocks.

### Effect
- rushed ornaments
- unstable melodic timing
- flams against steady percussion
- elastic phrase movement

### Great patch concept
- Main note trigger mostly stable
- Pitch-change trigger with probability
- Accent trigger with chaos
- Reset every few bars

This gives melodies that stay coherent but never loop exactly.

---

## 9. Swing and gate length as melodic articulation tools

Skippy’s **SWING** and **GATES** parameters are not just rhythmic—they strongly affect melodic feel.

### Swing
Apply to trigger tracks controlling:
- note articulation
- pitch updates
- accent layers

A swung pitch update track against a straight trigger track can create subtle delayed note changes.

### Gates
Longer gates can create:
- legato feeling
- tied notes
- sustained envelopes
- overlap effects in LPGs or VCAs

Short gates create:
- plucked notes
- staccato melodies
- sharper articulation

### Example
- Track 1: short gates for plucked melody
- Track 2: sparse long gates to open a secondary VCA or drone layer
- Track 3: accent triggers
- Track 4: transposition changes

---

## 10. Begin/End arcs for partial phrases

The **BEGIN** and **END** functions let you use only an arc of the circle instead of a full 0-to-0 traversal.

### Melodic implication
You can create:
- partial phrase windows
- clipped rhythmic loops
- phrase fragments
- asymmetrical entry/exit behavior

### Patch idea
Use one track with a shortened arc to trigger pitch changes only during part of the phrase while another track runs full-length note triggers.

### Result
The melody becomes sectional:
- one portion evolves
- another remains static
- then they loop together in long-form recombination

This is excellent for generative melodic form.

---

## 11. WAY and SPIN for melodic contour behavior

### WAY
Skippy supports:
- left
- right
- ping-pong
- stop

For melodic systems, **ping-pong** is especially useful if Skippy is clocking:
- a sequential switch
- a sample source
- transposition triggers
- multiple voice entrances

It can create a feeling of phrase reflection.

### SPIN
SPIN rotates matrix and Euclidean functions left/right and is not saved.

This is ideal for performance:
- nudging a melody off the beat
- rotating accent positions
- shifting when pitch-change triggers occur
- instantly generating call/response variations

A great live move is to keep pitch material unchanged and only rotate the trigger logic.

---

# Practical melodic patch recipes

## Patch 1: Quantized random melody
**Goal:** evolving melodic line

- Random CV source → quantizer → oscillator pitch
- Track 1 → envelope trigger for voice
- Track 2 → sample & hold clock sampling the random CV
- Track 3 → filter accent envelope
- Track 4 → reset a related sequencer every few bars

Suggested settings:
- T1 Euclid 5/16
- T2 Tiles or Euclid 3/16
- T3 Proba-enabled sparse pattern
- T4 very slow pulse

This yields a coherent but shifting melody.

---

## Patch 2: Broken arpeggiator
**Goal:** chord-based melodic fragments

- Chord or static CV row into sequential switch / addressable switch
- Quantizer after switch if needed
- Track 1 → trigger voice
- Track 2 → advance switch
- Track 3 → octave transposition trigger
- Track 4 → accent or second voice

Suggested settings:
- T1 JAZZY or TILES
- T2 steady matrix pulse
- T3 sparse Euclid
- T4 swing-enabled complementary rhythm

Result: a broken chord line with groove and variation.

---

## Patch 3: Two-voice canon / call-and-response
**Goal:** interlocking melodies

- One pitch source to two voices
- Track 1 → voice A trigger
- Track 2 → voice B trigger
- Track 3 → S&H clock for pitch updates
- Track 4 → transposition or reset

Suggested settings:
- T1 Euclid 7/16
- T2 same Euclid but SPIN shifted
- T3 slower regular or Gaussian trigger
- T4 long-cycle phrase control

Result: two voices share pitch material but articulate it differently.

---

## Patch 4: Generative ambient melody
**Goal:** slow, evolving line

- Smooth random or chaotic CV → quantizer
- Track 1 → sparse main trigger
- Track 2 → GAUSS pitch update
- Track 3 → very slow transposition sample
- Track 4 → occasional harmonic accent / drone swell

Suggested settings:
- T1 sparse Euclid or Tiles
- T2 high GAUSS with ping-pong WAY
- T3 low-probability long-cycle pattern
- T4 long gates

Result: very organic melodic unfolding.

---

## Patch 5: Melodic bassline with groove
**Goal:** syncopated bass sequence

- 8-step CV sequencer → quantizer → bass oscillator
- Track 1 → bass envelope trigger
- Track 2 → sequencer advance
- Track 3 → accent envelope to filter/VCA
- Track 4 → reset sequencer phrase

Suggested settings:
- T1 JAZZY or swung Tiles
- T2 steady pulse
- T3 sparse Euclid with spin
- T4 phrase-end reset

This gives tight groove with controlled note repetition.

---

# Best companion modules for Skippy in melodic use

Skippy pairs especially well with:

## Quantizers
To turn random, sequenced, or sampled voltages into scales.

## Sample & Hold / Track & Hold
One of the best companions. Skippy decides when pitch changes happen.

## CV sequencers
Skippy can clock them irregularly, partially, or in parallel.

## Sequential switches
Excellent for creating melodic selection logic from Skippy’s four outputs.

## Precision adders
Useful for transposition layers triggered by separate tracks.

## Envelope generators / function generators
For articulation, accents, and note shaping.

## Logic modules
Combine Skippy outputs for composite melody conditions:
- AND for rare notes
- OR for denser lines
- XOR for unexpected interplay

## Clock dividers / multipliers
Especially when using external clock modes.

---

# External clock and melodic synchronization

The manual’s **CLK IN** options matter a lot.

## RESET mode
Useful if you want Skippy to restart phrases from external transport or bar resets.

## POLY mode
Best if you want Skippy to retain its own fluid/non-metric character while still following an external pulse average.

Great for:
- semi-free melodies
- generative patches
- drifting but related phrasing

## MATRIX mode
Best if you want exact step-following from an external clock, including irregular/swing/random clocks.

Great for:
- strict synchronization with another sequencer
- manually stepped melodic progressions
- clocking from unusual external pulse trains

This is very powerful if another module is your pitch sequencer and Skippy is your articulation brain.

---

# Performance strategies

## Use RESET often
The manual notes Skippy can lose track of step alignment or tracks can drift unsynchronized depending on manipulations. For melodic use, RESET is important when:
- changing direction
- changing step counts
- using stop/pause-like states
- moving between phrases live

## Use Sync mode for bar-level phrase lock
Double-click RESET to force all tracks back to 0 on each rotation.

This is useful if you want:
- predictable recurring melodic phrases
- consistent downbeat alignment
- long-cycle ratios without complete free drift

Turn it off if you want more natural phase movement.

## Use PAUSE for performance muting
PAUSE mutes individual tracks with blinking buttons. This is useful for:
- dropping pitch updates while notes continue
- dropping accents
- muting the second melodic voice
- creating temporary ostinatos

---

# What Skippy is best at melodically

Skippy is especially strong for:

- **generative melody timing**
- **interlocking trigger networks**
- **polyrhythmic articulation**
- **phrase drift and realignment**
- **groove-oriented melodic gating**
- **irregular pitch-update logic**
- **humanized or mathematically structured phrasing**

It is less a “play notes 1–8 in order” module and more a **melodic behavior engine**.

---

# Best musical roles for Skippy

In a larger system, Skippy works best as:

- **melodic trigger brain**
- **phrase shaper**
- **pitch-change clock source**
- **accent and ornament sequencer**
- **countermelody trigger generator**
- **reset/conducting hub for melodic subsystems**

---

# Bottom line

If you want to make melodies with Skippy, think in layers:

1. **one track triggers notes**
2. **one track decides when pitch changes**
3. **one track adds accents or transposition**
4. **one track defines phrase-level behavior**

Paired with a quantizer, sample & hold, CV sequencer, or switch, Skippy becomes a highly expressive melodic engine capable of everything from tight syncopated basslines to drifting generative ambient lines.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)