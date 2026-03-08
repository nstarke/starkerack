# 2hp — Brst

- [Manual PDF](../../manuals/Brst_Manual.pdf)

---

[Manual PDF](attachment)

# Brst — using it for melodic components

Brst is **not a pitch/CV sequencer by itself**. It’s a **burst generator / trigger delay** that turns one trigger or gate into a fast series of triggers. That means its melodic usefulness comes from how it **drives other modules**:

- sequencers
- sample & hold
- quantizers
- envelopes/LPGs
- clock dividers/multipliers
- switches
- logic
- trigger-to-gate or trigger-to-envelope utilities

So for melody, think of Brst as a module that creates **repeated note events, ratchets, grace notes, strums, arpeggio-like trigger clusters, and delayed re-articulations**.

## What Brst does

From the manual:

- **TRIG input** starts a burst when it receives a trigger/gate
- **PULSES** sets how many triggers are generated
  - from **1 to 32**
- **RATE** sets the time between triggers
  - about **10 ms to 500 ms**
- **PULSES CV** and **RATE CV** let you voltage-control those two parameters
- **TRIG toggle**:
  - **left** = include the initial trigger
  - **right** = omit the initial trigger
- **OUT** emits the burst as **0–5 V triggers**

This makes it especially good for:
- ratcheting one note into many attacks
- creating repeated sampling events
- stepping a sequencer multiple times from one master clock
- making a melody “flutter” or “bounce”
- delayed note echoes in trigger form

---

# Best ways to use Brst for melodic music

## 1) Ratcheting a sequenced melody

### Patch
- Send your main rhythm trigger or sequencer gate to **Brst TRIG**
- Send **Brst OUT** to the envelope or LPG that opens your melodic voice
- Keep your pitch sequence going from another sequencer into the oscillator pitch input
- Adjust:
  - **PULSES** for number of ratchets
  - **RATE** for ratchet speed

### Result
Each note in your melody can fire multiple times quickly, creating:
- trance-style ratchets
- IDM stutters
- ornamented melodic phrases
- repeated plucks on a single pitch

### Musical use
This is the most direct melodic use:
- same pitch, multiple articulations
- great for plucks, FM bleeps, acid lines, and arpeggio voices

### Tip
Use the **TRIG toggle left** to include the first hit immediately, then the extra repeats follow.

---

## 2) Burst-clocking a sequencer for fast melodic runs

### Patch
- Main clock or manual trigger into **Brst TRIG**
- **Brst OUT** into the **clock input of a sequencer**
- Sequencer pitch CV into oscillator 1V/oct
- Envelope/VCA triggered either:
  - by the same **Brst OUT**, or
  - by a separate gate source

### Result
One incoming trigger can advance the sequencer several steps very quickly, producing:
- mini arpeggios
- melodic fills
- fast ascending/descending runs
- pseudo-strums if the sequencer has chord-related voltages

### Why this works
Brst effectively turns one musical event into **multiple sequencer advances**.

### Tip
If you modulate **PULSES CV**, some notes create short runs and some create long runs. That gives phrases more expression.

---

## 3) Quantized sample-and-hold melody generator

This is one of the strongest melodic pairings.

### Patch
- Noise, random CV, or slow modulation source into **Sample & Hold input**
- **Brst OUT** into **Sample & Hold trigger**
- Sample & Hold output into **Quantizer**
- Quantizer output into oscillator 1V/oct
- Use the same **Brst OUT** or a derived gate to trigger your envelope

### Result
Each burst creates several new quantized notes in quick succession:
- random melodic flourishes
- clustered ornamentation
- “bouncing ball” melodies
- generative lead lines

### Tip
- Slow **RATE** = clearly separated melodic notes
- Fast **RATE** = clustered trills or grace-note runs
- Low **PULSES** = subtle ornamentation
- High **PULSES** = long random cascades

---

## 4) Arpeggio-style phrases from sequential switching

If you have a switch or sequential switch, Brst gets very musical.

### Patch
- Feed several fixed voltages or pitch CVs into a sequential switch
- Clock the switch with **Brst OUT**
- Switch output into a quantizer or directly to oscillator pitch if tuned
- Trigger your envelope from **Brst OUT**

### Result
A single trigger produces a rapid sequence of different pitches:
- chord strums
- arpeggiated bursts
- broken chord ornaments
- harp-like plucks

### Great source material
Put into the switch:
- root / third / fifth / octave
- notes from a chord
- different rows of a sequencer
- transposition voltages

This turns Brst into a **melodic phrase generator**.

---

## 5) Delayed melodic echoes

Because Brst can omit the initial trigger, it can act like a trigger delay with repeats.

### Patch
- Send your main melody gate to **Brst TRIG**
- Set **TRIG toggle right** to omit the initial hit
- Use **OUT** to trigger a second envelope/voice or re-trigger the same voice

### Result
You get:
- delayed note repeats
- ghost notes
- call-and-response attacks
- melodic shadows

### Especially effective with
- two oscillators tuned in intervals
- a second voice an octave up/down
- filtered echoes from a parallel voice

Instead of audio delay, you get a **compositional trigger delay** that can generate new melodic articulations.

---

## 6) Ornament generation for sustained notes

### Patch
- Main gate opens a long envelope on a voice
- Same gate also goes to **Brst TRIG**
- **Brst OUT** triggers:
  - a second short envelope to FM index,
  - a wavefolder CV accent,
  - filter pings,
  - or a VCA on a parallel voice

### Result
The pitch may stay constant, but the burst adds melodic-style embellishment:
- mordents
- trills
- flutter-tongue effects
- repeated accenting on the note

This is useful when “melodic component” means not only changing pitch, but adding **expressive note structure**.

---

## 7) Using Brst to create trills between two pitches

