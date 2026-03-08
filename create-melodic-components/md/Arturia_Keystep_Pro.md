# Arturia — Keystep Pro

- [Manual PDF](../../manuals/keystep-pro_Manual_1_1_0_EN.pdf)

---

# [Arturia KeyStep Pro User Manual (PDF)](https://downloads.arturia.net/products/keystep-pro/manual/keystep-pro_Manual_1_0_0_EN.pdf)

## Overview

The attached manual is for the **Arturia KeyStep Pro**, which is not a Eurorack module itself, but is extremely useful as the **melodic brain** of a Eurorack system. From a modular musician’s perspective, it can function as:

- a **4-track pitch/gate sequencer**
- a **3-track arpeggiator**
- a **CV keyboard controller**
- a **drum trigger source**
- a **master or slave clock**
- a **performance arranger** with patterns, chains, scenes, transposition, scales, and chord memory

If your goal is to create **melodic components for music** with Eurorack, the KeyStep Pro is a powerful central controller because it provides:

- **4 independent CV/Gate voice outputs**
- **Pitch CV + Gate + Mod/Velocity CV per voice**
- **scale quantization**
- **chord memory**
- **polyphonic sequencing**
- **arpeggiation**
- **track splits**
- **pattern chaining and scenes**
- **drum gates for rhythmic modulation or percussion**

---

## What the KeyStep Pro gives a Eurorack melodic system

For each of the four voices, the rear panel provides:

- **Pitch**
- **Velo/Mod**
- **Gate**

These can be patched into a modular voice like this:

- **Pitch CV → oscillator 1V/oct input**
- **Gate → envelope gate input**
- **Envelope output → VCA CV input**
- **Oscillator output → filter → VCA → output**
- **Velo/Mod CV → filter cutoff CV input, VCA level CV input, wavefold amount, FM amount, etc.**

So even with a minimal modular setup, the KeyStep Pro can generate a full melodic structure.

---

## Basic melodic patching strategies

## 1. Single melodic voice

This is the simplest use.

### Patch
- **Voice 1 Pitch → VCO 1V/oct**
- **Voice 1 Gate → EG gate input**
- **EG out → VCA CV**
- **VCO audio → VCF → VCA**
- **Voice 1 Velo/Mod → VCF cutoff CV**

### Result
You get a classic monosynth voice where the KeyStep Pro:
- plays notes from the keyboard
- sequences melodies
- records pitch, gate, velocity
- lets dynamics affect timbre through the modulation output

This is ideal for:
- basslines
- leads
- modal melodies
- acid-like phrases
- transposable sequences

---

## 2. Four independent melodic voices

Because there are **4 separate CV/Gate voice outputs**, you can run four modular voices at once.

### Example arrangement
- **Track 1 / Voice 1** → bass voice
- **Track 2 / Voice 2** → lead voice
- **Track 3 / Voice 3** → counter-melody
- **Track 4 / Voice 4** → slow chord tones / drone line

### Result
You can build complete melodic interplay:
- bass ostinato
- arpeggiated upper line
- evolving counterpoint
- independent rhythmic lengths for polymeter/polyrhythm

This is one of the KeyStep Pro’s strongest uses in Eurorack.

---

## 3. One sequencer controlling multiple oscillators as a chord voice

The manual describes **CV routing**, which is especially important in modular use.

You can route one track to multiple voice outputs. So, for example:

- **Track 1 → Voices 1, 2, 3, 4**

If a step contains multiple notes, the KeyStep Pro distributes those notes across the routed voices.

### Patch
- Voice 1 Pitch/Gate → Oscillator A / envelope A
- Voice 2 Pitch/Gate → Oscillator B / envelope B
- Voice 3 Pitch/Gate → Oscillator C / envelope C
- Voice 4 Pitch/Gate → Oscillator D / envelope D

Mix those oscillators or voices together.

### Result
You can create:
- block chords
- stacked intervals
- harmonic pads
- four-note sequenced chords
- chord stabs

This is extremely useful if your modular contains several oscillators but no dedicated chord sequencer.

---

## 4. Shared pitch with different timbral destinations

Another good Eurorack strategy is not to think of the four voices only as “four synth voices.” Instead, use them as parallel melodic control streams.

For example:
- Voice 1 controls a sine oscillator bass
- Voice 2 controls a filtered saw voice
- Voice 3 controls a resonant FM voice
- Voice 4 controls a noise-based tuned percussion voice

