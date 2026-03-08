# Erica Synths — Drum Mixer

- [Manual PDF](../../manuals/MIXER_instrukcija_xs.pdf)

---

[Manual PDF: MIXER_instrukcija_xs.pdf](MIXER_instrukcija_xs.pdf)

# Erica Synths Mixer: using it for melodic patching

The attached manual is for the **Erica Synths Drum Mixer / Mixer** module. It’s primarily an **audio mixer**, not a pitch or sequencing module, but in a Eurorack system it can still play an important role in building **melodic components** when combined with oscillators, envelopes, VCAs, filters, sequencers, and effects.

## What this module does

From the manual images:

- **7 inputs**
- **3 inputs assignable** to:
  - Main out
  - Aux send
  - or both
- **Built-in compressor**
  - Amount control
  - Decay / release control
  - Up to **+6 dB input boosting**
- **Main out** and **Aux out**
- **Signal indicator LEDs** on the first three channels
- Designed with **drum mixing** in mind, but fully usable for synth voices too

This makes it useful as a **submixer**, **parallel routing tool**, and **performance mixer** for melodic material.

---

## Best role in a melodic system

Even though it’s labeled for drums, this module works very well for:

- **Mixing several melodic voices**
- **Layering oscillators into one melodic line**
- **Creating parallel dry/wet signal paths**
- **Adding punch and glue with compression**
- **Sending selected voices to effects**
- **Balancing harmonies, drones, basslines, and leads**

Think of it less as “the thing that creates melody” and more as “the thing that helps melodic voices become a finished musical part.”

---

## Key features that matter musically

## 1. Seven audio inputs
You can combine multiple sound sources such as:

- lead oscillator
- bass voice
- chord voice
- drone
- noise layer
- sampled melodic percussion
- external effect return

For melodic music, this is ideal for building a **small ensemble inside the rack**.

## 2. Three assignable inputs with LEDs
The first three channels can be routed to:

- **Main**
- **Aux**
- **Both**

This is very useful for melodic patch design because you can choose which voices stay dry, which get processed, and which appear in both paths.

## 3. Input gain / boost
The manual mentions **up to +6 dB boost** on inputs. That means you can:

- push quieter oscillators or voices
- overdrive downstream effects slightly
- make one melodic layer stand out in the mix

## 4. Compressor with amount and release
Compression is especially useful for melodic playing when:

- layered oscillators need to feel “glued”
- arpeggios are too spiky
- basslines need more consistency
- chords need to sit under a lead

A short release can make things feel tighter and more rhythmic; a longer release can create a smoother sustain.

## 5. Main out and aux out
This is one of the most compositionally useful parts of the module.

You can use:

- **Main out** for the core melodic mix
- **Aux out** for effects processing, resampling, filtering, or alternate performance paths

---

# How to use it with other modules for melodic creation

## 1. Mixing multiple pitched voices into a song-ready melodic layer

### Patch idea
Use several voice modules together:

- **VCO 1**: bassline
- **VCO 2**: lead melody
- **VCO 3 / chord source**: harmony or drone

Patch each voice’s final audio output into separate mixer inputs.

### Why it works
The mixer becomes the place where your melodic arrangement takes shape:

- bass sits lower in level
- lead sits forward
- harmony fills space
- compression glues the voices together

### Musical result
You get a more complete melodic texture rather than isolated single voices.

---

## 2. Layering oscillators for one richer melody

A classic Eurorack melodic trick is to use **multiple oscillators tuned to the same pitch CV**.

### Patch
- Send one sequencer pitch CV to 2–3 oscillators
- Tune them as:
  - unison
  - octave apart
  - fifth above
- Patch those oscillator outputs through their shaping chain, then into the mixer

### Use the mixer for
- balancing each layer
- boosting one layer for presence
- compressing the sum for cohesion

### Musical result
A single melody becomes:

- thicker
- more animated
- more harmonically rich

This is especially strong for:
- mono leads
- basslines
- Berlin-school sequences
- detuned techno riffs

---

## 3. Building chords from separate voices

If your system doesn’t have a dedicated chord oscillator, this mixer helps combine individual notes into a chord.

### Patch
- Send related pitch CVs to several oscillators:
  - root
  - third
  - fifth
  - octave
- Use separate envelopes/VCAs if available
- Patch the audio outputs into the mixer

### Why the mixer matters
You can shape chord voicing by level:

- quieter third = more ambiguous chord color
- stronger fifth = more open/powerful sound
- louder top octave = more shimmer

Compression can make the chord feel more unified.

### Musical result
The mixer becomes a chord balancing tool, like a mini console for harmony design.

---

## 4. Parallel effects for melodic voices using the aux path

The **assignable routing** is the most creatively melodic feature here.

### Patch
- Lead voice into Input 1
- Pad/chord voice into Input 2
- Bass into Input 3
- Route:
  - lead to **Main + Aux**
  - pad to **Aux only**
  - bass to **Main only**
- Send **Aux out** to:
  - delay
  - reverb
  - shimmer
  - resonator
  - wavefolder
  - filter

Then return that processed signal somewhere else in the system or to an external mixer.

### Why this is good for melody
Different melodic roles often need different spaces:

- bass usually stays drier
- leads often want delay
- pads often want reverb
- arps may want heavy ambience

This mixer lets you create those relationships inside the rack.

### Musical result
A more intentional melodic mix with depth and contrast.

---

## 5. Creating call-and-response lines

Because some channels can go to main, aux, or both, you can create alternate melodic identities.

