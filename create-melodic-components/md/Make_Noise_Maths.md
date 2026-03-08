# Make Noise — Maths

- [Manual PDF](../../manuals/MATHSmanual2013.pdf)

---

[Manual PDF](http://www.makenoisemusic.com/content/manuals/MATHSmanual2013.pdf)

# Make Noise MATHS: using it to create melodic components

MATHS is not an oscillator or sequencer in the traditional sense, but it is extremely useful for building **melodic structure** in a Eurorack patch. From the manual, its main strengths are:

- function generation: envelopes, LFOs, cycling slopes
- slew / portamento
- CV mixing, inversion, offset generation
- analog OR / max selection
- gate extraction, pulse delay, clock division
- comparator-like and logic-like patch behavior

That means MATHS is best understood as a **melody shaper, melody animator, and melody utility brain**. It can help generate, process, quantize-friendly, rhythmically reshape, and articulate pitch CV.

## What MATHS contributes to melody

To make melody in modular, you usually need some combination of:

- **pitch CV source**
- **timing / trigger source**
- **articulation / envelopes**
- **variation / modulation**
- **mixing / offsets / inversion**
- sometimes **portamento / slew**
- sometimes **clock division / rhythmic derivation**

MATHS covers most of the support roles.

## Core melodic uses

## 1. Portamento and glide for pitch lines

One of the most direct melodic uses:

- patch a sequencer or keyboard CV into **CH 1 or CH 4 Signal Input**
- take **Unity Output** or **Variable Output**
- send that to your oscillator’s 1V/oct input

Then use:

- **Rise** to control upward glide time
- **Fall** to control downward glide time
- **Vari-Response** to shape the glide curve

This is especially powerful because MATHS gives you **independent up/down slew**. That means:

- rising notes can glide slowly
- falling notes can snap quickly
- or the reverse

That produces melodic phrasing impossible with a simple one-knob slew limiter.

### Musical results
- acid-style slides
- “lazy” upward inflection on arpeggios
- asymmetrical lead phrasing
- humanized pitch movement

## 2. Mixing and offsetting pitch CV

Channels 2 and 3 can act as:

- attenuverters for incoming CV
- DC offsets when nothing is patched

This is very useful for melody because you can:

- transpose a melodic sequence
- add vibrato depth
- combine multiple pitch influences before they hit a quantizer or oscillator
- invert a melodic contour

For example:

- sequence into **CH 2**
- slow LFO into **CH 3**
- CH 2 and CH 3 mixed at **SUM OUT**
- send SUM to a quantizer or oscillator pitch input

This creates:
- transposed melody
- drifting melodic variation
- interval modulation

Because CH 2 can generate up to about **±10V offset** and CH 3 about **±5V**, they are also useful for manual transposition.

## 3. Creating stepped melodic variation via gate-derived timing

MATHS itself is not a pitch quantizer, but it can create **timing structures** that drive melodic events.

Using:

- **EOR** from CH 1
- **EOC** from CH 4
- cycling channels
- trigger inputs
- pulse delay / clock division patches

you can derive alternate clocks for:

- sequencer advance
- sample-and-hold triggering
- quantizer triggering
- envelope triggering for notes

### Why this matters melodically
A lot of melody comes from **when** notes happen, not just which pitches occur. MATHS can generate:
- delayed note entries
- divided trigger streams
- flams
- syncopated derived clocks
- self-modulated pulse trains

So even if another module produces pitch, MATHS can make it melodically expressive.

## 4. Envelope generation for melodic articulation

CH 1 and CH 4 can each be used as:
- AD envelopes via **Trigger Input**
- ASR-style envelopes via **Signal Input**
- cycling modulation sources

This helps with melody in several ways:

- shape amplitude per note
- shape filter per note
- shape FM amount per note
- shape wavefolder depth per note

That turns a static pitch sequence into an actual melodic line.

### Example
- sequencer pitch -> oscillator 1V/oct
- gate -> MATHS CH 1 Trigger
- CH 1 output -> VCA CV
- CH 4 cycling slowly -> filter cutoff or FM depth

Now melody has:
- note contour
- dynamic phrasing
- timbral movement

## 5. Vibrato and expressive pitch modulation

Set CH 1 or CH 4 to cycle as an LFO:

- linear response for triangle-like vibrato
- ramp or skewed shape for more character
- audio-rate if you want aggressive FM-like sidebands

Patch:
- Unity or Variable Output -> oscillator pitch input, ideally through attenuation

Or better:
- use CH 2 / CH 3 to scale the vibrato depth first

### Musical uses
- subtle lead vibrato
- delayed vibrato if triggered from a gate structure
- asymmetrical or vocal-style pitch wobble
- animated bassline tuning movement

## 6. Building more complex melodic modulation with SUM / INV / OR

The **SUM**, **INV**, and **OR** outputs are especially good for melody support.

### SUM OUT
Use it to combine:
- pitch sequence
- transposition offset
- vibrato
- envelope amount
- random drift

Then send to:
- quantizer
- oscillator pitch
- filter tracking destination

### INV OUT
Use it to create mirrored contour:
- melody rises while another parameter falls
- or invert a pitch modulation before mixing

### OR OUT
This outputs the maximum positive voltage among inputs. For melody, that can be used as:
- a “highest wins” contour selector
- a way to combine envelopes into one accent stream
- half-wave rectification of modulation before it affects pitch

This is less traditional for pitch itself, but very useful for **accent and phrasing logic** around melody.

---

# Practical melodic patch ideas from the manual

## 1. Glide sequencer patch

Use MATHS as an asymmetrical slew on pitch CV.

### Patch
- sequencer pitch CV -> **CH 1 Signal Input**
- **CH 1 Unity Output** -> oscillator 1V/oct
- tune Rise and Fall to taste
- Vari-Response near log or linear

### Result
- controlled glide between notes
- different feel going up vs down

### Nice additions
- send gate accent to **Rise CV** or **Fall CV**
- use CH 2 or CH 3 to attenuate that modulation

This can make only accented notes glide.

## 2. Manual transposition bus

### Patch
- sequencer pitch -> **CH 2 Signal Input**
- leave **CH 3 input unpatched** to use its offset
- mix with **SUM OUT**
- send SUM -> quantizer or oscillator

### Result
- CH 3 becomes a transpose knob
- CH 2 sets pitch scaling/polarity

Good for:
- key changes
- chorus lift
- bass transposition

## 3. Envelope-shaped pitch bend

### Patch
- trigger stream -> **CH 1 Trigger Input**
- **CH 1 Unity or Variable Out** -> oscillator pitch FM input or mixed into pitch CV path
- attenuate carefully
- short Rise, medium Fall

### Result
- each note gets a pitch sweep
- classic synth “pluck” or tom-like attack bend
- expressive lead attack inflection

If you run this into a quantizer after mixing, it creates stepped ornament behavior; if directly to pitch, it makes continuous bends.

## 4. Vibrato under performance control

### Patch
- CH 4 in cycle mode
- CH 4 output -> **CH 2 Signal Input**
- CH 2 output or SUM output -> oscillator pitch modulation input
- use CH 2 attenuverter as vibrato depth control

### Result
- manual vibrato amount
- can be faded in live

Further:
- patch gate or pressure CV to **CH 4 Cycle Input** for run/stop vibrato
- or to **Both CV** for vibrato speed changes

## 5. Delayed note trigger for melodic swing

From the manual’s pulse delay concept:

### Patch
- clock or gate -> **CH 1 Trigger Input**
- take **EOR OUT** as delayed trigger
- send EOR to:
  - envelope trigger
  - sequencer advance
  - sample & hold trigger

### Result
- delayed note onset
- laid-back phrasing
- pseudo-swing
- staggered melodic layers

Fall affects pulse width, Rise affects delay.

## 6. Clock division for melodic density control

### Patch
- master clock -> **CH 1 Trigger Input**
- use **EOR** or **EOC-like derived behavior** as divided output
- send that divided clock to sequencer advance or quantizer trigger

### Result
- melody moves slower than the master rhythm
- changing Rise changes the melodic division ratio feel
- useful for polyrhythmic note progression

## 7. Complex LFO as melodic source into quantizer

The manual includes triangle/ramp/self-cycling patches. If you patch a cycling channel into a **quantizer**, it becomes a pitch source.

### Patch
- CH 1 cycling, linear or skewed response
- output from **Unity Out**
- send to quantizer input
- quantizer output -> oscillator 1V/oct

### Result
- repeating melodic contour
- triangle gives pendulum-like melodies
- ramp gives rising phrases with reset
- skewed response changes how long notes dwell in parts of the scale

Very musical and simple.

## 8. Dual interacting functions into quantizer

Using both CH 1 and CH 4:

### Patch
- CH 1 cycling slowly
- CH 4 cycling at a different rate
- combine with **SUM OUT**
- send SUM -> quantizer
- quantizer out -> oscillator pitch

Optionally:
- use EOR and EOC to cross-trigger one another
- modulate each other’s Rise/Fall/Both

### Result
- semi-repeating melodic phrases
- evolving contour
- complex but still bounded pitch movement

This is one of the strongest “melody from utilities” uses of MATHS.

## 9. Sample-and-hold melodic system support

If you have a sample-and-hold or random voltage source elsewhere, MATHS makes it more melodic.

### Use MATHS for:
- divided or delayed triggers to clock the S&H
- slew on the sampled voltage
- offset/transposition before quantization
- envelope generation for note articulation

### Example
- noise/random -> S&H input
- MATHS EOR -> S&H clock
- S&H out -> CH 1 Signal Input for glide
- CH 2 offset added via SUM
- SUM -> quantizer -> oscillator

### Result
- random but shaped melodies
- smoother intervals
- playable transposition

## 10. Accent extraction and phrase shaping

Use the OR bus and end-of-stage outputs to derive accents.

### Patch idea
- multiple modulation sources to CH 1–4 variable outs
- **OR OUT** -> VCA CV or filter accent
- sequence pitch from elsewhere
- note trigger from MATHS-derived clocks

### Result
- melody gets dynamic accent patterns
- “strongest of several motions” becomes accent contour
- useful for techno, IDM, generative lines

---

# Best melodic workflows with MATHS

## A. With a sequencer
MATHS is best used to:
- slew pitch
- transpose
- generate envelopes
- derive alternate clocks
- add vibrato and bends

## B. With a quantizer
MATHS becomes much more melodic with a quantizer downstream:
- cycling functions become scale-based melodies
- mixed CV becomes harmonic motion
- offsets become musical transposition
- self-patched complexity becomes usable pitch material

## C. With oscillators and VCAs
MATHS gives:
- note articulation
- accent
- vibrato
- pitch glide
- timbral contour

## D. In generative systems
MATHS can act as:
- timing brain
- contour generator
- CV mixer
- event derivation source

That makes it excellent for evolving melodic patches even if no traditional sequencer is present.

---

# Particularly strong melodic patch combinations inside MATHS itself

## 1. CH 1 or 4 cycling into quantizer
Simple repeating melody source.

## 2. SUM of CH 1 + CH 4 into quantizer
More complex melodic phrase source.

## 3. CH 2 and CH 3 as transpose + interval offset
Great for harmonic movement.

## 4. EOR / EOC used as note clocks
Excellent for rhythmic melody generation.

## 5. Slewed sequence + envelope pitch bend
Classic expressive mono synth behavior.

---

# A few concrete musical examples

## Acid-style lead
- sequencer pitch -> CH 1 Signal In
- CH 1 Unity -> oscillator 1V/oct
- gate -> CH 4 Trigger
- CH 4 out -> VCA/filter
- use CH 1 Rise/Fall for slide
- use CH 4 for snappy envelope

## Generative melody
- CH 1 cycle slow
- CH 4 cycle medium
- SUM OUT -> quantizer
- quantizer -> oscillator
- EOC or EOR -> envelope trigger
- CH 2 offset for transposition

## Bassline with accents
- sequencer pitch direct to oscillator
- MATHS derives divided/delayed trigger stream
- CH 1 envelope -> VCA
- OR OUT -> filter accent
- CH 4 cycling slowly -> subtle pitch wobble

## Ornamented lead
- base pitch sequence -> oscillator
- CH 1 triggered envelope mixed lightly into pitch
- CH 4 cycle as vibrato
- CH 2 controls vibrato depth
- delayed EOR triggers occasional secondary envelope

---

# Bottom line

MATHS creates melodic components less by “playing notes” directly and more by controlling the things that make notes musical:

- **pitch movement**
- **glide**
- **transposition**
- **articulation**
- **timing**
- **accent**
- **phrase variation**
- **complex CV generation for quantized melodies**

If you pair it with:
- an oscillator,
- a quantizer and/or sequencer,
- a VCA/filter,

then MATHS becomes an extremely powerful melodic utility and generative composition tool.

For melody specifically, the most important tricks are:

1. **slew incoming pitch CV** for expressive glide  
2. **mix and offset CV** for transposition and interval shaping  
3. **use cycling outputs into a quantizer** for self-generated melodies  
4. **derive clocks with EOR/EOC** for rhythmic note structure  
5. **use envelopes for pitch bends and articulation**  
6. **combine channels with SUM/INV/OR** for evolving melodic modulation  

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)