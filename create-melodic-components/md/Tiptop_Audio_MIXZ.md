# Tiptop Audio — MIXZ

- [Manual PDF](../../manuals/Tiptop_Audio_mixz.pdf)

---

[Manual PDF](https://www.tiptopaudio.com/manuals/mixz_manual.pdf)

# Tiptop Audio MIXZ — using it for melodic components

The attached manual is for the **Tiptop Audio MIXZ**, a **dual 4-channel analog mixer** with optional **Tiptop Bus Mix** integration. By itself, MIXZ is not a sound source, oscillator, filter, envelope, or sequencer. So it does **not generate melody directly**. Its role in a melodic patch is to **combine, scale, layer, and route melodic signals**: audio, CV, and gates.

That said, it can be extremely useful in building melodic voices and arrangements when paired with oscillators, filters, envelopes, sequencers, and effects.

---

## What the module does

From the manual, MIXZ has three related mixing functions:

- **Mixer A**
  - 4 input channels
  - individual gain control per channel
  - output is **internally routed into Mixer B**
  - inserting a cable into **Out A** breaks that internal connection

- **Mixer B**
  - 4 input channels
  - master gain control
  - sums:
    - its 4 front-panel inputs
    - **Mixer A output** if Out A is unpatched
    - **Tiptop Bus Mix** if enabled

- **Bus Mix**
  - takes signals from Tiptop modules that support Bus Mix via the busboard
  - switched on/off with the BUS MIX toggle
  - internally feeds Mixer B

The manual also notes MIXZ is designed to mix **audio, CV, and gate signals**, which is important for melodic patching.

---

# How MIXZ helps create melodic material

## 1. Layer multiple oscillators into one melodic voice

A classic melodic use is to combine multiple VCOs into a richer lead, bass, or drone.

### Patch idea
- VCO 1 saw → **Mixer A In 1**
- VCO 2 pulse → **Mixer A In 2**
- Sub oscillator or noise texture → **Mixer A In 3**
- Another harmonic source / FM tone → **Mixer A In 4**
- **Mixer A Out** → filter → VCA → effects

### Why this is useful
Mixer A has per-channel gain, so you can:
- set oscillator balance
- bring in detuned layers
- create thicker unison leads
- blend different waveforms for timbral motion

This is probably the most straightforward way MIXZ supports melody: it helps make a single melodic line sound bigger and more expressive.

---

## 2. Use Mixer A as a pre-filter voice combiner, Mixer B as a final melodic submix

Because **Mixer A can feed Mixer B internally**, you can structure a patch in stages.

### Example melodic structure
- **Mixer A** = raw oscillator blend for one voice
- Send **Mixer A Out** into a filter/VCA chain
- Filter/VCA output → **Mixer B In 1**
- Second melodic voice → **Mixer B In 2**
- Delay/reverb return or texture layer → **Mixer B In 3**
- Accent/gate-derived click/percussion tone → **Mixer B In 4**
- **Mixer B Out** → output or stereo processor

This lets you build:
- a main melody voice
- a counterline or drone
- a supporting harmonic texture
- all in one compact mixer workflow

---

## 3. Mix pitch CV sources for transposition and melodic variation

Since the manual explicitly says MIXZ can mix **CV**, one powerful use is **combining control voltages** before they reach an oscillator’s 1V/oct or FM input.

### Example uses
- sequencer pitch CV + keyboard transpose CV
- sequencer pitch CV + slow offset/automation
- quantized melody + subtle vibrato CV
- envelope + LFO into FM amount control

### Important note
MIXZ is a plain mixer, not a precision adder. So:
- it is great for **creative CV blending**
- it may be less ideal for highly accurate pitch addition over wide ranges

Still, for:
- transposition by ear
- controlled drift
- vibrato depth blending
- modulation sums

…it can be very musical.

### Example patch
- Main sequencer CV → **Mixer A In 1**
- Manual offset voltage → **Mixer A In 2**
- Slow LFO (very low level) → **Mixer A In 3**
- **Mixer A Out** → oscillator pitch input

This creates a melody that can be:
- transposed
- gently animated
- made less static

---

## 4. Blend modulation sources to shape melodic timbre

Melodic interest often comes more from **motion** than from pitch alone. MIXZ can combine several modulation sources before sending them to:
- filter cutoff
- wavefolder amount
- FM index
- pulse width
- VCA CV

### Patch idea
- envelope → **Mixer A In 1**
- slow LFO → **Mixer A In 2**
- random stepped CV → **Mixer A In 3**
- performance controller / pressure / mod wheel CV → **Mixer A In 4**
- **Mixer A Out** → filter cutoff CV input

This gives a melodic line:
- attack contour from the envelope
- cyclic movement from the LFO
- variation from random CV
- live expressiveness from the controller

That is one of the most musically powerful uses of MIXZ.

---

## 5. Create parallel melodic voices and combine them

Because MIXZ has **two 4-channel mixers**, you can dedicate one section to each role.

### Suggested setup
#### Mixer A
Use for one voice’s source blend:
- VCO A
- VCO B
- sub
- noise or wavefolder return

#### Mixer B
Use for final melodic summing:
- processed output of Voice 1
- processed output of Voice 2
- drone / pad layer
- external effect return

This is especially effective for:
- bass + lead
- lead + harmony
- mono melody + drone
- arpeggio + sustained tonal bed

---

## 6. Use it to combine gate or trigger patterns into rhythmic melody control

The manual states MIXZ can mix **gate signals** too. That means you can use it experimentally for rhythmic melodic behavior.

### Examples
- combine trigger streams to create denser gate patterns
- mix clock divisions into a logic-like rhythmic control
- send mixed gates to envelopes or pinged filters

This is not the same as logic processing, but in practice it can create:
- more active plucks
- layered accents
- pseudo-melodic rhythmic structures

For example:
- Trigger pattern A → Mixer input
- Sparse accent gate → Mixer input
- Mixed output → envelope gate input

Now your melodic voice gets a more complex articulation pattern.

---

# Best ways this module works with other modules for melody

Since the manual’s example patch references Tiptop modules like **Z3000**, **Z2040**, and **Z-DSP**, here’s how MIXZ fits into a melodic system.

## With oscillators
Use MIXZ to:
- layer waveforms
- blend detuned oscillators
- combine primary tone and sub
- mix FM sidebands or secondary oscillators

## With filters
Use MIXZ to:
- feed a filter with richer harmonic material
- combine several modulation sources into the filter cutoff
- create pre-filter gain balance for tone shaping

## With VCAs/envelopes
Use MIXZ to:
- create a mixed voice before the VCA
- combine envelopes and modulation CV for dynamic articulation

## With sequencers/quantizers
Use MIXZ to:
- combine melodic CVs
- add transpose offsets
- blend sequence lanes
- create subtle pitch variation

## With effects
Use MIXZ to:
- combine melody voices before delay/reverb
- mix dry and effected layers
- group several melodic sources into one spatial processor

---

# Bus Mix: useful, but mostly not for melodic patching

The manual makes clear that **Bus Mix** is primarily intended for Tiptop modules with Bus Mix capability, especially their drum modules and ONE. It routes signals over the busboard into Mixer B without patch cables.

For melodic work, Bus Mix is usually **less central** than the front-panel inputs, unless:
- you have Bus Mix-capable melodic sample playback from Tiptop ONE
- you want certain supporting sounds permanently available in Mixer B
- you want a simple no-cable submix of compatible modules

### Important limitations from the manual
- If you have **more than one MIXZ in a row**, only **one Bus Mix switch** should be on at a time
- MIXZ should **not** be used on a row using **Doepfer CV/GATE bus** unless Bus Mix is off
- Bus Mix is **not as low-noise** as the front-panel mixers
- If Bus Mix is unused, keep it **off** to reduce noise

So for melodic patching, my advice is:
- use **Mixer A and B** as your primary creative tools
- use **Bus Mix** mainly as convenience routing for compatible modules

---

# Practical melodic patch recipes

## 1. Thick mono bass
- VCO saw → Mixer A In 1
- VCO pulse → Mixer A In 2
- Sub osc → Mixer A In 3
- Mixer A Out → lowpass filter → VCA
- VCA Out → Mixer B In 1
- Delay/reverb return → Mixer B In 2
- Mixer B Out → system output

Result:
- one powerful bass voice with controlled harmonic balance

---

## 2. Lead plus harmony
- Lead oscillator pair → Mixer A inputs
- Mixer A Out → lead filter/VCA chain
- Harmony voice output → Mixer B In 1
- Lead chain output → Mixer B In 2
- Drone/pad → Mixer B In 3
- Mixer B Out → effects

Result:
- a compact melodic submix with layered voices

---

## 3. Animated filter melody
- Envelope → Mixer A In 1
- LFO → Mixer A In 2
- Stepped random CV → Mixer A In 3
- Mixer A Out → filter cutoff CV input
- Oscillator audio → Mixer B or separate voice path

Result:
- a melody whose tone evolves over time, not just pitch

---

## 4. Semi-generative pitch movement
- Sequencer pitch CV → Mixer A In 1
- Slow random offset → Mixer A In 2
- Manual offset source → Mixer A In 3
- Mixer A Out → quantizer or oscillator pitch input

Best practice:
- if pitch accuracy matters, send the mixed CV to a **quantizer** before the oscillator

Result:
- more organic melodic variation

---

## 5. Melodic voice plus percussion support
This follows the spirit of the manual example.
- Oscillators mixed on Mixer A for a bass/lead line
- Voice goes through filter/VCA
- Voice output enters Mixer B
- Bus Mix adds compatible Tiptop percussion
- Mixer B Out goes to delay/reverb or main output

Result:
- a complete musical phrase where melody and groove are mixed together

---

# Strengths of MIXZ in melodic systems

## Excellent for
- blending oscillators
- creating submixes of melodic voices
- combining modulation sources
- routing processed and unprocessed melodic signals
- compact performance mixing in small systems

## Less ideal for
- precise pitch summing over large ranges
- stereo mixing
- voltage-controlled level changes
- muting/soloing with switches
- precision utility work better handled by dedicated precision adders/VC mixers

---

# Musical workflow suggestions

## In a small system
MIXZ can be your:
- oscillator layer mixer
- modulation combiner
- final mono melodic submix

## In a larger system
Use it as:
- dedicated voice builder for bass or lead
- drum + melody submixer
- effects send return combiner
- performance mixer for a specific section of the patch

## For live use
You can use the channel gains to:
- fade harmonic layers in and out
- rebalance melody and harmony
- bring in extra oscillator content at transitions
- reduce modulation intensity at key moments

---

# Bottom line

The **Tiptop Audio MIXZ** is best understood as a **melodic support and shaping module**, not a melody generator. It helps you create melodic components by:

- **layering oscillators into richer voices**
- **combining modulation sources for expressive movement**
- **submixing multiple melodic chains**
- **mixing CV and gates for more variation**
- **integrating compatible Tiptop Bus Mix sources into a broader musical patch**

If you pair it with oscillators, filters, VCAs, envelopes, and a sequencer, MIXZ becomes a very practical tool for building:
- bass voices
- leads
- drones
- harmonized lines
- animated timbral melodies

In short: **MIXZ is the glue that helps melodic modules work together musically.**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)