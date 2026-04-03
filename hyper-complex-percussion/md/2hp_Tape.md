# 2hp — Tape

- [Manual PDF](../../manuals/2hp_Tape_Stop.pdf)

---

[Manual PDF / 2hp Tape Stop](https://www.twohp.com/modules/tape-stop)

# Using 2hp Tape Stop for dense, hyper-complex rhythmic percussion

The **2hp Tape Stop** is not a drum sequencer, but in a rhythm-focused Eurorack system it becomes a very powerful **time-warp articulation tool**. Based on the manual, its key features for this use are:

- **Clock input** for syncing the stop length to an external clock
- **Trig gate input** to start the tape stop
- **Momentary / Latching modes**
- **Lag control + Lag CV** to set the stop duration
- **Clock-synced divisions**:  
  **Instant, 32nd, 16th, 8th, quarter, half, whole, 2 bars, 4 bars, 8 bars, 16 bars**
- **50/50 mode** at boot for parallel dry/wet-style layering

That means you can use Tape Stop less like a “DJ effect” and more like a **rhythmic disruption processor** for percussion buses, submixes, loops, or selected drum voices.

---

## What Tape Stop does well in complex rhythm systems

For dense percussion, Tape Stop is best understood as creating:

- **micro-decelerations**
- **syncopated drop gestures**
- **ratchet-to-collapse effects**
- **barline smears**
- **polyrhythmic drag events**
- **phrase-ending temporal modulation**

Instead of adding more hits, it adds **rhythmic deformation**. That is extremely useful when you already have busy patterns and want to create the feeling of deeper complexity.

---

# Best patch roles in a percussion system

## 1. Put it on a full drum bus
Patch:
- Drum mixer/submix out → **Tape Stop IN**
- **Tape Stop OUT** → main mixer / final VCA / FX chain

This gives you the classic whole-kit slowdown. In dense percussion music, this is ideal for:

- end-of-bar disruptions
- fake tempo shifts
- phrase punctuation
- asymmetrical transitions in odd meters

Especially effective in **7/8, 11/8, 13/16**, where the listener already has less footing.

### Tip
Use clock sync so the slowdown duration lands musically relative to your pattern length.

---

## 2. Put it only on a percussion subgroup
Better than full mix in many cases:
- hats + shakers bus
- toms + metallic bus
- claps + rimshots bus
- sample loop bus

This creates **layered rhythmic instability**:
- kick remains stable
- upper percussion smears and bends

That contrast is excellent for hyper-detailed rhythm because the groove stays anchored while selected layers become unstable.

---

## 3. Put it after a loop sampler
The manual specifically suggests pairing with **Play** or **Loop**, and that makes a lot of sense for percussion.

Patch:
- sliced percussion loop / breakbeat voice → Tape Stop
- trigger Tape Stop on selected loop fragments

This creates:
- stuttering pseudo-turntable breakdowns
- off-grid slowdowns inside a repeating loop
- phrase-dependent rhythmic corruption

Very strong for IDM, breakcore, experimental techno, footwork-adjacent patching, or polymetric drum architectures.

---

# Core rhythmic techniques

## 1. Clock-sync the stop time to your metric structure
The manual says with external clock patched to **CLOCK**, the **Lag** knob quantizes to note/bar lengths.

This is the single most important feature for your goal.

### Why it matters
If your percussion is already highly articulated, unsynced tape stops can become muddy. But clock-synced durations let you make the temporal distortion itself part of the composition.

### Use cases
- **32nd / 16th**: micro-stutters, glitch punctuation
- **8th / quarter**: obvious rhythmic drag
- **half / whole**: phrase-scale deceleration
- **2 bars+**: structural breakdowns in polymetric sections

### Advanced idea
Use different master clocks in different patch states:
- one clock from the main transport
- another from a divided or multiplied rhythmic source

If you repatch or switch the clock source, the same Tape Stop gesture can suddenly imply a different metric relationship.

---

## 2. Trigger Tape Stop with a sparse counter-rhythm
Patch a trigger pattern into **TRIG input** that is **less dense** than your drum programming.

For example:
- drums running in 16th-note complexity
- Tape Stop triggered every 5 steps, 7 steps, or 9 steps

This creates a meta-rhythm over the dense percussion fabric.

### Great trigger sources
- Euclidean trigger sequence
- trigger sequencer with non-power-of-two lengths
- logic-derived accents
- clock divider outputs
- probabilistic trigger stream with constrained density

### Example
If your main drums loop over 16 steps:
- trigger Tape Stop every 5 steps
- set Lag to 16th or 8th synced

The points of slowdown rotate against the bar, generating evolving asymmetry.

That is one of the easiest ways to get **polyrhythmic temporal modulation**.

---

## 3. Use odd-length trigger cycles for polymeter
Tape Stop becomes especially interesting when the trigger source has a different cycle length than the percussion source.

Examples:
- drums: 16-step pattern
- Tape Stop trigger: 7-step pattern

or:
- kick/snare phrase in **4/4**
- hi-hat accents in **5**
- Tape Stop triggered from a **3-beat** cycle

Result:
- the “slowdown events” phase against the groove
- repeated material feels continually recomposed
- phrase perception becomes unstable in a controlled way

This is excellent for **polyrhythms** and **complicated repeating structures**.

---

## 4. Modulate Lag CV for changing rhythmic subdivision
The manual gives the **Lag CV input range as -5V to +5V**.

This means you can animate the stop duration over time rather than keeping it fixed.

Patch ideas:
- stepped random CV → **LAG CV**
- sequencer row → **LAG CV**
- slow LFO → **LAG CV**
- sample & hold from a polymetric clock → **LAG CV**

When clock is patched, this effectively changes the synced slowdown duration across rhythmic values.

### Musical result
One trigger stream can produce:
- one event that feels like a 32nd-note drag
- next one an 8th-note slowdown
- next one a half-note collapse

That is where Tape Stop starts behaving like a **rhythmic form shaper** rather than a static effect.

### Best practice
Attenuate CV before it hits Lag CV if possible. For percussion applications, smaller controlled movement is often better than wild full-range jumping.

---

# Specific strategies for hyper-complex percussion

## A. Micro-glitch percussion bus
Patch:
- hats/claps bus → Tape Stop
- master clock → CLOCK
- dense but selective trigger stream → TRIG
- Lag around **Instant / 32nd / 16th**
- momentary mode

Result:
- tiny rhythmic droops
- “digitally unstable tape” feel
- controlled interruption without losing groove

Best for:
- granular techno
- glitch
- electro-acoustic percussion
- dense hats in 4/4 and 7/8

---

## B. Rotating bar-end collapse
Patch:
- full percussion mix → Tape Stop
- clock synced
- trigger from a pattern with a prime-number cycle, like 5, 7, or 11
- Lag at **quarter / half / whole**

Result:
- bar-end deceleration keeps landing in new places
- the ear hears a shifting formal structure
- great for polymeter and long-cycle composition

This works especially well if your drum material is itself tightly quantized and repetitive; Tape Stop introduces controlled phrase mutation.

---

## C. Polyrhythmic upper-layer drag
Patch:
- hats/shakers/ticks only → Tape Stop
- kick and snare remain dry outside the module
- trigger from a different rhythmic layer than the hats
- moderate synced Lag values

Result:
- lower groove stays fixed
- top-end sounds like it slips, bends, and recovers
- fantastic illusion of multiple simultaneous tempi

This is one of the best applications for dense rhythmic music because it preserves danceability while increasing complexity.

---

## D. Trigger-gated structural fills
Because the TRIG input is a gate input and the front-panel toggle selects **momentary** or **latching**, you can think in performance terms.

### Momentary mode
Tape stop is active while held/high.

Use this when you want:
- short fills
- pressure-controlled rhythmic bends
- manually performed interruptions
- gate-length-dependent gestural variations

Patch a gate sequencer with variable gate lengths to TRIG. Even if the internal slowdown behavior is defined by Lag, using varying gate durations can produce more performative rhythmic contour.

### Latching mode
One trigger starts the stop, another ends it.

Use this for:
- long phrase-level breakdowns
- asymmetrical structural disruptions
- “enter warped time / exit warped time” gestures

Very good in odd-meter live sets where you want to destabilize pulse perception across several beats or bars.

---

# Using Tape Stop in complex time signatures

## In 7/8
A classic approach:
- main clock into CLOCK
- trigger Tape Stop on the last eighth-note of the 7/8 bar
- set Lag to **16th** or **8th**

This exaggerates the unevenness of the bar and creates a lopsided, expressive cadence.

Alternative:
- trigger every second bar
- use quarter or half-note Lag for larger phrase deformation

---

## In 5/4
Try:
- kick structure remains stable
- percussion subgroup through Tape Stop
- trigger on beat 5 or every 3 bars
- Lag CV from a 4-step sequence

This sets up a beautiful contradiction:
- meter says 5
- slowdown behavior cycles in 4
- phrase relationship evolves over 20 beats

---

## In 13/16 or other fast asymmetrical meters
Use very short synced Lag settings:
- Instant
- 32nd
- 16th

Long slowdowns in fast odd meters can blur too much. Short values keep the complexity articulate.

Best source material:
- clicks
- hats
- foley percussion
- short samples
- FM percussion bursts

---

# Polyrhythm patch examples

## Patch 1: 4 against 5 slowdown field
- Main drum machine/sequencer runs **4/4**
- Percussion subgroup through Tape Stop
- CLOCK gets the main clock
- TRIG gets a trigger every 5 eighth-notes
- Lag set to **16th** or **8th**

Outcome:
- slowdown events drift against the bar
- repeating material never lands the same way twice until long cycle resolution
- ideal for hypnotic complexity

---

## Patch 2: Euclidean hats with rotating slowdowns
- Hat bus → Tape Stop
- CLOCK from master
- Euclidean trigger source, e.g. **5 hits over 12** or **7 over 16** into TRIG
- sequencer row into LAG CV

Outcome:
- each slowdown lands on a sparse but irregular accent
- duration changes each time
- hats feel alive, elastic, and structurally intelligent

---

## Patch 3: Long-cycle phrase mutation
- Full percussion loop → Tape Stop
- CLOCK from transport
- TRIG from a 15-step trigger pattern while drums are 16-step
- Lag at **quarter**, occasionally CV-modulated to **half**

Outcome:
- every phrase is subtly re-authored
- strong for abstract techno and generative rhythms
- especially good if loop contains ghost notes and syncopation

---

# 50/50 mode is especially useful for percussion

The manual notes:

> Holding the Trig button at boot up sets dry/wet mix to 50%, allowing the dry signal to be heard while tape stopping.

For dense percussion, this is extremely valuable.

## Why
A full wet tape stop can remove too much transient clarity. But with 50/50 mode:
- dry hits preserve pulse definition
- wet path creates drag/smear
- the result sounds layered and intricate rather than simply interrupted

This is often the sweet spot for complex percussion music.

## Best use
- busy hat lines
- breakbeat loops
- metallic percussion
- ghost-note-heavy clap/snare textures

It creates the illusion of simultaneous stable and unstable timing.

---

# External parallel processing idea

The manual also mentions using a **VCA** for more mixing control. That is a great idea.

Patch:
- mult audio source
- one path dry to mixer
- one path through Tape Stop
- use VCAs or mixer channels to control blend dynamically

Now you can:
- automate how much rhythmic corruption is present
- fade Tape Stop in only on selected structural moments
- exaggerate complexity without losing the main groove

For hyper-complex music, this is usually better than leaving Tape Stop permanently full-wet.

---

# Performance methods

## 1. Manual Trig as a live rhythm instrument
The front-panel **Trig button** can be played by hand.

Use it like:
- a manual fill button
- a phrase punctuation control
- a “deceleration accent” performer tool

In a live patch with many repetitive layers, manually applied Tape Stop gestures can make the rhythm feel far more composed and intentional.

---

## 2. Toggle between momentary and latching during performance
- **Momentary** for tiny cuts and drags
- **Latching** for entering a longer warped-time state

This lets you play the module at two structural scales:
- micro-rhythm
- macro-form

---

## 3. Use blinking LED as a timing reference
The manual notes the **Trig LED** blinks to an external clock rate and indicates active tape stopping.

That’s useful in a busy live patch:
- confirm sync status visually
- perform slowdowns against visible pulse
- monitor whether your trigger logic is behaving as expected

---

# What kinds of sounds work best

Tape Stop on percussion tends to shine most with:
- hi-hats
- rides
- shakers
- glitch clicks
- tom flurries
- sample loops
- rimshots
- metallic/noisy percussion textures

It can also work on kick/snare buses, but very low-end material can get smeared in a way that reduces impact. For dense rhythm music, selective subgroup processing is often stronger than processing the whole kit.

---

# A few compositional ideas

## 1. Treat tape stops as “negative fills”
Instead of adding extra notes before a transition, remove momentum by slowing existing material. This is often more sophisticated than another ratchet burst.

## 2. Use different structural layers
- percussion pattern complexity from sequencers
- metric complexity from odd bar lengths
- temporal complexity from Tape Stop events

These three layers together can create very rich results.

## 3. Let Tape Stop define phrase boundaries
In long polymetric music, listeners need clues. A recurring but shifting tape stop can become a high-level form marker.

---

# Practical starting recipes

## Recipe 1: Tight glitch hats
- hats bus into Tape Stop
- external clock patched
- momentary mode
- Lag at 32nd/16th
- trigger from irregular accent sequencer
- 50/50 mode on

## Recipe 2: Odd-meter phrase bend
- full percussion subgroup into Tape Stop
- clock synced
- trigger once near the end of each 7/8 or 11/8 phrase
- Lag at 8th or quarter
- occasional Lag CV shifts for variation

## Recipe 3: Polymetric loop corruption
- loop player into Tape Stop
- trigger from a sequence of different length than the loop
- latching mode for longer events
- Lag moves between 16th, 8th, quarter, and half with CV

---

# Limitations to keep in mind

Based on the manual, Tape Stop is focused and simple:
- one audio input / one audio output
- one main timing effect
- no internal sequencing memory
- no per-hit slicing or granular control

So it won’t generate complex percussion on its own. Instead, it excels at **reshaping** already-complex rhythmic material into something more animated, unstable, and compositionally rich.

Think of it as a **temporal accent processor**.

---

# Bottom line

For densely rhythmic, hyper-complex percussion, the 2hp Tape Stop is best used as a **clock-synced temporal disruption effect** on:
- percussion submixes
- loops
- hats/metallic layers
- occasionally the full drum bus

Its strongest applications are:

- **polyrhythmic trigger placement**
- **odd-cycle modulation of stop events**
- **clock-synced Lag changes**
- **parallel dry/wet layering via 50/50 mode or external mixing**
- **structural phrase bending in odd meters**

If you patch it with:
1. a **stable master clock**,
2. a **non-matching trigger cycle**,
3. **CV over Lag**, and
4. **selective percussion routing**,

you can get extremely sophisticated rhythmic motion without making the patch unreadable.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)