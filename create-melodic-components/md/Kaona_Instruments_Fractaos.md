# Kaona Instruments — Fractaos

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Fractaos User Manual v1.5](#)

# Using Fractaos to create melodic components in a Eurorack system

Fractaos is a **4-voice polyphonic, multitimbral fractal oscillator/synth voice** for Eurorack. From a musical perspective, it is not just a sound source—it can be the core of an entire **melodic layer**, from mono leads to poly chords, tuned percussion, drones, and evolving harmonic textures.

Since only one manual was provided here, I’ll focus on **how this module can be used in a system** to create melodic material and how to patch around its strengths.

---

## What Fractaos is good at melodically

Fractaos is especially strong for:

- **Polyphonic melodies** via MIDI or 1V/oct + trig
- **Chords and harmonic beds**
- **Animated leads and arps**
- **Layered multitimbral parts**
- **Hybrid melodic/percussive parts**
- **Drone-based harmonic movement**
- **Expressive, evolving timbres that stay pitch-related**

Its sound engine is unusual: each of 4 voices contains a **driver oscillator + follower oscillator**, with fractal algorithms creating the waveform structure in real time. That means melodic parts can be much more animated than a typical subtractive oscillator, especially when using:

- **Morph**
- **Spread**
- **Chaos**
- **Texture**
- **Primitive-derived modulation/LFO/FM**

---

# 1. Core melodic use cases

## A. Monophonic lead voice
Use one voice as a lead by driving Fractaos from:

- a MIDI keyboard
- a CV sequencer into one of the 1V/oct inputs
- corresponding trig/gate into one trig input

### Best settings for leads
Choose more pitch-coherent geometric fractals such as:

- Julia
- Mandelbrot
- Sierpinski
- Rössler
- Fibonacci
- Koch

These are likely to give the most stable harmonic behavior for melodic lines.

### Useful controls for lead shaping
- **Morph**: moves from a more direct tone toward a more modulated/complex tone
- **Spread**: in non-Drone mode, detunes driver vs follower; great for widening a lead
- **Texture**: adds formants/resonance/organic micro-detuning
- **Chaos**: adds instability and spectral complexity
- **Amount + Speed**: create internal animation for vibrato-like or timbral motion

### Musical result
This gives you a lead that can move from:
- clean and glassy
- to vocal/formant-like
- to unstable, metallic, or quasi-acoustic

That makes Fractaos great for **melodies that need motion without extra modulation sources**.

---

## B. Polyphonic chords
Fractaos supports **4-voice polyphony**, so it can function like a complete poly synth voice in a rack.

You can play chords through:
- **MIDI polyphonic mode**
- **4 separate 1V/oct + trig inputs**
- a polyphonic sequencer or MIDI-to-CV setup

### Why it works well for harmonic music
Each note has:
- its own oscillator pair
- its own ADSR envelope
- its own resonant fractal filter

So chord voicings have internal separation and movement rather than sounding flat.

### Good chord strategies
For stable harmonic content:
- Keep **Chaos moderate**
- Use **geometric fractals**
- Use **Spread subtly**
- Use **Texture carefully** for resonant color

For lush pads/chords:
- Use **Texture fractals** as the main oscillator
- Add a geometric primitive
- Slow **Speed**
- Medium **Amount**
- Long ADSR attack/release

This is ideal for:
- ambient harmony
- synth-pop chord beds
- cinematic sustained harmony
- slow-moving generative tonal clusters

---

## C. Arpeggios and sequenced melodic lines
Fractaos should shine with:
- gate sequencers
- pitch sequencers
- MIDI arp sources
- generative CV

Because the sound source is internally animated, even simple note patterns can feel complex.

### Patch idea
Feed:
- pitch CV to one voice or several voices
- synced triggers to the trig input(s)

Use:
- **Loop OFF / Trig ON** for note-retriggered modulation
- **Speed** to control modulation cycle
- **Amount** to control how much the primitive shapes each note event

This makes every note articulate with a slightly different internal contour, which is very useful for:
- plucky arps
- pseudo-acoustic phrases
- animated ostinatos

---

# 2. Best Fractaos parameters for melody writing

## Fractal Type
This is the main sound identity.

### Best for pitched melodic use
The manual suggests the **14 geometric fractals** are the most spectrally defined and reproducible.

Especially melodic:
- **Fibonacci**: warm, useful general-purpose tone
- **Koch**: crystalline highs, brass-like lows
- **Julia**: softer and smoother
- **Mandelbrot**: bright and harmonically rich
- **Rössler**: deformed-sine character
- **Sierpinski**: odd harmonic brightness

### More experimental melodic use
- **Lorenz**
- **Hénon**
- **Rule30**
- **Collatz**
- **Hilbert**

These can be good for melodies when you want notes to feel unstable, percussive, or semi-atonal.

---

## Primitive Type
This is the secondary fractal used as modulation source.

For melodic clarity, use primitive shapes that:
- complement the main fractal
- don’t destabilize pitch too much
- animate articulation rather than overwhelm it

A good practical approach:
- choose a stable main fractal
- choose a more animated primitive
- then adjust **Morph**, **Amount**, and **Speed**

This creates melodic tones with movement while preserving note identity.

---

## Morph
For melodic use, Morph is one of the most important controls.

It is not just a blend; the primitive still modulates the main fractal, so this affects both tone and behavior.

### Musical uses
- **Low Morph**: more direct, clearer pitch
- **Mid Morph**: expressive hybrid tones
- **High Morph**: more complex, transformed, animated tone

For melodies, the sweet spot is often **low to mid Morph**, where pitch remains clear but timbre is alive.

---

## Spread
In normal mode, Spread detunes the follower relative to the driver.

### Musical uses
- subtle chorus on melody lines
- intervallic widening
- richer harmonics on basslines or hooks

For melodies:
- low Spread = stable pitch center
- medium Spread = animated doubling
- high Spread = more dramatic harmonic shift

Because the follower can rise toward +1 octave, Spread can make simple melodies sound layered and “composed” rather than bare.

---

## Texture
Texture acts like a fractal filter/resonance/formant extractor.

### For melodic applications
Use it to make lines feel:
- vocal
- resonant
- organic
- hollow
- nasal
- wind-instrument-like

Texture is very good for turning simple sequenced notes into musically expressive phrases without needing an external filter.

---

## Chaos
Chaos adds instability and can be quantized depending on fractal type.

### Melodic advice
For tonal music:
- keep Chaos lower for basses, hooks, and chords
- increase Chaos for transitional phrases, fills, and lead intensity

A very effective technique is to **modulate Chaos slowly** so a melody evolves over time while staying on the same pitch sequence.

---

# 3. Internal modulation as melodic expression

Fractaos has an LFO/envelope behavior derived from the primitive and controlled by switches:
- Loop
- Trig
- Morph(FM)
- Spread
- Chaos

This matters a lot musically, because you can make a melody behave differently depending on note articulation.

## One-shot per-note articulation
Set:
- **Loop OFF**
- **Trig ON**

Each note retriggers the primitive modulation contour. This is great for:
- plucks
- mallet-like synth lines
- expressive phrases
- repeatable note attacks

This behaves somewhat like a timbral envelope on every note.

## Continuous movement
Set:
- **Loop ON**

Good for:
- pads
- sustained harmony
- long melodies
- legato-style evolving parts

## Simplified FM mode
Set:
- Loop OFF
- Trig OFF
- Morph ON
- Spread OFF
- Chaos OFF

Now **Amount** becomes bipolar around center:
- below center: internal feedback
- center: neutral
- above center: primitive modulates frequency of main fractal

### Musical uses of FM mode
- metallic bells
- sharp leads
- glassy keys
- clangorous tuned percussion

Important note from the manual:
- FM does **not** work when the main fractal is a Texture
- FM has **no effect on Drum curves**

So for melodic FM sounds, stick to the geometric fractals.

---

# 4. Using Drum fractals melodically

One of the most interesting parts of Fractaos is that its **Drum fractals are pitched and real-time synthesized**, not samples.

Available drum models:
- Kick
- Tom
- Snare
- HiHat
- Cymbal

The manual explicitly says MIDI pitch still affects them:
- **Kick and Tom** behave fairly tonally
- **Snare, HiHat, Cymbal** shift more in color/resonance than strict pitch

## Melodic uses for Drum fractals
This means Fractaos can do:
- tuned tom melodies
- pitched kick-bass lines
- hybrid percussive arps
- melodic strikes layered with tonal tails

### Especially useful trick
Because **Morph** can blend a Drum curve with a geometric primitive:
- you can create a note that starts as percussion
- then blooms into a pitched harmonic body

That is extremely useful for:
- marimba-like lines
- synthetic kalimba
- tuned techno percussion
- melodic IDM hits

This is one of the most distinctive melodic capabilities in the module.

---

# 5. Drone mode as a harmonic composition tool

Drone mode turns Fractaos into a continuously sounding 8-oscillator harmonic instrument.

In this mode:
- oscillators no longer act as simple voice pairs
- all 8 oscillators run simultaneously
- Spread has a special chord/microtuning behavior

## Why Drone mode is useful melodically
Even though it’s called “Drone,” it’s really also a **harmonic composition mode**.

### Spread zones in Drone mode
- **0–0.02**: unison
- **0.02–0.50**: linear spread up to +1 octave
- **0.50–1.00**: scans through **13 predefined chords/microtunings**

These include:
- major triad spread
- minor triad spread
- sus4/fifths
- major 7th
- minor 7th
- add9
- add11
- add13
- just intonation
- 7-limit flavor
- 19-TET slice
- Bohlen-Pierce subset

## Melodic/harmonic applications
Drone mode can be used for:
- harmonic pedal tones
- chord drones under a sequence
- evolving intros/outros
- ambient tonal centers
- modal beds for improvisation

### Powerful technique
Use the **1V/oct inputs or MIDI notes** to transpose the individual voice pairs while in Drone mode. That means you can:
- hold a fractal chord cluster
- then move parts of it melodically
- or transpose the whole harmonic field

This lets Fractaos behave like a **moving chord machine**.

---

# 6. Multitimbral mode for layered melodic arrangements

MULTI mode is where Fractaos becomes especially compositional.

You can assign:
- a different preset to each of the 4 voices
- or leave some voices in LIVE mode

Each voice can respond to its own MIDI channel.

## Practical melodic uses

### A. Bass + chord + lead + percussion from one module
Example assignment:
- Voice 1: bass preset
- Voice 2: chord stab preset
- Voice 3: lead preset
- Voice 4: tuned tom/snare hit preset

Now one Fractaos becomes a **mini ensemble**.

### B. Counterpoint
Use separate MIDI channels or CV control to play:
- one slow sustained line
- one faster arpeggio
- one chord voice
- one accent voice

Because each voice can have a different preset, timbral separation is built in.

### C. Layered melodic splits
Use LIVE on one voice for hands-on tweaking while the other voices play stable preset-based roles.

This is very useful in performance:
- one fixed harmonic bed
- one improvisable lead voice

## Important Spread behavior in MULTI
In MULTI mode:
- outside Drone mode, preset voices keep their saved Spread
- the panel Spread knob only affects LIVE voices

So for arrangement:
- save precise spreads in presets for stable parts
- use LIVE voices for manual expression

In Drone mode:
- global Spread takes control of all 8 oscillators, including preset voices

That means an entire multitimbral setup can be swept into chordal motion together.

---

# 7. Envelopes and melodic phrasing

Fractaos includes one ADSR per voice, with shared settings across voices.

Parameters:
- Attack: 1 ms to 8 s
- Decay: up to 8 s
- Sustain
- Release: up to 12 s
- Curve: linear, exponential, logarithmic

## Melodic implications

### Short attack + medium decay
Good for:
- plucks
- sequences
- bass lines
- arpeggios

### Slow attack + long release
Good for:
- pads
- chord swells
- ambient melodic overlays

### Sustain at 0
Interesting note from the manual: Release still matters even with Sustain at 0.

This is useful for:
- struck notes
- pseudo-percussion
- expressive decay tails
- melodic phrases where early note release changes the articulation

That makes Fractaos good for **dynamic phrase shaping**, especially from a MIDI keyboard.

---

# 8. CV patching ideas for melodic systems

Fractaos has:
- 8 CV inputs with attenuators for major parameters
- 4 x 1V/oct inputs
- 4 x trig inputs
- MIDI input

## Good melodic patch roles around Fractaos

### Pair with a sequencer
Send:
- pitch to one or more 1V/oct inputs
- gates/trigs to matching trig inputs

Then use Fractaos internally for timbral motion.

### Pair with modulation sources
Since Fractaos already has internal movement, external modulation works best for **slow macro changes**:
- slowly scan **Texture**
- gently modulate **Morph**
- animate **Pitch** for vibrato/gliss
- sweep **Spread** for widening

### Pair with precision CV
Because melodic use depends on pitch coherence, accurate 1V/oct sources will matter if using CV rather than MIDI.

### Pair with utilities
Useful helpers in a system:
- quantizer
- sequential switch
- clock divider
- logic
- performance mixer
- stereo effects

Fractaos already outputs stereo, so it pairs especially well with:
- reverb
- delay
- stereo chorus
- spectral processors

These can elevate melodic parts from “synth voice” to “full arrangement layer.”

---

# 9. Practical melodic patch examples

## Patch 1: Fractal poly pad
- MIDI keyboard into Fractaos
- Polyphonic mode on one MIDI channel
- Main fractal: Fibonacci or Julia
- Primitive: Mandelbrot or Rössler
- Slow attack, long release
- Loop ON
- Medium Texture
- Low to medium Chaos
- Slow Speed, moderate Amount

**Result:** lush evolving polyphonic harmonic bed.

---

## Patch 2: Metallic melodic sequence
- CV sequencer to 1V/oct input 1
- Trigger sequencer to trig 1
- Main fractal: Koch or Sierpinski
- Primitive: Julia or Dragon
- Simplified FM mode enabled
- Amount just above center
- Short envelope
- Moderate Texture

**Result:** tuned metallic melody, great for IDM/electro/experimental techno.

---

## Patch 3: Tuned drum melody
- Main fractal: Tom or Kick
- Primitive: geometric fractal
- Send melodic CV sequence
- Trigger with rhythmic gates
- Use Morph to blend attack and tonal tail
- Medium Depth
- Moderate Chaos

**Result:** tuned percussion line that reads as both rhythm and melody.

---

## Patch 4: Four-part multitimbral arrangement
- MULTI mode
- Voice 1: bass preset on MIDI ch.1
- Voice 2: chord preset on MIDI ch.2
- Voice 3: lead preset on MIDI ch.3
- Voice 4: percussion preset on MIDI ch.4

**Result:** one module handling multiple melodic roles in a track.

---

## Patch 5: Drone harmony with transposed movement
- Enable Drone mode
- Use Spread in upper zone to select Major 7th, Add9, or Just Intonation
- Feed slow CV transpositions to selected 1V/oct inputs
- Use long evolving modulation internally

**Result:** harmonic drone that still produces melodic motion through transposition of partial groups.

---

# 10. Best musical roles in a track

Fractaos can cover several melodic roles:

## Bass
Use:
- Fibonacci
- Rössler
- Julia
- Kick/Tom hybrid patches

Keep:
- low Chaos
- moderate Morph
- controlled Texture

## Lead
Use:
- Mandelbrot
- Koch
- Dragon
- Sierpinski
- FM mode

Great for:
- solo melodies
- hooks
- expressive improvisation

## Chords
Use:
- geometric fractals for harmonic clarity
- texture fractals for atmosphere
- long ADSR
- low/moderate Spread

## Arps and ostinatos
Use:
- trig-retriggered primitive behavior
- short envelopes
- moderate Amount
- rhythmic sequencer input

## Hybrid percussive melody
Use:
- Drum fractals + Morph toward geometric primitive
- short to medium envelopes
- sequenced pitch and rhythm

---

# 11. Performance advice

## Use presets as song sections
Because presets save:
- knob values
- switch states
- envelope parameters

You can prepare:
- verse pad
- chorus lead
- bridge percussion melody
- outro drone

## Use LIVE mode for expressive performance
Preset voices can stay fixed while LIVE voices are tweaked manually.

## Use MIDI velocity and aftertouch
The manual notes:
- MIDI velocity can be enabled/disabled
- aftertouch affects internal movement/timbral variation

That makes Fractaos especially playable as a melodic instrument from a keyboard.

---

# 12. Overall assessment for melodic use

Fractaos is best understood as a **polyphonic fractal synthesizer voice with unusually rich internal animation**. For melody creation, its strengths are:

- stable enough for tonal work when using the right fractals
- deep enough for evolving and expressive timbres
- flexible enough to cover lead, bass, chord, arp, and tuned percussion roles
- powerful in multitimbral arrangements
- uniquely good at drone-based harmony and microtonal chord fields

If your goal is to create **melodic components** rather than just sound design experiments, Fractaos is strongest when used in these ways:

1. **Geometric fractals for tonal parts**
2. **Moderate Chaos for pitch clarity**
3. **Morph and Texture as expressive tone shapers**
4. **Per-note primitive retriggering for articulation**
5. **MULTI mode for layered song arrangement**
6. **Drone mode for harmonic and modal foundations**
7. **Drum fractals for tuned rhythmic melody**

If you want, I can also turn this into:
- a **“best melodic patches for Fractaos” cheat sheet**
- a **quick-start guide**
- or a **genre-specific patch list** for ambient, techno, IDM, or cinematic music.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)