# Doepfer — A-160-5

- [Manual PDF](../../manuals/A-160-5.pdf)

---

[Manual PDF / Product Page: Doepfer A-160-5 Voltage Controlled Clock Multiplier / Ratcheting Controller](https://doepfer.de/a1605.htm)

# Using These Modules Together for Melodic Music
From the manual pages, the main module described is the **Doepfer A-160-5 Voltage Controlled Clock Multiplier / Ratcheting Controller**, shown in patch examples together with the **Doepfer A-155 sequencer** and **A-154 Sequencer Controller**.  
Used together, these modules are very good at creating **melodic lines with rhythmic variation**, especially **ratcheting melodies**, **accented note repeats**, and **step-dependent articulation**.

## What each module contributes

### A-160-5
The A-160-5 is a **voltage-controlled clock multiplier**. It takes an incoming clock and creates a faster clock at its output according to:
- the **CV at CV In** (0 to +5V)
- the **Mode switch**
- or the **Manual control** if no CV is patched

Important behavior:
- **0V CV = no output clock**
- Increasing CV selects higher multiplication factors
- The 3 switch modes choose different factor sets:
  - **integers**
  - **powers of two**
  - **mixed set**

This makes it ideal for **ratcheting**, where one sequencer step can produce:
- no trigger
- one trigger
- two triggers
- several triggers

### A-155 Sequencer
The A-155 is the core melodic sequencer in the patch examples. It provides:
- a stepped CV row for **pitch**
- another CV row that can be used to control the **ratchet amount per step**
- gate/trigger signals for note events

### A-154 Sequencer Controller
The A-154 expands sequencing control and helps with:
- clocking and transport control
- more flexible sequencing behavior
- easier integration of the A-155 into more complex performance patches

In the example, the A-154/A-155 combo is used as the sequencer source, while the A-160-5 adds **sub-step trigger multiplication**.

---

## Core melodic use case: ratcheting melody lines

This is the most direct melodic patch shown by the manual.

## Basic patch idea
Use:
- one sequencer CV row for **pitch**
- another sequencer CV row for **ratchet density**
- the A-160-5 to generate repeated triggers within a single step

### Patch flow
1. **Sequencer clock** goes to the **A-160-5 Clock In**
2. **A-155 pitch CV row** goes to your **VCO 1V/oct input**
3. **A-155 second CV row** goes to **A-160-5 CV In**
4. **A-160-5 Clock Out** goes to the **gate input of an envelope** or directly to a trigger destination
5. Envelope opens a VCA for the VCO

### Result
For each step:
- the **pitch row** determines the note
- the **second CV row** determines how many times that note retriggers during the step

So instead of a plain 8-step melody, you get:
- single notes on some steps
- fast repeated notes on others
- muted steps where CV = 0V

That gives a melody much more motion and phrasing than a standard one-trigger-per-step sequence.

---

## Why this is musically powerful

### 1. Per-step rhythmic articulation
A normal sequencer often gives each step equal weight.  
With the A-160-5, each step can behave differently:
- step 1: one note
- step 2: two repeats
- step 3: four repeats
- step 4: rest
- step 5: fast burst

This turns a static melody into something much more expressive.

### 2. Ratcheting without changing pitch
Because the pitch CV can stay constant during the step while only the trigger rate changes, one pitch can become:
- a stab
- a tremolo-like pulse
- a rising-energy repeated note
- a sequenced ornament

This is especially useful for Berlin-school, trance, techno, electro, and arpeggiated melodic music.

### 3. Built-in mute via 0V
The manual states that **0V at CV In produces no output clock**.  
This means a sequencer row controlling the A-160-5 can also create **rests**. That is extremely useful for melody shaping:
- not every pitch step has to sound
- some notes can be skipped entirely
- ratchet control doubles as articulation/mute programming

---

## Best musical strategies

## 1. One row for pitch, one row for ratchet
This is the most obvious and effective patch.

### Example
- Row 1: melodic notes
- Row 2:
  - 0V = rest
  - low CV = 1 pulse
  - medium CV = 2–3 pulses
  - higher CV = 4 or more pulses

This gives you a melody where every step has both:
- a note value
- a performance gesture

It feels almost like sequencing **pitch + picking pattern**.

---

## 2. Use powers-of-two mode for cleaner rhythmic structure
The middle mode uses **powers of two**.  
This is often best for musical consistency because the subdivisions tend to feel more regular:
- 1x
- 2x
- 4x
- 8x, etc.

For melodic work, this is excellent when you want:
- tight, grid-aligned repeats
- predictable rhythmic ornamentation
- less “odd” variation

Good for:
- arpeggios
- trance plucks
- sequenced basslines
- Berlin-school pulses

---

## 3. Use integer mode for more organic phrasing
The integer mode gives more conventional multiplying factors.  
This can create less symmetrical and more human-feeling variations across steps.

Good for:
- expressive melodic sequences
- less mechanical phrasing
- patterns that avoid always dividing into powers of two

---

## 4. Use mixed mode for evolving melodic figures
The mixed mode can be the most playful. It creates a wider range of subdivisions depending on CV.  
This is useful when your sequencer row is already programmed melodically and you want a broader range of ratchet behaviors.

Good for:
- live performance
- happy accidents
- evolving lead sequences
- generative or semi-generative melody work

---

## 5. Send the multiplied clock to envelopes, not pitch
The A-160-5 does not generate melody by itself; it generates **timing density**.  
The best melodic use is usually:
- pitch CV to oscillator
- A-160-5 output to envelope gate/trigger input

That way repeated clocks retrigger the same note within the step.

This creates:
- note repeats
- fluttering plucks
- mandolin-like repeated articulations
- classic sequencer ratchets

---

## Patch recipes for melodic components

## Patch 1: Berlin-school ratcheting lead
### Connections
- Master clock → A-154/A-155 clock input
- Same clock → A-160-5 Clock In
- A-155 Row 1 CV → VCO 1V/oct
- A-155 Row 2 CV → A-160-5 CV In
- A-160-5 Clock Out → ADSR gate in
- ADSR → VCA CV
- VCO → VCF → VCA

### Programming idea
- Row 1: simple minor-scale melody
- Row 2:
  - some steps at 0V for rests
  - some low for single notes
  - some medium for doubles
  - occasional high settings for dramatic bursts

### Musical result
A classic sequenced melody with animated repeated notes, very reminiscent of vintage electronic sequencing styles.

---

## Patch 2: Accented melodic ornamentation
Instead of ratcheting many steps, only ratchet selected notes.

### Programming idea
- Most steps = one pulse
- Key melody notes = multiple pulses
- Phrase endings = mute or single pulse

### Result
The melody remains clear, but some notes become:
- ornaments
- accents
- fills
- transitions

This is excellent for making a melody feel composed rather than purely looped.

---

## Patch 3: Bassline with rhythmic fill steps
Use the A-160-5 on a bass sequence.

### Programming idea
- Low notes on Row 1
- Row 2 mostly low values
- Every 4th or 8th step gets a higher ratchet amount

### Result
A bassline with occasional rapid retriggers, like:
- pick-style bass attacks
- sequenced rolls
- fill notes before loop restart

This is very effective in techno and electro.

---

## Patch 4: Dual-function melodic row with silence control
Because 0V mutes the A-160-5 output, the ratchet-control row can define:
- whether a note sounds
- how often it retriggers

### Result
You can separate:
- **pitch composition** from Row 1
- **phrase articulation** from Row 2

This is powerful because Row 2 becomes a true **performance lane**:
- mute
- normal note
- repeated note
- dense repeated note

That’s almost like sequencing picking, bowing, or strumming intensity.

---

## Important technical limitation for musical use
The manual notes that the A-160-5 needs **a few clock pulses to stabilize** if the incoming clock changes frequency.  
So for best melodic results:
- feed it a **steady clock**
- avoid rapidly varying the incoming clock tempo
- do not expect perfect output immediately after abrupt clock changes

In practice, this means it works best when driven by:
- a stable master clock
- a sequencer clock with fixed or slowly changing tempo

This is important if you want clean ratchets that stay musically tight.

---

## Practical performance advice

## Keep the incoming clock steady
Since multiplication is derived from averaging recent clock cycles, a jittery or wildly changing clock can make the output feel unstable.

## Use the manual knob for auditioning
If nothing is patched to CV In, the **Manual** knob selects multiplication.  
This is useful for:
- testing rhythmic densities by ear
- finding the best mode before applying sequencer CV
- live performance tweaks if you temporarily remove CV control

## Program musically, not maximally
Too many ratchets on every step can blur the melody. Usually the best results come from contrast:
- many normal notes
- a few repeated notes
- some rests
- occasional bursts

That creates phrasing instead of chaos.

## Match envelope settings to ratchet speed
If your envelope is too long, fast ratchets may smear together.  
For clearer melodic repeats:
- use shorter decay/release
- use snappy envelopes
- tune VCA/VCF response for articulation

---

## Best kinds of melodic content these modules make

These modules are especially strong for:

- **Berlin-school sequences**
- **Tangerine Dream-style ratcheting lines**
- **trance/arpeggiated leads**
- **techno melodic loops**
- **electro basslines with repeated triggers**
- **ornamented step-sequenced melodies**
- **plucked repeating note phrases**
- **gated melodic ostinatos**

They are less about freehand melody generation and more about **adding expressive rhythmic articulation to sequenced pitch material**.

---

## Summary
Used together, the **A-155/A-154** provide the **melodic pitch structure**, while the **A-160-5** provides **per-step trigger multiplication**.  
That means you can create melodic phrases where each note step has its own articulation:
- silent
- single-hit
- double-hit
- rapid repeated burst

This is one of the most effective classic Eurorack methods for creating **animated, musical, rhythmic melodies** from simple sequencer rows.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)