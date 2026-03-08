# Moog — Subharmonicon

- [Manual PDF](../../manuals/Subharmonicon_Manual.pdf)

---

[Moog Subharmonicon Manual (PDF)](https://api.moogmusic.com/sites/default/files/2020-09/Subharmonicon_Manual.pdf)

# Using These Modules Together to Create Melodic Components

Based on the manual you provided, the primary module/instrument here is the **Moog Subharmonicon**, with explicit integration examples for:

- **Subharmonicon**
- **DFAM**
- **Mother-32**

From a Eurorack musician’s perspective, these three make an excellent melodic ecosystem, with **Subharmonicon as the harmonic/polyrhythmic brain**, **Mother-32 as a clocked melodic voice or utility sequencer**, and **DFAM as a rhythmic companion that can also become a pitched melodic/percussive layer**.

---

## 1. What each module contributes musically

## Subharmonicon
Subharmonicon is the main melodic generator here.

It gives you:

- **2 VCOs**
- **4 subharmonic oscillators** total
- **2 independent 4-step sequencers**
- **4 rhythm generators**
- quantization in:
  - **12-ET**
  - **8-ET**
  - **12-JI**
  - **8-JI**
- patch outputs for:
  - **SEQ 1 / SEQ 2 CV**
  - **SEQ 1 CLK / SEQ 2 CLK**
  - **CLOCK**
  - oscillator audio outs
  - envelopes

This means it can generate:

- basslines
- counterpoint
- drones
- chord-like structures
- pseudo-arpeggios
- polymetric melodic motion
- just-intonation harmonic clusters

The big conceptual strength is that **pitch and rhythm are both integer-derived**:
- subharmonics are pitch divisions of the main oscillator
- rhythm generators are tempo divisions of the master clock

That makes it naturally good at **coherent, interlocked melodic structures**.

---

## Mother-32
From the manual’s sync example, Mother-32 is used mainly as:

- an external **master clock**
- a second synchronized sequenced system

In practice, alongside Subharmonicon, Mother-32 can serve as:

- a **lead voice**
- a **bass voice**
- a **transposing CV source**
- a **clock source/divider relationship partner**
- a way to add a more traditional single-line sequence against Subharmonicon’s harmonic motion

Musically, Mother-32 is ideal for giving you a **clear, conventional melodic line** while Subharmonicon supplies moving harmony and polyrhythmic phrasing.

---

## DFAM
The manual frames DFAM as a clock follower, but as Eurorack players know, DFAM is not just drums.

Used with Subharmonicon, DFAM can become:

- tuned percussion
- repeating ostinato
- bass accent voice
- rhythmic melody voice
- clocked textural pitch layer

Because Subharmonicon can send:
- **CLOCK OUT**
- **TRIGGER OUT**
- **SEQ 1 CLK**
- **SEQ 2 CLK**

to DFAM’s **ADV/CLOCK**, you can make DFAM participate in:
- straight pulse rhythm
- sequencer-specific pulse patterns
- polyrhythmic phrase structures

That means DFAM can reinforce melody not only as percussion, but as **a rhythmically displaced tonal line**.

---

# 2. Best overall melodic strategy

The most useful way to think about these together is:

- **Subharmonicon = harmonic/polyrhythmic composition engine**
- **Mother-32 = stable melodic narrator**
- **DFAM = rhythmic pitch accent / percussive melody**

This creates three melodic roles:

1. **Foundational harmony**  
   Subharmonicon’s VCOs + subharmonics establish chordal or modal space

2. **Primary melody**  
   Mother-32 provides a more readable line on top

3. **Rhythmic melodic punctuation**  
   DFAM locks to subdivisions or sequencer clocks for tuned rhythmic motifs

---

# 3. How Subharmonicon generates melody

## A. Two sequencers controlling two pitch centers
Subharmonicon has:
- **Sequencer 1** tied internally to VCO 1 and its subs
- **Sequencer 2** tied internally to VCO 2 and its subs

Each sequencer has 4 steps, but because of the rhythm generator assignments, those steps don’t have to advance uniformly.

This is where the melodic magic comes from.

You can make:

- Sequencer 1 advance at one rhythmic division
- Sequencer 2 advance at another
- one or both driven by multiple rhythm generators

Result: a simple 4-step pitch pattern becomes a **long-form evolving melody**.

### Practical melodic use
- Put **Sequencer 1** on a root/fifth pattern
- Put **Sequencer 2** on a third/sixth/upper extension pattern
- Mix VCOs and subs to form intervals and moving harmony

This gives you a compact system for:
- modal riffs
- rotating chord tones
- bass + upper voice interplay

---

## B. Sequencer assign buttons are the key to melodic complexity
Each sequencer can affect:

- the main VCO pitch
- SUB 1 integer
- SUB 2 integer

So melody is not limited to “notes.” You can sequence:

- fundamental pitch only
- subharmonic interval only
- or both simultaneously

### Why this matters
If you sequence only the VCO, the subs retain their interval relationship.

If you sequence the subs too, then each step can reconfigure the harmonic content itself.

That lets you create:

- moving dyads
- shifting chord voicings
- pseudo-inversions
- step-by-step harmonic modulation

This is one of the most unique melodic features in the whole system.

---

## C. Quantization makes it practical
Subharmonicon supports:

- **12-ET** chromatic equal temperament
- **8-ET** diatonic equal temperament
- **12-JI** chromatic just intonation
- **8-JI** diatonic just intonation
- or no quantization

### Best melodic use cases
- **12-ET**: standard melodic integration with other synths
- **8-ET**: modal or scale-limited melodies
- **12-JI / 8-JI**: pure interval drones, harmonic studies, ancient/choral feel
- **Unquantized**: gliding experimental tuning, microtonal tension

If you want Subharmonicon to work tightly with **Mother-32**, use **12-ET** first.

If you want Subharmonicon to generate the harmonic world and let Mother-32 float above it, try **8-JI** or **12-JI**.

---

# 4. How to combine Subharmonicon and Mother-32 melodically

The manual specifically shows **Mother-32 clocking Subharmonicon** by patching:

- **Mother-32 ASSIGN OUT -> Subharmonicon CLOCK IN**

This means Mother-32 can define global timing.

## Why this is musically useful
Mother-32’s sequence can act like the “song grid,” while Subharmonicon creates layered melodic events inside that grid.

### Good melodic arrangement
- Mother-32 plays a clear 8-step or 16-step melodic motif
- Subharmonicon runs two 4-step polyrhythmic harmonic sequences under it
- Reset Subharmonicon at phrase boundaries for structured repetition

This gives the music:
- a recognizable lead line
- evolving harmony underneath
- predictable song phrasing despite internal complexity

---

## Use case 1: Mother-32 lead, Subharmonicon harmony
**Patch/sync concept**
- Mother-32 clocks Subharmonicon
- Subharmonicon in **8-ET** or **12-ET**
- Sequencer 1 = low register root movement
- Sequencer 2 = upper chord tone movement
- Mother-32 = top-line melody

**Result**
- Mother-32 behaves like the singer
- Subharmonicon behaves like backing harmonic instruments

This is probably the most immediate “musical song” use.

---

## Use case 2: Subharmonicon transposed feel, Mother-32 fixed pattern
Even without a dedicated transpose workflow described in the manual, you can create the *effect* of transposed interaction by:

- keeping Mother-32 on a repetitive motif
- changing Subharmonicon’s VCO frequencies or step values live
- using RESET to realign phases

This produces:
- static melody against moving harmony
- sequence reharmonization
- minimalist phasing composition

---

## Use case 3: Mother-32 as rhythmic authority, Subharmonicon as polymetric melody engine
Since Subharmonicon’s rhythm generators divide a shared tempo, externally clocking it from Mother-32 makes the whole patch breathe together.

Try:
- Mother-32 steady clock
- Subharmonicon Rhythm 1 and 2 on Sequencer 1
- Rhythm 3 and 4 on Sequencer 2
- different divisions on each

Now both voices remain song-synced, but melodic accents feel alive and irregular.

This is excellent for:
- Berlin-school lines
- generative techno melodies
- cyclical ambient counterpoint

---

# 5. How to combine Subharmonicon and DFAM melodically

The manual shows:

- **Subharmonicon CLOCK OUT -> DFAM ADV/CLOCK IN**

It also suggests alternatives:
- **TRIGGER OUT -> DFAM ADV/CLOCK**
- **SEQ 1 CLK -> DFAM ADV/CLOCK**
- **SEQ 2 CLK -> DFAM ADV/CLOCK**

This is where melodic interaction gets really interesting.

## A. Straight clocked tuned DFAM
If you tune DFAM’s oscillators melodically and feed it the main Subharmonicon clock:

- DFAM advances at the global pulse
- Subharmonicon provides harmonic background
- DFAM gives a repeating tonal ostinato

This works well when:
- Subharmonicon is lush and slow
- DFAM is short-decay and punchy

DFAM becomes a kind of plucked bass or tuned percussion line.

---

## B. Sequencer-clocked DFAM for polyrhythmic melody
Better yet, patch:

- **SEQ 1 CLK OUT -> DFAM ADV/CLOCK**
or
- **SEQ 2 CLK OUT -> DFAM ADV/CLOCK**

Now DFAM advances only when that sequencer advances.

Since Subharmonicon sequencer clocks are already rhythm-generator-derived, DFAM inherits the polyrhythm.

### Musical result
DFAM no longer feels like “drums under a synth.”  
It becomes a **third melodic phrase**, rhythmically subordinate to one Subharmonicon lane.

This is excellent for:
- call and response
- bass reinforcement
- rhythmic canon
- melodic percussion

---

## C. Trigger-based DFAM accents
Patch:
- **Subharmonicon TRIGGER OUT -> DFAM ADV/CLOCK**

Because the trigger out reflects envelope triggering, DFAM can follow phrase articulation rather than raw clock.

This is good if you want DFAM to emphasize:
- note attacks
- phrase starts
- envelope activity

This yields a more performance-sensitive melodic rhythm.

---

# 6. Internal Subharmonicon patching for melody

Subharmonicon’s patchbay is not just for sync. It can re-route pitch and rhythm internally to create much richer melodic behavior.

---

## A. Use SEQ 1 to control VCO 2
The manual explicitly gives this example:

- **SEQ 1 OUT -> VCO 2 IN**

This lets Sequencer 1 control VCO 2 pitch.

### Musical implications
Now you can have:

- Sequencer 1 driving both voices
- Sequencer 2 disengaged or used separately
- parallel motion between oscillators
- offset melodic doubling

Great for:
- harmonized leads
- octave doubling
- fourth/fifth motion
- canon-like melodic movement

If VCO 2 is tuned to an interval from VCO 1 before patching, the result is a harmonized melody voice.

---

## B. Sequence subharmonics independently
Patching and assign buttons let you think of subharmonics as melodic voices rather than static support.

Try:
- Sequencer 1 assigned to **SUB 1** but not OSC 1
- Sequencer 2 assigned to **SUB 2** but not OSC 2

Now the fundamentals stay stable while the undertones move.

### Result
You get:
- drone root
- moving inner voices
- evolving chord color

This is extremely effective for ambient, folk-modal, and soundtrack composition.

---

## C. Use SEQ outputs elsewhere in the rack
The patchbay provides:
- **SEQ 1 OUT**
- **SEQ 2 OUT**

These output pitch CV from the current sequencer steps.

So if you add more Eurorack voices, Subharmonicon can sequence them too.

Even with just the systems mentioned:
- use Subharmonicon CV conceptually as the melodic master
- let Mother-32 or other oscillator-based voices track those sequences if compatible in your setup

This means Subharmonicon can be the **central composition module**, not just a sound source.

---

## D. Use rhythm CV inputs for evolving melodic phrasing
Subharmonicon has CV inputs for:
- RHYTHM 1
- RHYTHM 2
- RHYTHM 3
- RHYTHM 4

These control the integer division selection.

If you modulate them, your sequence timing changes dynamically.

### Melodic use
This is not pitch CV, but it directly shapes melodic identity by changing:
- note density
- accent placement
- phrase length
- repeat cycle

If another module in the rack can output slow CV, you can morph static sequences into evolving melodic structures.

---

# 7. Best melodic roles for each output on Subharmonicon

## SEQ 1 OUT / SEQ 2 OUT
Use for:
- sequencing external oscillators
- doubling melodic lines
- layered harmony
- sending Subharmonicon’s pitch structure elsewhere

## SEQ 1 CLK / SEQ 2 CLK
Use for:
- clocking DFAM differently for melody accents
- advancing other sequencers in the rack
- creating phrase-linked rhythmic melody

## CLOCK OUT
Use for:
- making all melodic modules share pulse
- keeping arpeggios and basslines aligned

## TRIGGER OUT
Use for:
- phrase accents
- triggering percussive melodic voices
- articulation-linked movement

## VCF EG / VCA EG outputs
These are not pitch outputs, but can be used creatively for melodic phrasing if routed to other CV destinations in a larger system:
- filter animation
- amplitude contouring
- dynamic phrase shaping

---

# 8. Strong melodic patch ideas

## Patch 1: Harmonic bed + lead + tuned percussion
**Goal:** full melodic arrangement

- Mother-32 clocks Subharmonicon
- Subharmonicon:
  - Sequencer 1 = bass/root movement
  - Sequencer 2 = chord/upper interval movement
  - Quantize = 12-ET
- DFAM clocked from **SEQ 2 CLK**
- DFAM tuned as short-decay percussive pitch line

**Musical result:**
- Mother-32 = lead melody
- Subharmonicon = harmonic accompaniment
- DFAM = syncopated melodic percussion

This is probably the most complete trio use.

---

## Patch 2: Just-intonation drone choir
**Goal:** lush melodic harmony

- Subharmonicon quantize = **8-JI** or **12-JI**
- VCOs tuned to consonant interval
- subs mixed prominently
- Sequencers move subharmonics more than fundamentals
- Mother-32 adds sparse top notes
- DFAM omitted or used minimally

**Result:**
- moving overtone/undertone harmony
- very pure interval relationships
- slow melodic evolution

Excellent for ambient and experimental tonal music.

---

## Patch 3: Bassline machine
**Goal:** strong low-end melody

- Subharmonicon Sequencer 1 on VCO 1 + subs
- low rhythm divisions on Seq 1
- DFAM clocked from **TRIGGER OUT** or **SEQ 1 CLK**
- DFAM tuned to reinforce the same root or fifth
- Mother-32 plays higher counterline

**Result:**
- Subharmonicon = complex bass harmony
- DFAM = punchy bass punctuation
- Mother-32 = agile upper melody

Very effective for techno, electro, and soundtrack pulses.

---

## Patch 4: One-sequence multi-voice harmony
**Goal:** parallel melodic motion

- Patch **SEQ 1 OUT -> VCO 2 IN**
- Tune VCO 1 and VCO 2 to different starting intervals
- Use Sequencer 1 as main pitch contour
- Assign Sequencer 2 only to subs or leave it unused
- Clock from one or two rhythm generators

**Result:**
- both VCOs track a related melodic shape
- subs provide extra harmony
- one compact sequence turns into a harmonized melodic stack

This is a great way to make Subharmonicon behave more like a compact polyphonic composition tool.

---

# 9. The most important musical strengths of this system

## A. Melodies can be harmonic, not just monophonic
Subharmonicon is especially good at making melody feel like harmony in motion.

Instead of one note at a time, you get:
- note + undertones
- two sequenced pitch centers
- interval shifts by step

So melodic writing becomes **voice-leading** rather than simple sequencing.

---

## B. Rhythm and melody are inseparable
Because rhythm generators determine step advancement, melodic identity depends heavily on clock division.

A 4-step sequence can feel like:
- a bass riff
- an arpeggio
- a rotating harmonic cell
- a generative phrase

just by changing rhythm assignments.

---

## C. You can create long evolving phrases from tiny materials
Two 4-step sequencers sounds limited on paper.

But once you add:
- four rhythm generators
- separate assignments
- two oscillators
- four subharmonic oscillators
- resets during performance

you get surprisingly long melodic cycles.

That makes the system perfect for:
- minimalist composition
- generative patches
- evolving accompaniment
- live performance variation

---

# 10. Practical advice for making it sound musical fast

## Start in 12-ET
If combining with Mother-32 or external gear, begin with **12-ET** for predictable pitch behavior.

## Use one sequencer for roots, one for color
A very reliable approach is:
- **Seq 1** = root/bass motion
- **Seq 2** = harmonic color or higher-register motion

## Don’t overuse all subs at once
All six sound sources can get dense fast. For melody, clarity often improves if:
- one main VCO is dominant
- one or two subs are supporting
- the others are introduced selectively

## Use RESET musically
RESET is not just technical. It is a phrase tool.
Use it:
- at bar starts
- to restart evolving patterns
- to bring harmony back into focus

## Use sequencer clocks as composition tools
Instead of only using main clock out, use:
- **SEQ 1 CLK** for one melodic follower
- **SEQ 2 CLK** for another

This creates structured interdependence across modules.

---

# 11. Bottom line

If your goal is to create **melodic components for music**, these modules work together best like this:

- **Subharmonicon** creates the harmonic and polymetric core
- **Mother-32** adds a stable, readable melodic line and/or master timing
- **DFAM** becomes a clocked rhythmic pitch accent or tuned percussive melody

The strongest musical workflows are:

1. **Subharmonicon as harmonic engine, Mother-32 as lead**
2. **Subharmonicon clocking or phrase-driving DFAM for tuned rhythmic motifs**
3. **Using Subharmonicon’s sequencer CV and sequencer clocks to spread one melodic idea across multiple voices**
4. **Using just intonation and subharmonic sequencing for rich, evolving interval-based music**

In short, this setup excels at:
- basslines
- drones
- harmonic ostinati
- melodic counterpoint
- polyrhythmic motifs
- evolving tonal texture

It is less about conventional keyboard-style melody writing and more about **composed interlocking melodic ecosystems**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)