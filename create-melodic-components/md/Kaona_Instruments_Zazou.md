# Kaona Instruments — Zazou

- [Manual PDF](../../manuals/Zazou_manual_ENG_V1-0.pdf)

---

[Manual PDF](attachment)

# Using Kaona Zazou Together With Gate/Trigger Sources To Create Melodic Parts

Zazou is a **4-track generative melody module**. It does **not make sound on its own**; instead, it outputs:

- **1V/oct pitch CV** for 4 tracks
- **Gate outputs** for 4 tracks
- **Velocity CV outputs** for 4 tracks
- **TRS MIDI output**

Its key musical idea is:

- **external gates define rhythm**
- **Zazou defines pitch, phrasing, harmony, and melodic behavior**

The manual repeatedly points to **Skippy** as a natural partner, so the clearest “used together” interpretation is:

- **Skippy or another trigger/gate sequencer = rhythm source**
- **Zazou = melodic/generative pitch engine**

---

# What Zazou Does in a Patch

Zazou generates notes on **4 independent channels**. Each track can have its own:

- root note
- scale
- sequence/chord progression
- algorithm
- note duration
- velocity behavior
- ornamentation

That makes it useful as:

- a **bassline generator**
- a **lead generator**
- a **countermelody generator**
- a **4-voice polyphonic harmonic source**
- a **multitimbral MIDI composer**

---

# The Core Relationship Between Modules

## 1. Rhythm module / trigger sequencer
A module like **Skippy** sends gate signals into Zazou’s four gate inputs.

These gate inputs tell Zazou **when** to play a note.

## 2. Zazou
Zazou uses its algorithm, scale, sequence, and track settings to decide **which note** to output.

It then sends:

- pitch via **note CV out**
- gate via **gate out**
- dynamics via **velocity CV**
- optionally MIDI notes out via TRS MIDI

## 3. Voice modules
Those CV/gate outputs then drive:

- analog oscillators + envelopes + VCAs
- full synth voices
- quantizer-free melodic patches
- MIDI synths / desktop synths / multitimbral synth modules

So the full musical chain is:

**Trigger source → Zazou → synth voices**

---

# Why Zazou and Skippy Pair Well

The manual explicitly says Zazou is a good companion to **Skippy**, Kaona’s rhythm generator.

That pairing is strong because:

- **Skippy creates evolving rhythmic gates**
- **Zazou turns those gates into scale-aware notes**
- each of the 4 trigger lanes can drive 1 of Zazou’s 4 melodic tracks
- gate length can matter musically if Zazou note duration is set to **GATE**
- live rhythmic changes on the gate source instantly reshape Zazou’s phrasing

This means you can separate composition into two layers:

- **rhythmic composition** on the trigger/gate module
- **pitch/harmonic composition** on Zazou

That is a very Eurorack-friendly division of labor.

---

# Best Ways To Use Them Together

## 1. Four independent melodic lines
Patch four gate lanes from a rhythm source into Zazou’s four gate inputs.

Then patch each Zazou track to a separate voice:

- Track 1 → bass voice
- Track 2 → chord/pluck voice
- Track 3 → lead voice
- Track 4 → texture/percussion-tuned voice

This is the most direct use.

### Good setup
- same scale on all tracks
- same sequence on all tracks
- different algorithms per track

Example:
- Track 1: **WalkingBass**
- Track 2: **Arpeggio**
- Track 3: **Random**
- Track 4: **Cantor** or **Sierpinski**

This yields a coherent harmonic center, but each track behaves differently.

---

## 2. Polyphonic chord generation
Use all 4 tracks with:

- same root
- same scale
- same sequence
- same or complementary algorithms
- different octave ranges or chord settings

Patch the 4 pitch CV outputs into 4 oscillators or 4 voices.

This can create:

- chord stacks
- contrapuntal harmony
- clustered generative harmony
- pseudo-polyphonic keyboard-like behavior

A particularly effective method is:
- set all tracks to the same progression
- vary root/octave/chord voicing behavior
- let each track trigger at slightly different rhythms

That gives “moving harmony” rather than block chords.

---

## 3. Bass + accompaniment + lead structure
One of the strongest musical uses of Zazou is assigning roles:

### Track 1: bass
Use:
- **WalkingBass**
- lower octave
- simple sequence like **I-IV-V** or **II-V-I**
- moderate velocity
- quarter-note style gate source

