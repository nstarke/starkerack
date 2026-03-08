# 2hp — 3 to 1

- [Manual PDF](../../manuals/3_To_1_Manual.pdf)

---

# [Manual PDF](#)

This manual covers the **2hp 3:1**.

## What this module does musically

The **3:1** is not a pitch generator by itself. It is a **voltage-controlled gate/trigger router and combiner**. That means its role in melodic patching is to decide:

- **which rhythmic source is allowed through**
- **when a melodic event happens**
- **how multiple rhythmic layers are combined**
- **how selection changes over time via CV**

So in a melodic system, the 3:1 is best understood as a **melody animator**, not a melody source. It helps create melodic components by shaping **when notes occur**, **which sequence is heard**, and **how phrasing evolves**.

## Key functions from the manual

- **3 inputs** for gates/triggers: **IN 1, IN 2, IN 3**
- **1 output**: **OUT**
- **Voltage-controlled selection** via:
  - **SEL knob**
  - **SEL CV** input, 0–5V, added to the knob position
- **Two modes**
  - **Switch mode**: routes the currently selected input to the output
  - **Sum mode**: combines selected inputs and outputs **5 ms triggers** regardless of input gate length

## Why that matters for melody

Melody in modular is usually a combination of:

1. **Pitch CV**
2. **Timing / gates**
3. **Articulation**
4. **Variation over time**

The 3:1 directly affects items 2–4.

If you pair it with:
- a sequencer,
- a quantizer,
- a sample-and-hold,
- an envelope/VCA/voice,
- or multiple clock/gate sources,

then the 3:1 becomes a very useful tool for building **musical phrasing and note selection logic**.

---

## Best ways to use the 3:1 for melodic components

## 1. Switching between different melodic rhythms

Patch:
- **IN 1** = simple clock (quarter notes)
- **IN 2** = divided clock (half notes or dotted rhythm)
- **IN 3** = more active trigger pattern
- **OUT** = sequencer advance, quantizer trigger, envelope gate, or voice trigger
- **SEL CV** = slow LFO, stepped random, or another sequencer row

### Result
Your pitch source stays the same, but **the rhythm that triggers notes changes over time**. This creates:
- phrase variation
- call-and-response structures
- evolving melodic density

### Musical use
A simple 8-step melody can feel much more alive if the trigger rhythm changes every bar or every few beats.

---

## 2. Switching between multiple sequencers or pitch-event lanes

Even though the 3:1 switches **gates**, that still helps when running several melodic sources in parallel.

Patch:
- Sequencer A pitch CV -> oscillator pitch
- Sequencer B pitch CV -> precision adder/switch/mixer path
- Sequencer C pitch CV -> another melodic lane
- Their corresponding gate outputs -> **IN 1, IN 2, IN 3**
- **OUT** -> envelope or LPG trigger
- Use the same selection logic elsewhere in the patch to decide which pitch lane is active

### Result
The 3:1 can act as the **rhythmic selector** that determines which melodic lane is currently articulated.

This is especially effective if:
- only one pitch source is active at a time,
- or each gate source corresponds to a different register, transposition, or voice.

### Musical use
You can create the impression of one melody “changing personality” by switching among:
- sparse bass notes
- midrange motif
- high accent notes

---

## 3. Creating melody from one pitch source plus three trigger logics

A common modular trick:
- one pitch CV source generates note values
- triggers determine **which notes are actually heard**

Patch:
- Random stepped CV or sequencer pitch -> quantizer -> oscillator pitch
- **IN 1** = regular clock
- **IN 2** = Euclidean rhythm
- **IN 3** = manual gate / burst / irregular trigger source
- **OUT** = sample-and-hold clock, quantizer trigger, or envelope trigger

### Result
The 3:1 chooses how the pitch stream is articulated. The same stored pitch material produces very different melodies depending on trigger selection.

### Why this is strong
In modular, changing trigger structure often changes perceived melody as much as changing notes.

---

## 4. Voltage-controlled phrase morphing

Because **SEL CV** accepts 0–5V and is added to the knob position, you can automate which input is selected.

Patch:
- **IN 1** = rhythm for verse
- **IN 2** = rhythm for variation
- **IN 3** = dense fill pattern
- Slow modulation into **SEL CV**
- **OUT** -> melodic voice envelope

### Result
The patch slowly drifts between different melodic articulations.

### Good modulation sources
- slow triangle LFO
- stepped random
- sequencer CV row
- envelope from another voice
- keyboard/mod wheel CV

### Musical use
This gives you:
- phrasing changes
- section transitions
- fills and emphasis without repatching

---

## 5. Gate summing mode for richer melodic trigger generation

In **sum mode**, multiple selected channels are combined and the output becomes **5 ms triggers**.

This is very useful for melodic patching because many pitch devices prefer short triggers:
- sample & hold
- sequencers with step advance
- quantizers with trigger input
- envelope generators for plucky notes

Patch:
- **IN 1** = base clock
- **IN 2** = off-beat syncopation
- **IN 3** = ratchet or accent trigger
- Set module to **sum mode**
- Use **SEL/SEL CV** to determine how many sources are active
- **OUT** -> sample-and-hold clock, envelope trigger, or sequencer advance

### Result
As selection increases, your melody becomes more active because additional trigger streams are included.

### Manual behavior that matters
In sum mode:
- far left = **IN 1 selected**
- far right = **IN 1 + IN 2 + IN 3 selected**

So the knob/CV can act like a **density control** for note events.

