# 4ms — Rotating Clock Divider

- [Manual PDF](../../manuals/RCD-manual-1.2.pdf)

---

[Manual PDF](#)

# 4ms Rotating Clock Divider — melodic use in a Eurorack patch

The attached manual is for the **4ms Rotating Clock Divider (RCD)**. This module is fundamentally a **rhythm and timing utility**, but in Eurorack that very often means it can become a **melodic structure generator** when paired with sequencers, quantizers, switches, sample & holds, oscillators, envelopes, and logic.

Since only one manual is attached here, I’ll explain how **this module can be used with other common Eurorack module types** to create melodic parts.

---

## What the RCD does musically

The RCD takes one incoming clock and produces **8 divided clocks**. Each output is a different division of the master pulse:

- /1, /2, /3, /4, /5, /6, /7, /8 by default
- or divisions across larger ranges up to **/64**
- and all outputs can be **rotated together** with CV

This matters melodically because melodic phrasing in modular often comes from:

- **when notes happen**
- **how often notes change**
- **when a sequence resets**
- **which lane or voice is selected**
- **how accents and phrase lengths drift against each other**

The RCD gives you all of that from one master pulse source.

---

## Key features that are especially useful for melody

From the manual, the most important melody-building features are:

- **8 clock outputs** at different divisions
- **CV Rotate** to shift all divide values at once
- **CV Reset** to re-align phrase starts
- **Up-beat / Down-beat counting**
- **Trigger or Gate mode**
- **Spread mode**
- **Auto-reset**
- **Selectable max divide range: 8 / 16 / 32 / 64**

These let you turn one stable clock into **evolving note timings, phrase resets, harmonic movement, and polymetric melody generation**.

---

# Core melodic patch ideas

## 1. Use the RCD as a sequencer clock distributor

This is the simplest and most immediately musical use.

### Patch concept
- Master clock → **RCD Clock In**
- RCD outputs to different sequencers / sample & hold / envelope triggers:
  - /1 → fast sequencer clock
  - /2 → bassline sequencer
  - /3 or /5 → melody sequencer
  - /8 → phrase reset or transposition trigger

### Musical result
You get multiple melodic layers moving at related but different rates:

- bass changes every 2 pulses
- melody changes every 3 or 5 pulses
- transposition changes every 8 pulses

This creates **polymeter**, which is one of the easiest ways to make modular melodies feel alive.

### Why it works
If one pitch source changes every /3 and another every /4, the relationship between them constantly shifts before lining up again.

---

## 2. Clock a Sample & Hold to generate stepped melodies

The RCD is excellent for controlling **when random or semi-random voltages become notes**.

### Patch concept
- Noise / random CV / slow modulation source → **Sample & Hold input**
- RCD output (say /4) → **Sample & Hold clock**
- Sample & Hold output → **Quantizer**
- Quantizer output → **Oscillator 1V/oct**

### Variations
- /3 clock for odd phrasing
- /5 for long looping melodic asymmetry
- Rotate CV for changing note density over time

### Musical result
You get a melody that updates at a controlled subdivision of the master clock.

### Better version
Use multiple RCD outputs:
- /4 → melody note changes
- /8 → transpose the quantizer root or switch scales
- /16 → reset a second modulation source

Now the melody has **notes, phrases, and sections** all derived from one clock tree.

---

## 3. Build a melody from sequential switching

One of my favorite uses of an RCD is to drive **switches**.

### Patch concept
- Several fixed voltages or sequencer rows → sequential switch inputs
- RCD outputs → switch advance / switch reset / gate different paths
- Switch output → quantizer → oscillator

### Example
- /1 → trigger main note envelope
- /2 → advance switch
- /8 → reset switch
- /3 → trigger a second accent envelope

### Musical result
The switch chooses different pitch sources at different rates, generating melodies that feel composed rather than random.

This is especially strong if your switch selects among:
- chord tones
- different sequencer rows
- intervals
- octave offsets

---

## 4. Use Rotate CV as a melodic variation control

The **CV Rotate** input is the RCD’s signature feature.

Instead of outputs always being /1 to /8, Rotate shifts them. So what used to be /1 becomes /2, /2 becomes /3, etc., wrapping around.

### Musical meaning
Rotate changes the **timing roles** of each jack without needing to repatch.

### Patch concept
- LFO / envelope / manual CV / pressure / random stepped CV → **CV Rotate**
- Patch several RCD outputs into:
  - sequencer clocks
  - reset inputs
  - sample & hold clocks
  - switch advance
  - envelope triggers

### Result
As Rotate moves:
- the melodic sequencer may slow down
- a reset may happen earlier or later
- transposition may become more or less frequent
- accents shift positions

This feels like **arrangement-level mutation** from a single CV.

### Great performance use
Send a slow triangle or stepped random CV to Rotate to create evolving melodic phrasing without touching cables.

---

## 5. Use Spread mode for wider phrase spacing

The manual explains that **Spread mode** spaces the divisions across the selected max range.

For example:
- with Max Div 32 and Spread On, outputs become:
  - /4, /8, /12, /16, /20, /24, /28, /32

This is excellent for melodic patching because it separates musical functions by time scale.

### Patch concept
With Spread On:
- /4 → note changes
- /8 → ornament trigger
- /12 → chord change
- /16 → sequence reset
- /24 or /32 → octave or transposition shift

### Musical result
Instead of all outputs being clustered around fast divisions, you get **clear hierarchies**:
- note level
- bar level
- phrase level
- section level

This is one of the best ways to make a modular patch sound intentional and “song-like.”

---

## 6. Use odd divisions for melodic phrasing

The odd outputs (/3, /5, /7) are where the real magic often happens.

### Why odd divisions matter
They create patterns that don’t line up in the usual 4/4 way, which gives:
- rotating accents
- evolving phrase starts
- melodic syncopation
- cross-rhythmic note placement

### Patch concept
- /5 → trigger a melodic voice
- /4 → trigger another melodic voice
- /7 → reset a transposition sequencer or switch
- /8 → envelope for a bass voice

### Musical result
Melodic parts phase against each other, producing emergent patterns.

For techno, electro, generative ambient, or Berlin-school style sequencing, this is gold.

---

## 7. Use the RCD to control transposition

A very strong melodic technique is to separate:
- **note rhythm**
- **pitch rhythm**
- **transposition rhythm**

The RCD can control all three.

### Patch concept
- Sequencer row A → quantizer → oscillator
- A second CV source (or precision adder input) provides transposition
- RCD /8 or /16 triggers a sample & hold that captures a new transpose voltage
- RCD /4 triggers main notes

### Result
The notes move regularly, but the key center changes more slowly.

This creates a melody with clear phrasing:
- note events happen often
- harmonic movement happens less often

---

## 8. Drive quantizer scale changes or root changes

If your quantizer has inputs for:
- root
- scale select
- shift
- transpose

then the RCD becomes a very musical macro-controller.

### Patch concept
- /4 → note sample & hold
- /8 → root change trigger
- /16 → scale change trigger
- /32 → global reset

### Musical result
Melodies can evolve from:
- minor to major
- pentatonic to chromatic
- root C to root F
- then reset cleanly

This is especially useful in generative patches where you want change without chaos.

---

## 9. Use CV Reset for phrase structure

The manual notes that **CV Reset resets on the next clock pulse**, keeping things rhythmically aligned.

That makes it ideal for phrase control.

### Patch concept
- Slow divided output from same RCD or another clock divider → **CV Reset**
- Faster outputs → sequencers / sample & hold / switch

### Example
- /3 clocks melody note changes
- /5 clocks ornament
- /16 resets everything

### Musical result
You get complex interplay inside a repeating larger phrase.

This gives you the best of both worlds:
- local complexity
- global repetition

That balance is what often makes a modular melody feel memorable.

---

## 10. Auto-reset for looping melodic cycles

The manual says auto-reset can reset after:
- 16
- 32
- 64
- 128 pulses depending on max divide range

### Why that matters
Without reset, divisions can create long drifting relationships.
With auto-reset, you force those relationships into a repeating form.

### Patch use
If you want:
- a 16-step melodic phrase that still uses odd divisions internally,
then set auto-reset so the whole system comes back to the start every 16 clocks.

### Musical result
This is very useful for:
- structured techno
- melodic IDM
- repeating bassline systems
- performance patches where you need repeatability

---

# Trigger mode vs Gate mode for melody

The manual makes an important distinction.

## Trigger mode
Outputs are short pulses based on the input clock width.

Best for:
- advancing sequencers
- triggering sample & hold
- pinging envelopes
- striking LPGs

For melodic note generation, this is often the most straightforward mode.

## Gate mode
Outputs stay high for 50% of the divided waveform.

Best for:
- opening VCAs for sustained notes
- controlling logic patches
- making note lengths proportional to division
- creating tied or held melodic notes

### Musical implication
In gate mode:
- /2 creates longer sustained notes
- /5 creates asymmetrical gate timing
- odd divisions create especially interesting note-length behavior

This can turn the RCD from a pure rhythm source into a **phrase articulation generator**.

---

# Up counting vs Down counting for melody

The manual describes two behaviors:

## Up-beat counting
Each jack fires after N pulses.

This feels like:
- delayed entrances
- pickup-style phrasing
- staggered melodic activity

Great for generative melodies where events “arrive” at different times after reset.

## Down-beat counting
All jacks fire after reset, then cycle.

This feels like:
- stronger phrase downbeats
- more obvious bar starts
- immediate layered attacks

Better for patches where you want every voice to line up at the beginning of the phrase.

### Musical advice
- Use **up counting** for evolving, less obvious melodic structures
- Use **down counting** when you want phrase starts to hit hard together

---

# Best module pairings for melodic use

## With a quantizer
Probably the single best pairing.

RCD handles:
- timing
- resets
- phrase lengths

Quantizer handles:
- pitch organization
- scale coherence

### Example
- random CV → S&H → quantizer
- RCD /5 clocks S&H
- RCD /16 changes root
- RCD /32 resets pattern

Result: coherent generative melody.

---

## With a sequencer
The RCD can make one sequencer behave like several.

### Example uses
- /1 clocks the main sequencer
- /4 clocks row advance on another sequencer
- /8 resets sequencer
- /3 toggles a switch between two pitch rows

Result: a simple sequencer becomes a much richer melodic engine.

---

## With sequential switches
Extremely powerful.

Use divided clocks to:
- step through note sources
- alternate melodies
- swap octaves
- insert rests

This creates melodic arrangement from clocks alone.

---

## With logic modules
A logic module plus RCD can generate note triggers that feel composed.

### Example
- /3 and /4 into AND/OR/XOR
- result clocks a sample & hold or envelope

This produces note timings from the intersections or unions of divided pulses.

### Musical feel
- AND = sparse coincidence notes
- OR = busier melodic activity
- XOR = syncopated, unstable patterns

---

## With sample & hold / track & hold
Ideal for stepped melodies and phrase control.

Use one divided output to sample pitch, another to sample transposition, and another to reset or reseed random motion.

---

## With precision adder / mixer
Use slow RCD outputs to bring in interval offsets:
- octave jumps
- fifths
- chord roots

You can create harmonic motion from timed voltage additions.

---

## With envelope generators and VCAs
Trigger mode gives note onsets.
Gate mode gives actual note durations.

This is a big deal melodically, because note length is as important as note pitch.

---

# Concrete melodic patch recipes

## Patch 1: Generative lead melody
- Master clock → RCD Clock In
- Smooth random CV → Sample & Hold in
- RCD /5 → Sample & Hold clock
- Sample & Hold out → Quantizer
- Quantizer out → VCO 1V/oct
- RCD /5 → Envelope trigger
- Envelope → VCA
- RCD /16 → Quantizer root change or reset

**Result:** a repeating-but-evolving lead line with phrase resets.

---

## Patch 2: Bassline + melody from one clock
- Master clock → RCD
- /2 → bass sequencer clock
- /3 → melody sequencer clock
- /8 → both sequencers reset
- /5 → transpose melody every few beats

**Result:** bass and lead stay related but cycle against each other.

---

## Patch 3: Shifted arpeggio machine
- Fixed chord voltages or sequencer row → sequential switch inputs
- RCD /1 or /2 → envelope trigger
- RCD /3 → switch advance
- RCD /8 → switch reset
- Switch out → quantizer → oscillator

Add:
- slow CV to Rotate

**Result:** the order and pacing of chord tones keeps morphing.

---

## Patch 4: Polymetric dual melody
- RCD /4 → voice A note generator
- RCD /5 → voice B note generator
- Both voices quantized to same scale
- /16 → reset voice A
- /20 or /24 in spread mode → reset/transposition for voice B

**Result:** two melodies weave around each other and rejoin over longer cycles.

---

## Patch 5: Gate-mode melodic phrasing
- Set RCD to **Gate mode**
- /2 gate → VCA for bass voice
- /3 gate → VCA for lead voice
- /5 gate → open secondary modulation VCA
- pitch comes from sequencer or quantized random source

**Result:** timing and note lengths are derived from divisions, giving organic phrasing.

---

# Advanced melodic strategies

## 1. Rotate the structure, not just the rhythm
If outputs are patched to several critical destinations, Rotate CV can transform the whole melodic architecture.

For example:
- one output clocks notes
- one output changes octave
- one output resets a phrase
- one output changes scale

As Rotate moves, these roles shift in time. This feels almost like a composed variation system.

---

## 2. Use slow CV into Rotate for evolving form
Because Rotate responds to 0–5V and moves outputs through division assignments, you can automate form over time.

Good CV sources:
- stepped random
- sequencer row
- pressure controller
- slow envelope
- joystick

This is excellent for live performance.

---

## 3. Use audio-rate clocking for crude subharmonic pitch structures
The manual notes the RCD can run into audio range and can “crudely step pitch downward.”

That means if you patch an audio-rate square wave as the input clock, the outputs become sub-divided square-like signals at lower frequencies.

### Musical use
- use outputs as crude suboscillators
- mix /2, /3, /4, /5 for organ-like or subharmonic tones
- then sequence filters or VCAs melodically

This is not precise V/oct melody generation, but it is musically interesting.

---

## 4. Build phrase memory with resets
Patch one of the slower outputs back into Reset.

The manual explicitly notes this is valid and independent of Auto-reset.

### Example
- /7 patched to Reset
- faster outputs drive note events

Now the system creates a repeating 7-pulse phrase, even if other divisions would normally run longer.

This is a very modular way to “compose” phrase lengths.

---

# Practical musical advice

## Best settings for immediate melodic use
If you want the RCD to be musical quickly:

- **Trigger mode**
- **Up counting** for staggered phrase emergence, or **Down counting** for obvious phrase starts
- **Spread On** if you want phrase hierarchy
- **Max Divide 16 or 32** for more structural timing options
- Use **CV Rotate** from a slow source

That setup gives a lot of melodic variation without becoming too chaotic.

---

## When to use Spread Off
Use **Spread Off** when you want neighboring outputs to be closely related:
- /1, /2, /3, /4...
- ideal for tight rhythmic melody work
- good for dense arpeggiation and quick note changes

## When to use Spread On
Use **Spread On** when you want the outputs to occupy different time scales:
- note events
- accents
- phrase changes
- section changes

This is better for complete musical structures.

---

## When to use max divide 8 vs 16/32/64

### Max 8
- immediate musical divisions
- compact rhythmic relationships
- easy to understand live

### Max 16
- more melodic phrase variation
- still manageable

### Max 32 or 64
- long-form generative structures
- slower harmonic changes
- excellent for ambient, generative, and evolving techno patches

---

# Summary

The **4ms Rotating Clock Divider** is not a pitch sequencer by itself, but it is an extremely powerful **melodic organizer**.

It creates melody by controlling:

- when notes happen
- how long they last
- when patterns reset
- how transpositions are timed
- how multiple voices phase against each other
- how phrase structure changes over time

Its most musically powerful features for melody are:

- **odd divisions**
- **CV Rotate**
- **Spread mode**
- **Reset behavior**
- **Trigger/Gate mode**
- **Up/Down counting**

In practice, the RCD shines when paired with:

- quantizers
- sequencers
- sample & hold
- switches
- logic
- envelope generators
- VCAs
- precision adders

If you want, I can also turn this into:
1. a **set of specific patch recipes by genre** (techno, ambient, IDM, Berlin school), or  
2. a **“best companion modules for the RCD” guide**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)