Even if they play related material, they can occupy different musical roles.

---

## Melodic tools in the KeyStep Pro that matter for Eurorack

## Sequencers

There are **4 sequencers**, each capable of:
- up to **64 steps per pattern**
- **16 patterns per track**
- polyphonic step content
- editable:
  - pitch
  - gate
  - velocity
  - time shift
  - randomness/probability

For modular use, this means you can create very expressive pitch/gate sequences, not just rigid note rows.

### Why this matters in Eurorack
Eurorack often excels at tone generation and modulation, but can lack a fast compositional interface. The KeyStep Pro provides that.

You can:
- enter sequences from the keyboard
- overdub chords
- set step probability
- nudge timing
- vary gate lengths
- transpose in performance

That makes modular voices feel more like playable instruments than static patches.

---

## Arpeggiators

Tracks 2–4 each have an arpeggiator.

Arp patterns include:
- Up
- Down
- Exclusive pendulum
- Inclusive pendulum
- Random
- Order played
- Poly

Arp octave ranges:
- -1
- 0
- +1
- +2
- +3

### Eurorack use
Arpeggiators are especially effective when driving:
- plucked voices
- LPG-based voices
- FM bell voices
- ratcheting acid lines
- modal ostinatos

You can hold an arpeggio and use your modular hands-on:
- open filters
- change wavefolder depth
- modulate delay feedback
- shift rhythm clocks
- repatch while the arp keeps running

This is a very modular-friendly workflow.

---

## Scale quantization

The manual highlights built-in scales:
- Major
- Minor
- Dorian
- Mixolydian
- Harmonic Minor
- Blues
- User scales

This is huge for melodic modular work.

### Why it matters
In Eurorack, raw sequencer voltages can drift into atonal territory quickly unless quantized. The KeyStep Pro lets you stay musical before CV even reaches the rack.

You can:
- keep melodies in key
- transpose live without wrong notes
- use modal harmony
- shift root notes while preserving interval relationships

### Practical uses
- Dorian for jazzy/minor grooves
- Mixolydian for synth-funk and cosmic lines
- Harmonic minor for darker cinematic sequences
- Blues scale for pentatonic riffing
- User scales for custom interval sets

---

## Chord mode

The KeyStep Pro can memorize a chord and let you trigger that chord from a single key.

### Eurorack use cases
1. **Feed one track into multiple voice outputs** to distribute the chord tones
2. **Use chord mode with arpeggiators** to generate harmonically rich note cascades
3. **Record chord patterns** into sequences for structured harmonic movement

This is a great way to get harmonic composition into a modular rig without needing a dedicated chord module.

---

## Velocity / Mod output as melodic expression

Each voice has a **Velo/Mod output** that can send either:
- velocity
- pressure/aftertouch

This is very important for expressive Eurorack patching.

### Patch ideas
- **Velocity → filter cutoff**
  - harder notes sound brighter
- **Velocity → VCA CV attenuator**
  - dynamic amplitude phrasing
- **Velocity → wavefolder amount**
  - accented notes become harmonically richer
- **Aftertouch → vibrato amount**
  - finger pressure adds expression
- **Aftertouch → FM index**
  - press into notes for aggressive timbral bloom
- **Aftertouch → reverb/delay modulation**
  - expressive ambient performance

This is one of the best ways to make a modular patch feel alive and playable.

---

## Track splits for melodic performance

The manual describes keyboard splits.

### Example split
- Lower keyboard zone → bass sequence or arp
- Upper keyboard zone → lead voice

### Modular use
You could:
- play a bassline on Track 1 into Voice 1
- play a melody on Track 2 into Voice 2
- or keep one side arpeggiated and the other manually played

This is ideal for live modular performance because one controller becomes a two-part instrument.

---

## Time division and polyrhythmic melody

Each sequence or arp can have independent time division:
- 1/4
- 1/8
- 1/16
- 1/32
- triplet variants

Each sequencer can also have independent lengths.

### Result in Eurorack
You can build:
- a 7-step bassline
- against a 12-step melody
- against a 16-step arp
- against a 5-step modulation contour

That gives you evolving melodic relationships without needing a large collection of in-rack sequencers.

This is excellent for:
- generative-feeling structures
- Berlin school patterns
- Steve Reich style phasing
- polymetric techno
- ambient counterpoint

---

## Step probability / randomness for melodic variation

Each step can carry randomness/probability.