### Track 2: accompaniment
Use:
- **Arpeggio**
- chord-restricted notes
- mid register
- regular trigger pattern

### Track 3: lead
Use:
- **Random**, **Fibonacci**, **Mandelbrot**, or **Julia**
- longer durations
- ornamentation
- wider octave range

### Track 4: counterline or drone accent
Use:
- **Interval**
- **Cantor**
- sparse rhythm
- fixed lower or upper range

This is an easy way to create a full arrangement from one module pair.

---

# How Sequences Help the Modules Work Musically Together

Zazou’s **Sequences** are not step sequencer melodies. They are more like **harmonic progression rules**.

Examples include:

- ROOT
- RANDOM
- II-V-I
- CIRCLE OF 5
- CIRCLE OF 4
- ANATOLE
- I-IV-V
- BLUES 12
- SCALE UP
- SCALE DOWN
- TIERCE UP / DOWN

These sequences transpose or reinterpret the active harmonic center over time.

That means even if the trigger source is static, the music can still evolve harmonically.

## Practical result
If Skippy sends a repeating rhythm loop, Zazou can make that loop feel like a developing song because:

- the same rhythm repeats
- but the harmonic target changes
- and algorithms react to that changing target

This is ideal for:
- jazz-like progression
- modal looping
- ambient harmonic drift
- generative tonal movement

---

# How the Gate Source Changes the Melody

A big point in the manual: **Zazou requires gate signals to trigger each note.**

So the external rhythm source has huge influence over the resulting melody.

## Short gates
With short trigger pulses:
- notes are articulated more like plucks
- if duration = GATE, notes stay short
- rhythmic detail becomes prominent

## Long gates
With longer gate lengths:
- notes sustain longer
- phrasing becomes legato-like
- good for drones, pads, slow melodic movement

## Dense rhythms
If the gate module generates dense patterns:
- Zazou can become animated and busy
- great for arpeggios and fractal algorithms

## Sparse rhythms
If the gate module is sparse:
- melodies become more spacious
- fractal/random algorithms become easier to hear
- good for ambient or soundtrack composition

So the partner rhythm module is not just a clock source—it is really a **phrase shaper**.

---

# Important Duration Behavior

Zazou has two main note timing behaviors:

## GATE duration
If duration is set to **GATE**:
- note length follows incoming gate length exactly

This is excellent with live-playable rhythm modules because changing gate width changes articulation immediately.

## Fixed duration
If a duration is set numerically:
- Zazou plays the full note value
- incoming gates during that note are ignored

This makes Zazou feel more like a phrase generator than a direct gate follower.

### Musical implication
Use:
- **GATE mode** for expressive rhythmic interaction with Skippy or another trigger sequencer
- **fixed durations** for more composed, stable melodic phrasing

---

# Useful Algorithm Pairings for Multi-Track Melodic Patches

## Random
Best for:
- melodic variation
- generative motifs
- subtle line changes

Works well when:
- scale is constrained
- octave range is limited
- repeat is disabled for more motion

Use it for:
- leads
- auxiliary melodies
- soft background lines

---

## Arpeggio
Best for:
- harmonic accompaniment
- sequenced synth lines
- classic modular melodic motion

Works especially well with:
- shared sequence progression
- regular gates from an external trigger source

Use it for:
- plucks
- polysynth-style patterns
- ostinatos

---

## WalkingBass
Best for:
- bass foundations
- tonal grounding
- jazz/blues/pop movement

Use it on one track while other tracks do freer motion.
That creates an anchored composition.

---

## Serial
Best for:
- experimental / atonal material
- academic or modernist composition
- tension lines

Important:
- only really meaningful with the **chromatic scale**
- less suited if you want strong tonal consonance

Use sparingly or on one voice only if the rest of the patch is tonal.

---

## Cantor / Sierpinski / Mandelbrot / Julia
Best for:
- self-similar melodic patterns
- evolving ambient lines
- generative experimentation

These are ideal if you want:
- repetition with mutation
- mathematically flavored phrasing
- a sense of emergence rather than explicit composition

They work best when paired with:
- limited octave range
- slower note durations
- restrained sequences

Otherwise things can become too chaotic.

---

## Fibonacci
Best for:
- natural-feeling expansion
- melodic growth
- pattern-based lines that feel ordered but not obvious

