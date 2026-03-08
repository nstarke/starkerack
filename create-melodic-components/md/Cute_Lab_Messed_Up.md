# Cute Lab — Messed Up

- [Manual PDF](../../manuals/messed-up-manual-rev2.pdf)

---

[Manual PDF](attachment)

# CuteLab Messed Up — using it to create melodic components

Messed Up is **not a pitch generator by itself**. It’s a **clock processor / metric modulation source** that creates related pulse streams: **beat**, **divide**, **downbeat**, **truncate**, and **EoM**. So its role in melodic patching is to become the **timing brain** for sequencers, quantizers, sample-and-holds, shift registers, envelopes, and switches.

If you pair it with melodic modules, it can generate surprisingly rich melodic behavior by controlling **when notes happen**, **when patterns reset**, and **when phrase structure changes**.

---

## What the module contributes musically

From the manual, Messed Up provides:

- **Beat output**: the main pulse stream
- **Divide output**: a mathematically related subdivision/superdivision based on the `divide : beat` ratio
- **Down output**: measure reset / phrase marker
- **Truncate output**: syncopated variation of the divide rhythm
- **EoM output**: trigger when a metric modulation actually occurs

Its central trick is **metric modulation**:

- new tempo = current tempo × `divide / beat`

Example:
- if tempo is 120 BPM
- beat = 4
- divide = 3
- modulation moves to 90 BPM

That means it can transform one rhythmic grid into another while staying structurally related. For melody, that is extremely useful.

---

# Best melodic uses

## 1. Clocking a pitch sequencer with evolving note density

The simplest use:

- Patch **Beat out** to the clock input of a sequencer
- Send sequencer CV to an oscillator through a quantizer
- Use **Down out** to reset the sequencer

This gives you a stable melodic phrase.

Now introduce motion:

- Patch **Divide out** to a second sequencer, or to a switch that occasionally advances the melodic line differently
- Trigger **modulation**
- After modulation, the former subdivision can become the new felt pulse

### Result
Your melody feels like it has **changed gear** without becoming unrelated. This is excellent for:
- transitions
- verse/chorus tempo illusions
- polymetric lead lines
- gradual destabilization of repetitive pitch loops

---

## 2. Creating call-and-response melodies with Beat vs Divide

Because **Beat** and **Divide** are related but different clocks, they work well as two melodic lanes.

### Patch idea
- **Beat out** → clock sequencer A
- **Divide out** → clock sequencer B
- Sequencer A and B both go to different oscillators, or into a precision adder/mixer
- **Down out** resets both

Try settings like:
- beat = 4, divide = 3
- beat = 5, divide = 4
- beat = 3, divide = 2

### Why it works
You get two melodies that:
- share a common phrase structure
- drift against each other
- periodically realign

This is one of the easiest ways to produce:
- canon-like lines
- ostinato + lead relationships
- pseudo-counterpoint in a small rack

---

## 3. Using Downbeat as phrase reset for melodic coherence

The manual emphasizes that the **down output** marks the beginning of the measure defined by `beat`.

That’s incredibly valuable for melody.

### Use Down out to:
- reset a step sequencer
- reset a shift register melody
- fire an accent envelope
- trigger a sequential switch reset
- re-seed a random source at phrase boundaries

### Musical effect
You can let a melody get rhythmically strange between downbeats while the phrase still feels intentional.

For example:
- **Divide** clocks note changes
- **Down** resets the sequence every 4 or 5 beats

This gives:
- polymetric inner activity
- stable phrase start
- easier “hook”-style repetition

---

## 4. Truncate output for syncopated melodic rhythms

The **truncate output** is one of the most interesting parts of the module. It follows the divide rate, but the pattern is cut off and reset within the beat-defined span.

This is excellent for melody because it can drive:
- note triggers for syncopated basslines
- arpeggiator advance inputs
- sample-and-hold clocks
- envelope gates for plucked voices

### Patch idea
- Pitch source: sequencer or quantized random
- **Truncate out** → envelope gate or sequencer clock
- **Beat out** → another layer, such as a bass pulse
- Modulate truncate amount by CV

### Result
Your melodic rhythm gains:
- clipped phrases
- repeated partial cells
- syncopation that still remains locked to the larger structure

This is especially strong for:
- techno stabs
- IDM melodies
- broken arps
- syncopated bass counterlines

---

## 5. EoM output as a melodic event trigger

The **End of Modulation (EoM)** output sends a trigger when the modulation actually happens.

That means it can mark **formal change** in a patch.

