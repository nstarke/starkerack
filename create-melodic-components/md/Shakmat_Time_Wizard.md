# Shakmat — Time Wizard

- [Manual PDF](../../manuals/TW-User_Manual.pdf)

---

[Manual PDF](#)

# Shakmat Time Wizard — using it for melodic components

The **Shakmat Time Wizard** is not a pitch/CV source by itself, but it is extremely useful for creating the **timing structure that makes melodies feel alive**. Think of it as a **multi-clock brain** for sequencers, quantizers, sample & holds, switch modules, and envelope-driven voices.

## What the module does

The Time Wizard is a:

- **6-channel clock divider**
- with **independent division settings**
- plus **routing and logic options**
- plus **reset relationships between groups of dividers**

From the manual, it provides:

- **A column**: A1, A2, A3
- **B column**: B4, B5, B6
- **main clock input**
- **reset / alternate B clock input**
- switches for:
  - **Multiply A**: x1 / x3 / x4
  - **Clock B**: normal / B4 clocks B5+B6 / independent B clock input
  - **Logic A2**: off / `A2 AND B5` / `A2 OR A3`
  - **Reset B6**: off / B6 resets A / B6 resets A+B

Outputs are 0–5V triggers, with optional **half-period gates on dividers 5 & 6** via rear jumper.

---

## The musical role of Time Wizard in a melodic patch

For melody, this module excels at:

- creating **different rhythmic layers** that drive multiple sequencers
- generating **phrase resets**
- making **odd-length melodic cycles**
- producing **polyrhythmic note changes**
- deriving **accent, transposition, ratcheting, or note-hold events**
- adding **structural evolution** to otherwise repetitive sequences

It is especially strong when paired with:

- **pitch sequencers**
- **quantizers**
- **sample & hold**
- **sequential switches**
- **precision adders**
- **envelope generators**
- **logic modules**
- **Bernoulli gates / probability**
- **clocked LFOs**

---

# How to use it melodically

## 1. Clock multiple sequencers at different divisions

A classic melodic use is to send different Time Wizard outputs to different note-generating devices.

Example:

- **A1** → main pitch sequencer clock
- **A2** → modulation sequencer clock for filter/pitch offset
- **B5** → sample & hold clock sampling noise or random CV
- **B6** → reset input of pitch sequencer or switch sequencer

This creates melody from the interaction of:

- one repeating note stream
- one slower contour stream
- one random or semi-random event stream
- one long-form phrase reset

### Why this works
Even if your pitch sequencer is simple, the Time Wizard lets note changes, transpositions, and resets happen on **different cycle lengths**, which generates evolving melodic patterns.

---

## 2. Build odd-length phrases

The manual specifically mentions unusual time signatures and strange clock decompositions. This is one of the best melodic applications.

Patch idea:

- master clock into **CLK**
- set:
  - **A1 = /5**
  - **A2 = /7**
  - **A3 = /8**
- use:
  - **A1** to clock a 5-step sequencer
  - **A2** to advance a sequential switch selecting between 2–3 CV sources
  - **A3** to trigger a transposition envelope or precision adder step

Now your melody won’t loop in a short obvious way, because timing layers realign only after a long cycle.

### Musical result
You get:

- asymmetrical motifs
- evolving phrase lengths
- less “16-step box” feel
- more generative, composed-sounding lines

---

## 3. Use Multiply A for triplets and alternate subdivisions

The **Multiply A** switch can multiply the clock feeding the A column by **3 or 4**.

This is powerful for melody because it lets one part of the patch move at a different feel from the rest.

### Example uses

#### Triplet melody against straight rhythm
- send a straight clock to Time Wizard
- set **Multiply A = x3**
- use **A1/A2/A3** to clock melodic sequencers or S&H

Now melodic note changes can happen in **triplet subdivisions** while percussion or another sequencer remains straight.

#### Fast ornament layer
- set **Multiply A = x4**
- use one A output to trigger a second sequencer controlling:
  - grace notes
  - octave jumps
  - wavefolder amount
  - quantized ornament CV

This can create melodic flutter, pseudo-ratchets, or fast counter-lines.

---

## 4. Use Clock B as a phrase hierarchy

The **Clock B** switch is one of the most interesting features.

### Mode 1: normal
B column behaves as regular dividers from the main clock/reset structure.

### Mode 2: B4 clocks B5 and B6
In the middle position, **B4 becomes the clock source for B5 and B6**.

This creates a **clock division inside a division**, which is ideal for phrase-level melody control.

### Melodic application
Use:

- **A column** for note-to-note activity
- **B4** for bar-level motion
- **B5/B6** for phrase resets, transposition, or variation changes

Example:

- **A1** → clock 8-step pitch sequencer
- **B4** → clock a 4-step transposition sequencer
- **B5** → advance a switch choosing one of several modulation CVs
- **B6** → reset the transposition sequencer or entire melody phrase

This feels like having:

- notes
- bars
- phrases

all derived from one compact timing network.

### Mode 3: independent B clock input
In the lower position, the reset input becomes an **independent clock input for B column**.

This is huge for melody because you can run two interacting rhythmic worlds:

- **A column** from one clock
- **B column** from another

Example:

- A clock = steady 16th-note pulse
- B clock = swung clock, Euclidean rhythm, or manually tapped trigger pattern

Then use B outputs to affect melody by:

- resetting the main sequencer
- opening a switch to a second pitch source
- transposing only on B events
- clocking an alternate random voltage source

This creates very musical cross-rhythmic melodies.

---

## 5. Use Logic A2 to create note masks and alternate note timing

The **Logic A2** switch changes the **A2 output** into a logic function.

Available functions:

- middle: **A2 AND B5**
- lower: **A2 OR A3**

This is extremely useful for melodic articulation.

## A2 AND B5
This gives a trigger only when both clocks are high together.

### Use it for:
- selective note advancement
- accent clocks
- occasional sample & hold updates
- opening a VCA for only some notes
- triggering an envelope for “allowed” notes only

#### Patch example
- **A1** → clock sequencer every note
- **A2 AND B5** → trigger a second envelope that adds FM or filter accent
- or use **A2 AND B5** to clock a quantized random source

Result: the melody continues, but only certain notes receive ornamentation or pitch changes.

## A2 OR A3
This creates a denser trigger stream from either A2 or A3.

### Use it for:
- more active melodic gates
- switching between sparse and dense note updates
- clocking a secondary sequencer that “fills in” around the main line

#### Patch example
- main sequencer runs from **A1**
- **A2 OR A3** clocks a second CV source
- mix or switch between those CV sources before quantization

Result: composite melodies with implied call-and-response or fills.

---

## 6. Use B6 reset for phrase closure

The **Reset B6** switch lets B6 reset:

- **A only**
- or **A and B**

This is one of the most compositionally useful features.

### Why it matters
A long divider can act like a **phrase-ending marker**.

### Patch idea
- use A outputs to drive main melodic motion
- use B outputs for slower structural changes
- set B6 to a long division
- enable **B6 resets A** or **A+B**

Now the whole melodic system periodically comes back to the top.

This gives you:

- long-form cycles
- recurring hooks
- controlled generative behavior
- melodies that wander but eventually resolve

That “eventual resolution” is often the difference between random clocks and musical phrasing.

---

# Practical melodic patch ideas

## Patch 1: Polymetric lead line

**Goal:** evolving lead melody with repeating macro-structure.

### Connections
- master clock → **CLK**
- **A1** → clock main pitch sequencer
- sequencer pitch CV → quantizer → oscillator V/oct
- **A2** → clock modulation sequencer for octave offset
- modulation sequencer → precision adder with main pitch CV
- **B6** → reset main pitch sequencer
- set **Reset B6 = A**

### Suggested divisions
- A1 = /5
- A2 = /7
- B6 = /16 or /32 depending on tempo context

### Result
The lead changes notes and octave contour at different rates, then periodically restarts into a recognizable phrase.

---

## Patch 2: Triplet ornament melody

**Goal:** straight melody with triplet embellishments.

### Connections
- master clock → **CLK**
- **Multiply A = x3**
- **A1** → clock a small sequencer generating ornament notes
- normal external clock → another sequencer for main melody
- both pitch CVs into a sequential switch or CV mixer
- **B5** → switch control or VCA envelope trigger
- quantizer after mixing/switching

### Result
The main melody stays grounded, while triplet-timed notes appear as flourishes or alternate inserts.

---

## Patch 3: Two-clock melodic conversation

**Goal:** create a melody that responds to another rhythm source.

### Connections
- steady clock → **CLK**
- irregular trigger pattern or Euclidean clock → **RST/IN B**
- set **Clock B = IN B**
- **A1** → main sequencer clock
- **B4** → transposition sequencer clock
- **B5** → reset sample & hold
- **B6** → switch between two pitch rows or two quantizer scales

### Result
The main melody runs steadily, while another rhythm injects phrase changes, harmonic shifts, and alternate note selections.

---

## Patch 4: Melodic gate masking with logic

**Goal:** same pitch sequence, but changing articulation creates the melody.

### Connections
- **A1** → clock sequencer
- sequencer CV → quantizer → oscillator
- **A2 AND B5** → envelope trigger for VCA
- or use **A2 OR A3** for denser gate pattern
- keep sequencer running continuously, but only audible when the logic output fires

### Result
Pitch may be stable underneath, but audible note rhythm changes in a structured way. This can sound like a completely new melody from the same CV source.

---

## Patch 5: Sample-and-hold melody generator

**Goal:** create generative quantized melodies.

### Connections
- noise / slow random / chaotic CV → sample & hold input
- **A1** → S&H clock
- S&H output → quantizer → oscillator pitch
- **A2** → trigger envelope for notes
- **B5** → clock a second S&H for transposition or timbre
- **B6** → reset a switch or sequencer that changes scales/root notes

### Result
The Time Wizard turns simple random voltage into a multi-layered melodic system with phrase structure.

---

# Best companions for melodic use

The Time Wizard works especially well with these module types:

## Sequencers
Use Time Wizard outputs to clock:

- a main pitch sequencer
- a transposition sequencer
- a modulation sequencer
- a gate sequencer

This is the most direct melodic use.

## Quantizers
Since Time Wizard produces timing rather than pitch, quantizers are crucial when using it with random voltages, switches, or CV mixers.

## Sample & Hold
A perfect pairing. Different divider outputs can determine:

- when a new note is sampled
- when a transposition is sampled
- when timbre changes are sampled

## Sequential switches
Clock the switch with one divider and feed it multiple pitch sources:
- sequencer row 1
- sequencer row 2
- random voltage
- fixed interval voltage

This creates melodic form from routing.

## Precision adders
Use slower Time Wizard outputs to add:
- octave jumps
- chord-tone transpositions
- modal root changes

## Envelope generators / VCAs
Even if the pitch source is unchanged, Time Wizard can define when notes are heard, accented, or doubled.

---

# Tips for musical results

## Use one output for notes, another for changes to the note system
A very effective strategy is:

- one divider clocks the note sequencer
- another divider changes:
  - transposition
  - switch state
  - scale
  - reset point

That gives motion on two timescales.

## Let B6 define phrase length
A long B6 division resetting A or A+B creates musical form.

## Use odd divisions
Set values like:
- 5
- 7
- 3 against 8
- 7 against 16

These make melodies feel less grid-locked.

## Use logic for accents, not only note clocks
`A2 AND B5` is especially good for:
- occasional accent envelopes
- clocking a second oscillator layer
- triggering glide only on selected notes

## Try the rear jumper option
Setting dividers 5 & 6 to **half-period gates** instead of triggers can help with:
- longer note holds
- tied notes
- drone openings
- switching sustained harmonic layers

That can turn short trigger-based sequencing into more legato melodic material.

---

# Limitations to understand

The Time Wizard does **not** generate pitch CV directly. So by itself it won’t create melody in the traditional “notes out” sense.

Instead, it creates melody by controlling:

- **when notes happen**
- **when sequences advance**
- **when phrases reset**
- **when transpositions occur**
- **when alternate pitch sources are chosen**
- **when random voltages are sampled**

In modular, that is often just as important as the pitch source itself.

---

# Bottom line

The **Shakmat Time Wizard** is best understood as a **melodic structure module** rather than a note module.

Used with sequencers, quantizers, switches, and S&H, it can produce:

- polymetric melodies
- evolving generative lines
- triplet or multiplied subdivisions
- phrase resets
- melodic masks and accents
- two-clock interactions
- long non-repeating forms that still resolve musically

If you want, I can also turn this into:
1. a **set of concrete patch recipes with knob settings**, or  
2. a **“best pairings” guide for your other specific modules**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)