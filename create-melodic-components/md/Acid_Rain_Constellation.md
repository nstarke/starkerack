# Acid Rain — Constellation

- [Manual PDF](../../manuals/Constellation_Manual_Firmware_1.1_4.7.2025.pdf)

---

[Constellation Firmware V1.1 Manual (PDF)](https://acidraintechnology.com/support)

# Using Acid Rain Constellation to Create Melodic Components

Constellation is not a pitch sequencer in the traditional sense, but as a eurorack musician I’d absolutely use it as a **melodic rhythm engine**. Its real strength is generating highly structured trigger/gate relationships that can drive pitch, articulation, transposition, variation, and phrase switching across other melodic modules.

## What Constellation contributes musically

From the manual, Constellation gives you:

- **8 trigger/gate channels**
- **8 Euclidean patterns per channel**
- Per-pattern:
  - divide
  - length
  - events
  - rotate
  - burst
  - ratchet
  - chance
- Per-channel:
  - logic combining patterns: **AND / OR / XOR**
  - **width**
  - **flop**
- Per-channel clock scaling for **true polyrhythms**
- CV control over many pattern parameters
- Save/load/live performance switching

That means Constellation is ideal for generating the **time structure** behind melody, even if another module supplies the actual voltages for pitch.

---

# Best melodic use cases

## 1. Drive a CV sequencer with better rhythm than the sequencer alone

The most obvious melodic patch:

- Constellation channel output -> **clock input** of a pitch sequencer
- Pitch sequencer CV out -> oscillator 1V/oct
- Pitch sequencer gate out or Constellation gate -> envelope -> VCA/filter

### Why this works
Most pitch sequencers become much more musical when their advance clock is not just straight 16ths. Constellation can create:

- uneven phrase lengths
- fills via burst
- ornamental repeats via ratchet
- probabilistic note omissions via chance
- polyrhythmic note movement with channel clock scaling

### Musical result
A basic 8-step pitch sequence suddenly behaves like:

- syncopated bassline
- evolving arpeggio
- generative pluck line
- shifting ostinato

### Good strategies
- Use one channel as the **main note advance**
- Use another as **accent or envelope retrigger**
- Use a third to **transpose** another sequencer or switch quantizer input
- Keep pitch sequence simple; let Constellation create the phrasing complexity

---

## 2. Separate pitch rhythm from articulation rhythm

This is one of the best ways to get expressive melody.

Patch like this:

- **Channel 1** -> advance a pitch sequencer
- **Channel 2** -> trigger envelope/VCA
- Sequencer CV -> quantizer -> oscillator pitch
- Envelope -> VCA controlling oscillator

Now pitch changes and audible notes are no longer identical events.

### What this gives you
- some pitch steps happen silently
- some notes repeat without changing pitch
- some new pitches sustain across multiple articulations
- some notes become staccato while others become legato

### How to shape it
- Use **narrow width** for short articulated notes
- Use **high width** for longer gate-like phrasing
- Use **flop** on a channel to create alternating gate states and longer held phrases
- Use **chance** on articulation separately from pitch advancement

This is one of the easiest paths from “sequenced notes” to “actual melody.”

---

## 3. Use channels as phrase layers for one melodic voice

Each Constellation channel combines up to 8 patterns. That makes each output more like a compositional layer than just a trigger stream.

For one melodic voice, you can assign:

- **Channel 1** = main melody trigger
- **Channel 2** = octave jumps / transposition trigger
- **Channel 3** = ornament trigger
- **Channel 4** = phrase reset or sequence direction change
- **Channel 5** = envelope accent
- **Channel 6** = filter envelope trigger
- **Channel 7** = sample & hold for pitch variation
- **Channel 8** = save-slot performance switching or mutes

### Why this is powerful
You can build a complete melodic ecosystem where:
- one rhythm determines when the melody advances
- another determines when it speaks
- another changes register
- another introduces random movement
- another switches to a different phrase

That’s much more musical than using a single gate source everywhere.

---

# Melodic patch ideas

## A. Euclidean bassline generator

### Patch
- Channel 1 -> clock input of pitch sequencer
- Sequencer CV -> quantizer -> oscillator
- Channel 1 or 2 -> envelope -> VCA
- Channel 3 -> filter envelope trigger
- Channel 4 -> reset input of sequencer every longer phrase

### Constellation setup
- Channel 1:
  - OR logic
  - pattern 1: length 8, events 3
  - pattern 2: length 5, events 1
  - pattern 3: chance around 70%
- Channel 2:
  - lower density articulation pulses
- Channel 4:
  - longer cycle, maybe length 15 or 16, sparse events

### Result
A bassline with recurring structure but enough asymmetry to feel written rather than looped.

---

## B. Generative lead melody with quantized sample-and-hold

If you don’t have a pitch sequencer, Constellation can still help generate melody indirectly.

### Patch
- Noise or slow CV source -> sample & hold input
- Constellation Channel 1 -> sample & hold trigger
- Sample & hold output -> quantizer -> oscillator 1V/oct
- Channel 2 -> envelope trigger
- Channel 3 -> second envelope or accent
- Optional: Channel 4 -> transpose quantizer root or switch scales

### Why it works
Constellation determines **when new pitches are sampled**, which is effectively melodic phrasing. Because the rhythm is structured and not random-clutter, the sampled melody feels intentional.

### Tips
- Use sparse Euclidean patterns for melody triggers
- Add ratchets sparingly for trills and grace-note-like clusters
- Use chance to occasionally skip new pitch sampling so notes repeat

---

## C. Arpeggiator with irregular gate architecture

### Patch
- Arpeggiator or sequential voltage source -> oscillator pitch
- Constellation Channel 1 -> arp clock
- Channel 2 -> envelope trigger
- Channel 3 -> switch arpeggiator mode / reset / octave shift

### Constellation advantage
Instead of a static up/down arp, you get:
- asymmetrical note timing
- recurring phrase variation
- occasional burst clusters
- phrase-length drift via different pattern lengths and channel clock ratios

This is especially strong for techno, ambient, and Berlin-school style sequences.

---

## D. Counterpoint from multiple melodic voices

Because there are 8 channels, Constellation can drive multiple melodic systems at once.

### Example
- Channel 1 -> bass sequencer clock
- Channel 2 -> lead sequencer clock
- Channel 3 -> pluck voice envelope
- Channel 4 -> chord voice re-articulation
- Channel 5 -> sequence reset
- Channel 6 -> transposition trigger
- Channel 7 -> melodic mute logic
- Channel 8 -> phrase switch/load control

### Why this matters
Per-channel clock multiplication/division means each melodic voice can exist in a different rhythmic grid.

For example:
- bass on straight quarter/8th-note logic
- lead in triplet-derived movement
- pluck voice on a longer polymetric cycle

That creates the illusion that the melodic lines are independently composed.

---

# Features especially useful for melody

## 1. Channel clock scaling = melodic polyrhythm
The manual explains each channel can run at its own multiplier/divider relative to the main clock.

This is huge for melody because you can make:
- one voice move in straight time
- another voice move in triplets
- another move more slowly as a phrase voice

### Musical use
- Bass: channel scaler 1/1
- Lead: channel scaler 3/2
- Harmony stabs: channel scaler 1/4

This creates layered melodic interplay without needing multiple clock processors.

---

## 2. Pattern divide = phrase spacing
Pattern divide slows individual patterns relative to the channel clock.

For melody this is great for:
- accents that only happen every few notes
- octave changes that recur over long cycles
- occasional phrase resets
- cadential events

Think of divide as a tool for large-scale melodic architecture.

---

## 3. Burst = repeated notes or ornaments
Burst repeats events on subsequent clocks.

Melodically, this can become:
- repeated notes
- stuttered pitch advance
- decorative figures
- rhythmic insistence before a phrase turn

If burst clocks a sequencer, you may get repeated step advances or repeated gate clusters depending on the destination.

If burst triggers articulation while pitch holds, it creates repeated-note ornaments.

---

## 4. Ratchet = trills, rolls, fast embellishment
Ratchet repeats events between clock edges.

This is fantastic for:
- lead flourishes
- fast reiterations
- pseudo-trills
- note pressure/intensity effects if patched to envelopes

A good melodic trick:
- Channel 1 advances pitch normally
- Channel 2 ratchets the envelope only
- Result: one pitch with rapid repeated articulation

That sounds much more intentional than ratcheting the whole sequencer.

---

## 5. Chance = selective melodic variation
Chance applies probability to pattern events.

For melodic work, this is best used to control:
- occasional note skips
- rare accents
- phrase fills
- occasional transposition events
- non-repeating articulation

A powerful move is using chance not on the main melody clock, but on a **secondary modulation function**:
- transposition trigger
- accent trigger
- filter articulation
- note repeat layer

That keeps the melody intelligible while adding life.

---

## 6. Logic modes = compositional filtering
The logic section is easy to overlook, but for melodic patches it’s one of the most compositional features.

### OR
Best for:
- dense composite trigger streams
- melodic activity
- lively advancing sequences

### AND
Best for:
- rare, significant melodic events
- phrase boundaries
- transposition moments
- accent conditions

Use AND when you want something to happen only when multiple cycles align.

### XOR
Best for:
- syncopated alternation
- unstable lead rhythms
- call-and-response style trigger behavior

XOR is especially interesting for melodic articulation because it removes overlaps and emphasizes contrast.

---

## 7. Width = note length shaping
Width controls pulse width per channel.

For melody:
- low width = plucky, percussive, articulated
- high width = connected, legato-ish, gate-like
- very high width can blend events into held gates

This can dramatically affect perceived melodic style even when pitch content stays the same.

---

## 8. Flop = phrase-level gate toggling
Flop turns combined pulses into alternating high/low gate states.

Melodically, this is useful for:
- opening/closing sustained drones
- alternating between held and silent states
- creating slow phrase masks over faster rhythmic events
- turning rhythmic event streams into structure gates for sequential switches or VCAs

One great use:
- Use a normal channel for note triggers
- Use a flop-enabled channel to open a VCA or sequential switch only during alternating phrase blocks

Now the same melody appears in sections, like arranged composition.

---

# CV modulation for evolving melody

Constellation’s CV inputs can modulate many pattern parameters, sampled on the channel clock.

This is excellent for slow melodic evolution.

## Best parameters to modulate for melody

### Length
Changes phrase size over time.  
Great for evolving ostinati.

### Events
Changes density.  
Excellent for moving between sparse and busy phrases.

### Rotate
Shifts accents and note placement without destroying the basic pattern.

### Chance
Lets a melody become more or less assertive over time.

### Width
Changes articulation from tight to legato.

### Mute
Can drop whole melodic functions in and out.

### Load
The manual notes CV can momentarily load a save slot. This is huge.

You can use a gate source to:
- switch between melodic scenes
- alternate verse/chorus-like phrase sets
- momentarily recall fills
- create call-and-response between saved pattern states

That turns Constellation into a performance-arrangement brain for melody.

---

# Advanced melodic strategies

## 1. Use save slots as harmonic scenes
Even though Constellation doesn’t store pitch directly, save slots can store totally different rhythmic structures for melodic control.

Create slots like:
- Slot 1 = verse rhythm
- Slot 2 = chorus rhythm
- Slot 3 = break / sparse
- Slot 4 = fill / ratchets
- Slot 5 = long-note ambient mode

Then use:
- live mode
- manual loading
- CV load assignment

to “perform” the melody structure.

If your external sequencer keeps the same pitch material while Constellation changes timing, the musical result feels like arrangement-level composition.

---

## 2. Drive transposition events
A very musical trick is to dedicate one channel to transposition rather than note generation.

### Patch
- Base pitch sequencer -> quantizer transpose-capable input or precision adder
- Constellation channel -> trigger sample-and-hold, sequential switch, or transpose gate

Uses:
- occasional octave jumps
- switching between root notes
- enabling alternate quantizer offsets
- chord tone shifts

Because Constellation can create long, sparse, logic-derived events, transposition changes can happen at meaningful phrase points rather than every bar.

---

## 3. Create melody from logic intersections
Use logic modes to distinguish:
- normal notes
- emphasized notes
- rare phrase markers

For example:
- Channel 1 OR logic -> main note stream
- Channel 2 AND logic -> only when multiple patterns align, trigger octave accent
- Channel 3 XOR logic -> trigger alternate timbre or second oscillator

Now the melody has internal hierarchy:
- common notes
- accented notes
- special notes

That’s a very compositional way to patch.

---

## 4. Build call-and-response with two sequencers
### Patch
- Channel 1 -> sequencer A clock
- Channel 2 -> sequencer B clock
- Channel 3 flop gate -> switch/VCA enabling one voice at a time
- Both sequencers to different oscillators or timbres

### Result
Two melodic identities can alternate, overlap, or answer each other.

Constellation’s long polymetric cycles make this feel organic rather than repetitive.

---

# Practical patch templates

## Template 1: Melodic techno line
- Ch1 -> main sequencer advance
- Ch2 -> amp envelope trigger
- Ch3 -> filter accent trigger
- Ch4 -> occasional reset
- Ch5 -> transpose event
- Ch6 -> ratcheted ornament trigger

Use:
- OR on Ch1
- chance on Ch5
- ratchet on Ch6
- width medium on Ch2
- long cycle lengths on Ch4 and Ch5

Result: driving but evolving melodic pattern.

---

## Template 2: Ambient generative melody
- Ch1 -> sample & hold trigger
- S&H -> quantizer -> oscillator
- Ch2 -> VCA envelope
- Ch3 -> LPG ping
- Ch4 -> reverb duck/envelope
- Ch5 flop -> drone gate
- Slow LFO into CV input modulating length or rotate

Use:
- sparse Euclidean events
- long lengths
- low event counts
- moderate chance
- slow channel clocks

Result: drifting melodic fragments with recurring structure.

---

## Template 3: Polyrhythmic dual melody
- Ch1 -> bass sequencer clock
- Ch2 -> lead sequencer clock
- Ch3 -> bass articulation
- Ch4 -> lead articulation
- Ch5 -> bass transposition
- Ch6 -> lead ornament
- Different channel clock scalers for bass and lead

Result: interlocking melodic voices sharing one master rhythm source but living in different metric worlds.

---

# What Constellation is best paired with

To make actual melody, Constellation pairs especially well with:

- **pitch sequencers**
- **quantizers**
- **sample & hold modules**
- **precision adders**
- **sequential switches**
- **switchable voltage memories**
- **envelopes / LPGs / VCAs**
- **clockable arpeggiators**
- **logic-addressed or gate-addressed switch modules**

In other words: Constellation excels when another module handles **what pitch**, while it handles **when, how often, how long, and under what condition**.

---

# Bottom line

Constellation is best understood as a **melodic structure generator**, not just a drum trigger source.

It can create melodic components by controlling:

- **note timing**
- **articulation**
- **repetition**
- **ornamentation**
- **phrase length**
- **transposition events**
- **voice alternation**
- **scene switching**

If you pair it with a quantizer, pitch sequencer, sample & hold, or switch-based pitch system, it becomes an extremely powerful tool for writing melodies that feel alive, polyrhythmic, and performable.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)