### Good uses for EoM
- transpose a sequencer at the exact moment of modulation
- switch to another stored sequence
- open a VCA for a lead voice
- trigger a new random voltage for a melodic section
- change quantizer scale
- advance a song-stage sequencer

### Musical effect
Metric modulation stops being only rhythmic; it becomes a **harmonic or melodic scene change** too.

For instance:
- EoM → sample-and-hold new transposition voltage
- Beat clock continues the sequence
- At each modulation, the melody shifts key center

That gives very performable melodic form.

---

## 6. Round Trip mode for tension and release in melody

In **Round Trip** mode, one modulation moves away from the original tempo, and the next returns.

This is very musical for melody.

### Patch
- Beat clocks main melody
- Divide clocks ornamentation or grace-note sequencer
- Use Round Trip mode
- Trigger modulation manually during transitions

### Result
You can create:
- “stretch away / snap back” phrasing
- melody sections that temporarily re-interpret the pulse
- dramatic fills that resolve exactly back to the original framework

This is especially good live because it behaves like a rhythmic equivalent of harmonic departure and return.

---

## 7. One Way mode for melodic drift and escalation

In **One Way** mode, each modulation is relative to the already modulated tempo.

That means repeated modulations can move the melody progressively farther from the starting groove.

### Melodic applications
- increasingly dense arpeggios
- slowing melodic ostinati
- evolving generative lines
- unstable polyrhythmic canon structures

### Patch idea
- Beat → main sequencer
- Divide → secondary sequence or ratchet trigger
- Repeatedly modulate in One Way mode
- Use Down out to keep occasional phrase resets

This can make a melodic system feel as if it is **spiraling** without becoming random.

---

## 8. Beat/Divide latch for phrase-safe melodic changes

The manual notes that beat and divide changes can be **latched to the next downbeat**.

This matters a lot for melody.

If you change rhythmic ratios while clocking sequencers directly, the resulting melodic phrase can jump awkwardly. Latch avoids that.

### Good performance workflow
- Turn on latch for beat and/or divide
- Queue a new ratio during playback
- Let it take effect on the downbeat

### Musical benefit
- phrase-preserving timing changes
- cleaner pattern transitions
- less accidental derailment of sequencers

This is ideal when driving tonal sequencers that should stay musical during live tweaking.

---

## 9. Internal clock + modulation as a self-contained melodic conductor

Messed Up can run on its **internal clock**, so it can be the master transport for a whole melodic patch.

### Self-contained melodic patch
- Internal clock as master
- Beat → main sequencer clock
- Divide → modulation sequencer or auxiliary melodic trigger
- Down → reset
- Truncate → occasional ornament notes
- EoM → transpose or switch scales

Now the whole melodic patch is governed from one panel:
- BPM
- beat length
- subdivision ratio
- modulation timing
- phrase change events

This makes it a strong composition/performance module even though it doesn’t output pitch CV.

---

# Specific melodic patch recipes

## Patch 1: Metric-modulating bassline

**Goal:** bassline that changes rhythmic identity but stays coherent.

- Beat out → bass sequencer clock
- Down out → bass sequencer reset
- Sequencer CV → quantizer → oscillator
- Envelope from sequencer gate or Beat
- Set beat = 4, divide = 3
- Trigger modulation at phrase end

**What happens:**  
The bassline initially feels quarter-note based; after modulation, the triplet relation becomes the new pulse. Great for modular techno and electro.

---

## Patch 2: Dual melody canon

**Goal:** two melodies from one timing structure.

- Beat out → sequencer A clock
- Divide out → sequencer B clock
- Down out → reset both
- Sequencer A → oscillator 1
- Sequencer B → oscillator 2
- Optionally use same pitch row but different sequence lengths

**What happens:**  
You get melodies that braid together. Changing beat/divide changes the relationship dramatically.

Recommended ratios:
- 3:4
- 4:5
- 5:7

---

## Patch 3: Syncopated arpeggio machine

**Goal:** animated melodic rhythm.

- Pitch CV source: arpeggiator or quantized random voltage
- Truncate out → sample-and-hold clock or envelope trigger
- Beat out → reset arpeggiator every phrase
- Down out → reset switch or sequencer
- Slowly modulate truncate amount

**What happens:**  
The same pitch source is articulated in changing syncopated slices. Feels composed rather than random.

---

## Patch 4: Harmonic scene changes on modulation

**Goal:** make modulation trigger harmonic movement too.

- Beat out → sequencer clock
- Down out → reset
- EoM out → sample-and-hold a transposition voltage
- Transposition voltage → precision adder with sequencer CV
- Quantizer after adder

