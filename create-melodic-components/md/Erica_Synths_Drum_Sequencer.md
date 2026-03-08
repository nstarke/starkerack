# Erica Synths — Drum Sequencer

- [Manual PDF](../../manuals/Erica-Drum-Sequencer-Manual-New.pdf)

---

[Erica Synths Drum Sequencer Manual (PDF)](https://www.ericasynths.lv/media/Drum_Sequencer_manual_v1_056.pdf)

# Using the Erica Synths Drum Sequencer to Create Melodic Parts in Eurorack

Although this module is named **Drum Sequencer**, the manual makes clear that it is also a capable **melodic sequencer** because each pattern contains:

- **16 trigger tracks**
- **1 dedicated CV/Gate track**
- **2 LFOs**

That combination makes it useful not just for drums, but for building:

- basslines
- lead lines
- arpeggios
- quantized melodic patterns
- transposed motifs
- animated modulation for melodic voices

## What the module provides for melody

From the manual, the key melodic tools are:

- **CV OUT** for pitch
- **GATE OUT** for note triggers/gates
- **Dedicated CV/Gate Track** in every pattern
- **Quantized note entry** with scales and root note
- **Per-step note editing**
- **Per-step gate length**
- **Step events** like:
  - microtiming
  - probability
  - retrigger/ratcheting
- **Slide and tie**
- **Track shuffle**
- **Track direction**
- **CV track randomization**
- **Real-time performance / record mode**
- **2 syncable LFOs** per pattern for melodic modulation

So in practice, this single module can serve as the central source for both **rhythm and melody**.

---

# Core melodic patch concept

The most direct melodic patch is:

- **CV OUT** → oscillator or voice **1V/Oct**
- **GATE OUT** → envelope gate input, LPG trigger, or voice gate input
- Voice audio → filter / VCA / mixer

This makes the Drum Sequencer’s **CV/Gate track** act like a normal monophonic sequencer.

## Best voice types to pair with it

Based on the manual, it works especially well with:

- analog oscillators for basslines
- complete synth voices
- digital oscillators with 1V/Oct tracking
- LPG-based west coast voices
- acid/bassline voices
- sampler voices that accept pitch CV and trigger/gate
- quantized melodic percussion voices

---

# The CV/Gate track: the main melodic engine

Each pattern includes **one CV/Gate track**, which is separate from the 16 trigger tracks.

## What it does

The CV/Gate track outputs:

- **continuous pitch CV** from **CV OUT**
- **trigger/gate information** from **GATE OUT**

This means one pattern can contain:

- a drum arrangement on trigger tracks
- one synchronized melodic line on the CV/Gate track
- LFO modulation for additional movement

That is a very strong combination for live techno, electro, IDM, acid, or modular groove performance.

---

# Melodic sequencing workflow

## 1. Select the CV track

From Pattern Edit Mode:

- hold **TRIG SEL** and press **ENC2**
- or scroll the **TRIG** parameter to **CV**

Once selected, the step keys edit the melodic sequence.

## 2. Enter steps

In CV/Gate Pattern Edit Mode:

- press a step key to add a note event
- press again to remove it

This creates the rhythmic skeleton of your melodic phrase.

## 3. Edit pitches in Note Edit Mode

Press **ENC1** from CV/Gate Pattern Edit Mode to enter **Note Edit Mode**.

Here you can edit per-step:

- **NTE** = note
- **OCT** = octave
- **LENG** = gate length

This is where the sequence becomes musical rather than just rhythmic.

---

# Scales and quantized melody

One of the strongest musical features in the manual is scale quantization.

Available scales include:

- Chromatic
- Major
- Minor
- Major Pentatonic
- Dorian
- Phrygian
- Lydian
- Mixolydian
- Locrian

You can also choose:

- **Root note**
- **Octave**

## Why this matters musically

This means you can quickly build:

- techno basslines in minor
- melodic house lines in dorian or mixolydian
- pentatonic riffs
- modal drones and ostinatos
- chromatic acid lines

Since the sequencer constrains notes to the selected scale, improvising with step entry or live performance is much safer musically.

---

# CV/Gate Track Perform mode: playing melodies live

The manual describes **CV/Gate Track Perform Mode**, accessed by pressing **STEP/TAP** while the CV track is selected.

In this mode, the step keys become a kind of keyboard:

- they output **pitch CV**
- they output **gate**
- they can be **loop recorded**

## Musical uses

This is ideal for:

- improvising basslines
- entering melodies by feel instead of menu editing
- performing transpositions live
- recording riffs in real time
- auditioning scales and tonal material while patching

You can also set:

- **Scale**
- **Root**
- **Octave**

So it behaves like a compact quantized performance keyboard.

---

# Note Edit Mode for expressive melodic phrasing

This mode is the main place where a melody becomes expressive.

## Per-step note control

For each step you can set:

- pitch
- octave
- gate length

That allows you to make:

- short plucky notes
- long held tones
- syncopated bass patterns
- accented-feeling note durations, even without velocity

## Gate length

Per-step **LENG** is especially important for melody because it changes articulation:

- short gates = staccato bassline or sequence
- medium gates = standard synth line
- long gates = legato phrases
- **TIE** = sustained connection between notes

This lets the module drive very different voices musically.

---

# Slide and tie: acid and legato sequencing

The manual notes **CV Slide** and **Gate Tie** features.

## Slide

In CV track note edit, pressing two adjacent step keys can enable slide from left step to right step.

This is excellent for:

- acid lines
- portamento-style melodic movement
- gliding basslines
- expressive monosynth phrases

## Tie

By extending gate length to **TIE**, the gate remains high until the next note trigger.

This is useful for:

- legato lines
- held notes over multiple steps
- phrasing against shorter drum grids
- reducing repeated envelope retriggers

Together, **slide + tie** make the melodic engine much more than a simple trigger sequencer.

---

# Step Events for melody

The CV track can use **Step Events Mode**, which gives per-step modulation of performance behavior.

## Microtiming (uTM)

You can nudge individual notes earlier or later.

Musical uses:

- humanized basslines
- swung melodic parts independent of drum swing
- pushing notes ahead for urgency
- laying notes behind the beat for groove

## Probability (PRO)

Each note can have a ratio or probability.

Musical uses:

- occasional passing tones
- evolving motifs
- generative melody variations
- unstable techno sequences
- “ghost notes” in melodic phrases

## Retrigger / Ratchet (RTRG)

You can repeat triggers within a step.

Musical uses:

- repeated note flurries
- ratcheted arp-style effects
- ornamentation on leads
- rolls into phrase endings
- pseudo-trills

For melodic patching, ratchets become especially interesting when sent to:

- envelopes controlling filter cutoff
- LPGs
- percussive pluck voices
- FM voices for metallic arp gestures

---

# Shuffle and direction for melodic development

The manual provides shuffle and direction at multiple levels.

## Shuffle

You can apply shuffle to:

- pattern
- track
- CV/Gate track

For melody this creates:

- swung basslines
- loping lead phrases
- less rigid step motion
- better interaction with straight drums

## Direction

Available directions:

- Forward
- Backward
- Ping-pong
- Random

On a melodic line, this can transform a simple pattern into:

- palindrome phrases
- reverse motifs
- random quantized melodies
- evolving ostinatos

A short 5–8 step melodic loop in ping-pong or random mode can become highly musical very quickly.

---

# CV Track Randomization

The manual includes a dedicated **CV/Gate Track Randomization** mode.

It can randomize:

- **NTE** = note
- **OCT** = octave
- **STP** = step on/off
- **LENG** = gate length

Each with probability values.

## Why this is powerful

This is a compact generative composition tool.

Examples:

### Bassline variation
- keep **STP** low randomization
- moderate **NTE**
- low **OCT**
- low **LENG**

Result: recognizable groove, changing pitches.

### Melodic ambient sequence
- high **NTE**
- medium **OCT**
- medium **LENG**
- some **STP**

Result: drifting melodic figures with varying density.

### Controlled mutation in performance
Since undo reloads the last saved pattern, you can:
- save a stable sequence
- randomize it live several times
- keep a variation if it works
- revert if it doesn’t

That is very performance-friendly.

---

# LFOs as melodic companions

Each pattern has **2 programmable LFOs** with outputs:

- **LFO1**
- **LFO2**

Waveforms include:

- sine
- triangle
- saw
- square
- sample & hold

They can be:
- free-running by frequency
- synced to clock divisions

## How to use them with melodic voices

Patch LFOs to:

- oscillator FM amount
- filter cutoff
- wavefold amount
- pulse width
- VCA CV for tremolo
- effect parameters
- modulation depth inputs

## Example melodic applications

### Bassline animation
- CV track drives pitch/gate
- LFO1 modulates filter cutoff slowly
- LFO2 modulates oscillator shape in sync

### Lead phrasing
- LFO1 to vibrato via attenuator
- LFO2 to wavefolder or resonance
- ratchets in the CV track create bursts of activity

### Generative melody texture
- CV track in random direction
- sample & hold LFO to timbre
- probability on selected notes
- long gate lengths and occasional ties

This makes the module capable of generating full melodic movement, not just note order.

---

# Using trigger tracks alongside the CV track for melody

The melodic side is not limited to the CV/Gate track. The 16 trigger tracks can support melodic structure in several ways.

## 1. Triggering envelopes or events on the melodic voice

Use a trigger track to fire:

- secondary envelopes
- filter plucks
- accent envelopes
- wavefolder bursts
- sample-and-hold clocks
- sequencer resets on external modules

For example:

- CV/Gate track controls pitch and gate
- Trigger track 1 opens a filter envelope on selected accents
- Trigger track 2 triggers a second envelope for FM hits
- Trigger track 3 clocks a sequential switch to alternate timbres

This creates the effect of one melodic line with rich articulation.

## 2. Accent outputs as melodic modulation sources

Tracks 1–12 have **accent outputs**.

These can be used not only for drum accents, but as extra rhythmic CV pulses to control melodic voice behavior:

- filter emphasis
- VCA boost
- distortion amount
- envelope depth
- oscillator sync bursts
- LPG strike intensity

So a single melodic voice can become much more expressive by patching:

- **CV OUT** → 1V/Oct
- **GATE OUT** → main gate
- **ACC output** → filter/env accent or VCA CV pulse

That gives a pseudo-accented bassline or lead.

## 3. Trigger tracks as clock/modulation companions

Use trigger tracks to drive other modules that shape melody:

- clock divider for octave switching
- logic modules for variation
- burst generators
- envelope followers
- switched multiples
- analog shift registers
- secondary sequencers

In this way, the Drum Sequencer can be the central control hub for an entire melodic patch.

---

# Patch ideas for melodic music

## 1. Simple monophonic bassline

Patch:

- **CV OUT** → oscillator 1V/Oct
- **GATE OUT** → envelope gate
- envelope → VCA CV
- oscillator → filter → VCA

Program:

- CV track notes in Note Edit Mode
- short to medium gate lengths
- minor or chromatic scale
- some slide between adjacent steps

Great for:
- acid
- electro bass
- techno sequences

---

## 2. Accent-shaped bass voice

Patch:

- **CV OUT** → oscillator 1V/Oct
- **GATE OUT** → amp envelope gate
- **ACC1** (or another accent out) → filter envelope trigger or VCA CV boost
- voice audio → mixer

Program:

- melody on CV track
- accent rhythm on trigger track 1
- enable accents on that trigger track

Result:
- certain notes hit harder or brighter
- more groove and articulation

---

## 3. Lead line with modulation

Patch:

- **CV OUT** → complex oscillator or digital voice 1V/Oct
- **GATE OUT** → envelope or LPG
- **LFO1** → subtle vibrato or wavetable position
- **LFO2** → filter cutoff or effect depth

Program:

- pentatonic, dorian, or minor scale
- probability on a few notes
- ratchets on phrase endings
- ping-pong direction for repetition with variation

Result:
- animated melodic lead with evolving timbre

---

## 4. Generative melodic voice

Patch:

- **CV OUT** → oscillator 1V/Oct
- **GATE OUT** → LPG or envelope
- **LFO1 sample & hold** → filter cutoff
- **LFO2** → VCA bias or FM amount

Program:

- CV randomization probabilities
- random direction
- varied gate lengths
- some tied notes
- sparse trigger density

Result:
- evolving modular melody that stays rhythmically synchronized

---

## 5. One voice, many articulations

Use trigger tracks around the CV voice:

- CV/Gate track = pitch + main note gate
- TR1 = filter pluck trigger
- TR2 = sub-oscillator burst / wavefolder envelope
- TR3 = delay send gate or effect ducking
- ACC1 = “accent” CV to VCA or filter

This turns one synth voice into a performance-ready line with motion and internal variation.

---

# Song mode for melodic arrangement

The manual’s **Song Mode** allows chaining patterns into larger forms.

This is useful melodically because you can create:

- verse / chorus bassline changes
- different root notes across patterns
- transposed phrase groups
- A/B variations of a lead
- breakdown and drop arrangements

For example:

- Pattern A1: main bassline
- A2: bassline with ratchets
- A3: transposed variation
- A4: sparse breakdown phrase

Then arrange these in Song Mode to build a full melodic structure.

---

# Pattern copy and mutation workflow for composition

A very modular-friendly composition workflow from the manual is:

1. Create a melodic pattern
2. **Save**
3. Copy it to another pattern slot
4. Change:
   - scale
   - root
   - gate lengths
   - probability
   - direction
   - shuffle
   - note randomization
5. Chain or arrange patterns

This is especially effective for writing full tracks because you preserve groove while changing pitch material.

---

# Tuning considerations

The manual includes tuning guidance for matching the sequencer with a sound source.

Important practical point:

- **CV OUT** should be patched to a **1V/Oct** input
- Tune the oscillator carefully against the sequencer’s default note references

This matters because the Drum Sequencer’s melodic usefulness depends on accurate tracking. Once tuned, the scale and note functions become much more reliable musically.

---

# Best musical roles for this module

Even though it is a drum sequencer, the manual shows it is very strong for:

## Basslines
Because it has:
- quantized pitch
- gate length
- slide
- tie
- shuffle
- probability
- ratchets

## Leads
Because it has:
- real-time performance mode
- scale modes
- octave transpose
- per-step note editing
- LFO modulation

## Arps and ostinatos
Because it has:
- short lengths
- direction modes
- ratcheting
- randomization
- pattern chaining

## Generative melody
Because it has:
- random direction
- step probability
- CV randomization
- synced LFOs
- save/undo workflow

---

# Practical “used together” view of the outputs

Here’s the most musically useful way to think about the module as a melodic ecosystem.

## CV/Gate Track
Use for:
- main note sequence
- bassline
- lead
- arp
- drone phrasing

## Trigger Tracks
Use for:
- modulation triggers
- filter accents
- envelope fires
- resets
- timbral events
- parallel sequencing utilities

## Accent Outputs
Use for:
- dynamic emphasis
- rhythmic CV bursts
- opening filters
- boosting VCA
- driving auxiliary modulation

## LFO1 / LFO2
Use for:
- vibrato
- timbral movement
- synced modulation
- random stepped modulation
- animated melodic texture

Together, these functions allow one Drum Sequencer pattern to behave like a small compositional system:
- notes
- gates
- articulations
- modulation
- arrangement

---

# Example full melodic techno patch

A strong complete patch using only the melodic-capable parts described in the manual:

## Main voice
- **CV OUT** → analog oscillator 1V/Oct
- **GATE OUT** → ADSR gate
- ADSR → VCA
- oscillator → filter → VCA

## Articulation
- **TR1** → filter envelope trigger
- **ACC1** → extra CV to filter cutoff input

## Motion
- **LFO1** → oscillator PWM or shape
- **LFO2** → subtle filter modulation

## Sequence setup
- CV track in minor scale
- root set to track key
- 8–16 step bassline
- several notes with slide
- one or two tied notes
- probability on a passing tone
- ratchet on final step of bar
- moderate shuffle

## Performance setup
- copy pattern to nearby slots
- make variations with:
  - different roots
  - different note randomization
  - changed gate lengths
  - alternate track direction
- chain patterns or use Song Mode

This gives a complete, performable melodic subsystem from one module.

---

# Conclusion

From the manual, the Erica Synths Drum Sequencer is much more than a drum trigger source. For melodic work, it acts as:

- a **quantized monophonic sequencer**
- a **performance keyboard/recorder**
- a **per-step melodic editor**
- a **probability and ratchet sequencer**
- a **modulation hub** with 2 LFOs
- a **live arrangement tool** through patterns and songs

## In short:
Use the **CV/Gate track** for notes, the **trigger/accent tracks** for articulation and modulation, and the **LFO outputs** for movement. Together, they can drive a full melodic voice with enough control for basslines, leads, arps, and evolving generative phrases.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)