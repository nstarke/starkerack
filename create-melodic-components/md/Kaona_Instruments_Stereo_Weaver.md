# Kaona Instruments — Stereo Weaver

- [Manual PDF](../../manuals/stereoweaver.pdf)

---

[Manual PDF](attachment)

# Kaona Stereoweaver — using it for melodic components

Stereoweaver is **not a pitch or note generator**. It’s a **mono-to-stereo spatial processor**. So when thinking about “melodic components,” its role is:

- making a mono melody feel wider, deeper, and more alive
- adding motion to repeated note lines
- turning simple sequences into evolving stereo phrases
- creating contrast between lead, bass, arp, and drone parts

## What the module does

From the manual, Stereoweaver takes:

- **1 mono input**
- and creates **2 stereo outputs: L and R**

Core controls:

- **Depth** — controls perceived depth and effect interaction
- **Phase** — shifts phase relationship between channels from 0–180°
- **Motion** — controls animation speed; includes **Rotary** mode
- **Haas** — adds inter-channel micro-delay for spatial spread
- **Width** — widens stereo image; includes **Move** behavior
- CV inputs for:
  - Depth
  - Phase
  - Haas
  - Width

Other important details:

- **Input gain** with clip indication
- **Independent L/R output levels**
- CV inputs are **bipolar ±5V**
- CV amount is influenced by the corresponding knob position

---

# Best use in a melodic Eurorack patch

## 1. Stereo lead voice enhancement

Patch a complete mono melodic voice into Stereoweaver:

- VCO → VCF → VCA/envelope
- voice output → **Stereoweaver IN MONO**
- **OUT L / OUT R** → mixer or output module

Use settings like:

- **Depth:** low to medium
- **Phase:** low to medium
- **Motion:** slow
- **Haas:** moderate
- **Width:** medium

Result:

- lead stays centered enough to remain intelligible
- stereo field opens around it
- repeated notes feel less static
- small differences in phase and Haas give presence without sounding like delay

This is ideal for:

- melodies
- arpeggios
- plucked lines
- acid-style leads that need space without reverb

---

## 2. Make a simple sequence feel expressive

A basic 8-step melody can feel mechanical. Stereoweaver helps by adding **micro-movement**.

Patch:

- sequencer → oscillator pitch
- gate → envelope
- mono synth voice → Stereoweaver
- slow LFO → **Phase CV**
- another slow or unsynced LFO → **Haas CV** or **Width CV**

Why this works:

- the notes themselves do not change
- but the *space around each note* evolves
- this creates the perception of phrasing and development

This is especially good for:

- repeating ostinatos
- Berlin-school sequences
- techno arps
- generative melodic loops

---

## 3. Animated stereo arpeggios

Arps benefit a lot from spatial differentiation because the note content is already active.

Suggested patch:

- arpeggiated mono voice → Stereoweaver
- clocked triangle or sine LFO → **Width CV**
- slower LFO → **Phase CV**
- set **Motion** between slow and medium

Try:

- **Depth:** medium-high
- **Phase:** medium
- **Haas:** low-medium
- **Width:** medium-high

Result:

- different notes seem to occupy slightly different places in stereo
- the arp becomes less “flat”
- it feels like one melodic line unfolding in space

If you push Depth and Phase, you can get:

- micro-chorus
- slight phasing
- a glassy or dreamlike animated arp texture

---

## 4. Leslie-like melodic motion with Rotary mode

The manual notes that **Motion** has a **Rotary** region that simulates a Leslie-type effect with:

- separate low/high “speaker” behavior
- speed offset
- amplitude variation
- phase variation

This is very musical on:

- sustained leads
- organ-like patches
- drones with melodic articulation
- legato mono lines

Patch idea:

- saw or pulse voice with gentle filter movement
- into Stereoweaver
- set **Motion** to **Rotary**
- modulate **Phase CV** slowly
- keep **Haas** moderate

This can make a static melody feel:

- spinning
- breathing
- vintage
- harmonically richer due to phase interaction

For melodic use, avoid maxing everything at once unless you want abstraction.

---

## 5. Make counterpoint from one melodic line

Even though Stereoweaver doesn’t create new notes, it can make one melody behave like **multiple spatially interacting strands**.

Use:

- **Width** up
- **Move** behavior engaged
- **Motion** controlling displacement speed
- **Phase** raised enough to increase channel differentiation

The manual says in Move mode:

- left and right channels progressively exchange levels
- speed is defined by Motion
- amplitude depends on Phase
- at maximum, displacement becomes more chaotic

Musically, that means a single line can feel like:

- it is being answered from side to side
- notes are “thrown” across the stereo field
- a melodic figure has internal motion similar to call-and-response

Great for:

- FM plucks
- percussive melodies
- minimalist repeating motifs

---

## 6. Bassline support with careful stereo widening

Bass melodies can be widened, but carefully.

Recommended:

- **Depth:** low
- **Phase:** low
- **Haas:** very low
- **Width:** subtle
- **Motion:** slow

This preserves:

- punch
- center stability
- mono compatibility

Useful when:

- the bassline has upper harmonics
- you want subtle spatial animation without smearing the low end

A good trick is to feed Stereoweaver a bass voice with some filtered harmonics or wavefolding, so the spatial effect is heard more in the upper partials.

---

## 7. Turn drones into melodic beds

A drone or held note can become a melodic support layer if its spatial structure evolves.

Patch:

- sustained oscillator or chord-like mono sum
- slow envelope or random voltage to timbre/filter
- into Stereoweaver
- random stepped CV or smooth chaos → **Width CV**
- slow sine → **Haas CV**
- slow offset LFO → **Phase CV**

This creates:

- a stereo bed that shifts over time
- a background layer that supports foreground melodies
- the illusion of melodic movement even when pitch is static

Especially effective in ambient and soundtrack work.

---

# How each parameter affects melodic material

## Depth
This is the “immersion” control.

- **Low:** direct, forward, focused
- **High:** deeper, more enveloping
- **Very high:** can produce micro-chorus and micro-phasing

For melody:

- use **low-medium** for intelligible leads
- use **medium-high** for dreamy arps and pads
- use **high** for experimental melodic textures

## Phase
This defines much of the stereo character.

It affects:

- coherence
- strangeness
- diffusion
- stability

For melody:

- lower values keep lines more solid
- higher values can make notes shimmer or sound uncanny
- CV on Phase is excellent for long-form evolution

## Motion
This determines animation speed and can enter Rotary mode.

For melody:

- slow = natural movement
- medium = noticeable stereo animation
- rotary = expressive sustained lead treatment

If Width is in **Move mode**, Motion sets displacement speed.

## Haas
Adds micro-delay between channels.

For melody:

- moderate settings add presence and natural width
- higher settings make it more dramatic and characterful

Useful for making a mono voice sound immediately larger without obvious echo.

## Width
Controls stereo spread and center hollowness.

For melody:

- subtle width keeps focus
- higher width makes a line cinematic
- Move mode adds dynamic left/right exchange

This is one of the strongest controls for making repeated notes feel active.

---

# CV strategies for musical patches

Since the CV inputs are bipolar and summed with knob settings, modulation can be very expressive.

## Good modulation sources
Use:

- sine LFOs for smooth stereo drift
- random smooth voltage for organic variation
- envelopes for note-dependent widening
- stepped random for more experimental placement
- sequencer CV for phrase-based spatial changes

## Especially useful assignments

### Width CV from envelope
Each note opens wider at attack, then narrows.

Effect:

- melodies “bloom” on each note

### Haas CV from slow LFO
Stereo depth breathes over bars.

Effect:

- long phrases feel alive

### Phase CV from random smooth source
Creates subtle instability and uniqueness.

Effect:

- repeated melodic loops avoid sounding identical

### Width CV + Motion in Move mode
Creates side-to-side phrase travel.

Effect:

- spatial rhythm emerges from a static sequence

---

# Example melodic patch recipes

## Patch 1: Wide techno sequence
- 8-step sequencer → VCO
- gate → envelope → VCA
- saw voice → lowpass filter
- filter/VCA output → Stereoweaver

Settings:
- Depth: 11 o’clock
- Phase: 10 o’clock
- Motion: 9–10 o’clock
- Haas: 11 o’clock
- Width: 1 o’clock

Modulation:
- slow LFO → Width CV
- slower LFO → Haas CV

Result:
- wide, stable, modern stereo sequence

---

## Patch 2: Dreamy ambient lead
- triangle/sine + subtle FM
- long envelope
- mono voice → Stereoweaver

Settings:
- Depth: 2 o’clock
- Phase: 1 o’clock
- Motion: slow
- Haas: noon
- Width: 2 o’clock

Modulation:
- smooth random → Phase CV
- slow sine → Width CV

Result:
- floating melodic line with evolving stereo aura

---

## Patch 3: Rotating organ melody
- organ-like patch or additive voice
- mono output → Stereoweaver

Settings:
- Depth: medium
- Phase: medium
- Motion: Rotary
- Haas: low-medium
- Width: medium

Modulation:
- slow CV to Phase
- optional envelope to Width

Result:
- animated rotary-style melodic performance

---

## Patch 4: Nervous experimental plucks
- short-decay pluck voice
- mono output → Stereoweaver

Settings:
- Depth: high
- Phase: medium-high
- Motion: medium-fast
- Haas: medium
- Width: high / Move region

Modulation:
- stepped random → Width CV
- smooth random → Haas CV

Result:
- melody turns into spatially fragmented, glitchy motion

---

# Practical performance advice

## Keep the center for important melodies
If the melody must remain clear in a mix, do not overuse:

- Phase
- Haas
- Width

A little goes a long way.

## Use stronger settings on secondary melodies
Countermelodies, echoes, and background arps can tolerate:

- more Depth
- more Width
- more motion
- more phase weirdness

## Watch mono compatibility
Because phase and Haas processing affect inter-channel relationships, extreme settings may collapse oddly in mono.

So for club-focused or mono-sensitive music:

- keep bass nearly centered
- test the lead in mono
- use the wildest settings on upper textures

## Use clipping musically
The manual notes the input can be driven intentionally. That means you can feed a hot melodic voice for extra coloration and interaction with the spatial effect.

This can be great for:

- aggressive leads
- acid lines
- distorted drones

---

# Bottom line

Stereoweaver is best thought of as a **melodic space animator** rather than a melody generator.

It helps create melodic components by:

- widening mono leads into stereo
- adding movement to repetitive sequences
- making arps and plucks feel more dimensional
- creating rotary and phasing-like character for sustained notes
- turning static phrases into evolving stereo performances

If you pair it with:

- a sequencer
- one mono synth voice
- a few LFOs or random CV sources

you can get a lot of melodic richness from otherwise simple material.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)