### Eurorack advantage
Instead of repatching random voltage sources, you can keep melodic structure while introducing controlled instability.

Use this for:
- occasional passing tones
- probabilistic melody notes
- semi-generative basslines
- varied ostinatos
- evolving arpeggios

This is especially powerful with voices patched through delays and reverbs.

---

## Looper strip for modular performance

The looper strip can temporarily loop subdivisions of the current playback.

### Use in melodic performance
This can create:
- stutters
- rhythmic phrase slicing
- glitch fills
- melodic repeats
- short loop captures before dropping back to the full phrase

For Eurorack this is excellent when combined with:
- delay
- granular modules
- resonators
- LPGs
- clocked modulation

It gives you immediate performance variation without altering the original sequence.

---

## Drum gates as melodic modulators

The KeyStep Pro has **8 drum gate outputs**. These are not limited to drums.

You can use drum gates to trigger:
- envelopes
- clock dividers
- sample-and-hold
- sequential switches
- logic modules
- burst generators
- reset inputs
- LPG strikes

### Melodic uses
This is where a Eurorack musician can get clever.

For example:
- melodic CV comes from Track 1 Voice outputs
- drum gates trigger supporting modulation events:
  - accent envelopes
  - filter pings
  - delay throws
  - transposition pulses
  - switch events between oscillators
  - trigger quantized random voltages for ornamentation

So the drum section can become a **melodic articulation system**, not just percussion.

---

## Clocking and synchronization with modular

The KeyStep Pro includes:
- Clock In
- Clock Out
- Reset Out

This means it can either:
- **clock your rack**
- or **follow your rack**

### As master
Use KeyStep Pro to send clock to:
- clock divider/multiplier
- trigger sequencers
- modulation clocks
- synced delays
- Euclidean trigger generators

Then your melodic sequences stay tightly integrated with the rest of the patch.

### As slave
Use a modular clock source or trigger source to drive the KeyStep Pro.

This is useful if:
- your rack has a master clock module
- you want irregular/burst-derived tempo relationships
- you want modular timing fluctuations to affect the external sequencer

The manual specifically notes that burst-like or clock-based modulation can affect the KeyStep Pro timing creatively.

---

## Best ways to use KeyStep Pro with common Eurorack building blocks

## With oscillators
Pitch CV goes directly to 1V/oct.
Use multiple voices for:
- intervals
- unison detune stacks
- chord distribution
- canon/counterpoint

## With filters
Use Velo/Mod CV for dynamic brightness.
This gives your melodies articulation beyond pitch.

## With VCAs
Gate drives the envelope; velocity can control loudness or modulation depth.

## With function generators / envelopes
Gate outputs are perfect triggers.
Drum gates can fire secondary envelopes for accents and ornament.

## With quantizers
Usually not necessary if using KeyStep Pro pitch sequencing, since it already handles scale logic.
But quantizers can still be used on secondary modulation voltages.

## With switches
Drum gates or melodic gates can clock sequential switches to route voices or modulation differently each phrase.

## With random modules
Use KeyStep Pro for intentional pitch structure and let the rack provide:
- timbral variation
- accent variation
- ornamentation
- probabilistic modulation

## With samplers / granular modules
Pitch CV can transpose sample playback while drum gates and Velo/Mod add articulation and texture changes.

---

## Concrete melodic patch examples

## Patch 1: Modular bassline with accents
- Voice 1 Pitch → analog VCO 1V/oct
- Voice 1 Gate → ADSR gate
- ADSR → VCA CV
- Voice 1 Velo/Mod → filter cutoff CV
- Sequencer Track 1 in minor scale

Use:
- short gate on most steps
- longer gate on phrase endings
- higher velocity on accents
- occasional probability drops

Result:
A dynamic, musical bassline with phrasing and tonal consistency.

---

## Patch 2: Two-voice counterpoint
- Voice 1 → bass oscillator voice
- Voice 2 → lead oscillator voice
- Track 1 sequence length = 12
- Track 2 sequence length = 15
- same scale, different root emphasis

Result:
Interlocking melodies that evolve against each other over time.

---

## Patch 3: Chord-distributed poly patch
- Track 1 in Seq mode
- route Track 1 to Voices 1–4
- each voice patched to separate oscillator/envelope/VCA chain
- sequence polyphonic chords
- Velo/Mod from one or more voices to filter CV or LPG response

