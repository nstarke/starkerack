# Nervous Squirrel — Conway's Game

- [Manual PDF](../../manuals/Nervous Squirrel - Conway's Game.pdf)

---

[Manual PDF / source](https://nervoussquirrel.com/conways_game)

# Nervous Squirrel — Conway’s Game
## How it can be used for melodic components in a Eurorack system

This module is unusual: it is **not a pitch CV sequencer**, but a **64-output trigger/gate matrix** driven either by:

- **Conway’s Game of Life** on an 8×8 grid, or
- **MIDI note input** mapped to 64 outputs

That means its strongest melodic role is as a **rhythmic and structural brain** for melody generation rather than as the direct source of note voltages.

## What the manual shows

### Core functions
- 8×8 LED matrix displays Conway’s Game of Life
- 64 outputs correspond to the 64 cells
- Outputs can operate as:
  - **Triggers**: 20ms pulses
  - **Gates**: held high while a cell is alive
- Internal clock defaults to **10 Hz**
- External **CLOCK IN** can drive it up to about **270 Hz**
- **RESET** starts a new random cell population
- **MIDI mode** responds to notes **C2 (36) to E7 (100)** across the 64 outputs
- Output level: **8V**

### Musical implication
This is essentially a **large parallel event generator**. It excels at:
- distributing timing events,
- creating conditional note changes,
- generating layered phrase structures,
- animating quantizers, switch networks, sequential switches, sample & holds, and envelopes.

---

# Best ways to use Conway’s Game for melody

## 1. Use it as a trigger source for a pitch-generating voice
The simplest melodic use:

**Patch concept**
- One Conway output → envelope trigger
- Same output or another related output → sample & hold clock
- Random or structured CV source → quantizer → oscillator pitch

**Result**
- Conway determines **when notes happen**
- The quantizer determines **what notes happen**

This works well because Conway produces patterns that feel more organic than a regular step sequencer.

### Example patch
- Noise / random CV → S&H input
- Conway output 1 → S&H clock
- S&H out → quantizer
- Quantizer out → VCO 1V/oct
- Conway output 1 → envelope → VCA

This gives you a melodic line whose rhythm is derived from one cell’s activity.

---

## 2. Use multiple outputs to build phrase hierarchy
Because there are 64 outputs, you can treat different cells as different musical layers.

### Suggested layer roles
- **Fast cell outputs** → note triggers
- **Slower/looping cells** → phrase reset or transposition
- **Sparse cells** → accent or ratchet triggers
- **Long-lived gates** → drone enable / sustained note hold

### Example
- Output A → main melodic trigger
- Output B → transpose quantizer by +5th when high
- Output C → switch quantizer scale
- Output D → reset a sequential switch
- Output E → open a secondary VCA for harmony voice

This is where the module becomes powerful melodically: one automaton creates **correlated control structure** across many parameters.

---

## 3. Use gate mode to create sustained melodic states
The **TRIGGERS / GATES** switch matters a lot for melody.

### In trigger mode
Good for:
- plucks
- short envelopes
- clocking S&H
- advancing sequencers

### In gate mode
Good for:
- sustained notes
- holding switches in one state
- enabling quantizer transpose inputs
- keeping a voice active while a cell remains alive

### Melodic application
A gate from one cell can:
- hold a note open,
- keep a sub-oscillator harmony active,
- maintain a transposition offset,
- keep a sequencer direction or range altered.

That lets the Game of Life behave like a **phrase-state generator** rather than only a trigger source.

---

## 4. Turn 64 outputs into note selection logic
If you have utility modules such as:
- logic,
- OR combiners,
- trigger combiners,
- matrix mixers,
- sequential switches,
- addressed switches,

then Conway’s 64 outputs can become a **decision field** for melody selection.

### Patch idea: note pool selector
- Prepare 4–8 fixed voltages representing scale degrees
- Use Conway outputs to clock/select a sequential switch
- Other Conway outputs enable or mute certain note lanes
- Quantizer or precision adder organizes the final pitch

**Result:** the melody evolves according to automaton behavior, not just random voltage.

---

## 5. Use Conway to animate a sequencer instead of replacing it
This is probably the most practical musical use.

### Patch concept
Traditional sequencer + Conway modulation

- Pitch sequencer provides stable tonal material
- Conway outputs affect:
  - clock skips
  - stage advance
  - reset
  - transpose
  - rests
  - octave jumps
  - envelope variation

### Example
- 8-step CV sequencer → quantizer → VCO
- Conway output 1 → master trigger to envelope
- Conway output 2 → sequencer reset
- Conway output 3 → precision adder +1 octave
- Conway output 4 → switch between two sequencer rows
- Conway output 5 → disable trigger path for rests

This preserves musical intention while adding evolving melodic variation.

---

## 6. Use the MIDI mode as a 64-way note-to-trigger decoder
The manual states that MIDI input can control **64 separate trigger outputs** across notes 36–100.

This is very useful if you compose from a DAW, hardware sequencer, or MIDI keyboard.

### Melodic uses of MIDI mode
- Convert specific MIDI notes into individual modular events
- Use MIDI clips to “draw” melodic activation patterns across the 64 outputs
- Trigger different melodic functions from different incoming notes

### Example hybrid patch
From DAW MIDI:
- C2 → trigger note event
- D2 → transpose +2 semitones
- E2 → switch to a different scale
- F2 → trigger harmony voice
- G2 → reset sequencer
- A2 → clock burst generator
- B2 → accent

So instead of using MIDI to directly play pitch, you use it to **orchestrate modular melodic logic**.

This is especially strong for:
- generative composition with controlled form,
- live performance cueing,
- complex melodic state changes from a single MIDI track.

---

# Musical strategies for actual melody creation

Since Conway’s Game does not generate pitch CV directly, you’ll want one or more of these companion module types in your rack:

## A. Quantizer
Essential if you want tonal melodies.

**Why**
Conway gives timing and logic, not note voltages.

**How to use together**
- Random CV or stepped CV → quantizer
- Conway output clocks the note changes
- Additional Conway outputs transpose or switch scales

This produces coherent melodies from otherwise abstract activity.

---

## B. Sample & Hold / Track & Hold
Very strong pairing.

**How**
- Source CV: noise, chaotic CV, sequencer row, LFO, Wogglebug-like source
- Conway trigger → sample clock
- Quantize sampled voltage

Different Conway cells will sample at different moments, creating multiple interrelated melodic lines.

---

## C. Sequential switch / addressed switch
Excellent for melody.

**How**
Use Conway outputs to:
- advance the switch,
- reset the switch,
- choose between several pitch sources.

Pitch sources could be:
- fixed voltages,
- sequencer rows,
- quantizer outputs,
- intervals from a precision adder.

This creates melodies with recurring but non-linear form.

---

## D. Precision adder / transposer
One of the best pairings.

**How**
- Main melody from sequencer or quantizer
- Conway gates add interval offsets:
  - +octave
  - +fifth
  - +third
  - modal shifts

Because Conway cells often form loops, these transpositions can feel motif-like rather than random.

---

## E. Clock divider / multiplier
Useful for extracting musically different time scales.

**How**
- Master clock → divider/multiplier → Conway CLOCK IN or downstream modules
- Conway outputs then interact with divided clocks for:
  - slower transposition
  - faster ornaments
  - phrase resets on long cycles

This gives structure to the melodic motion.

---

## F. Envelope generators and VCAs
Needed to hear the triggers as notes.

**How**
- Conway trigger output → envelope
- Envelope → VCA
- Quantized pitch CV → oscillator

Different cells can trigger:
- main voice,
- harmony,
- accent voice,
- bass punctuations.

---

# Strong patch recipes

## Patch 1: Organic mono melody
**Modules needed**
- Conway’s Game
- random CV source
- sample & hold
- quantizer
- VCO
- envelope
- VCA

**Patch**
- Random CV → S&H in
- Conway output 1 (trigger mode) → S&H clock
- S&H → quantizer → VCO 1V/oct
- Conway output 1 → envelope → VCA
- VCO → VCA → mixer

**What happens**
A single Conway cell becomes a melodic trigger stream with nontrivial phrasing.

---

## Patch 2: Melodic line with evolving transposition
**Add**
- precision adder

**Patch**
- Main melody as above
- Conway output 2 in gate mode → precision adder transpose input (+7 semitones)
- Conway output 3 in gate mode → another transpose input (+12 semitones)
- Sum into oscillator pitch

**What happens**
The melody shifts between root, fifth, and octave regions according to cell life states.

---

## Patch 3: Two-voice canon from neighboring cells
**Modules**
- two S&H paths or two oscillators
- one quantizer with multiple channels, or two quantizers

**Patch**
- Random / slow CV source shared by both voices
- Conway output 10 → voice A S&H clock + envelope
- Conway output 11 → voice B S&H clock + envelope
- Each S&H → quantized pitch for separate oscillator

**What happens**
Because nearby cells in Game of Life are related, the two melodic voices often feel connected but not identical.

---

## Patch 4: Sequencer mutation engine
**Modules**
- CV sequencer
- quantizer
- precision adder
- resettable switch or sequencer controls

**Patch**
- Sequencer CV → quantizer → VCO
- Conway output 1 → note gate
- Conway output 2 → sequencer reset
- Conway output 3 → transpose +12
- Conway output 4 → switch between 2 sequencer rows
- Conway output 5 → trigger extra ornament envelope

**What happens**
Your composed sequence becomes a living melody machine.

---

## Patch 5: MIDI-directed melodic architecture
**Use MIDI mode**
- Feed MIDI notes from DAW or keyboard
- Assign selected notes to structural events via specific outputs

**Patch**
- Certain MIDI notes trigger melody
- Others transpose
- Others switch scale or route voices
- Others trigger harmony or bass

**What happens**
You can “play” the modular’s melodic behavior with MIDI notes instead of only playing pitches directly.

---

# Performance ideas

## 1. Use RESET as a phrase refresh
The manual says RESET starts a new set of cells and also clears stuck MIDI notes.

Musically, this means RESET is a **form control**:
- hit it at section changes,
- trigger it every 8 or 16 bars,
- let the patch evolve within a bounded phrase length.

This is one of the best ways to keep the melody interesting but manageable.

## 2. Modulate the clock source
Because CLOCK IN can be driven externally up to around 270 Hz, you can:
- use a steady clock for structured phrases,
- use a divided clock for slow melodic evolution,
- use audio-rate or irregular clocks for glitch ornamentation.

For melody, modest clock variation can create:
- denser note clusters,
- rubato-like irregularity,
- sudden fills and embellishments.

## 3. Use trigger mode for articulation, gate mode for harmony states
A good live strategy:
- one group of outputs in trigger role via selected patches
- another group in gate role for longer state changes

This creates a melody that has:
- note events,
- phrase-level modulation,
- harmonic motion.

---

# Limitations to understand

## It does not output pitch CV by itself
This is the main thing. To make melody, you need companion modules:
- quantizer
- sequencer
- random source
- fixed voltage source
- precision adder
- switch

## 64 outputs can become patch-dense very quickly
You likely won’t use all 64 directly for melody. More practical is:
- select 4–10 musically interesting outputs,
- route them to utilities,
- create a smaller controllable melodic ecosystem.

## Internal behavior may settle into loops
The manual notes it resets when patterns die out or become stationary; loops can persist in forms like blinkers or gliders.
That’s actually musically useful: loops create recurring motifs. But if you want more variety, patch RESET periodically.

---

# Best overall role in a melodic rack

Conway’s Game is best thought of as:

- a **melodic event ecosystem generator**
- a **phrase and articulation controller**
- a **multi-lane trigger source for quantized pitch systems**
- a **MIDI-to-64 trigger decoder for compositional control**

It is **not** the voice of melody by itself, but it can become the **behavioral engine** that makes melodies feel alive.

## Most effective pairings
If your goal is melody, pair it with:
1. **Quantizer**
2. **Sample & hold**
3. **Precision adder**
4. **Sequential switch**
5. **Traditional CV sequencer**
6. **Envelope/VCA voice chain**

That combination turns Conway’s Game from a trigger novelty into a deep melodic composition tool.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)