**What happens:**  
Every actual metric modulation also shifts the key center or melodic register. This is one of the most elegant uses of EoM.

---

## Patch 5: Controlled generative melody

**Goal:** generative line with phrase structure.

- Divide out → clock random CV source / Turing machine / shift register
- Beat out → trigger envelope for notes
- Down out → reset random source or sequencer
- EoM out → change scale or probability setting
- Use One Way mode for evolving timing

**What happens:**  
The note stream mutates, but downbeats keep the melody feeling sectional.

---

# Useful settings for melodic work

## Beat Count / Div Count
These settings change pulses-per-note:
- 1PPN
- 2PPN
- 4PPN
- 8PPN

This is very handy if your melodic sequencer expects faster clocking. You can:
- keep the same phrase logic
- but drive ratcheting, denser arps, or faster note advances

A strong trick:
- Beat Count = 1PPN for main melody
- Div Count = 4PPN for ornament sequencer

---

## Duty Cycle mode
Two pulse modes:
- **1:2** = 50% duty-cycle pulse
- **0.01** = fixed 10 ms trigger

For melodic modules:
- use **0.01** when clocking sequencers or trigger inputs that prefer short pulses
- use **1:2** when driving gear that wants more gate-like behavior

This can matter a lot when envelopes or sequencers double-trigger unexpectedly.

---

## Beat Input Reset mode
The beat CV input can become a **reset input**.

That means an external sequencer or master phrase trigger can force Messed Up back to the top of its measure.

For melodic systems, this is excellent if you want:
- one master sequencer controlling all phrase starts
- Messed Up still generating complex internal subdivisions
- hard synchronization between melody and clock modulation structure

---

## Modulation Style
The manual lists three styles:

- **SynC**: after modulation, beat count adjusts to equal divisions
- **StAY**: beats/divisions do not change after modulation
- **FLIP**: beats and divisions swap after modulation

These are extremely important musically.

### SynC
Best when you want the whole patch to feel like it has cleanly landed in the new tempo.  
Good for:
- melodic sections
- obvious transitions
- “now this is the new pulse”

### StAY
Best when you want the exact same pattern relationships to remain, but the whole module perceptually speeds up or slows down.  
Good for:
- generative melodic systems
- gradual surreal tempo migration

### FLIP
Best for dramatic melodic reinterpretation.  
Good for:
- swapping foreground and background rhythms
- making accompaniment become lead timing
- mirrored call/response behavior

For melodic patching, **FLIP** is particularly inspiring when Beat and Divide clock two different voices.

---

# Performance ideas

## 1. Phrase-aware live modulation
- Use latch-to-downbeat
- Queue modulation before the end of a bar
- Send EoM to transpose your melody

This creates very “composed” live changes.

## 2. Manual polyrhythm scanning
- Leave melody patch constant
- Only change beat/divide
- Keep latches on

The same notes will feel different because the attack timing changes.

## 3. Truncate as ornament generator
- Main sequencer on Beat
- Ornament voice on Truncate
- Shared pitch source, different octave

This can produce beautiful melodic decoration from a single sequence.

---

# Limitations to understand

Messed Up does **not** directly generate:
- pitch CV
- scales
- quantized melodies
- note order

So by itself it won’t make melody. It makes **melody timing architecture**.

Think of it as controlling:
- note onset
- phrase boundary
- rhythmic reinterpretation
- formal transitions

If you combine it with:
- a pitch sequencer
- quantizer
- random voltage
- precision adder
- switch
- envelope/VCA voice

then it becomes a very powerful melodic composition tool.

---

# Best companion module types

To create melodic components, pair Messed Up with:

- **Step sequencers** — for note order
- **Quantizers** — for tonal control
- **Sample & hold / random CV** — for generative melody
- **Sequential switches** — for phrase variation
- **Precision adders** — for transposition
- **Logic modules** — to combine Beat/Divide/Truncate into more melodic trigger patterns
- **Clocked switches / burst modules** — for ornamentation
- **Envelope generators + VCAs** — to turn pulse structures into articulated notes

---

# Bottom line

CuteLab **Messed Up** is best understood as a **melodic timing composer** rather than a melody source.

It excels at:

- clocking melodic sequencers with polyrhythmic structure
- resetting phrases with downbeats
- creating syncopated note triggers with truncate
- marking formal changes with EoM
- transforming the perceived pulse through metric modulation
- producing live-playable tension/release with Round Trip mode
- pushing melodies into evolving temporal space with One Way mode

If you already have modules that generate pitch, Messed Up can make them feel much more musical, structural, and performable.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)