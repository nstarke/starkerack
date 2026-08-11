# xaoc Devices — Sopot

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Fractaos User Manual v1.5](#)

# Using Fractaos to Create Melodic Components in Eurorack

Fractaos is a **4-voice polyphonic, multitimbral fractal oscillator/synth voice** for Eurorack. From the manual, it’s best understood not as a typical oscillator, but as a **self-contained melodic sound source** with:

- 4 polyphonic voices
- 8 real-time fractal oscillators arranged as driver/follower pairs
- per-voice ADSR
- per-voice resonant fractal filter
- stereo output
- MIDI and CV/gate polyphonic control
- preset and multitimbral operation

Because it already contains oscillators, envelopes, and filtering behavior, Fractaos can serve as the **main melodic engine** in a system.

---

## What kind of melodic roles Fractaos can play

Based on the manual, Fractaos is especially strong for:

- **Polyphonic pads**
- **Chords and harmonic drones**
- **Monophonic leads**
- **Animated arpeggios**
- **Layered multitimbral parts**
- **Hybrid pitched-percussive lines**
- **Evolving counterpoint across 4 voices**

It is less like a plain VCO and more like a **complex digital voice module** that can generate complete melodic material with minimal support.

---

## Core melodic features that matter most

## 1. Four-voice polyphony
Fractaos can be played melodically in two main ways:

- **Via MIDI**
- **Via 4x 1V/oct + 4x trig inputs**

This means you can use it for:

- keyboard-style polyphony
- sequenced 4-part harmony
- paraphonic-feeling chord work with independent voice triggers
- layered melodic phrases across separate sequencer lanes

If you want actual melodic composition in Eurorack, this is the big advantage: **Fractaos can hold multiple notes at once**.

---

## 2. Driver/follower oscillator pairing per voice
Each voice contains two oscillators:

- a **main fractal** (“driver”)
- a **secondary fractal** (“primitive” / follower)

The **Morph** control blends and interrelates them, not just as a crossfade, but as a more complex timbral interaction.

For melodic use, this means each note can have:

- a stable core pitch
- internal harmonic motion
- timbral animation that tracks note events

This is excellent for:
- expressive lead sounds
- harmonically rich chord voicings
- evolving sustained notes that don’t feel static

---

## 3. Fractal families and how they affect melody

The manual divides the sound engines into 3 groups:

### Geometric fractals
These are the most useful for tonal/melodic work.

Examples:
- **Mandelbrot**: crystalline, harmonically rich
- **Julia**: softer and smoother
- **Cantor**: articulated, edgy
- **Sierpinski**: odd-harmonic brightness
- **Dragon**: beating, expressive
- **Rule30**: dense, granular
- **Lorenz / Hénon / Rössler / Logistic**: unstable, evolving, experimental
- **Fibonacci**: warm and musically friendly
- **Koch**: crystal highs, brass-like lows
- **Hilbert**: stepped/evolving rectangle character

For melody, these are your primary palette.

### Texture fractals
These are more atmospheric, noisy, and pad-oriented:
- Cloud
- Storm
- Aliasing
- String
- Ensemble
- Cluster

These are still useful melodically, especially for:
- ambient harmonic beds
- blurred chord clouds
- sustained note clusters
- textural melodic layers behind a lead

### Drum fractals
These are one-shot percussion models:
- Kick
- Tom
- Snare
- HiHat
- Cymbal

Interesting melodic use:
- tuned tom melodies
- kick-bass lines
- pitched percussive ostinatos
- percussive attacks morphed into harmonic tails

This is one of the more unusual strengths of Fractaos: it can create **pitched melodic percussion** without needing samples.

---

## How to use Fractaos for melodic patching

## A. Polyphonic chord voice
This is the most obvious melodic use.

### Patch concept
- Send MIDI chords into Fractaos, or
- Use 4 pitch CVs plus 4 triggers from a polyphonic sequencer
- Use a geometric fractal as the main oscillator
- Set a moderate ADSR
- Use low/moderate Morph and Texture
- Use stereo outputs into mixer/effects

### Good settings
- **Main fractal**: Fibonacci, Julia, Koch, Mandelbrot
- **Primitive**: Rössler, Sierpinski, Julia
- **Spread**: low in normal mode for subtle detune
- **Texture**: moderate for resonant body
- **Speed/Amount**: slow for movement

### Result
A playable 4-note harmonic voice that can produce:
- pads
- chord stabs
- moving harmony
- modal progressions

This makes Fractaos a strong “all-in-one” melodic voice for polyphonic composition.

---

## B. Sequenced lead voice
Although polyphonic, Fractaos can also be used monophonically for a focused melodic line.

### Patch concept
- Sequence one voice via MIDI or one CV/gate lane
- Use a geometric fractal with expressive Chaos response
- Trigger ADSR per note
- Use primitive LFO behavior for note-synced motion

### Good settings
- **Dragon** or **Mandelbrot** for lively harmonics
- **Hilbert** for stepped/edgy digital lines
- **Fibonacci** for warmer leads
- **Chaos modulation enabled**
- **Morph or Spread modulation active**
- Medium attack/decay for articulation

### Result
A lead line with:
- animated timbre per note
- expressive internal movement
- more complexity than a traditional subtractive voice

Because the primitive can restart per note depending on Loop/Trig settings, the lead can feel highly articulated and “composed,” not just modulated.

---

## C. Arpeggios and moving ostinatos
Fractaos should pair extremely well with external Eurorack or MIDI arpeggiators.

### Patch concept
- Feed repeating melodic notes into the polyphonic engine
- Use retriggered primitive modulation
- Use short ADSR
- Keep Spread low to maintain pitch clarity
- Use Texture carefully to avoid losing note definition

### Best switch behavior
The switch section matters a lot here:

- **Loop OFF + Trig ON**: per-note one-shot modulation
- **Loop ON + Trig ON**: looping while note held
- **Morph ON**: timbral sweep on each note
- **Chaos ON**: animated spectral attack
- **Spread ON**: wobbling detuned movement

### Result
Each arpeggiated note can have a repeating internal contour, like:
- a tiny envelope on timbre
- pseudo-acoustic attack behavior
- evolving brightness from note to note

This is especially effective for melodic ostinatos that need motion without extra modulation modules.

---

## D. Chord drones that remain melodic
Drone mode is one of Fractaos’ signature features.

In Drone mode:
- all 8 oscillators run continuously
- Spread behaves differently
- upper Spread range scans preset chord/microtuning structures

### Why this matters melodically
Drone mode is not just for noise beds. It can create:

- held harmonic centers
- modal pedal tones
- sustained chord foundations
- microtonal harmonic fields
- evolving tonic/dominant beds behind other voices

### Spread in Drone mode
The manual describes 3 zones:

- **0–0.02**: unison
- **0.02–0.50**: linear spread up to one octave
- **0.50–1.00**: scans 13 predefined chord/microtuning structures

These chord structures include:
- major triad spread
- minor triad spread
- sus/fifths
- major 7
- minor 7
- add 9
- add 11
- add 13
- just intonation
- 7-limit flavor
- 19-TET slice
- Bohlen-Pierce subset

### Musical use
This is incredibly useful for melodic composition because you can create:

- a harmonic bed in just intonation
- a sustained add9 or maj7 field
- a microtonal drone under a lead sequence
- chordal transitions by slowly moving Spread

This is one of the most direct ways to generate **melodic harmony** from the module itself.

---

## E. Multitimbral layered melodic arrangement
MULTI mode is where Fractaos becomes especially powerful compositionally.

Each of the 4 voices can:
- load a different preset, or
- remain in LIVE mode

Each voice can also respond to a separate MIDI channel.

### What this enables
You can use a single module as:

- voice 1: bass
- voice 2: chord stab
- voice 3: lead
- voice 4: pluck/countermelody

Or:
- one preset for warm harmonic support
- one preset for noisy upper extension
- one preset for tuned percussion
- one LIVE voice for manual improvisation

### Melodic significance
MULTI mode turns Fractaos into a **mini ensemble** rather than a single oscillator.

In a composition, this means one module can generate:
- independent melodic lines
- register-separated harmonic parts
- contrapuntal voices
- call-and-response phrases

For a small Eurorack system, this is a huge space saver.

---

## Good melodic strategies by fractal type

## Best fractals for tonal melody
These seem most suitable from the descriptions:

- **Fibonacci** – warm, foundational, friendly for melodies
- **Julia** – softer, smoother lines
- **Koch** – bright highs, brass-like lows
- **Mandelbrot** – rich, crystalline, detailed
- **Sierpinski** – odd-harmonic, assertive melodic presence
- **Rössler** – deformed sine-like motion, useful for expressive tones

Use these when you want:
- recognizable pitch
- harmonic stability
- musical repeatability

---

## Best fractals for edgy/modern melodies
- **Cantor**
- **Dragon**
- **Hilbert**
- **Rule30**
- **Logistic**

These are great for:
- IDM lines
- glitch melodies
- aggressive synth hooks
- mechanistic or sequencer-forward phrasing

---

## Best fractals for unstable evolving melodic parts
- **Lorenz**
- **Hénon**
- **Rössler**
- **Rule30**

These are ideal when you want pitch to remain present but timbre to feel alive and semi-chaotic.

Use for:
- generative melodies
- evolving ambient top lines
- unstable harmonic color

---

## Best sound engines for melodic percussion
- **Tom** for tuned lines
- **Kick** for bass-note pulse
- **Snare** + Morph for pitched attack/tail hybrids

A very musical trick from the manual is that Drum curves can be blended with the second geometric fractal using Morph. That means you can create:

- percussive attacks with pitched sustain
- mallet-like voices
- tom-to-tone transitions
- transient-rich bass motifs

This is excellent for melodic techno, electro, experimental ambient, and broken beat styles.

---

## Modulation behaviors that help melody

## Primitive as note-synced modulation source
The primitive-derived modulation can affect:
- Morph
- Spread
- Chaos

For melody, this lets each note have internal shape.

### Strong melodic use cases
- **Morph modulation**: notes bloom from one harmonic shape to another
- **Chaos modulation**: notes brighten or destabilize over time
- **Spread modulation**: subtle chorusing or dramatic pitch animation

This can make repeated notes feel more expressive without changing the sequence itself.

---

## Simplified FM mode for harmonic complexity
The manual describes a simplified FM mode:

- Loop OFF
- Trig OFF
- Morph ON
- Spread OFF
- Chaos OFF

Then **Amount** becomes bipolar:
- lower half: internal feedback
- center: neutral
- upper half: primitive 2 modulates main fractal frequency

### Melodic usefulness
FM mode is especially useful for:
- metallic leads
- bell-like melodies
- complex bass tones
- harmonically rich plucks

Caveat:
- FM is not active when main fractal is a Texture
- FM has no effect on Drum curves

So for clear melodic FM-like playing, stick to geometric fractals.

---

## Texture as a melodic enhancer
Texture is more than a filter amount. It affects:
- resonant fractal filtering
- formant extraction/application
- organic micro-detunings
- filter intensity

For melody, Texture can function like a macro control for:
- vowel-like tone
- body and resonance
- subtle acoustic-feeling instability
- animated overtones

### Practical advice
For clear melodic lines:
- keep Texture moderate

For ambient or emotional harmonic content:
- increase Texture gradually

Too much may obscure pitch clarity, especially with already unstable fractals.

---

## Envelope use for melody

Fractaos has shared ADSR settings across all four voices.

### Practical melodic applications
- **Short attack, medium decay, low sustain**: plucks and arps
- **Fast attack, high sustain, medium release**: chord pads
- **Long attack, long release**: ambient swells
- **Short decay, zero sustain**: struck or mallet-like notes
- **Zero sustain with release**: expressive fading notes depending on note length

Because release remains active even with sustain at zero, you can make notes respond differently based on gate length, which is musically useful for expressive sequencing.

---

## How Fractaos works with other Eurorack modules

Even though only one manual is provided, we can still say a lot about how Fractaos fits into a rack for melody.

## Best companions for melodic use

### 1. Sequencers
Use with:
- pitch/gate sequencers
- polyphonic CV sequencers
- MIDI sequencers
- keyboard controllers

Fractaos needs melodic instruction from somewhere, and it responds well to either MIDI or 1V/oct inputs.

Ideal uses:
- one sequencer lane per voice
- polyphonic chord progression input
- separate melodic channels in MULTI mode

---

### 2. Quantizers
If generating pitches from random or CV sources, quantizers are very useful before the 1V/oct inputs.

This helps keep Fractaos in:
- scales
- modes
- chord tones
- microtonal frameworks if desired

Because the timbre can already be highly complex, stable pitch organization helps melodic intelligibility.

---

### 3. Utility modulation
Even though Fractaos has internal motion, external CV into:
- Pitch
- Spread
- Morph
- Texture
- Speed
- Amount
- F-Chaos
- P-Chaos

can create evolving melodic expression.

Especially useful:
- slow CV into Morph for phrase development
- stepped CV into Chaos for section changes
- performance CV into Texture for emphasis
- light modulation of Spread for ensemble width

---

### 4. Effects
Stereo output makes Fractaos especially attractive with:
- reverb
- delay
- chorus
- spectral FX
- shimmer
- resonators

Melodic roles improved by FX:
- chords become lush pads
- leads become cinematic
- arps become spatially animated
- drones become harmonic environments

---

### 5. Mixers and VCAs
Because it is stereo and multitimbral, a mixer is helpful downstream.

In MULTI mode especially, you may want:
- voice balancing
- external processing chains
- dynamic arrangement control

---

## Example melodic patch ideas

## Patch 1: Polyphonic ambient chords
- MIDI keyboard or poly sequencer into Fractaos
- Main fractal: Julia or Fibonacci
- Primitive: Rössler
- Moderate Morph
- Low Chaos
- Medium Texture
- Long attack/release
- Stereo reverb after output

**Result:** warm evolving chord clouds with internal movement.

---

## Patch 2: Metallic melodic techno lead
- Single-note sequencer into one voice
- Main fractal: Mandelbrot or Koch
- Primitive: Sierpinski or Dragon
- Simplified FM mode enabled
- Medium Amount above center
- Short attack, medium decay, low sustain
- Small delay after output

**Result:** bright, metallic, cutting lead with animated harmonics.

---

## Patch 3: Tuned percussive melody
- Main fractal: Tom
- Primitive: geometric fractal
- Morph around low-to-mid range
- Short envelope
- Moderate Chaos
- Sequence pitch melodically

**Result:** tom/mallet hybrid riffs with defined pitch and transient attack.

---

## Patch 4: 4-part multitimbral composition in one module
In MULTI mode:
- Voice 1: bass preset
- Voice 2: chord preset
- Voice 3: lead preset
- Voice 4: LIVE mode for manual tweaks

Assign separate MIDI channels or distinct sequencing.

**Result:** one module handling multiple melodic layers at once.

---

## Patch 5: Drone harmony plus top melody
- Enable Drone mode
- Use Spread chord zone for maj7, add9, or just intonation
- Set texture-based or geometric harmonic bed
- Feed CV/MIDI transposition to shape harmonic center
- Play another module or another Fractaos voice above it

**Result:** sustained harmonic field supporting melodic content.

---

## Limitations to keep in mind for melody

A few manual-based considerations:

- Some fractals are intentionally unstable and may not sound identical across registers.
- Texture fractals are less pitch-defined.
- Drum fractals are not traditional oscillators.
- Depth is stepped and not CV-modulatable.
- In LOAD mode, physical pots/CVs don’t control the sound until you return to LIVE.
- In MULTI mode, Spread behavior differs between LIVE and preset voices.

These are not flaws, but they do affect how predictable melodic patching will be.

---

## Best overall uses for melodic music

If I were using Fractaos in a Eurorack composition, I’d see it as best suited for:

1. **Primary polyphonic voice**
2. **Multitimbral melodic hub**
3. **Chord drone generator**
4. **Animated lead source**
5. **Pitched percussion synth**
6. **Experimental harmonic texture layer**

Its biggest melodic strength is that it combines:
- pitch handling
- polyphony
- timbral evolution
- preset recall
- multitimbral arrangement

in one module.

That makes it unusually effective for writing actual melodic/harmonic music in Eurorack, especially if your system is otherwise more modulation- and sequencing-oriented.

---

## Bottom line

Fractaos can be used to create melodic components by functioning as:

- a **4-voice polyphonic synth voice**
- a **multitimbral 4-part melodic ensemble**
- a **chord and drone generator with built-in harmonic spreads**
- an **expressive lead and arp source**
- a **pitched percussion voice for melodic rhythm**

For the clearest melodic results, focus on:
- **geometric fractals**
- **moderate Chaos**
- **careful Morph/Texture settings**
- **ADSR shaping**
- **MULTI mode for layered arrangements**
- **Drone Spread chord sets for harmony**

If you want, I can also turn this into:
1. a **musical cheat sheet**,  
2. a **“best patch recipes” guide**, or  
3. a **module pairing guide** for Fractaos with sequencers, filters, and effects.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)