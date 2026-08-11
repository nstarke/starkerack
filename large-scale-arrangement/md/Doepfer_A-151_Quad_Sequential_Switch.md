# Doepfer — A-151 Quad Sequential Switch

- [Manual PDF](../../manuals/A151_man.pdf)

---

[Manual PDF](https://doepfer.de/a100_man/a151_man.pdf)

# Doepfer A-151 Quad Sequential Switch: using it to build full-length songs

The **Doepfer A-151** is deceptively simple, but for song-making it’s one of the most useful “arrangement” tools in Eurorack. It is basically a **4-step sequential switch**: each trigger advances the common jack to the next of four jacks, and a reset returns it to step 1. Version 2 also adds a **2/3/4 step selector** and supports the full **±12V** A-100 range.

The key idea for full-length songs is this:

> The A-151 is not just for switching signals — it is for switching *states*, *roles*, *sections*, and *musical decisions over time*.

That makes it ideal for moving from “cool loop” to **structured progression**.

---

## What the module does well

From the manual:

- 1 common **O/I** jack
- 4 switched **I/O** jacks
- **Trigger input** advances step-by-step
- **Reset input** returns to stage 1
- **Bidirectional switching**
  - 4 inputs → 1 output
  - or 1 input → 4 outputs
- LEDs show current stage
- Version 2 can limit to **2, 3, or 4 steps**

In musical terms, that means:

- rotate between **different modulation sources**
- rotate between **different destinations**
- create **repeating sections**
- create **fills and variations**
- route one sequence to different voices
- route multiple timbres into one signal chain
- reset the “form” of a patch at musically meaningful moments

---

# Why it matters for full songs

A lot of modular patches fail to become songs because they lack:

1. **Section changes**
2. **Contrast**
3. **Repeatable structure**
4. **A way to return to “home”**
5. **Controlled variation without repatching**

The A-151 solves all five.

It can act like a **mini arrangement brain** when driven by clocks, clock dividers, trigger sequencers, logic, or manual gate buttons.

---

# Core song-building strategies

## 1. Use it as a section selector

Patch four different CV or audio “scenes” into the four I/O jacks, and use the common jack as your active output.

Examples of scene sources:

- four different melodic CV patterns
- four different transposition voltages
- four different envelope shapes
- four different drum trigger patterns
- four different filter settings via offset voltages
- four different submixes of voices

Then clock the A-151 **slowly**, not per 16th note. Think:

- advance every 8 bars
- advance every 16 bars
- reset every 32 bars

This turns the switch into:

- **Verse**
- **Pre-chorus**
- **Chorus**
- **Breakdown**

### Patch idea
- Four sequencer rows or four stored voltages → A-151 I/O 1–4
- A-151 O/I → oscillator 1V/oct transposition input via precision adder
- Clock divider output → A-151 Trigger
- Master “start of bar 1” pulse → A-151 Reset

Result: each section gets its own harmonic center or melodic contour, but the whole piece remains synchronized.

---

## 2. Use it to swap rhythmic patterns over longer timescales

A common modular trap is one great drum loop forever. The A-151 fixes that immediately.

### Patch idea
- Four trigger pattern sources into I/O 1–4:
  - straight kick pattern
  - denser kick variation
  - sparse breakdown pattern
  - fill pattern
- O/I → kick drum trigger input
- Advance A-151 every 4 or 8 bars
- Reset every 16 or 32 bars

Do the same on another A-151 for hats or snares.

This creates **macro-rhythm evolution**:
- section A: restrained groove
- section B: busier groove
- section C: stripped-down groove
- section D: fill / transition

Because the A-151 is sequential and resettable, you can make these changes happen at predictable musical points.

---

## 3. Use it as a destination router for one melodic source

Because the switch is bidirectional, you can send one common source to four different outputs.

This is powerful for arrangement.

### Patch idea
- Sequencer melody → A-151 O/I
- I/O 1 → bass voice pitch
- I/O 2 → lead voice pitch
- I/O 3 → FM voice pitch
- I/O 4 → sampler / pluck voice pitch
- Trigger A-151 every 8 bars

Now one melodic source gets reassigned to different instruments across the song.

This creates:

- intro: bass only
- verse: lead takes over
- bridge: weird FM reinterpretation
- outro: pluck variation

Very song-like, very efficient.

---

## 4. Use it to rotate modulation “moods”

One of the best ways to make sections feel different is not changing notes, but changing **motion**.

### Patch idea
Patch four modulation sources into the A-151:

- I/O 1: slow triangle LFO
- I/O 2: stepped random
- I/O 3: envelope loop
- I/O 4: manual offset / fixed voltage

O/I goes to:
- filter cutoff CV
- wavefolder CV
- delay time CV
- reverb size CV
- VCA CV depth control

Advance every few bars.

This gives each section a new animation style:
- smooth
- jagged
- pulsing
- static

That’s often enough to turn a repetitive loop into an arranged performance.

---

## 5. Use reset to enforce song form

Reset is where the A-151 becomes a real arranger instead of a fancy variation switch.

If you feed the reset input from a master sequencer, clock divider, or end-of-cycle event, you can force the arrangement to return to section 1 at exact boundaries.

Examples:
- reset every 64 bars
- reset at the start of each performance take
- reset after a fill
- reset after a manually triggered transition

This makes structures like:

- **A A B A**
- **Verse Verse Chorus Verse**
- **3-step phrase plus reset**
- **4-bar loop with 1-bar fill, then restart**

Even on a pure modular system, that gives you a repeatable backbone.

---

# Best full-song use cases

## A. Intro → groove → breakdown → climax

Use the four steps as four energy states.

### Step assignments
1. **Intro**
   - sparse percussion
   - low filter cutoff
   - no bass
   - lots of reverb

2. **Groove**
   - kick + hats active
   - bass sequence enters
   - moderate modulation

3. **Breakdown**
   - drums reduced
   - lead or pad emphasized
   - long envelopes
   - transposed harmony

4. **Climax / fill**
   - full drums
   - open filter
   - extra modulation
   - denser trigger pattern

Advance one step every 8 or 16 bars, then reset after step 4.

This is probably the most direct way to use the A-151 for song form.

---

## B. Verse / chorus harmonic switching

If you already have a melodic loop, the easiest way to make it song-length is to change harmony while preserving rhythm.

### Patch idea
- Main melody CV stays constant
- A-151 switches among four transposition voltages:
  - 0 semitones
  - +5 semitones
  - +7 semitones
  - -2 semitones
- Output goes through a precision adder with the melody CV
- Advance every 8 bars

Now the same motif behaves differently across sections.

This is especially strong for techno, ambient, synth-pop, and Berlin-school style modular songwriting.

---

## C. Drum arrangement manager

The A-151 is excellent for selecting among several trigger streams for one drum voice.

### For example, on the snare:
- I/O 1: backbeat only
- I/O 2: backbeat + ghost note
- I/O 3: sparse breakdown snare
- I/O 4: snare roll fill

Or on hats:
- I/O 1: 8ths
- I/O 2: 16ths
- I/O 3: offbeat only
- I/O 4: burst pattern

By clocking the switch from a divider or trigger sequencer, you gain arrangement without touching the patch.

---

## D. Bassline evolution without changing voice

Take four pitch or gate variations of one bassline and let the A-151 rotate through them.

### Example
- same rhythm, four pitch variants
- or same pitch row, four gate densities
- or four different accent envelopes

Use:
- Trigger every 4 bars
- Reset every 16 bars

This gives a familiar repeated motif that still develops, which is exactly what full songs need.

---

## E. Call-and-response with one sequencer

Because the switch is bidirectional, one sequence can address different voices in turn.

### Patch
- Sequencer CV/gate to O/I or parallel utility routing
- I/O 1 → bass
- I/O 2 → lead
- I/O 3 → chord voice
- I/O 4 → percussion modulation destination

Each section sends the same compositional material somewhere else.

This produces a strong sense of **orchestration over time**, even with limited gear.

---

# Advanced song-form techniques

## 1. Pair it with a clock divider for long arrangements

The biggest mistake is clocking the A-151 too fast. For song structure, use divided clocks.

Useful sources:
- /16
- /32
- /64
- end-of-pattern pulse from a sequencer

Examples:
- advance every 2 bars for lively IDM
- every 4 bars for pop-like phrasing
- every 8 bars for techno sections
- every 16 bars for long-form ambient evolution

A clock divider or trigger sequencer is almost essential here.

---

## 2. Use the 2/3/4 step switch for asymmetrical sections

On version 2, the step-count switch is very useful musically.

### 2-step mode
Perfect for:
- verse/chorus alternation
- A/B harmonic toggling
- dry/wet alternation
- kick pattern variation

### 3-step mode
Great for:
- 3-part phrases
- “expectation breaking” loops
- polymetric song movement
- A/B/C forms

### 4-step mode
Best for:
- full cycle song structures
- intro / verse / bridge / chorus
- four-stage energy build

Three-step mode in particular can help avoid the too-square feeling many modular patches have.

---

## 3. Use it with logic modules for fills and conditional transitions

If you combine the A-151 with logic or comparator modules, you can get more performable structures.

Examples:
- trigger advance only when a gate is high
- reset only when a manual button and end-of-bar pulse coincide
- alternate between two steps unless a fill trigger forces step 4
- use probability to occasionally skip to the next state

This lets the A-151 behave more like a song-aware router than a simple rotary switch.

Useful partner modules:
- logic
- AND/OR combiners
- comparators
- Bernoulli/probability gates
- sequential trigger generators

---

## 4. Build “scene memories” with fixed voltages

The A-151 doesn’t store voltages itself, but it can select among four prepared voltages.

If you patch four offsets into it, each step can define a different global setting for:
- filter cutoff
- effect send amount
- wavefolding depth
- drum decay
- VCA bias
- oscillator FM amount

Think of these as **song scenes**.

If one A-151 changes pitch/transposition and another changes timbre offsets at the same time, your sections become much more convincing.

---

## 5. Switch submixes, not just single signals

A high-leverage technique is feeding the A-151 with outputs from mixers or VCAs rather than individual raw voices.

For instance:
- I/O 1 = dry drum bus
- I/O 2 = drum bus + clap send
- I/O 3 = filtered drum bus
- I/O 4 = FX-heavy drum fill bus

Or:
- I/O 1 = bass voice only
- I/O 2 = bass + pad
- I/O 3 = lead + hats
- I/O 4 = full ensemble

Now the A-151 is selecting between **arrangement layers**, not just single waveforms.

That’s much closer to how songs are actually structured.

---

# Practical full-song patch recipes

## Patch 1: 4-section techno arranger

### Modules
- master clock
- clock divider
- drum sequencer or trigger sequencers
- bass sequencer
- 1–2 voices
- filter
- VCA
- mixer
- A-151

### Patch
- Four kick patterns → A-151 #1 I/O 1–4
- A-151 #1 O/I → kick trigger
- Four transposition voltages → A-151 #2 I/O 1–4
- A-151 #2 O/I → precision adder → bass voice pitch
- Clock divider /32 → both A-151 triggers
- Reset at 64-bar boundary → both reset inputs

### Section plan
1. intro: no kick or sparse kick, low bass transpose
2. groove: main kick pattern, bass enters
3. breakdown: reduced kick, alternate transposition
4. peak: denser kick/fill, brighter bass section

This creates a loop with real macro-development.

---

## Patch 2: Ambient evolving composition

### Use case
Less about verse/chorus, more about gradual scene morphing.

### Patch
- Four modulation sources → A-151 I/O 1–4
- O/I → filter cutoff CV
- Another A-151:
  - four audio sources or four FX-return levels
  - selected into one main path
- Trigger both from a very slow clock or manual gate
- Reset only occasionally or by hand

This works well for:
- drone albums
- generative pieces with recurring structure
- live ambient sets where section changes should be subtle but intentional

---

## Patch 3: Songified acid line

### Problem
Classic acid patches loop endlessly.

### Solution
Use the A-151 to rotate among:
- four accent patterns
- or four gate patterns
- or four transposition offsets

### Patch
- one 303-style pitch line remains constant
- A-151 switches among four gate/accent variants every 8 bars
- reset every 32 bars

Result:
- same hook
- changing phrase articulation
- recognizable identity with long-form variation

Very effective.

---

## Patch 4: Keyboard performance song mode

The manual notes that a keyboard gate can trigger switching. This is excellent for performable songs.

### Patch
- keyboard gate → A-151 trigger
- four envelopes into A-151
- A-151 output → filter CV

Each played note advances to a new articulation.

Expand that concept:
- use one A-151 for filter envelope choice
- one for oscillator waveform source selection
- one for effects send amount

Now playing successive notes naturally creates song progression. This is especially good for:
- live synth-pop
- modular lead performance
- arpeggiated melodic storytelling

---

# Great module partners for the A-151

## Sequencers
Use with:
- pitch sequencers
- trigger sequencers
- gate sequencers
- CV recorders

Why:
- switch between phrases
- direct one phrase to multiple roles
- arrange patterns across bars

## Clock dividers / multipliers
Use with:
- Pam’s-style clocks
- divider trees
- trigger delays

Why:
- create musically meaningful section lengths
- sync transitions to bars and phrases

## Precision adders / quantizers
Use with:
- transposition voltages
- melodic scene changes

Why:
- preserve tuning while changing section harmony

## VCAs and mixers
Use with:
- layered voice groups
- envelope-dependent scenes
- submix switching

Why:
- turn simple switching into arrangement-level changes

## Logic / probability
Use with:
- fills
- conditional resets
- performance interaction

Why:
- make transitions less mechanical

## Envelopes and modulation sources
Use with:
- different animation profiles for each section

Why:
- sections feel composed, not merely switched

---

# Important musical tips

## 1. Think in bars, not triggers
For full songs, don’t ask:
- “what happens every pulse?”

Ask:
- “what happens every 4 bars?”
- “what happens every 8 bars?”
- “what returns every 32 bars?”

That is where the A-151 shines.

## 2. Reset is composition
Without reset, the switch just cycles.
With reset, it becomes form.

## 3. Use multiple A-151s for coordinated scene changes
One can change:
- rhythm

Another:
- harmony

Another:
- timbre

Triggered together, they create convincing section shifts.

## 4. Don’t switch too many things at once
If every parameter changes on every section, it can sound arbitrary.
Usually best:
- 1 rhythmic change
- 1 harmonic/timbral change
- 1 textural change

## 5. Create tension by delaying one layer
For example:
- drums change at bar 9
- bass changes at bar 13
- melody changes at bar 17

You can do this with separate A-151s driven by different clock divisions or reset structures.

---

# Limitations and how to work around them

## No voltage address
The A-151 is sequential, not CV-addressed.
So you can’t directly jump to arbitrary steps via CV.

### Workaround
Use:
- reset cleverly
- different trigger streams
- companion sequential switches
- manual triggers for performance

## It switches one path at a time
So it doesn’t mute/unmute many parts independently like a matrix mixer.

### Workaround
Use it upstream of:
- VCAs
- mixers
- submixes
- logic-controlled gates

## Audible switching may be noticeable with some material
That can be a feature or a bug.

### Workaround
- switch at phrase boundaries
- use envelopes/VCAs to soften transitions
- embrace it for rhythmic cuts and glitches

---

# My favorite full-song roles for the A-151

If I were using this module specifically to turn loops into songs, I would prioritize these roles:

1. **Section transposition selector**
2. **Drum pattern rotator**
3. **Envelope/timbre scene selector**
4. **Voice reassignment router**
5. **Breakdown/fill reset controller**

Those five uses alone can create surprisingly complete arrangements.

---

# Example full arrangement concept

Here’s one practical “whole song” concept using a single A-151.

## Song structure
- 8 bars intro
- 16 bars verse groove
- 8 bars breakdown
- 16 bars chorus/peak
- reset and repeat with small live tweaks

## A-151 assignment
- I/O 1: sparse drum pattern + dark filter offset
- I/O 2: full groove pattern + root bass transpose
- I/O 3: reduced drums + higher reverb send
- I/O 4: dense hats/fill pattern + brighter filter + fifth transpose

### Control
- advance every 8 bars
- reset after step 4

Even with just one switch, that’s a real song form.

With two or three A-151s, it becomes a serious modular arrangement system.

---

# Bottom line

The **Doepfer A-151** is a classic “small utility, big compositional impact” module.

It helps create full-length songs by giving you a way to:

- organize **sections**
- rotate **patterns**
- vary **timbre**
- redirect **melodies**
- control **energy flow**
- create **repeatable form with resets**

In other words, it helps solve the modular problem of being stuck in a great 8-bar loop.

Used with clocks, dividers, sequencers, VCAs, mixers, logic, and a few carefully chosen modulation sources, the A-151 can become a compact but powerful **song-arrangement engine**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)