If you have a switch, logic-controlled transposition, or dual pitch source:

### Patch idea
- Main pitch CV goes to oscillator
- A second interval voltage is available, such as +2 semitones or +7 semitones
- Use **Brst OUT** to toggle a switch between the base pitch and interval pitch
- Also use a related trigger to articulate the note

### Result
One note becomes a fast alternation:
- trill
- mordent
- alternating dyad gesture
- baroque-style ornament

Brst is excellent for this because the **rate** is controllable and can be CV-modulated.

---

## 8) Humanizing or varying melodic clocks

The manual specifically mentions humanizing a clock signal. For melody, that means:

### Patch
- Main clock/gate into **Brst TRIG**
- Use low **PULSES** and moderate **RATE**
- Feed **OUT** to a sequencer clock or auxiliary melodic event

### Result
Instead of every melodic step being equally plain, some steps have:
- extra ticks
- repeated notes
- little rushes
- phrase-ending fills

This is great in generative patches where a melody feels too rigid.

---

# Voltage control strategies for melodic use

## PULSES CV
Use this to vary how many notes/articulations a phrase produces.

Good modulation sources:
- slow random CV
- sequencer row
- envelope
- keyboard velocity/mod wheel if interfaced
- another rhythmic modulation source

### Musical effect
- some notes are single hits
- some are double/triple ratchets
- some become long flourishes

This adds **phrase hierarchy**.

## RATE CV
Use this to vary the spacing of repeated notes.

Good modulation sources:
- random stepped CV
- LFO
- envelope for accelerating/decelerating burst feel
- sequencer accent row

### Musical effect
- fast grace notes on some steps
- slower echoed notes on others
- changing density across a phrase

This is one of the easiest ways to make Brst feel alive.

---

# Concrete melodic patch recipes

## Patch 1: Simple ratcheted lead
**Needs:** pitch sequencer, oscillator, envelope, VCA

- Sequencer pitch CV → oscillator 1V/oct
- Main gate pattern → Brst TRIG
- Brst OUT → envelope trigger
- Envelope → VCA CV
- Oscillator → VCA → output

**Settings**
- TRIG toggle left
- PULSES: 2–5
- RATE: fast

**Sound**
A lead line where selected notes repeat rapidly.

---

## Patch 2: Random burst melody
**Needs:** noise/random source, sample & hold, quantizer, oscillator, envelope

- Random CV/noise → S&H input
- Brst OUT → S&H trigger
- S&H out → quantizer
- Quantizer out → oscillator 1V/oct
- Brst TRIG fed from a slow clock or manual gate
- Brst OUT → envelope trigger

**Sound**
Each trigger creates a little cluster of quantized notes.

---

## Patch 3: Chord strum
**Needs:** sequential switch or multiple fixed pitch voltages, quantizer optional

- Several tuned voltages or chord tones → switch inputs
- Brst OUT → switch clock/advance
- Switch output → oscillator pitch
- Main gate → Brst TRIG
- Brst OUT → envelope trigger

**Sound**
One trigger strums through chord tones like a harp or guitar rake.

---

## Patch 4: Sequencer fill generator
**Needs:** step sequencer, oscillator, envelope

- Master clock or fill trigger → Brst TRIG
- Brst OUT → sequencer clock
- Sequencer CV → oscillator pitch
- Brst OUT → envelope trigger

**Sound**
Instead of one note, a single event makes the sequencer run through several notes quickly.

Great for:
- phrase endings
- transitions
- fills between bass notes

---

## Patch 5: Delayed octave echo
**Needs:** 2 voices or one voice with transposition path

- Main melody gate → voice 1 envelope
- Same gate → Brst TRIG
- TRIG toggle right
- Brst OUT → voice 2 envelope
- Voice 2 tuned one octave above or fifth above

**Sound**
Each note gets a delayed answering note above it.

---

# Performance ideas

## Manual triggering
Brst is very playable when fed from:
- a manual gate button
- keyboard gate
- pressure pad gate
- gate sequencer accents

You can use it to inject:
- trills
- fills
- grace-note bursts
- sudden arpeggios

## Accent-based use
Instead of sending every note to Brst, only send:
- accented steps
- every 4th bar trigger
- end-of-sequence trigger
- probability-generated gates

That keeps the melodic bursts special.

## Modulate only one parameter at a time
For musical clarity:
- modulate **PULSES** if you want varying phrase length
- modulate **RATE** if you want varying urgency
- modulate both only if you want chaos

---

# Important limitations

Brst does **not** itself produce pitch CV. So to make truly melodic material, pair it with at least one of these:

- quantizer
- sequencer
- sample & hold
- precision adder/transposer
- sequential switch
- oscillator/envelope voice

Without those, Brst only creates rhythmic trigger structures.

But in a Eurorack system, that’s often exactly what turns static pitch material into something musical and expressive.

---

# Best musical roles for Brst in a melody-focused rack

Brst is especially strong as a:

- **ratchet generator** for sequenced notes
- **ornament generator** for trills and grace notes
- **burst clock** for fast sequencer runs
- **random melody trigger source** for S&H + quantizer patches
- **strum engine** for chord tone switching
- **delayed re-trigger tool** for echoes and call-response phrasing

If your system already has pitch sources, Brst adds the **articulation layer** that makes melodies feel less static.

---

# Bottom line

Brst is best understood as a **melodic event multiplier** rather than a melody source. It takes one trigger and turns it into a cluster of note opportunities. When combined with sequencers, quantizers, switches, or sample-and-hold, it can produce:

- ratchets
- trills
- grace notes
- arpeggiated runs
- chord strums
- delayed melodic echoes
- generative note cascades

In short: **Brst adds phrasing, ornamentation, and motion to melodic patches**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)