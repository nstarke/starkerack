# IO Labs — Flux Sequencer

- [Manual PDF](../../manuals/IO Labs - Flux Sequencer - 107 User Manual.pdf)

---

[Manual PDF](attachment)

# Using IOLabs Flux to Create Melodic Components in a Eurorack System

Flux is presented primarily as a **4-channel rhythm sequencer**, but the manual makes it clear that it can also be a very capable **melodic control source** when you treat its CV lanes, quantization, modulation buses, and auxiliary trigger logic as pitch-and-phrase tools rather than only percussion tools.

## What Flux gives you for melody

Each of the 4 channels includes:

- **1 main rhythm output**
- **2 auxiliary rhythm outputs**
- **1 CV output**

So across the module you effectively get:

- **4 independent CV lanes**
- **12 trigger/gate lanes** total if you count main + aux outputs per channel

That combination is enough to build complete melodic structures:
- pitch CV
- note gates
- accent/variation gates
- transposition or articulation modulation
- phrase resets and derived clocks

## The key melodic features in the manual

### 1. Per-step CV sequencing
On **Main UI Page 2: CV Outs**, each step can output one of several CV modes:

- **VOLT** — fixed voltage per step
- **LFO** — free-running modulation source
- **ENV+ / ENV-** — envelope shapes
- **RANDS** — random voltage once per step
- **RANDT** — random voltage once per trigger within a step

For melody, **VOLT** is the most direct pitch sequencer mode.  
Set a channel’s CV output to **VOLT**, then program **MAXV** per step as your note value.

Because each step has independent values, you can create:
- basslines
- lead melodies
- repeating motifs
- transposition sequences

### 2. Built-in quantization
Flux’s CV output includes **per-step quantization** via:

- **QUAN** — number of equally spaced nodes per volt, from 1–24
- **QUAN NODES** — enable/disable individual notes in that division

This is extremely useful for melodic work.

Examples:
- Set **QUAN = 12** for semitone division across each volt
- Turn on only scale tones in **QUAN NODES** to create a custom scale
- Change quantization settings per step for modal movement or unusual harmonic behavior

This means Flux can behave like:
- a pitch sequencer
- a scale-locked melody generator
- a constrained random melodic source

### 3. Per-step voltage range
Each step has:
- **MINV**
- **MAXV**

For melody this is powerful because you can define:
- fixed pitch by setting VOLT mode and using MAXV
- pitch windows for random generation in **RANDS** or **RANDT**
- limited register zones for phrases

For example:
- bass channel: keep MINV/MAXV low
- lead channel: set higher voltage range
- harmony channel: use same quant scale, different voltage span

### 4. Trigger generation for note articulation
Flux’s main strength is timing. Its rhythm engine can generate very intricate trigger structures using:

- **DENS**
- **CURV**
- **VAL**
- **LENG**
- **PHAS**
- **COMP**
- **MASK**
- **PROB**
- **HUMA**

For melody, these parameters do not just make rhythms—they shape **note articulation**.

Patch idea:
- CV out → oscillator pitch input
- main rhythm out → envelope gate or LPG trigger

Then Flux determines:
- **which pitch** is heard via CV
- **when it is heard** via trigger output

This lets you make melodies that are:
- straight and clocked
- ratcheted
- polyrhythmic
- sparse
- humanized
- probability-based

## Practical melodic patching strategies

---

## 1. Basic 1V/oct melodic sequencer

### Patch
- **Channel CV out** → oscillator **1V/oct**
- **Channel main rhythm out** → envelope gate in
- **Envelope out** → VCA CV in
- **Oscillator audio** → VCA → mixer/filter

### Setup
- On CV page, set **CVSEL = VOLT**
- Set **QUAN = 12**
- Enable desired scale degrees in **QUAN NODES**
- Program per-step **MAXV** values
- On rhythm page, set note timing with:
  - **DENS = 1** for one note per step at first
  - adjust **LENG** for note duration framework
  - use **GATE** to control note length feel

### Result
Flux acts like a melodic step sequencer, but with more flexible timing than a standard 16-step pitch sequencer.

---

## 2. Ratcheting melodic lines

Because trigger density can exceed 1 per step, a single step can generate multiple note events.

### Patch
- CV out → oscillator 1V/oct
- Main rhythm out → envelope gate

### Setup
- Use **CVSEL = VOLT**
- For selected steps increase **DENS**
- Experiment with **CURV** and **VAL**
  - **VAL = 0** gives even subdivisions
  - positive/negative values skew trigger spacing
- Adjust **GATE** for tight plucks or longer ties

### Result
You get:
- repeated notes
- clustered attacks
- accelerating/decelerating note bursts
- ornamental melodic figures

This is especially effective for:
- Berlin-school lines
- IDM-style ratchets
- generative arpeggio embellishments

---

## 3. Quantized random melody generator

### Patch
- CV out → oscillator 1V/oct
- Main output → envelope gate