Result:
Modular chord progressions and harmonic stabs.

---

## Patch 4: Arpeggiated modal voice with aftertouch timbre
- Track 2 in Arp mode
- Voice 2 Pitch → digital oscillator
- Voice 2 Gate → LPG or envelope
- Voice 2 Mod set to Pressure
- Pressure CV → wavefolder depth or FM amount

Result:
Expressive arp performance where pressing harder changes timbre, not just loudness.

---

## Patch 5: Melodic voice plus support triggers
- Voice 1 controls melody
- Drum Gates 1–4 trigger:
  - accent envelope
  - resonator ping
  - switch reset
  - delay send envelope

Result:
A melody with structured articulations and support events tied to rhythm.

---

## Patch 6: Split keyboard live modular setup
- Lower split: Track 1 bass sequence into Voice 1
- Upper split: Track 2 lead played live into Voice 2
- Track 3 arpeggio held in background into Voice 3

Result:
A compact live performance system with bass, lead, and harmonic motion from one controller.

---

## Composition features that help melodic modular work

## Patterns
Each track has 16 patterns.
Use these for:
- verse / chorus / bridge melodic ideas
- alternate basslines
- variations on a motif
- harmonic changes

## Chains
String patterns together into longer structures.

For modular music this means:
- less repetitive looping
- more song-like evolution
- live arrangement without repatching

## Scenes
Scenes store current combinations of patterns/chains/states.

This is valuable for performance:
- one scene = sparse intro
- next scene = full bass + arp
- next scene = transposed or denser arrangement
- next scene = reduced outro

---

## Why this is especially good for melodic Eurorack

A lot of Eurorack systems are strong at:
- sound design
- modulation
- texture
- rhythm

But melodic writing can become awkward if you rely only on in-rack sequencing. The KeyStep Pro solves that by offering:

- immediate keyboard input
- proper pitch organization
- scales and chords
- multi-track arrangement
- expressive outputs
- CV and MIDI integration
- fast performance access without menu diving

In practical terms, it lets your modular system behave more like:
- a playable synth ensemble
- a compositional instrument
- a live melodic workstation

---

## Recommended melodic workflows

## Workflow 1: Bass + lead + drone
- Track 1: bass sequence
- Track 2: lead arp
- Track 3: slow drone or counterline
- Track 4: spare voice for live performance

## Workflow 2: Harmonic modular
- Route one track across multiple voices
- use polyphonic steps for chords
- use a second track for bass root movement

## Workflow 3: Modal live improvisation
- choose a scale
- hold arp
- transpose with root changes
- manually play leads over top
- modulate timbre in the rack

## Workflow 4: Semi-generative melody
- fixed melodic sequence in one track
- probability and random step behavior
- support modulation from drum gates
- different track lengths for long-form evolution

---

## Limitations to be aware of

From a Eurorack point of view:

- It is an **external controller**, not a rack module
- CV outputs are **monophonic per jack**, unless distributing poly notes across multiple voices
- true in-rack generative voltage interaction is still separate from the KeyStep Pro’s internal sequencing logic
- modulation over CV is limited to the provided outputs, though MIDI CC opens further possibilities outside pure analog paths

Still, these are minor relative to its strength as a melodic controller.

---

## Bottom line

If you're building melodic music with Eurorack, the **KeyStep Pro** can serve as the central compositional hub for your system.

It works best when you use it to provide:
- **pitch structure**
- **gate rhythm**
- **harmonic logic**
- **performance transposition**
- **arranged pattern changes**
- **expressive modulation control**

while the rack provides:
- **tone generation**
- **timbre shaping**
- **animation**
- **space**
- **voltage-based variation**

That combination is ideal:  
**KeyStep Pro for intentional melody and arrangement, Eurorack for sonic character and modulation depth.**

---

## Best use summary

Use the KeyStep Pro with Eurorack melodic modules to create:

- **basslines**
- **lead sequences**
- **arpeggios**
- **chord voicings**
- **counterpoint**
- **polymetric melodic layers**
- **expressive keyboard-played voices**
- **structured live arrangements**

The most effective patching pattern is:

1. **Pitch CV to oscillator**
2. **Gate to envelope**
3. **Envelope to VCA**
4. **Velo/Mod to timbre**
5. **Use scales/chords/arps/patterns/scenes for composition**
6. **Use drum gates for articulation and secondary modulation**

That gives you a complete melodic ecosystem around your modular rig.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)