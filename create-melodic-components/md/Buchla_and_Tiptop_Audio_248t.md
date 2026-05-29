# Buchla and Tiptop Audio — 248t

- [Manual PDF](../../manuals/Buchla_&_Tiptop_Audio_248t.pdf)

---

[248t MARF Manual PDF](https://tiptopaudio.com/manuals/248t/248t_user_manual.pdf)

# Using the Tiptop/Buchla 248t MARF to Create Melodic Components

The **248t MARF (Multiple Arbitrary Function Module)** is essentially a highly programmable **16-stage melodic and timing sequencer/function generator**. From the manual, the most important musical idea is this:

- each **stage** stores:
  - a **voltage**
  - a **time**
  - optional **gate/pulse assignments**
  - optional **pitch behavior** like **quantize**, **slew/sloped**, and **range limits**
  - optional **performance logic** like **stop**, **sustain**, **enable**, **first**, and **last**

Used together with oscillators such as the **259t** and supporting modules like envelopes/LPGs, it can generate melodies, glides, phrases, transpositions, rhythmic variation, and semi-generative note structures.

---

## Relevant modules mentioned in the manual

The manual explicitly describes using the **248t** with:

- **259t oscillator**
  - especially via **ART output** for precise pitch control
  - firmware update recommended for correct ART high-speed pitch slide behavior
- **292t LPG**
  - via the **Reference Output** for a natural decaying control shape
- external CV sources patched into inputs **A–D**
  - for modulating stage voltage or stage time

So the core “melodic system” here is:

- **248t** = pitch/timing/programming brain
- **259t** = sound source
- **292t or envelope/VCA/LPG** = articulation
- optional other CV/gate utilities = variation and control

---

# What the 248t contributes melodically

## 1. Per-stage pitch sequencing

The **Output Voltage Level** sliders define the pitch value for each of the 16 stages.

That means you can create:

- traditional step melodies
- repeating riffs
- evolving phrases
- non-repeating melodic contours

When **Quantize** is enabled on a stage, the voltage becomes musically constrained to a scale. The manual says quantized output is **1V/Oct** in Eurorack.

This makes the 248t much more than a free-running CV sequencer: it can act as a **scale-aware melodic sequencer**.

---

## 2. Scale and key control

The preset/scale section lets you choose:

- **Key**: C through B
- **Scale**:
  - **Major**
  - **Minor**
  - **Chromatic**

This is very useful for melody writing because you can:

- sketch a melodic contour with the sliders
- enable **Quantize** on chosen stages
- then shift the whole phrase into a different key quickly
- swap between major/minor flavors without reprogramming the sliders

### Practical musical use
- Build a 16-step contour by ear
- Quantize all stages
- Choose **C minor**
- Save as preset 1
- Change to **Eb major** and save as preset 2
- Now you have two harmonically related versions of the same phrase

---

## 3. Glides and portamento between notes

The **Sloped/Stepped** stage modifier is one of the most musically valuable features.

- **Stepped** = classic sequencer note jumps
- **Sloped** = pitch glides between stages

The manual notes that slew time is based on the **interval time** of the stage, and the 259t ART firmware update enables **accurate pitch slides and glide effects** from the MARF.

### This enables:
- acid-like slides
- Buchla-style fluid melodic motion
- expressive phrase transitions
- hybrid sequences where some notes are discrete and others melt into the next

A strong trick is to make only a few stages **sloped**, so the melody is mostly stepped but includes intentional legato slides.

---

## 4. Variable note lengths per stage

The **Interval Time** sliders determine how long each stage lasts.

This means melody is not locked to equal note values. You can program:

- long-held tones
- short passing notes
- uneven phrase structures
- rubato-like movement
- repeating patterns with internal rhythmic asymmetry

This is a major reason the MARF feels musical rather than just mechanical.

### Example
In a 16-stage phrase you might set:

- stage 1 = long tonic
- stages 2–4 = shorter ornament notes
- stage 5 = medium duration
- stage 6 = very short pickup
- stage 7 = long destination note

Now the pitch sequence also becomes a phrase with articulation and direction.

---

## 5. Independent gate programming for note articulation

Each stage can independently output:

- **Pulse 1**
- **Pulse 2**

These are separate programmable gate streams.

This lets you separate **pitch movement** from **articulation**.

### Musical possibilities
- every stage changes pitch, but only some stages fire an envelope
- one pulse stream triggers a main voice
- the other pulse stream triggers an accent, second envelope, second oscillator, or percussion
- legato phrases can be created by sliding pitch across stages without retriggering every note

This is extremely useful melodically because not every pitch change must become a newly articulated note.

---

# Best ways to combine the 248t with the 259t for melody

## A. ART pitch sequencing into the 259t

The manual recommends using the **black ART output** of the MARF into the **259t ART input** and setting the oscillator to **ART mode**.

Why this matters:

- pitch is digitally communicated for precision
- slides/glides are handled accurately
- better integration than ordinary CV in this specific ecosystem

The switch above the ART outputs selects the gate source:

- **Pulse 1**
- **Pulse 2**
- **ALL**

So the MARF can send pitch and gate behavior in a tightly integrated way.

### Musical result
This makes the 248t + 259t pair behave like a highly expressive melodic voice generator:
- stage-based pitches
- programmable note lengths
- selective retriggers
- scale quantization
- glide
- structured looping

---

## B. Voltage output for standard 1V/oct melodic sequencing

The **blue Voltage Output** jack can be used as standard pitch CV.

Use this when:
- controlling a non-ART oscillator
- multing pitch to multiple oscillators
- layering voices
- sending pitch elsewhere, such as quantizer-adjacent or modulation destinations

If a stage is quantized, the output behaves musically in **1V/oct** terms.

So even without the 259t, the 248t is a serious melodic sequencer for any Eurorack oscillator.

---

## C. Reference output into a 292t LPG

The manual notes the **Reference Output** produces a **downward ramp spanning the interval time of the stage**, and is useful for directly driving a **292t LPG** without a separate envelope.

This is a very Buchla-style melodic patch.

### Patch concept
- 248t pitch out/ART out -> 259t pitch
- 259t audio -> 292t audio in
- 248t reference out -> 292t CV in

Result:
- each note gets a shaped decay related to the programmed stage length
- long stages create longer decays
- short stages create tighter plucks
- melody and articulation remain linked in a very organic way

This is one of the most elegant “melodic voice” uses described in the manual.

---

# Advanced melodic techniques from the manual’s feature set

## 1. Create phrase loops with First/Last stage markers

The **First** and **Last** operating mode modifiers define the cycle boundaries.

This means your 16 stages do not need to behave as one fixed 16-step loop. You can create:

- 3-note motifs
- 5-step loops
- 7-step polymetric phrases
- 9-stage melodies inside a larger programmed grid

### Why this matters musically
Odd-length melodic loops create evolving relationships against regular drum patterns.

For example:
- set a 5-stage melodic phrase
- run it against a 4/4 rhythm
- the phrase shifts against the bar line over time

This is one of the easiest ways to get “alive” melodies.

---

## 2. Use Stop, Sustain, and Enable as melodic phrase logic

These are not just utility functions—they are compositional tools.

### Stop
A stage marked **Stop** halts advance until a start pulse is received.

Use it to:
- create phrase endings
- make melodic fragments that wait for external trigger
- build call-and-response structures

### Sustain
A stage with **Sustain** holds while a high gate is present at the start input.

Use it to:
- extend important melody notes
- create performable held tones
- let an external keyboard gate or sequencer decide note duration

### Enable
A stage with **Enable** waits until voltage above 5V is received at the start input.

Use it to:
- probabilistically unlock notes
- tie melodic advancement to another sequencer or logic source
- make generative melodies that only proceed when certain conditions occur

Together, these let melody behave like a reactive musical system, not just a fixed pattern.

---

## 3. External CV inputs A–D for transposition and melodic variation

The 248t has four external CV inputs that can be used either for **timing** or for **voltage source processing**.

For voltage programming, if a stage’s source is set to **External**, the slider selects **A, B, C, or D** instead of directly setting pitch.

This is powerful.

### Melodic uses
- one stage uses internal programmed note
- another stage pulls pitch from external CV A
- another from CV B
- some stages are fixed, some are externally driven

So a melody can mix:
- fixed composition
- transposition input
- random CV
- another sequencer’s CV
- keyboard CV

### Example use
- Input A = slow transposition CV
- Input B = random stepped voltage
- Input C = keyboard pitch
- Input D = second sequencer row

Then assign different stages to different sources. The melody becomes a hybrid between composed and live/generated material.

---

## 4. Time output as a second melodic/modulation source

The manual states the **Time Output** emits a CV based on the interval time slider. If time source is set to **External**, this can be used as a second CV source without affecting timing.

This is very useful for coordinated melodic patches.

### Example uses
Use time CV to modulate:
- oscillator timbre
- wavefold amount
- LPG response
- filter cutoff
- FM amount

Now note duration and timbre can be related:
- long notes are darker or brighter
- short notes are more percussive
- specific phrase shapes become timbral as well as melodic

This creates “melodic components” that feel more expressive and less flat.

---

## 5. All Pulses output as a master clock or articulation layer

The **All Pulses Output** sends a pulse each time a new stage is addressed.

Use it to:
- trigger a second envelope on every stage
- clock another sequencer or divider
- synchronize melodic accompaniment
- add a regular articulation layer while Pulse 1/Pulse 2 remain selective

For melody, this allows multiple layers of articulation:
- selective note trigger from Pulse 1
- accent trigger from Pulse 2
- every-step utility clock from All Pulses

---

# Practical patch ideas for melodic music

## Patch 1: Classic 16-step tonal melody
**Goal:** stable musical sequence with quantized notes

Patch:
- 248t Voltage Out or ART Out -> oscillator pitch in
- Pulse 1 Out -> envelope gate in
- envelope -> VCA/LPG CV
- oscillator audio -> VCA/LPG -> mixer

Program:
- set 16 pitch sliders by ear
- enable **Quantize** on all stages
- choose **Key** and **Major/Minor**
- set mostly equal interval times
- assign Pulse 1 to notes you want articulated

Result:
- conventional but very expressive sequenced melody

---

## Patch 2: Sliding lead line
**Goal:** expressive melody with selected portamento

Patch:
- 248t ART Out -> 259t ART In
- Pulse 1 -> envelope
- 259t -> LPG/VCA

Program:
- quantize stages
- set some stages to **Sloped**
- vary interval time per stage
- use half-range for easier pitch programming
- set pulse only on certain notes for legato feel

Result:
- some notes retrigger, others glide into the next, very playable and lyrical

---

## Patch 3: Buchla-style plucked melodic voice
**Goal:** melody and dynamics linked without separate envelope complexity

Patch:
- 248t ART/Voltage Out -> 259t pitch
- 259t audio -> 292t input
- 248t Reference Out -> 292t CV in
- optional Pulse 1 -> extra strike or transient source

Program:
- mix short and long interval times
- use quantize on desired stages
- add slope to some notes

Result:
- each note gets a natural decay contour tied to its stage duration

---

## Patch 4: Generative melody with controlled randomness
**Goal:** semi-predictable melodic movement

Patch:
- random stepped CV -> External Input A
- slow transposition CV -> External Input B
- 248t Voltage Out -> oscillator pitch
- Pulse 1 -> envelope
- All Pulses -> clock for another modulation source

Program:
- some stages set to **Internal** voltage
- some stages set to **External** voltage
- sliders select A or B on those external stages
- use First/Last to make an odd-length loop
- use Enable on a few stages, controlled by external gates

Result:
- recurring motif with occasional external-note injection and evolving phrase structure

---

## Patch 5: Two melodic articulations from one phrase
**Goal:** one pitch line, two rhythmic interpretations

Patch:
- one 248t pitch output -> oscillator 1 and oscillator 2
- Pulse 1 -> envelope/VCA for voice 1
- Pulse 2 -> envelope/VCA for voice 2

Program:
- same pitch sequence feeds both voices
- Pulse 1 triggers main notes
- Pulse 2 triggers syncopated notes or accents

Result:
- one melodic contour produces two interlocking musical layers

---

# Why the 248t is especially strong for melody

Compared with many step sequencers, the manual shows the 248t is unusual because it combines:

- **pitch programming**
- **per-stage time programming**
- **per-stage articulation**
- **per-stage quantization**
- **per-stage glide**
- **external CV substitution**
- **loop boundary logic**
- **conditional advancement behavior**

That means it does not just produce “notes in order.” It produces:

- **phrases**
- **contours**
- **timed gestures**
- **responsive melodic structures**

In practice, this makes it excellent for:

- lead lines
- bass sequences
- generative motifs
- evolving tonal patterns
- plucked Buchla-style sequences
- gliding electronic melodies

---

# Important setup notes from the manual

## 259t preparation
Before using the 248t with the 259t via ART:

- update the **259t ART firmware**
- confirm status on power-up:
  - all range LEDs off = update needed
  - high LED on = update done

If ART hasn’t been used before, **initial tuning** may be required.

---

## Recommended pitch range
The manual recommends using the 248t in:

- **Half range (5 octave)** or
- **Limited range**

when pairing with the 259t, to avoid notes outside the oscillator’s range.

This is also musically useful because smaller voltage ranges make it easier to dial in intentional melodies.

---

## Presets for composition
You can save **12 presets**, including slider values and stage settings.

This is very useful for melodic composition:
- verse phrase
- chorus phrase
- transposed variation
- alternate mode
- denser articulation version

Because the 248t is deep, preset recall makes it practical in real music rather than just experimentation.

---

# Best overall melodic workflow

A very effective workflow from the manual’s feature set is:

1. **Set a loop length** with First/Last
2. **Dial pitch contour** with output voltage sliders
3. **Set stage durations** with interval time sliders
4. **Enable quantize** where needed
5. **Choose key/scale**
6. **Add slope** to selected transitions
7. **Program Pulse 1/2** for articulation
8. **Use Reference or envelopes** for dynamics
9. **Save presets** for alternate phrases
10. **Introduce external CV** on selected stages for variation

This turns the 248t into a full melodic composition engine.

---

# Summary

From the manual, the **248t MARF** is best understood as a **deeply programmable melodic sequencer/function generator** that works especially well with the **259t oscillator** and **292t LPG**.

Together they can create melodic components such as:

- quantized tonal sequences
- gliding leads
- variable-length note phrases
- articulated basslines
- Buchla-style plucked melodies
- generative melodic systems
- transposable motifs
- multi-layer rhythmic/pitch interactions

The strongest pairings described are:

- **248t ART Out -> 259t ART In** for precise melodic pitch and slides
- **248t Pulse outputs -> envelopes/LPG triggers** for note articulation
- **248t Reference Out -> 292t CV In** for dynamic, duration-linked shaping

If you want, I can also turn this into:
1. a **beginner patch cookbook**,
2. a **“melodic patch recipes” table**, or
3. a **signal-flow diagram** in markdown.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)