### Setup
- Set **CVSEL = RANDS** for one random note per step  
  or **RANDT** for a new random note on every trigger
- Set **MINV/MAXV** to constrain register
- Set **QUAN = 12**
- Use **QUAN NODES** to define the scale
- Use **PROB**, **MASK**, and **DENS** to control phrase density

### Result
This creates scale-constrained generative melodies.

Use:
- **RANDS** for stable note-per-step random sequencing
- **RANDT** for volatile, trigger-level melodic motion

This is one of the strongest melodic uses of Flux.

---

## 4. Four-part melodic system

Because Flux has **4 channels**, it can function as a small compositional brain for multi-voice music.

### Example allocation
- **CH1**: bassline pitch + gate
- **CH2**: lead melody
- **CH3**: harmony or countermelody
- **CH4**: modulation lane or additional voice

### Possible patching
- Each channel CV out → separate oscillator or voice 1V/oct
- Each channel main output → each voice envelope gate
- AUX outputs → accents, resets, chord changes, clocking other modules

### Result
You can create:
- interlocking melodic polyrhythms
- canon-like patterns
- polymetric harmony
- percussion-plus-melody hybrids

Because each channel has independent loop points and timing behavior, voices can cycle against one another.

---

## 5. Using AUX outputs as melodic articulators

Each channel has **AUX1** and **AUX2** with many modes, including:

- delayed copies
- first/last trigger
- start-of-step
- dividers
- boolean logic
- clock divisions
- CV threshold comparisons

For melody, AUX outs are excellent for:
- accents
- opening a second envelope
- switching wavefolders or filters
- clocking sample-and-hold
- triggering octave jumps or transposition events
- selectively firing a second oscillator layer

### Example
- Main out triggers the note envelope
- AUX1 triggers a second, shorter envelope to open a filter only on selected steps
- AUX2 sends a divider or logic-derived pulse to transpose another sequencer

This can make a simple melody feel animated and phrased.

---

## 6. Melodic modulation with Macro Pots, CV inputs, and Evolve LFOs

Flux has 3 modulation sources:

- **Macro Pots**
- **CV Inputs**
- **Evolve internal LFOs**

These can modulate many parameters including rhythm and CV behavior.

### Why this matters melodically
You can modulate:
- **MAXV / MINV** for transposition or pitch drift
- **ATK / REL / ACUR / RCUR** for note shape
- **DENS** for phrase activity
- **VAL / CURV / COMP / PHAS** for articulation timing
- **SHUF** for groove changes
- even **BPM** in internal mode

### Musical uses
- a macro knob for live transposition
- CV input to animate note range
- slow Evolve LFO to drift melody density over time
- performance macros that move from sparse to busy lines

The manual notes that modulation is controlled through **mod buses**:
- Yellow
- Grey
- Purple

Per step, you choose which bus affects it.  
That means modulation can be active on some steps and absent on others, which is very useful for melodic phrasing.

### Example phrase design
- Put transposition modulation only on steps 5–8
- Apply density modulation only to end-of-bar steps
- Apply CV modulation to one phrase section but not another

This creates evolving melody with intentional structure.

---

## 7. Envelopes and LFOs as melodic support signals

The CV outputs are not limited to pitch.

A channel can instead generate:
- **AR envelopes**
- **inverted envelopes**
- **free-running LFOs**

So one channel can sequence melody, while another channel’s CV out can modulate:
- filter cutoff
- wavefold amount
- FM index
- VCA level
- stereo placement

### Melodic use case
- CH1 CV = pitch for oscillator A
- CH1 main out = note gate
- CH2 CV = synced envelope controlling filter
- CH2 main or AUX = accent trigger

Now Flux is doing both pitch and expression.

---

## 8. Scale-based melodic probability and masking

The rhythm side includes:
- **PROB**
- **MASK**
- **MSK>**
- **LOOP**
- **STEP on/off**
- **GEN** on/off generator

For melody, these functions create phrase variation.

### Good uses
- **PROB St**: occasionally skip an entire note group
- **PROB Tr**: probabilistically thin ratchets within a step
- **MASK**: create repeating omission patterns
- **LOOP**: set shorter phrase loops inside longer harmonic movement
- **ON/OFF generator**: algorithmically create active/inactive steps

If the pitch stays the same but note occurrence changes, you get melodic variation without reprogramming the line.

---

## 9. Shuffle and humanization for melodic groove

The module provides:
- **SHUF**
- **SH16**
- **HUMA**

These are often thought of as drum tools, but they are equally important for melody.

Use them to make:
- basslines swing
- leads feel less rigid
- arps become more playable and human

A very mechanical pitch sequence can become musically convincing with just subtle timing movement.

---

## 10. Burst mode for triggered melodic phrases

In **BURST** mode, a channel’s step can be triggered from gate inputs or MIDI notes. This can be used for melodic bursts or ornaments.

