# Erogenous Tones — Radar

- [Manual PDF](../../manuals/radar-instructions.pdf)

---

[Manual PDF](http://erogenous-tones.com)

# Erogenous Tones RADAR — melodic patch analysis

RADAR is not a voice or pitch sequencer by itself, but as a **dense bank of 8 envelopes/LFOs** it is extremely useful for building **melodic motion** when paired with oscillators, quantizers, VCAs, filters, wavefolders, switches, logic, and sequential controllers.

## What RADAR gives you musically

From the manual, RADAR provides:

- **8 independent AD/AR/repeating envelopes** in **Envelope Mode**
- **2 groups of quadrature modulation** in **Quad Mode**
- **8 phase-offset modulation lanes** in **Oct Mode**
- Per-lane behavior:
  - **Repeating**
  - **AD**
  - **AR**
- Envelope/LFO shaping:
  - **Log / Lin / Exp** and everything between
- Two response models:
  - **Digital**
  - **Analog modelling**
- Composite “max” outputs on:
  - **Lane 4** = max of lanes 3+4
  - **Lane 8** = max of lanes 6+7+8
- Trigger normalization down the lanes in Envelope Mode

That means RADAR is best understood as a **high-density modulation composer**. For melody, that matters because melody in Eurorack is often built from:

- **pitch CV movement**
- **rhythmic articulation**
- **accent**
- **timbral contour**
- **phase-related modulation**
- **repetition with controlled variation**

RADAR can drive all of those.

---

# Best ways RADAR contributes to melodic components

## 1. Envelope-shaped pitch modulation

One of the most direct melodic uses is sending RADAR outputs to an oscillator’s **1V/oct input through an attenuator/attenuverter and ideally a quantizer**.

### Why this works
An envelope is just a control curve. If you:
- trigger it rhythmically,
- attenuate it to musically useful intervals,
- and quantize the result,

you get **stepped or contour-derived melodic lines**.

### Patch idea
- RADAR lane 1 in **AD mode**
- Trigger lane 1 from a clock or gate sequencer
- Lane 1 output → attenuverter → quantizer CV in → oscillator 1V/oct
- Same trigger also goes to your VCA envelope or LPG strike

### Musical result
- Short attack/short release = tight repeated notes
- Longer release = falling melodic tails
- Log/exp shapes create different pitch gestures:
  - **EXP rise** can feel like quick “snap-to-note”
  - **LOG fall** can feel like expressive downward bends

### Best use
This is especially effective for:
- acid-like lines
- plucks with pitch sweep
- pseudo-sequenced motifs from one trigger stream

---

## 2. AR mode as expressive note shaping

The manual notes that in **AR mode**, especially in **analog modelling mode**, the attack can depend on how long the incoming gate stays high.

### Melodic implication
If gate length varies, pitch or timbre modulation varies too. That creates **phrase-sensitive melody**, not just static repeated notes.

### Patch idea
- Use a gate sequencer with variable gate lengths
- RADAR lane 2 in **AR mode**, analog modelling
- Lane 2 output → quantizer or oscillator FM/1V-oct (lightly attenuated)
- Same gate triggers your voice

### Result
- Short gates may not reach full envelope height
- Longer gates produce larger pitch movement
- This creates **different interval sizes based on note duration**

This is great for:
- human-feeling lead lines
- dynamic ornamentation
- “the same rhythm, but different note behavior”

---

## 3. Repeating mode as melodic LFO source

RADAR’s repeating mode effectively turns lanes into LFOs. The manual notes:
- triggers can reset the waveform
- analog and digital behave differently
- Quad/Oct modes provide phase offsets

### Melodic use
A resettable LFO becomes a **phrase-synchronous CV generator**. If sent through a quantizer, it becomes a melody source.

### Patch idea
- Lane 1 in **Repeating**
- Output → quantizer → oscillator pitch
- Reset lane 1 from a bar clock or phrase trigger
- Adjust rise/fall time and shape for contour

### Result
You get:
- cyclic melodies
- phrase-locked repeating pitch patterns
- evolving scalar motion if speed is modulated

This is one of the strongest “RADAR as melody engine” uses.

---

## 4. Use multiple lanes as note, accent, and timbre layers

RADAR becomes particularly powerful when you stop thinking “one lane = one note envelope” and instead think:

- one lane for **pitch movement**
- one lane for **VCA level**
- one lane for **filter cutoff**
- one lane for **wavefolder/fm index**
- one lane for **accent logic or secondary voice**

### Example voice architecture
For one melodic voice:
- **Lane 1** → VCA envelope
- **Lane 2** → pitch contour
- **Lane 3** → filter envelope
- **Lane 4** → composite max envelope for accent or wavefolder depth

### Why this matters
This makes each note feel composed:
- pitch opens upward
- amplitude swells
- brightness blooms
- accent changes selected notes

That is how melodic parts become **musically legible**, not just CV movement.

---

# Envelope Mode for melodic patching

Envelope Mode is the most straightforward mode for melody building.

## Trigger normalization is very useful
Each trigger input is normalized to the next lane below it. So one trigger stream can cascade through lanes unless interrupted.

### Musical advantage
You can create:
- several related envelopes from one rhythm source
- multiple contours for one voice
- parallel envelopes for multiple voices sharing a pulse structure

### Patch example: one rhythm, several melodic roles
- Trigger into lane 1
- No trigger cables in lanes 2–4, so they inherit the same rhythm
- Lane 1 = amplitude
- Lane 2 = pitch sweep
- Lane 3 = filter motion
- Lane 4 = accent composite

This makes RADAR ideal for **one trigger, one voice, many expressive dimensions**.

---

## Composite outputs as accent/melodic emphasis tools

The manual says:

- **Lane 4 output** can become the max of lanes 3 and 4
- **Lane 8 output** can become the max of lanes 6, 7, and 8

These are not summing outputs; they take the **maximum** instantaneous value.

### Melodic use
This is excellent for:
- accent extraction
- “highest active contour wins” behavior
- deriving a more animated envelope from multiple simpler envelopes

### Patch idea
- Lane 3 = short accent pulse
- Lane 4 = slower contour
- Lane 4 switched to composite output
- Output → filter cutoff or pitch modulation amount

### Result
The contour gains selective emphasis without clipping into a constant maxed signal like a sum might.

For melody this means:
- certain notes brighten more
- selected phrases jump out
- contour complexity increases while staying controlled

---

# Quad Mode for melodic relationships

Quad Mode is one of the most musically rich features in RADAR.

The manual says:
- it can operate as **two quad envelopes**, or **one quad + four regular envelopes**
- the four lanes in a group are **90° apart**
- lane 1 or 5 sets timing for the whole group
- lanes 2/3/4 add CV roles like:
  - **SPEED**
  - **GRAVITY**
  - **SDELTA**
- Quad mode is **digital only**

## Why quadrature matters melodically
Four phase-related CVs are perfect for:
- call-and-response pitch contours
- canon-like melodic offsets
- staggered accents
- rotating voice allocation
- chord arpeggiation from one contour source

---

## 5. Four-note cyclic melodies from quadrature + quantizer

### Patch
- Quad Mode for lanes 1–4
- Outputs 1–4 → precision adder or CV mixer channels → quantizer inputs or switched quantizer destinations
- Or route each lane to four oscillators / four voices

### Result
Because each lane is 90° apart, each voice receives the same contour at a different point in time:
- lane 1 = note 1
- lane 2 = note 2 offset in phase
- lane 3 = note 3
- lane 4 = note 4

This gives:
- rotating arpeggios
- melodic rounds
- interlocking lines

If all lanes drive separate VCAs or LPGs, you get **phase-derived poly-rhythmic melody**.

---

## 6. Gravity as phrase warping

The manual describes **GRAVITY** as changing how the 90/180/270 degree waveforms are attracted or repelled in time relative to the first lane.

### Musical meaning
This is not just simple phase shift — it changes the **temporal relationship** among voices.

### Melodic use
Send the quad outputs through a quantizer and each lane becomes a related but differently warped pitch contour.

This is fantastic for:
- melodies that “lean” toward a central voice
- flams in pitch timing
- chorale-like inner motion
- organic broken chord figures

If lane 1 is the “lead phrase,” the others can become:
- anticipations
- delays
- shadows
- harmonic echoes

---

## 7. SDELTA for interval spread across voices

The manual defines **SDELTA** as shape delta, effectively creating an interpolated shape offset from first to last position.

### Melodic use
If each phase output is quantized:
- differing shapes create different contour trajectories
- those trajectories quantize into different note sequences

So one timing structure can yield:
- lane 1 = smoother scalar contour
- lane 2 = steeper note jumps
- lane 3 = flatter movement
- lane 4 = more dramatic leaps

That is a very strong source of **related but non-identical melodic material**.

---

## 8. Speed modulation for phrase-rate transposition behavior

The SPEED parameter affects rise/fall proportionally across the quad.

### Melodic implication
If a quantizer is sampling these CVs:
- faster cycles = denser note repetition
- slower cycles = broader phrase arcs

If speed is modulated by another slow source, you get:
- phrase acceleration/deceleration
- ratcheting-like melodic compression
- elastic looping melodies

---

# Oct Mode for larger melodic systems

Oct Mode extends the quadrature idea to **8 lanes at 45° spacing**.

This is excellent for:
- long cyclic melodies
- 8-step phase-derived pitch structures
- pseudo-polyphonic counterpoint
- distributing one contour across many events

## 9. Eight related notes from one moving shape

### Patch
- Oct Mode
- Outputs 1–8 into:
  - 8 sample-and-holds triggered sequentially, or
  - an 8-channel switch/scanner, or
  - 8 quantizer channels / polyphonic quantizer
- Each sampled/processed output drives a voice or sequence position

### Result
You derive a full melodic system from one shape engine:
- all notes are related
- all have consistent contour DNA
- phase spacing creates ordered variation

This is superb for:
- generative melody
- marimba/minimalist patterns
- evolving ostinati
- pseudo-sequencer behavior without a traditional sequencer

---

# Digital vs analog modelling in melodic practice

The manual’s distinction here is very important.

## Digital mode
- retriggers reset the envelope to zero
- repeating frequency is constant
- behavior is more sharply defined

### Best melodic role
Use digital when you want:
- precise rhythmic note articulation
- consistent transients
- repeatable phrase shapes
- clock-tight melodic loops

This is ideal for:
- arpeggios
- basslines
- sequenced techno melodies
- clocked patterns

---

## Analog modelling mode
- attacks can begin from the current level
- release behavior feels more capacitor-like
- short gates in AR may not reach full level

### Best melodic role
Use analog modelling when you want:
- legato-feeling pitch movement
- less abrupt resets
- natural contour carryover
- expressive transition between notes

This is ideal for:
- lead lines
- portamento-like contour behavior
- semi-organic generative phrases
- modulated drones with melodic emergence

---

# Practical melodic patch recipes

## Patch 1: Quantized envelope melody
**Goal:** turn RADAR into a melodic contour generator

- Envelope Mode
- Lane 1 in Repeating or AD
- Lane 1 out → attenuverter → quantizer → oscillator 1V/oct
- Trigger/reset from a clock divider
- Lane 2 out → VCA CV
- Lane 3 out → filter cutoff

**Why it works:**  
One contour creates notes, one shapes volume, one shapes brightness. This gives coherent melodic phrasing.

---

## Patch 2: Variable-interval melody from gate length
**Goal:** note duration changes pitch movement

- Lane 1 in AR, analog modelling
- Feed variable-length gates from sequencer
- Lane 1 out → attenuverter → quantizer → pitch
- Same gate to VCA envelope or LPG

**Result:**  
Short notes and long notes generate different melodic intervals naturally.

---

## Patch 3: 4-voice canon melody
**Goal:** one contour, four phase-shifted voices

- Quad Mode on lanes 1–4
- Each output → its own quantizer channel / oscillator
- Common voice architecture for all 4
- Use staggered VCAs or LPGs

**Result:**  
Interlocking melodic lines from one motion source. Great for ambient, minimalism, berlin-school, and rhythmic polyphony.

---

## Patch 4: 8-step generative melody source
**Goal:** use Oct Mode as a contour sequencer

- Oct Mode
- Outputs 1–8 sampled in sequence by a clocked switch or S&H chain
- Quantize the resulting CV
- Use a bar reset for phrase restart

**Result:**  
A coherent but evolving 8-note melodic loop without programming a note sequencer directly.

---

## Patch 5: Accent-driven melodic filter articulation
**Goal:** make melody speak more clearly

- Lane 1 = amplitude envelope
- Lane 2 = pitch contour
- Lane 3 and 4 = different filter envelopes
- Lane 4 switched to max composite mode
- Lane 4 out → filter cutoff or resonance CV

**Result:**  
Some notes “pop” forward depending on which envelope dominates, making the melodic line more expressive.

---

## Patch 6: Repeating lane as arpeggio oscillator
**Goal:** LFO-driven arpeggio

- Lane 1 in repeating mode
- Sync/reset from master clock
- Lane 1 out → quantizer set to chord tones or scale
- Use a trigger sequencer to articulate notes separately via VCA
- Lane 2 slowly modulates shape or speed

**Result:**  
An arpeggio that loops with a recognizable phrase but morphs over time.

---

# Best module pairings for melody

RADAR will be most effective with these kinds of modules:

## Essential partners
- **Quantizer**
  - absolutely key for turning envelopes/LFOs into tuned notes
- **Attenuverters / CV mixers**
  - necessary because RADAR CV often needs scaling and offset
- **Oscillator**
  - destination for melodic pitch
- **VCA / LPG**
  - articulation of notes
- **Trigger/gate sequencer or clock source**
  - controls phrase timing

## Strong advanced partners
- **Sequential switch**
  - scan among RADAR lanes for pseudo-sequencing
- **Sample & hold**
  - freeze envelope stages into discrete note values
- **Logic / comparators**
  - derive triggers when envelopes cross thresholds
- **Precision adder**
  - combine RADAR contour with transposition sequence
- **Matrix mixer**
  - blend several RADAR lanes into composite melodic CV

---

# Most musical strategies with RADAR

## Use RADAR as a contour sequencer, not just an envelope generator
The most productive melodic mindset is:
- envelopes become note shapes
- repeating envelopes become phrase oscillators
- phase offsets become melodic relationships
- max outputs become accent logic

## Quantization unlocks melody
Without quantization, RADAR mostly gives expressive bends and glides. With quantization, it becomes:
- a generative sequencer
- an arpeggiator source
- a counterpoint generator
- a phrase morphing engine

## Pair lanes by function
A strong melodic patch often uses:
- one lane for pitch
- one for articulation
- one for timbre
- one for accent

Rather than trying to get all melody from one lane, RADAR shines when multiple lanes define a single musical line.

---

# Summary

RADAR creates melodic components best by acting as a:

- **quantized pitch contour source**
- **resettable LFO melody generator**
- **phase-related multi-voice melody engine**
- **accent and timbre animator for notes**
- **generative control source for sequencer-like behavior**

Its strongest melodic uses come from:

1. **Envelope Mode** for independent pitch/timbre/articulation contours  
2. **Quad Mode** for 4 related melodic voices or 4-step cyclic motion  
3. **Oct Mode** for larger generative melodic structures  
4. **Analog modelling** for fluid expressive phrases  
5. **Digital mode** for clock-tight melodic precision  

On its own, RADAR is not a melody module in the conventional sense. But in a Eurorack system, it can absolutely become the **core movement source behind melodies, arpeggios, counterpoint, and expressive note phrasing**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)