Very good for:
- leads
- secondary phrases
- semi-predictable melodic development

---

## Interval
Best for:
- strict intervallic hooks
- sequenced motifs
- pattern-based melodic riffs

Because it does not ensure scale membership of resulting notes, it can be:
- consonant
- modal
- dissonant

depending on interval and context.

Great for:
- techno patterns
- minimalist ostinatos
- experimental counterpoint

---

# How To Build Strong Melodic Components

## A. Tonal generative patch
For music that stays musical and coherent:

- choose one scale for all tracks
- use one sequence for all tracks
- vary algorithms
- keep octave ranges moderate
- use passing notes and ornaments sparingly

### Example
- Scale: D Dorian
- Sequence: II-V-I or ROOT
- Track 1: WalkingBass
- Track 2: Arpeggio
- Track 3: Fibonacci
- Track 4: Random

Result:
- bass anchors harmony
- arpeggio defines chord feel
- Fibonacci creates melody
- random adds variation

---

## B. Evolving ambient patch
For slowly shifting melodic atmospheres:

- sparse external gates
- longer note durations
- fractal algorithms
- shared scale, different roots or octaves
- low to medium velocity
- ornamentation minimal

### Example
- Scale: Lydian or Pentatonic Minor
- Sequence: Circle of 5 or Scale Up
- Track 1: Cantor
- Track 2: Sierpinski
- Track 3: Mandelbrot
- Track 4: Julia

Result:
- drifting harmonic motion
- repeating but evolving phrases
- wide ambient melodic field

---

## C. Groove-based patch
For rhythmic electronic music:

- use Skippy or another rhythm generator with active patterns
- duration = GATE on some tracks
- one track for bass, one for arp, one for stab, one for lead
- use velocity CV to animate timbre or VCA level

### Example
- Track 1: WalkingBass
- Track 2: Arpeggio
- Track 3: Interval
- Track 4: Random

Patch velocity CV not only to amplitude but also to:
- filter cutoff
- wavetable position
- FM depth
- envelope decay

This makes the melodies more expressive.

---

# Velocity CV Is Very Useful

A strong feature of Zazou is that it outputs **velocity as CV** per track.

That means dynamics are not limited to MIDI.
In Eurorack, that velocity CV can control:

- VCA level
- filter cutoff
- wavefolder amount
- envelope depth
- FM index
- effect send amount

So one melody line can have pitch, gate, and expressive modulation all coming from Zazou.

This is one of the best ways to make generative lines feel alive.

---

# Sequence Change Tricks

Zazou also has **Change** and **Reset** controls, by button or CV.

This lets you coordinate form with other modules.

## Change input/button
Advances sequence by one step.

Use this to:
- manually push chord changes
- trigger formal changes from another module
- make a pattern progress only at chosen moments

## Reset input/button
Resets playback to the start.

Use this to:
- resync all tracks to bar 1
- restart harmonic structure
- recover from intentional chaos during performance

## Sequence setting: CHANGE GATE = EXT
This is especially powerful.
In this mode, sequence changes happen only from the external change gate/button.

That allows a separate module or performer gesture to control **when harmony moves**.

So rhythm can continue constantly while harmony only changes when you decide.

---

# Manual Performance Ideas

Zazou is not just a set-and-forget generator.

## In Algorithms and Sequences screens
The colored buttons can manually play notes.

That means you can:
- audition per-track behavior
- tap notes manually
- test parameter changes live

## In Live mode
The colored buttons become **mute** for each track.

This is excellent for arrangement:
- mute bass
- bring in lead
- strip back accompaniment
- drop to one fractal line

## Play/Stop
Stops all tracks together.

## Reset
Restarts and also sends MIDI all-notes-off if needed.

So even with generative material, Zazou can be performed like a structured instrument.

---

# MIDI and CV Hybrid Use

Zazou can drive both:

- **modular voices via CV/gate**
- **external synths via MIDI**

This opens useful combined setups.

## Example hybrid setup
- Track 1 CV/gate → analog bass voice
- Track 2 CV/gate → pluck voice
- Track 3 MIDI → polysynth pad
- Track 4 MIDI → FM desktop synth lead

Or:
- all 4 tracks on different MIDI channels into one multitimbral synth
- while velocity CV outputs modulate modular effects or envelopes