### Musical use
This is one of the strongest melodic applications of the module:
- low selector setting = sparse melody
- medium = more notes
- high = energetic fills and ornamentation

---

## 6. Turning long gates into short melodic triggers

The manual notes that in **sum mode**, the output emits **5 ms trigger signals regardless of input pulse width**.

That means you can feed it long gates from:
- keyboard gate
- sequencer gate
- clock divisions with long pulse widths

and get short, clean triggers out.

### Why this helps melody
Short triggers are often better for:
- plucked envelopes
- precise sample-and-hold updates
- advancing sequencers cleanly
- clocking quantized random voltages

### Patch idea
- Long gates from three phrase sources into IN 1–3
- Sum mode
- OUT clocks a sample-and-hold that samples a changing CV
- Quantizer after sample-and-hold
- Quantized output to oscillator

### Result
The 3:1 becomes a **melodic event conditioner**, converting broad gate structures into crisp note triggers.

---

## 7. Building melodic fills and accents

Patch:
- **IN 1** = main melody trigger stream
- **IN 2** = occasional fill triggers
- **IN 3** = manually tapped gate button or burst generator
- **OUT** = envelope trigger for lead voice

Use:
- **switch mode** for hard switching between normal phrase and fill phrase
- **sum mode** for layering fills on top of the main phrase

### Result
You can generate:
- temporary melodic embellishments
- phrase endings
- accent clusters
- dynamic lead variations

---

## 8. Using the 3:1 to control when a sequencer advances

Instead of sending OUT directly to a voice, use it to **clock a sequencer** or **advance a shift register**.

Patch:
- **OUT** -> sequencer clock in
- Sequencer CV out -> quantizer/oscillator
- IN 1–3 fed by different clocks/rhythms

### Result
The module determines not just when notes fire, but **when the melody itself moves to the next pitch**.

This can create:
- held notes
- rushed notes
- syncopated advancement
- structural rhythmic variation in the melodic line

### Especially useful with
- 8-step sequencers
- Turing machine style modules
- shift registers
- sample-and-hold melodic patches

---

## 9. Creating call-and-response melodic structures

Patch:
- **IN 1** = sparse trigger pattern for phrase A
- **IN 2** = contrasting trigger pattern for phrase B
- **IN 3** = denser trigger pattern for answer/fill
- **OUT** = melodic voice trigger
- **SEL CV** driven by a slower sequence or manual performance gesture

### Result
The same pitch source can sound like it’s speaking in alternating phrases.

This is a very musical use because melody is often more about **phrasing** than raw note content.

---

## 10. Manual performance control over melody density and phrase choice

The **SEL knob** is performable.

### In switch mode
You can manually choose which rhythmic pattern drives the melody.

### In sum mode
You can manually increase the number of active trigger sources, effectively opening up note density.

This makes the 3:1 a strong **live performance utility** for melodic sets:
- select sparse rhythm for breakdown
- switch to syncopated pattern for groove
- add combined triggers for climax

---

## Important constraints from the manual

A few practical points:

- Inputs are for **gate/trigger signals**, threshold **2.5V**
- **SEL CV** range is **0–5V**
- **OUT** range is **0–5V**
- In **switch mode**, OUT mirrors the selected input
- In **sum mode**, OUT emits **5 ms triggers**
- The module does **not** process pitch CV directly

So if your goal is melodic content, you’ll want to pair the 3:1 with at least one of these:
- sequencer
- quantizer
- random voltage source
- sample-and-hold
- oscillator + envelope/VCA
- clock divider / logic / trigger sequencer

---

## Three especially musical patch recipes

## Patch 1: Evolving quantized random melody
- Noise/random CV -> sample-and-hold input
- **3:1 OUT** -> sample-and-hold clock
- Sample-and-hold -> quantizer -> oscillator pitch
- IN 1 = steady clock
- IN 2 = swung or divided rhythm
- IN 3 = burst/irregular trigger
- SEL CV = slow random or LFO

### What happens
The 3:1 changes when new notes are sampled, creating an evolving melody with shifting rhythmic character.

---

## Patch 2: One sequencer, many phrases
- Sequencer pitch out -> oscillator
- IN 1 = basic step clock
- IN 2 = syncopated trigger pattern
- IN 3 = fill trigger pattern
- OUT = envelope trigger or sequencer advance
- MODE = switch mode

### What happens
The same note sequence gets rephrased in multiple ways, which sounds like variations on a melodic theme.

---

## Patch 3: Density-controlled arpeggio generator
- Arpeggiator/sequencer pitch -> oscillator
- IN 1 = quarter-note trigger
- IN 2 = eighth-note trigger
- IN 3 = ratchet/accent trigger
- MODE = sum mode
- SEL CV = envelope, slider, or sequencer row
- OUT = envelope trigger

### What happens
As selection rises, the arpeggio becomes denser and more energetic, ideal for builds and transitions.

---

## Bottom line

The **2hp 3:1** is best used for melody as a **trigger architecture tool**:

- it selects between rhythmic sources,
- combines them for note density,
- converts gates to short triggers in sum mode,
- and allows CV-controlled phrase changes.

By itself it doesn’t generate notes, but in a melodic Eurorack patch it can be central to:
- note timing,
- phrase switching,
- melodic density,
- variation,
- and live performance control.

If you want, I can also turn this into:
1. a **beginner-friendly patch guide**,  
2. a **generative melody patch recipe list**, or  
3. a **“how to use with common module types” compatibility guide**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)