### Patch concept
- External keyboard gate / sequencer pulse into gate input
- Flux in Burst mode
- CV out to oscillator pitch
- Main output to envelope gate

### Result
Each incoming trigger can launch:
- a ratcheted note burst
- a predesigned ornament
- a short melodic flourish

This is great for:
- fills
- grace-note clusters
- responsive live performance phrases

---

## Best melodic workflows from the manual

## Workflow 1: Flux as a classic melody sequencer
Use:
- **CVSEL = VOLT**
- **QUAN = 12**
- **QUAN NODES** = scale
- **DENS = 1**
- main out as note gate

This gives you a stable, scale-aware melodic sequencer.

## Workflow 2: Flux as a generative melodic composer
Use:
- **CVSEL = RANDS or RANDT**
- quantization enabled
- probability, masking, and modulation buses active
- AUX outputs for accents and phrase changes

This gives you self-varying melodic material.

## Workflow 3: Flux as melody + articulation brain
Use one channel for pitch and note gate, and the AUX outs for:
- accent triggers
- filter pings
- phrase resets
- clock divisions

This turns one melodic line into a complete articulated performance lane.

## Workflow 4: Flux as a 4-voice polymetric melody engine
Use all 4 channels with different:
- loop lengths
- quantization scales
- step lengths
- densities
- shuffle amounts

This creates layered melodic counterpoint.

---

## Especially strong pairings with other Eurorack module types

Flux will work particularly well with:

### Oscillators / voices with 1V/oct input
Use CV outs for pitch and main outs for note triggers.

### Quantizer-adjacent voices
Flux already has internal quantization, so it works especially well with voices that want clean stepped pitch CV.

### LPGs and percussion voices
Because Flux is rhythm-centric, it excels at plucked and percussive melodic patches.

### Sequential switches
Use AUX logic/dividers to switch between oscillators, timbres, or transposition sources.

### Sample & hold / shift register modules
RANDT and AUX clocks can feed or synchronize generative melodic systems.

### VCAs and filters
Use additional CV channels or envelope modes for dynamic shaping of melodic voices.

### MIDI-connected systems
The manual notes MIDI I/O support from v1.06 onward, including clocks, note outs, and control messages, so Flux can coordinate melodic structures across modular and external synths.

---

## Important caveats for melodic use

The manual warns about parameters that can cause silence. For melodic patches, watch out for:

- **DENS = 0**
- **MASK** muting all effective triggers
- **PHAS** pushing triggers outside step boundaries
- **negative COMP** expanding triggers beyond step length
- **MOD = OFF** if you expect macro/CV modulation on that step

If a melodic line disappears, these are the first things to check.

Also note:
- the CV output range is **0–8V**
- many oscillators expect **1V/oct**, so this is musically useful, but you may want to constrain the range to avoid excessively wide pitch spans
- use **MINV/MAXV** carefully to keep melodies in register

---

## A few concrete melodic patch recipes

## 1. Scale-locked bassline
- CH1 CV out → bass oscillator 1V/oct
- CH1 main out → envelope gate
- CH1 CVSEL = VOLT
- QUAN = 12
- enable minor scale notes in QUAN NODES
- DENS = 1
- SHUF slightly above 0

Result: tight bassline with swing.

## 2. Generative lead
- CH2 CV out → lead voice 1V/oct
- CH2 main out → envelope gate
- CVSEL = RANDS
- MINV/MAXV limited to 1–3V equivalent range
- QUAN = 12 with pentatonic nodes enabled
- PROB < 100
- HUMA moderate
- AUX1 = DEL or 1st for accents

Result: melodic but controlled random lead phrasing.

## 3. Ratcheting arp
- CH3 CV out → oscillator pitch
- CH3 main out → envelope gate
- CVSEL = VOLT
- some steps with high DENS
- CURV and VAL adjusted for acceleration/deceleration
- AUX output triggers filter envelope

Result: animated arpeggio line with timbral articulation.

## 4. Harmony drone with motion
- CH4 CV out = LFO or ENV to modulate filter/FM on another voice
- AUX outs provide divider clocks or logic gates
- another channel handles pitch

Result: Flux provides harmonic motion and expression, not just notes.

---

## Bottom line

Flux can absolutely be used to create **melodic components**, not just drum patterns. Its most useful melodic strengths are:

- **4 independent CV/gate sequencing lanes**
- **per-step fixed or random voltages**
- **built-in quantization and selectable quantization nodes**
- **complex rhythmic articulation**
- **AUX outputs for accents, dividers, logic, and phrase control**
- **deep modulation via macros, CV inputs, and internal LFOs**
- **per-step modulation bus assignment for structured variation**

In practice, Flux is best understood as a **composition and articulation engine**:  
it can generate pitch, timing, dynamics, variation, and phrase structure all at once. If paired with oscillators, VCAs, filters, and envelopes, it can drive entire melodic and harmonic systems with a level of rhythmic sophistication that most pitch sequencers do not offer.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)