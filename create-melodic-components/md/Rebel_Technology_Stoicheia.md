# Rebel Technology — Stoicheia

- [Manual PDF](../../manuals/Stoicheia – Rebel Technology.pdf)

---

[Manual PDF / Source](https://www.rebeltech.org/product/stoicheia/)

# Rebel Technology Stoicheia: using it for melodic components

Stoicheia is **not a pitch sequencer**. It’s a **dual Euclidean trigger/gate sequencer**. So its role in melody-making is to create the **rhythmic structure** that drives melodic events: when notes happen, how often they happen, how two lines interlock, and how phrase lengths evolve.

## What the module does
From the manual:

- **Dual Euclidean sequencer**
- Two independent sequences
- Each side has:
  - **Length**: 1–16 steps
  - **Fills**: how many active beats
  - **Rotation**: shifts the pattern start point
  - **Mode switch**:
    - Off
    - **Trigger mode**
    - **Alternating mode**
- Shared functions:
  - **Reset input**
  - **Manual reset**
  - **Chained mode** to play seq A then seq B as one longer pattern

Outputs are gates around **0V / 5.1V**, so they’re ideal for triggering envelopes, clocks, sample & holds, logic, switches, and many quantizer/sample functions.

---

# How Stoicheia contributes to melody

To make melody in Eurorack, you usually need these building blocks:

1. **Pitch source**  
   quantizer, sequencer, random voltage, joystick, keyboard, S&H, etc.

2. **Rhythm / note timing**  
   this is where **Stoicheia** shines

3. **Articulation**  
   envelopes, VCAs, accents, legato/tied gates

4. **Phrase structure**  
   resets, polymeter, pattern chaining, variation

Stoicheia mainly handles **2, 3, and 4**.

---

# Best melodic uses

## 1. Triggering notes from a pitch source
Patch idea:

- Clock/LFO → Stoicheia clock input
- Stoicheia output A → envelope gate input
- Envelope → VCA CV
- Oscillator → VCA → filter/output
- Separate CV sequencer or quantized random voltage → oscillator 1V/oct

Result:
- Pitch source determines **what note**
- Stoicheia determines **when the note speaks**

This is the most direct melodic use. Even a simple 8-note pitch loop becomes musical when Euclidean spacing changes the note onsets.

### Why it works
Euclidean rhythms distribute pulses evenly, so note timing often feels balanced and musical:
- sparse fills = airy melodic fragments
- dense fills = active arpeggio-like lines
- rotation = syncopation without rewriting pitches

---

## 2. Using the two channels for melody + accent
Since Stoicheia has two sequences, one can drive notes and the other can shape emphasis.

Patch idea:

- Seq A output → main envelope trigger
- Seq B output → accent envelope or filter envelope trigger
- Pitch sequencer → oscillator pitch
- Seq B also to a second VCA/CV input for louder accented notes

Result:
- A note line plays on Seq A
- Seq B adds accents on selected steps
- The same pitch pattern feels far more melodic because phrasing emerges

Good settings:
- A = E(5,8) type density
- B = E(3,8) or E(2,5)-like accent rhythm
- Rotate B relative to A for evolving accents

---

## 3. Triggering sample-and-hold for stepped melodies
One of the strongest pairings:

- Noise / random CV / smooth CV / LFO → Sample & Hold input
- Stoicheia output A → S&H trigger
- S&H output → quantizer → oscillator pitch
- Same Stoicheia output or another gate → envelope

Result:
- Stoicheia creates the rhythm of pitch changes
- Quantizer turns random voltages into scales
- You get Euclidean melodies instantly

### Variations
- Use **Seq A** to sample new pitches
- Use **Seq B** to trigger the envelope

This creates:
- some pitches change without sounding immediately
- some notes repeat the same pitch before a new one is sampled

That’s a classic trick for more intentional-sounding melodic lines.

---

## 4. Creating call-and-response melodies
Because Stoicheia is dual, you can patch two voices:

- Seq A → envelope/VCA for voice 1
- Seq B → envelope/VCA for voice 2
- Different pitch sources or related quantized voltages to each oscillator

Result:
- two interlocking melodic lines
- one can answer the other
- differing lengths/fills create evolving counterpoint

Example:
- Voice 1: length 8, fills 3
- Voice 2: length 5, fills 2
- Same master clock to both

This yields polymetric melodic interplay that cycles over a long phrase.

---

## 5. Driving a sequential switch for melodic order changes
Patch idea:

- Several fixed voltages, row outputs, or interval sources → sequential switch inputs
- Stoicheia output A → switch advance
- Switch output → quantizer → oscillator pitch
- Stoicheia output B → envelope gate

Result:
- Seq A determines when the next pitch source is selected
- Seq B determines when notes are articulated

This separates:
- **pitch movement**
- **note articulation**

That separation is extremely useful for building melodies that feel composed rather than merely random.

---

## 6. Alternating mode as melodic gate/tie generator
The manual says **Alternating Mode** toggles output high on each “on” beat and stays high until the next “on” beat.

Musically, this is excellent for:

- **tied notes**
- **legato phrasing**
- **phrase masks**
- **sub-octave or harmonic switching**
- **opening/closing a VCA or wavefolder over longer spans**

Patch idea:
- Seq A in Trigger mode → main note triggers
- Seq B in Alternating mode → controls:
  - VCA level for drone layer
  - filter mode switch via logic/comparator
  - slew enable / glide gate
  - sequential switch between two pitch rows

Result:
- the melody has sections of connected phrasing or changing harmonic color

A very useful melodic application:
- Trigger mode handles note attacks
- Alternating mode defines **longer melodic gestures**

---

## 7. Chained mode for longer melodic phrases
In **Chained mode**, sequence A plays, then sequence B plays, one after another, available at both outputs.

This is powerful for melody because it creates phrase lengths beyond a single short loop.

Example:
- Seq A length 12 fills 5
- Seq B length 4 fills 2

Now you have a 16-step composite rhythm with uneven internal structure.

Use this to:
- trigger a quantized CV source
- advance a pitch sequencer at non-uniform points
- make verse-like / response-like melodic phrasing

Especially effective if the pitch material is also 16 steps or longer.

---

## 8. Rotating patterns to reshape a melody without changing pitch
The **rotation** control changes where the Euclidean pattern begins.

If your pitch sequence stays fixed and only rhythm rotates:
- the melody becomes newly syncopated
- downbeats shift
- the same notes feel reharmonized against the bar

This is one of the easiest live-performance tools on Stoicheia.

Try:
- fixed 8-step pitch sequence
- Seq A length 8 fills 5
- move rotation slowly

The pitch order remains unchanged, but perceived melodic contour changes because note emphasis moves.

---

## 9. Different sequence lengths for melodic polymeter
Each channel can have independent lengths. This is gold for melody.

Example:
- Seq A: length 7, fills 3
- Seq B: length 11, fills 4

Use cases:
- A triggers pitch changes
- B triggers envelopes
- or A/B trigger two related voices

This creates long non-repeating melodic structures from simple material.

A favorite patch:
- A → S&H trigger for new note selection
- B → envelope trigger for audible note events

Because pitch-update rhythm and note-output rhythm differ, the line develops a semi-generative melodic identity.

---

# Practical patch recipes

## Patch 1: Euclidean arpeggio
**Goal:** rhythmic melodic ostinato

- Master clock → Stoicheia clock A
- Stoicheia output A → envelope trigger
- Quantized CV sequence/arpeggiator → oscillator 1V/oct
- Envelope → VCA
- Oscillator → VCA → mixer

Suggested settings:
- Length 8
- Fills 5
- Rotate to taste
- Trigger mode

This gives a classic syncopated arp line.

---

## Patch 2: Generative melody with controlled repetition
**Goal:** melodic randomness with coherent rhythm

- Slow random CV → S&H input
- Stoicheia output A → S&H trigger
- S&H out → quantizer → oscillator 1V/oct
- Stoicheia output B → envelope trigger
- Envelope → VCA

Suggested settings:
- A: length 5, fills 2
- B: length 8, fills 5

Why it works:
- pitch changes and audible notes happen on different schedules
- repeated notes emerge naturally
- melody feels intentional instead of purely random

---

## Patch 3: Two-voice counterpoint
**Goal:** interlocking melodic lines

- Same clock to Stoicheia
- Seq A → envelope 1
- Seq B → envelope 2
- Pitch source 1 → osc 1
- Pitch source 2 → osc 2
- Both voices mixed together

Suggested relationships:
- Voice 1 brighter / higher register
- Voice 2 lower / slower attack
- Rotate B off from A

Good settings:
- A = 8 steps / 3 fills
- B = 5 steps / 2 fills

You get compact polymelodic interplay.

---

## Patch 4: Accent + melody line
**Goal:** one melodic voice with dynamic phrasing

- Seq A → main envelope gate
- Seq B → filter envelope trigger or accent VCA CV
- Pitch sequencer → oscillator
- Main envelope → VCA
- Accent envelope → filter cutoff or VCA CV depth

Settings:
- A denser than B
- B rotated to avoid obvious downbeat accents

This makes a simple melody breathe.

---

## Patch 5: Euclidean note selection
**Goal:** switch between pitch sources rhythmically

- Fixed voltages / sequencer rows / intervals → sequential switch inputs
- Seq A → switch advance
- Switch output → quantizer → oscillator pitch
- Seq B → envelope trigger

This creates melodies from source selection rather than from one continuous pitch sequencer.

---

# Performance strategies

## Use one channel for structure, one for surprise
A very musical setup is:
- **Seq A:** stable, medium density, main notes
- **Seq B:** sparse, rotated, for accents / secondary voice / pitch refresh

That gives you both familiarity and movement.

## Change fills before changing length
For live melodic evolution:
1. keep length fixed
2. vary fills
3. then rotate
4. then change length

This tends to preserve groove while evolving the melody.

## Use reset musically
The reset input/manual reset is useful when:
- syncing phrase starts to a bar
- re-aligning two melodic voices
- forcing a generative patch to “come home”

## Chained mode for section changes
Use chained mode to move from:
- phrase A
- into phrase B
- then repeat

Great for melodic hooks that need asymmetry.

---

# Limits to understand

Stoicheia does **not** generate pitch CV on its own. To build full melodic content, pair it with at least one of these:

- quantizer
- CV sequencer
- random voltage source
- sample & hold
- keyboard/controller
- precision adder
- sequential switch

Think of Stoicheia as the **rhythmic brain** of a melody patch.

---

# Most effective module pairings for melodic work

Stoicheia works especially well with:

- **Quantizer**  
  turns triggered/random voltages into scale-based melodies

- **Sample & Hold**  
  generates stepped pitch events at Euclidean timings

- **Sequential switch**  
  creates melodic routing and note-order variation

- **Envelope + VCA**  
  articulates each note

- **Precision adder / offset source**  
  transposes repeating patterns

- **Clock divider / multiplier**  
  creates different melodic timescales

- **Logic modules**  
  combine Seq A and B into more complex note masks

---

# Summary

Stoicheia is best used for melody by controlling:

- **when notes happen**
- **when pitch changes**
- **when accents happen**
- **how two melodic layers interlock**
- **how a phrase resets or extends**

Its strongest melodic applications are:

1. triggering envelopes for a pitched voice  
2. clocking sample-and-hold into a quantizer  
3. separating pitch-change rhythm from note-trigger rhythm  
4. generating accent patterns  
5. creating two-voice interlocking melodic lines  
6. using alternating mode for tied/legato phrase behavior  
7. using chained mode for longer melodic forms

In practice, Stoicheia turns plain pitch material into **musical phrasing**. If you already have any CV source that can produce notes, Stoicheia can make it feel alive.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)