### Patch idea
- Put a melodic voice into an assignable channel
- Send **Aux out** into a different processing chain:
  - filter with modulation
  - granular effect
  - pitch shifter
  - delay
- Alternate hearing:
  - dry line on main
  - transformed line on aux
  - both together

### Musical use
This is great for:
- question/answer phrasing
- verse/chorus contrast
- evolving repetitions
- dub-style melodic echoes

---

## 6. Using compression to shape melodic phrasing

The onboard compressor is more than utility. It can affect how a melodic part feels.

### Shorter release / lower setting
- tighter
- punchier
- more rhythmic
- better for sequences and basslines

### Longer release / stronger setting
- smoother
- more sustained
- more “glued”
- better for pads, layered leads, or drones

### Example
If you have a plucky sequence that feels too pokey and disconnected, mix the voice through this module and add moderate compression. The notes can feel more connected, making the sequence read more like a melodic phrase.

---

## 7. Mixing sub-voices of one complex voice

Many melodic patches produce multiple outputs:

- oscillator main out
- sub oscillator
- wavefolder out
- filtered version
- noise component

You can patch several of these into different inputs and use the mixer as a **voice construction module**.

### Example
For a lead:
- saw wave into input 1
- sub oscillator into input 2
- wavefolded copy into input 3
- route folded copy to aux for delay/reverb treatment

### Result
You create one highly designed melodic voice from multiple layers.

---

## 8. Combining dry and compressed textures

Because the module has separate routing and a compressor, you can use it almost like a performance submixer for expressive leads.

### Patch concept
- Main out carries your primary melodic balance
- Aux path carries a more processed version
- Blend externally or elsewhere in the rack

This can make a melody feel:
- intimate and direct in one path
- wide and atmospheric in another

---

# Practical patch examples

## Patch 1: Thick mono lead

### Modules used
- sequencer
- 2 VCOs
- envelope
- VCA
- filter
- Erica Mixer
- delay or reverb

### Steps
1. Send one pitch CV to both VCOs.
2. Tune one at unison, the other an octave up or slightly detuned.
3. Mix or process them through your voice chain.
4. Send resulting audio layers into separate mixer inputs.
5. Route one of the first three inputs to **Main + Aux**.
6. Send **Aux out** to delay.
7. Use compressor lightly.

### Result
A lead that is:
- full in the center
- spacious in the effects path
- dynamically controlled

---

## Patch 2: Bass + lead + chord stack

### Inputs
- Input 1: bass voice
- Input 2: lead voice
- Input 3: chord voice
- Other inputs: drone, effect return, extra percussion-melody layer

### Routing
- Bass: Main only
- Lead: Main + Aux
- Chord: Aux only or both

### Processing
- Aux out to stereo reverb or delay
- Moderate compression on full mix

### Result
A complete melodic arrangement from one submixer:
- dry punchy bass
- prominent lead
- atmospheric harmonic layer

---

## Patch 3: Arpeggio with parallel shimmer

### Modules used
- quantizer/sequencer
- VCO
- envelope/VCA
- filter
- Erica Mixer
- pitch shifter or shimmer reverb

### Steps
1. Build a plucky arp voice.
2. Patch into Input 1.
3. Route Input 1 to **Main + Aux**.
4. Send Aux out to shimmer reverb.
5. Keep dry signal strong, wet signal softer.
6. Add a touch of compression.

### Result
An arpeggio that remains articulate while gaining a lush harmonic halo.

---

## Patch 4: DIY chord mixer

### Modules used
- 3 oscillators
- 3 VCAs or one shared articulation path
- sequencer/precision adder/quantizer
- Erica Mixer

### Steps
1. Tune oscillators to root, third, and fifth.
2. Patch all three into separate mixer channels.
3. Set levels to voice the chord.
4. Add compression for glue.
5. Route one component, such as the top note, to aux for delay.

### Result
A chord patch with controllable voicing and spatial separation.

---

# Strengths for melodic use

This module is especially good at:

- **submixing multiple voices**
- **layering tones into one melody**
- **parallel effects routing**
- **controlling dynamics**
- **building polished live-performance mixes**

It is ideal if your melodic patches already exist, but need:
- blending
- glue
- routing
- space
- punch

---

# Limitations

To be clear, this module does **not** itself generate melody. It does not provide:

- pitch CV generation
- quantization
- sequencing
- envelopes
- VCAs
- oscillation
- filtering

So for melodic creation you’ll still want companion modules such as:

- **sequencer**
- **quantizer**
- **VCO / complex oscillator**
- **filter**
- **envelope generator**
- **VCA**
- **delay / reverb**
- possibly a **precision adder** or **switch** for harmony

The Mixer’s role is to help all of those melodic pieces function together as a musical whole.

---

# Best companions in a melodic rack

If I were patching this in a melody-focused Eurorack system, I’d pair it with:

- **1–3 oscillators** for lead, bass, and harmony
- **quantizer + sequencer** for tonal structure
- **envelopes and VCAs** for articulation
- **filter** for tone shaping
- **stereo effect module** for ambience
- **output module or external mixer** for final monitoring

This Erica mixer would then act as the **central melodic submixer**.

---

# Bottom line

The Erica Synths Mixer in this manual is best used for melodic music as a:

- **voice blender**
- **layering mixer**
- **parallel FX router**
- **compressing glue stage**
- **live performance submixer**

It won’t compose melodies on its own, but it can make multiple melodic voices feel like a coherent instrument or finished track element. In a modular context, that’s often the difference between a patch that sounds technical and one that sounds musical.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)