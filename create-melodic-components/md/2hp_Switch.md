# 2hp — Switch

- [Manual PDF](../../manuals/2hp_Switch.pdf)

---

[Manual PDF](#)

# 2hp Switch: using it for melodic patching

The attached manual is for the **2hp Switch**, a **4-in / 1-out voltage-controlled signal router**. It can switch **audio, CV, or gate signals**, and the active input can be chosen either by the **SEL knob** or by **SEL CV**.

## What the module does

### Core behavior
- **4 inputs**
- **1 output**
- Routes **one selected input** to the output
- Selection can be:
  - set manually with the **SEL** knob
  - changed dynamically with **SEL CV**

### Important specs from the manual
- **Input level:** ±10V
- **SEL CV range:** ±5V
- **CV is added to the current knob position**
- **Very fast switching**, low noise
- Works with:
  - audio
  - control voltage
  - gates/triggers

---

# How Switch helps create melodic components

Even though Switch is not a pitch generator by itself, it is very useful for **melody construction**, because melodies in Eurorack are often built by choosing between:
- different pitch CV sources
- different rhythmic gate streams
- different transpositions
- different quantized sequences
- different audio voices playing melodic material

Switch is basically a **decision point** in the patch. It lets you create melodies by selecting which source is currently active.

---

# Best melodic use cases

## 1. Switch between multiple pitch CV sources

Patch four different pitch-related CVs into the inputs:
- Input 1: a sequencer line
- Input 2: a random voltage source
- Input 3: a transposed copy of the sequencer
- Input 4: a slow modulation source into a quantizer

Then send **OUT** to:
- a quantizer input, then to oscillator 1V/oct
- or directly to an oscillator if the voltages are already musical

### Result
You get a melody that can jump between four different pitch behaviors.

### Why this works musically
This is one of the easiest ways to create:
- verse/chorus-like variation
- call-and-response melodic motion
- controlled unpredictability

---

## 2. Switch between different transpositions of the same sequence

A very musical patch is to mult one melodic CV sequence into several processors:
- Input 1: original sequence
- Input 2: sequence + 2 semitones
- Input 3: sequence + 5 semitones
- Input 4: sequence + 7 semitones

Send the output to your oscillator pitch path.

### Result
The same melodic contour is preserved, but the active harmony changes.

### Musical effect
This gives you:
- modal shifts
- chord-root movement
- bassline variation
- instant harmonic structure from one phrase

If you clock the switching rhythmically, you can make the melody outline harmonic changes without needing a second sequencer.

---

## 3. Switch between quantizer inputs or quantized outputs

If you have a quantizer in the system, Switch becomes especially useful.

### Option A: switch unquantized sources into one quantizer
- Inputs: different modulation/pitch CV sources
- OUT → quantizer → oscillator

This makes four raw sources become one playable melodic stream.

### Option B: switch between already-quantized melodies
- Inputs: four different quantized pitch lines
- OUT → oscillator 1V/oct

This is cleaner if each source already has a distinct scale or pattern.

### Musical effect
You can move between:
- stable melody
- semi-random melody
- arpeggio-like motion
- transposed variations

---

## 4. Switch gate patterns that drive melodic events

Melody is not just pitch; it is also **when notes happen**.

Patch four gate or trigger sources into Switch:
- Input 1: straight clock division
- Input 2: syncopated trigger pattern
- Input 3: random triggers
- Input 4: Euclidean rhythm

Then send **OUT** to:
- envelope trigger input
- sequencer advance input
- sample-and-hold trigger
- quantizer trigger, if applicable

### Result
You can keep the same pitch source but radically change the melodic phrasing.

### Why this matters
A single pitch sequence can sound like entirely different melodies when the note timing changes.

---

## 5. Switch audio from different melodic voices

Because Switch also handles audio, you can patch:
- Input 1: sine lead
- Input 2: square bass voice
- Input 3: filtered pluck
- Input 4: FM voice

Then switch which voice reaches the output.

### Result
One melodic line can jump between different timbres or instruments.

### Performance use
This is great for:
- live arrangement
- fills
- alternating lead sounds
- turning one sequence into a multi-voice phrase

Because the module switches quickly, it can create abrupt, stylized phrase changes.

---

## 6. Create stepped melodic selection with CV over SEL

The most interesting part of this module is **SEL CV**.

Since the **SEL CV is added to the knob position**, you can offset the range manually and then animate selection with another CV source.

Patch a CV source to SEL:
- stepped random voltage
- sequencer CV lane
- LFO
- sample & hold
- gate-derived stepped voltage

### Result
The chosen melodic source changes over time automatically.

### Musical uses
- every bar, choose a different sequence
- probabilistic melody path changes
- evolving motif selection
- generative melodic arrangement

This turns Switch into a kind of **meta-sequencer**, where it sequences which sequence is active.

---

# Example melodic patches

## Patch 1: Four-part melodic phrase selector
**Goal:** build a melody from four phrase fragments.

### Patch
- Input 1: phrase A pitch CV
- Input 2: phrase B pitch CV
- Input 3: phrase C pitch CV
- Input 4: phrase D pitch CV
- OUT → quantizer or oscillator 1V/oct
- Clocked stepped CV → SEL CV

### What happens
Each incoming control step at SEL chooses a different phrase source. Instead of one linear melody, you get a modular phrase system.

### Great for
- generative leads
- evolving basslines
- non-repeating motifs

---

## Patch 2: Harmonic movement from one sequence
**Goal:** use one sequence to imply chord changes.

### Patch
Take one sequence and create 4 versions:
- Input 1: root
- Input 2: +3 or +4 semitones
- Input 3: +7 semitones
- Input 4: +12 semitones

- OUT → oscillator pitch
- slow clocked CV or manual changes → SEL

### What happens
The same melodic shape moves through harmonic positions.

### Great for
- basslines
- ostinatos
- techno hooks
- arpeggiated motifs

---

## Patch 3: Gate-switched melody articulation
**Goal:** change note rhythm while keeping pitch constant.

### Patch
- Pitch sequencer → oscillator pitch
- Inputs 1–4: four different gate patterns
- OUT → envelope trigger

### What happens
The same pitch material gets different rhythmic articulation depending on which gate stream is active.

### Great for
- turning a loop into a song structure
- creating fills
- live improvisation

---

## Patch 4: Random-but-musical note source selector
**Goal:** mix predictable and unpredictable melody sources.

### Patch
- Input 1: sequencer
- Input 2: sequencer transposed up a fifth
- Input 3: random stepped CV
- Input 4: slow envelope or LFO into quantizer
- OUT → quantizer → oscillator
- Sample & hold or random stepped CV → SEL CV

### What happens
The melodic voice alternates between stable and unstable sources.

### Great for
- generative ambient
- experimental melodies
- evolving Berlin-school style patterns

---

## Patch 5: Timbral melody switching
**Goal:** one melody, multiple instrumental identities.

### Patch
- One pitch sequence controls several oscillators/voices
- Audio outputs of those voices → Inputs 1–4
- OUT → filter/VCA/mixer
- rhythmic CV → SEL CV

### What happens
Different notes or note groups appear with different timbres.

### Great for
- melodic fills
- pseudo-round-robin voicing
- choppy electro phrasing

---

# Practical advice for melodic use

## Use quantization when switching pitch CV
If the inputs contain free CV rather than tuned pitch, the output may jump to non-musical voltages. Sending **OUT** to a **quantizer** makes the result much more melodic.

## Use slow or clocked CV for intentional source changes
If SEL CV moves too freely, the routing may change too often. For more musical results:
- use stepped voltages
- sample-and-hold
- sequencer rows
- clock divisions

## Use the knob as a bias or range control
Because the CV is **added to the knob position**, the knob can act like a manual “center” or source preference. This is useful in performance.

## Great for form and arrangement
Switch is especially strong at the **phrase level**:
- choose which melody source is active this bar
- choose which rhythm drives the melody
- choose which transposition is active in the chorus

So it is less a note sequencer, and more a **melodic structure and variation tool**.

---

# Strengths of this module in melodic systems

## Excellent for:
- selecting between melodic CV lanes
- switching transpositions
- switching quantized sources
- changing rhythmic articulation
- routing different audio voices
- generative melody structures

## Less ideal for:
- smooth crossfades between sources
- polyphony
- direct note creation without external CV/audio sources

This is a **router**, not a sequencer or quantizer. Its power comes from how you combine it with those modules.

---

# Bottom line

The **2hp Switch** is best understood as a **melodic selector and structure tool**. It creates musical interest by choosing among:
- multiple pitch sources
- transposed variants
- different rhythm generators
- different melodic voices

In a Eurorack patch, that makes it extremely useful for:
- evolving melodies
- performance variation
- generative composition
- compact harmonic movement

If you want, I can also turn this into:
1. a **beginner-friendly patch recipe list**,  
2. an **advanced generative melody guide**, or  
3. a **“best modules to pair with 2hp Switch” companion chart**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)