This makes Zazou a strong center for a mixed hardware setup.

---

# Good “Used Together” Patch Recipes

## Patch 1: Simple song starter
- 4 rhythm outputs from Skippy to Zazou gate inputs
- Zazou Track 1 note/gate → bass synth
- Zazou Track 2 note/gate → pluck synth
- Zazou Track 3 note/gate → lead synth
- Zazou Track 4 note/gate → pad or bell synth

Settings:
- same root and scale on all tracks
- same sequence on all tracks
- different algorithms on each track

This immediately creates a layered melodic arrangement.

---

## Patch 2: One rhythm source, many harmonic voices
If your gate source is less complex, you can still:
- feed similar rhythmic material to multiple tracks
- let Zazou create differentiated pitch content by algorithm

Use:
- same trigger density
- different octave ranges
- different chord settings
- different ornaments

This yields tightly related but non-identical lines.

---

## Patch 3: Controlled generative improviser
- Set sequence progression to **II-V-I**, **Anatole**, or **Circle of 5**
- Keep one track as WalkingBass
- Use Random/Arpeggio/Fibonacci on other tracks
- Advance harmony using the **Change** input manually or from another trigger stream

This acts like a generative accompanist that can follow song form.

---

## Patch 4: Fractal texture over tonal bass
- Track 1 = WalkingBass in a simple scale
- Tracks 2–4 = Cantor/Sierpinski/Mandelbrot
- sparse trigger inputs for fractal voices
- longer durations
- same root/scale shared

This keeps the overall patch musical while allowing abstract upper motion.

---

# Recommended Practical Approaches

## For tonal music
Start with:
- Major, Minor, Dorian, Mixolydian, Pentatonic
- WalkingBass + Arpeggio + Random/Fibonacci
- simple sequences like ROOT, I-IV-V, II-V-I

## For jazzier results
Start with:
- Bebop Major / Bebop Minor / Blues / Dorian
- WalkingBass
- Anatole or II-V-I
- voicing enabled where available

## For experimental music
Start with:
- Chromatic scale
- Serial / Interval / Julia / Mandelbrot
- independent sequences per track
- random chord and duration behavior

## For ambient
Start with:
- sparse gates
- long durations
- fractal algorithms
- muted sequence motion
- velocity CV to timbre rather than volume

---

# Limitations To Keep In Mind

## Zazou is not a sound source
You still need:
- oscillators or voices
- envelopes / VCAs if using raw CV
- or MIDI synths

## It is gate-driven, not clock-driven
The manual is clear:
- Zazou does not use a normal clock input
- it depends on incoming gates to trigger notes

So if you want more notes, more rests, or different phrasing, the gate generator matters a lot.

## Some settings can get chaotic
Because Zazou can combine:
- randomization
- ornaments
- fractal logic
- sequence transposition
- wide octave range

it can quickly go from musical to wild.
Usually the most usable patches come from **limiting a few parameters**.

---

# Best Overall Strategy

The best way to use these modules together for melodic creation is:

1. Use the rhythm/gate module to generate **when** notes happen.
2. Use Zazou to generate **what** notes happen.
3. Send Zazou’s outputs to several voices for bass, harmony, lead, and texture.
4. Keep all tracks in one scale/sequence at first.
5. Differentiate tracks by algorithm, octave, duration, and velocity.
6. Use Live mutes and Change/Reset for performance structure.

In short:

- **Skippy or another gate source gives the groove**
- **Zazou gives the melody and harmony**
- **your voices and modulation turn that into a complete musical arrangement**

---

# Quick Starter Patch

If you want one immediate patch from the manual:

## Connections
- 4 gate outs from Skippy → 4 Zazou gate ins
- Zazou Track 1 note/gate → bass voice
- Zazou Track 2 note/gate → pluck voice
- Zazou Track 3 note/gate → lead voice
- Zazou Track 4 note/gate → pad voice
- velocity CVs → filter cutoff or VCA CV on each voice

## Zazou settings
- Root: C or D
- Scale: Minor or Dorian
- Sequence: I-IV-V or II-V-I
- Track 1: WalkingBass
- Track 2: Arpeggio
- Track 3: Fibonacci
- Track 4: Random
- Duration: GATE on bass/arp, longer fixed values on lead/pad

This should produce a playable, coherent, multi-part generative composition quickly.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)