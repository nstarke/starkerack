# Abstract Data — ADE-33 Event Boss

- [Manual PDF](../../manuals/ADE33_Manual_v1_0.pdf)

---

[Manual PDF](http://www.abstractdata.biz/downloads/ADE-33_Event_Boss_User_Guide_v1_0_1.pdf)

# Abstract Data ADE-33 Event Boss — using it to create melodic components

The **ADE-33 Event Boss** is not a pitch sequencer by itself. It is a **gate/trigger/rhythm processor and pattern generator**. So for melody, its role is:

- creating **when notes happen**
- creating **phrase structure**
- creating **variations and repetitions**
- switching between melodic sources
- generating rhythmic conditions that drive quantizers, sample & holds, envelopes, sequential switches, logic patches, and transposition events

In a melodic Eurorack patch, think of the ADE-33 as the module that gives your pitch source **musical timing and phrasing**.

---

## What the module does best for melody

From the manual, the ADE-33 processes:

- **clock / gate / trigger / square LFO / PWM LFO inputs**
- **0–5V CV inputs**
- and outputs **0–5V gates/events**

It has:

- **6 Global Modes**
- each with **6 Local Modes**
- input selection between **A1** and **A2**
- CV or event control over **mode selection**
- CV or event control over **A1/A2 switching**

This means it can become the rhythmic brain in front of a melodic chain such as:

- clock → **ADE-33** → envelope → VCA for note articulation
- clock → **ADE-33** → sample & hold trigger → quantizer → oscillator pitch
- two rhythm sources → **ADE-33 logic/probability** → trigger melodic changes
- **ADE-33** output → sequential switch advance → rotate through stored voltages/pitches

---

# Best musical use cases for melody

## 1. Generate note triggers for a quantized melody
This is the most obvious use.

### Patch idea
- Master clock into **IN: GATE A1**
- ADE-33 **OUT** into:
  - envelope generator trigger, and/or
  - sample & hold trigger
- Random CV / sequencer CV / modulation source into pitch path
- Pitch CV then into a **quantizer**
- Quantizer out to oscillator 1V/oct

### Result
ADE-33 determines **which clock pulses become notes**.  
That means it shapes the rhythmic contour of the melody.

### Best modes
- **Global Mode 1: Variables**
- **Global Mode 3: Probability**
- **Global Mode 6: Gates**

These are especially useful for turning a straight clock into:
- sparse melodies
- syncopated motifs
- repeating 8-step phrasing
- evolving note density

---

## 2. Use it as a phrase mask over an existing sequencer
If you already have a CV sequencer producing pitch, the ADE-33 can decide **which steps sound**.

### Patch idea
- Pitch sequencer → quantizer → oscillator pitch
- Same sequencer clock → ADE-33 input A1
- ADE-33 OUT → envelope / LPG / VCA gate

### Result
The pitch sequence keeps running, but only selected steps are heard.  
This creates:
- implied new melodies
- rests
- accents
- phrase reshaping

This is one of the strongest melodic uses of the ADE-33.

---

## 3. Switch between two melodic rhythms
The A1/A2 input selection is very useful.

### Patch idea
- Clock pattern 1 into **A1**
- Clock pattern 2 into **A2**
- Use **A1/A2 SELECT** manually or by CV/event
- OUT triggers a melodic voice or sample & hold

### Result
You can morph between:
- straight notes and syncopated notes
- sparse and dense note streams
- verse and chorus phrasing
- two independent trigger lanes driving one melodic voice

This can make one pitch source feel like multiple composed phrases.

---

# Global modes and how they help with melody

## Global Mode 1: Variables
This is an 8-event patterning system based on a CV-defined variable **n** from 1–8.

### Why it matters melodically
This is great for building:
- repeating note masks
- periodic emphasis
- phrase cycles
- pseudo-sequenced rhythmic motifs

### Good melodic applications
#### Local Mode 1: `<nth> Pass`
Lets every nth event through.

Use this to create:
- regular accents
- every-3rd or every-4th note triggers
- structured ostinatos

#### Local Mode 2: `<nth> Block`
Blocks every nth event.

Use this to:
- remove predictable notes
- create syncopation from a straight clock
- carve holes into a sequence

#### Local Mode 3: `<n> Pass`
Only passes n of 8 events.

Good for:
- note density control
- turning a constant clock into 1/8, 2/8, 3/8... melodic activity

#### Local Mode 4: `<n> Block`
Blocks n of 8 events.

Useful for:
- phrase thinning
- dynamic note omission

#### Local Modes 5 and 6
Hybrid/toggling behaviors. Great for animated patterns when modulated.

### Best melodic pairing
- send slow LFO or envelope into **GATE B/CV**
- use output to trigger **sample & hold + quantizer**
- now the melody breathes in repeating but changing 8-step forms

---

## Global Mode 2: Multiples
Clock multiplication and division.

### Why it matters melodically
This directly changes **note rate**:
- slower divisions = fewer notes, more spacious melodies
- multiplications = ratchets, trills, ornamentation, fast runs

### Great melodic uses
#### Local Modes 1, 3, 5: Divides
Use for:
- reducing note density
- creating half-time or polyrhythmic lead lines
- making one pitch source feel more deliberate

#### Local Modes 2, 4, 6: Multiplies
Use for:
- ratcheting
- repeated notes
- ornamentation
- fast bursts before the next pitch change

### Important patch trick
If your pitch changes more slowly than the multiplied trigger stream:
- one pitch can be retriggered several times
- this creates **ratchets** and **embellishments**

### Example
- Sequencer pitch changes every quarter note
- ADE-33 multiplies gate into 3x or 6x
- envelope retriggers several times on same pitch
- result: melodic flutter or Berlin-school articulation

---

## Global Mode 3: Probability
Pseudo-random chance-based event processing.

### Why it matters melodically
This creates controlled unpredictability in:
- note occurrence
- note length
- phrase variation
- repetition probability

### Best melodic local modes
#### Local Mode 1: Percentage Pass
A note happens only with a chosen probability.

Perfect for:
- generative melodies
- sparse ambient lines
- evolving arps

#### Local Mode 2: Percentage Block
Like above, but from the opposite perspective.

Good when you want a mostly full pattern with occasional omissions.

#### Local Mode 3: Gate Tie
Can tie one note into the next.

Musically this means:
- longer held notes
- legato phrasing
- fewer re-articulations

If your pitch source is stable during the tie, you get sustained tones.  
If pitch changes underneath, you can get glide-like phrase behavior depending on the rest of your patch.

#### Local Mode 4: Gate Tie/Pass
Only tied events pass.

This can create:
- long-note-only melodic moments
- selective sustain gestures
- fewer but more expressive notes

#### Local Mode 5: Flip-Flop (Coin Toss)
Each event has a chance to be “tossed” into high or low.

Great as a generative trigger stream for:
- sample & hold melodies
- transposition triggers
- secondary voice call/response

#### Local Mode 6: Flip-Flop (Inversion)
Chance-based inversion of the gate result.

Useful for making a rhythmic melody line become its own opposite.

### Best melodic pairing
- ADE-33 probability output triggers **sample & hold**
- noise / stepped random / chaotic CV into S&H input
- S&H out into **quantizer**
- quantizer to oscillator pitch

This gives extremely playable melodic generation.

---

## Global Mode 4: Logic
Classic logic between selected A input and B input.

### Why it matters melodically
Logic is powerful for melody because it combines two rhythmic streams into one new note pattern.

### Patch idea
- A1 = master clock division
- A2 = Euclidean rhythm or second trigger source
- B = another gate rhythm
- OUT = melodic gate trigger

### Local modes
- **AND**: notes only when both patterns overlap
- **NAND**: almost inverse overlap behavior
- **OR**: broader note activity
- **NOR**: sparse inverted space
- **XOR**: notes only when one source is high but not both
- **XNOR**: notes when sources agree

### Musical outcomes
This is excellent for:
- interlocking melodies
- call-and-response note masks
- generating new trigger lines from two simple sources
- composing with rhythmic relationships rather than step programming

### Very strong melodic patch
- Source A = regular 16th-note pulse
- Source B = slower modulation pulse
- XOR output triggers melodic voice
- quantized random voltage supplies pitch

Result: melody appears only at changing relational positions.

---

## Global Mode 5: Phase
Phase shifting, delay, and mark/space manipulation.

### Why it matters melodically
Melody is not only pitch and note choice — it is also **placement**.  
This mode changes note timing relative to the beat.

### Useful local modes
#### Quantised Shift / Percentage Shift
Shift triggers later in time.

Good for:
- syncopation
- laid-back melodies
- off-beat counter-melodies

#### Short Shift / Long Shift
Time delay in milliseconds.

Great for:
- echoes in trigger space
- humanized melodic timing
- delayed secondary voice triggering

#### Quantised Mark/Space / Percentage Mark/Space
Changes pulse width / gate length.

Useful for:
- altering articulation
- staccato vs legato behavior
- changing how long envelopes remain open
- affecting portamento behavior in some systems

### Strong melodic use
Duplicate a clock:
- one copy directly clocks your pitch sequencer
- another copy goes through ADE-33 Phase mode to trigger envelopes

Now pitch remains grid-locked, but note articulation shifts in time.  
This can make a melody feel swung, dragged, or offset.

---

## Global Mode 6: Gates
Gate extension and gate-logic-style note shaping.

### Why it matters melodically
This mode is about **articulation** and **phrase length**.

### Useful local modes
#### `<n> High`
Output stays high for n of 8 events.

Can turn pulses into sustained note regions.

#### `<n> High/Low`
Alternating blocks of held and silent time.

Excellent for:
- phrase on/off structure
- drone vs melody alternation
- periodic legato passages

#### Logic Pass
Gate passes depending on input and CV threshold.

Use as a conditional note generator.

#### Logic Hold
Can create held notes based on threshold state.

Very useful if you want:
- sustained melodic notes under CV control
- notes that latch into longer phrases

#### Hybrid modes 5 and 6
Great for animated articulation when CV is moving.

### Best melodic outcome
Use Gates mode after a busy trigger source to make:
- some notes short
- some tied
- some sustained

This gives melodic lines more expressive shape.

---

# Practical melodic patch recipes

## Patch 1: Generative melody from one clock
### Modules needed
- clock
- ADE-33
- sample & hold
- random CV source
- quantizer
- oscillator
- envelope + VCA

### Patch
- Clock → ADE-33 A1
- Slow LFO → ADE-33 B/CV
- ADE-33 OUT → S&H trigger
- Random CV → S&H input
- S&H out → quantizer → oscillator 1V/oct
- ADE-33 OUT also → envelope trigger → VCA

### Suggested mode
- **Global 1 Variables** or **Global 3 Probability**

### Musical result
A melody with stable rhythmic identity but changing note selection.

---

## Patch 2: Ratcheting melodic sequencer
### Patch
- Pitch sequencer → quantizer → oscillator
- Clock → ADE-33 A1
- ADE-33 OUT → envelope trigger
- Set ADE-33 to **Multiples**
- Use CV on B/CV to vary multiplier

### Result
Same melody, but selected notes become repeated bursts.

### Best for
- techno leads
- acid articulation
- arpeggio embellishment

---

## Patch 3: Two-pattern melodic phrase switching
### Patch
- Straight 8th-note clock → A1
- Syncopated trigger pattern → A2
- Use A1/A2 selection manually or by gate/CV
- OUT → envelope trigger for melodic voice
- Pitch source remains the same

### Result
One pitch line, two rhythmic interpretations.

### Why it works
This feels like switching between composed melodic phrases without changing pitch material.

---

## Patch 4: Logic-composed melody
### Patch
- Trigger source 1 → A1
- Trigger source 2 → B/CV
- ADE-33 in **Logic mode**
- OUT → trigger S&H
- Slow CV source into S&H input
- S&H → quantizer → oscillator pitch

### Result
The note timings are generated by interaction of two rhythms, producing emergent melody.

### Best logic mode
- **XOR** for lively syncopation
- **AND** for sparse, intentional notes
- **OR** for fuller melodic lines

---

## Patch 5: Legato and sustain sculptor
### Patch
- Existing melodic trigger pattern → A1
- Slow CV → B/CV
- ADE-33 in **Probability Gate Tie** or **Gates mode**
- OUT → envelope/gate input of voice

### Result
Some notes become tied or held longer, creating more expressive phrasing.

---

## Patch 6: Phase-shifted counter melody
### Patch
- Main clock → mult
- One copy to sequencer clock
- One copy to ADE-33 A1 in **Phase mode**
- ADE-33 OUT triggers second voice envelope or S&H
- Same or related pitch source feeds second voice

### Result
Countermelody lands slightly after or around the main sequence, creating groove and depth.

---

# Best companion modules for melodic use

The ADE-33 becomes especially melodic when paired with:

## Quantizer
Because ADE-33 does not generate pitch itself, a quantizer is essential if you're making melody from sampled CV.

## Sample & Hold / Track & Hold
ADE-33’s output is perfect as a trigger source for capturing voltages as notes.

## Sequential switch
Use ADE-33 OUT to advance through:
- stored voltages
- multiple pitch rows
- transposition sources

## Envelope generator / function generator
Since ADE-33 outputs gates/events, it naturally controls note articulation.

## Clock divider / multiplier / Euclidean trigger source
Feeding rhythmic material into A1, A2, and B makes Logic/Variables/Probability especially rich.

## Precision adder / transposer
Use ADE-33 to trigger when transpositions occur rather than when notes occur.

---

# Performance strategies

## 1. Modulate B/CV slowly
This is the main “musical evolution” input in many modes.  
A slow triangle LFO, random slew, or envelope can make a melody gradually transform.

## 2. Sequence mode changes
The **MODE SELECT/RESET** input can step through local modes or jump by CV.  
That means one melody engine can move through different rhythmic algorithms over time.

This is powerful for:
- verse/chorus differences
- fills
- changing note densities live

## 3. Animate A1/A2 switching
Feed two clocks or trigger patterns and let the module switch between them via gate/CV.  
This is one of the easiest ways to get “composed” phrase variation.

## 4. Use reset/count functions
Several modes use the **MODE SELECT/RESET** input to reset counters or freeze values.  
Resetting phrases against bar lines helps the melody feel intentional rather than drifting.

---

# Limitations to understand

## It does not output pitch CV
So it cannot directly create melodies without external pitch-related modules.

## It reads events rather than syncing like a transport-aware sequencer
Per the manual, it does not “sync” in a DAW-like sense; it just interprets incoming signals.

## Best thought of as a melodic rhythm processor
Its real strength is creating:
- note timing
- articulation
- gate variation
- structural rhythm
- phrase transformations

---

# Most useful modes for melody, ranked

## 1. Probability
Best for generative and evolving melodic triggers.

## 2. Variables
Best for repeatable rhythmic phrases and note masks.

## 3. Multiples
Best for ratchets and note-rate control.

## 4. Phase
Best for groove, swing, delay, and articulation timing.

## 5. Gates
Best for sustain, ties, and phrase-length changes.

## 6. Logic
Best for combining multiple rhythmic sources into melodic trigger structures.

---

# Bottom line

The **ADE-33 Event Boss** is best used for melody as a **rhythmic composer for pitch systems**.  
It does not choose notes, but it can strongly shape melodic identity by controlling:

- when notes occur
- how often they repeat
- whether they are tied or blocked
- how phrases evolve
- how different rhythmic sources combine
- when a melody becomes sparse, dense, swung, delayed, or probabilistic

If you pair it with:
- a **quantizer**
- a **sample & hold**
- a **pitch CV source**
- or an existing sequencer

it becomes a very powerful module for creating melodic phrases that feel alive rather than mechanically stepped.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)