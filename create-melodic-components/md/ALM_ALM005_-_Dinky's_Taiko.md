# ALM — ALM005 - Dinky's Taiko

- [Manual PDF](../../manuals/alm005-manual.pdf)

---

[Manual PDF](attachment)

# ALM-005 — Dinky’s Taiko: using it for melodic components

Dinky’s Taiko is presented as a **12-bit digital drum voice**, but it can absolutely be pushed into **pitched, repeating, and quasi-melodic territory**. It is not a precision oscillator and the manual explicitly says **“don’t expect 1v/octave”**, but in Eurorack that still leaves a lot of room for tuned percussion, basslines, metallic melodies, and animated tonal sequences.

## What the manual tells us matters most for melodic use

From the manual:

- It has **two sound generators**:
  - a **digital noise source**
  - a **wavetable oscillator** with **24 waveforms**
- The oscillator has:
  - **Start Freq**
  - **End Freq**
  - **Speed**
  - **Release**
  - **Wave**
- There are trigger inputs for:
  - **Trigger**
  - **Accent**
  - **Choke**
- There is an output section with:
  - **Mix** between noise and oscillator
  - **Tilt EQ**
- Most importantly:
  - **all settings except tone/EQ are voltage controllable**
  - **incoming CV is added to the knob setting**
  - **values are snapshotted when a trigger is received**

That last point is especially important for melody building: **the timbre/pitch state is sampled at each trigger**, so stepped CV and rhythmic triggers become a very effective way to “play notes.”

---

## The key limitation: it is melodic, not chromatic

Dinky’s Taiko is **not a tuned VCO**. So if your goal is exact semitone tracking over several octaves, this is the wrong tool by itself.

But if your goal is any of the following, it works very well:

- **pitched percussion**
- **tom/conga lines**
- **metallic riffs**
- **FM-like pseudo-basslines**
- **atonal or modal sequences**
- **repeating “note-like” motifs**
- **electro-style tuned drum melodies**

Think of it as a **voice for contour-based pitch** rather than exact keyboard pitch.

---

## How to get melodic behavior from it

## 1. Use the oscillator as the main pitched source

For the clearest melodic result:

- turn **Mix** toward the **oscillator**
- reduce the **noise** contribution
- use **Wave** settings that are less noisy and more stable
- keep **EQ** centered or tilted to emphasize the fundamental/body

This gives you the most “note-like” core.

### Good starting settings
- **Mix**: mostly or fully oscillator
- **Noise Release**: low
- **Spectrum**: low or irrelevant if noise is mostly out
- **Oscillator Release**: medium
- **Start Freq**: set by ear
- **End Freq**: near Start Freq for more stable pitch
- **Speed**: low to medium
- **Wave**: start with sine-ish or less complex waves

The manual mentions the wavetable starts with **sines with increasing overtones**, then progresses into **squares, saws, blips, crunchy noise and vocal tracts**. For melody, start with the earlier, smoother waves.

---

## 2. Treat Start Freq as your main “note” control

If you want note changes, **Start Freq CV** is the most obvious place to send sequenced voltage.

Because the module snapshots CV at trigger time:

- send a **stepped CV sequence** to **Start Freq**
- send matching **triggers** to **Trigger**
- each hit reads a new oscillator frequency setting

This creates a line of distinct pitched hits.

### Best use cases
- 8-step tuned percussion sequence
- bass drum / tom melody
- industrial bell-like line
- quasi-arp patterns

Since it’s not 1V/oct, you’ll want to tune it **by ear**, not by scale expectations.

---

## 3. Use End Freq and Speed to shape pitch motion within each note

This is where Dinky’s Taiko becomes uniquely musical.

The oscillator moves from **Start Freq** to **End Freq** at a rate set by **Speed**. If the end is reached, it resets back to start. At higher settings this can become **metallic and FM-like**.

So instead of thinking only in static notes, think in **pitched gestures**:

- **Start high, End low** → tom drop, kick-like pitch envelope
- **Start low, End high** → rising synthetic percussion
- **Start ≈ End** → more stable note impression
- **High Speed** → complex metallic “pitched” timbres
- **Moderate Speed + close freq settings** → plucky tonal hits

### Melodic trick
Keep **Speed** fixed and sequence **Start Freq** while keeping **End Freq** near it.  
This yields a family of related pitches that feels like a melody rather than random drum variation.

### Expressive trick
Sequence **End Freq** separately from **Start Freq**.  
Then the “same note” can bend differently per step, giving you melodic phrasing instead of just pitch change.

---

## 4. Use trigger snapshotting like sample-and-hold performance logic

Because control values are captured only when a trigger arrives:

- slow LFOs into frequency inputs become **stepped melodic variation**
- random CV becomes **note-per-hit pitch sampling**
- envelopes won’t continuously sweep the note after trigger; instead they define the next note’s character

This is excellent for:

- **generative melodies**
- **controlled random tuned percussion**
- **rhythmically quantized timbral note changes**

In practice:
- Send a slow triangle LFO to **Start Freq**
- Clock a trigger pattern into **Trigger**
- Each trigger captures a different point on the LFO
- Result: repeating but evolving melodic contour

---

## 5. Accent and Choke add phrasing, not just drum dynamics

The manual says:

- **Accent** further emphasizes the hit
- **Choke** immediately stops it

For melodic use, these are powerful articulation tools.

## Accent as phrasing
Use Accent on selected steps to create:

- stronger “downbeats”
- implied note emphasis
- pseudo-accented melodic rhythm
- call-and-response patterns

This can make a simple 1-note or 2-note tuned percussion line feel much more musical.

## Choke as note length control
Because Choke immediately stops the sound, you can use it like a crude **gate length/articulation input**.

Examples:
- choke long releases to make syncopated short notes
- let some hits ring while cutting others short
- create open/closed hat style phrasing, but with pitched material

For melody, this is useful because note length is a huge part of perceived phrasing.

---

## Patch ideas for melodic components

## 1. Tuned tom melody
A classic use.

### Patch
- Trigger sequencer → **Trigger**
- Stepped CV sequencer → **Start Freq**
- **Mix** mostly oscillator
- **Wave** in the smoother part of the table
- **End Freq** slightly lower than **Start Freq**
- **Speed** low to moderate
- **Osc Release** medium

### Result
A tom/conga-like melodic line with identifiable pitches.

### Improve it
- Send accents on steps 1 and 5
- Use choke on occasional offbeats for groove punctuation

---

## 2. Metallic bassline
This module can make aggressive pseudo-bass very well.

### Patch
- Sequencer CV → **Start Freq**
- A second row or offset CV → **End Freq**
- **Speed** medium-high
- **Wave** on a richer harmonic table entry
- **Mix** fully oscillator
- **EQ** toward low frequencies
- Trigger on 8th or 16th notes

### Result
A distorted, metallic, pitch-bending bassline.

Because the pitch is not exact, it works best in:
- techno
- EBM
- industrial
- electro
- experimental

---

## 3. Bell/chime sequence
Use the reset/rollover behavior musically.

### Patch
- **Start Freq** relatively high
- **End Freq** close but not identical
- **Speed** medium-high
- **Release** medium-long
- **Wave** from the brighter/harmonic section
- sequence small CV movements into **Start Freq**

### Result
Bell-like or struck-metal melodic tones.

Add sparse Accent triggers to create “featured” notes.

---

## 4. Vocal/percussive lead fragments
The wavetable includes **vocal tract** type waves.

### Patch
- **Wave** in the vocal section
- Sequence **Start Freq**
- Modulate **Wave** with stepped CV
- Short to medium release
- Mix mostly oscillator, a little noise
- Trigger in a syncopated rhythm

### Result
Talking, formant-like melodic stabs.

This is especially effective when used as a secondary melodic hook rather than the main tonal center.

---

## 5. Generative melodic percussion
Since CV is snapshotted, random sources become very playable.

### Patch
- Random stepped CV → **Start Freq**
- Slow random or sequenced CV → **Wave**
- Euclidean rhythm or clock pattern → **Trigger**
- Sparse trigger pattern → **Accent**
- Another rhythm source → **Choke**

### Result
A self-varying line of pitched hits with coherent rhythm.

To keep it musically usable, attenuate external CV before it reaches the module, since the module’s knobs are offsets only and **do not attenuate incoming CV**.

---

## How it works with other Eurorack modules

Even though only Dinky’s Taiko is shown here, the manual itself mentions it pairs very well with **Pamela’s Workout**. More broadly, here’s how it combines with common module types to create melodic material.

## With a trigger sequencer or clock source
Essential. Since the sound is trigger-based, melodic structure starts with rhythm.

Use:
- regular clocked triggers for basslines
- sparse triggers for melodic punctuation
- polyrhythmic triggers for evolving phrases

## With a CV sequencer
Best partner for pitched use.

Send stepped CV to:
- **Start Freq** for note changes
- **End Freq** for contour changes
- **Wave** for timbral note identity
- **Mix** for morphing between tonal and noisy states

## With a quantizer
A quantizer can still help, but not in the normal exact-pitch sense.

Use it to:
- constrain the incoming CV to musically spaced voltages
- create repeatable interval relationships
- make pitch movement more intentional

Even though Dinky’s Taiko won’t track perfectly, quantized CV often still produces more coherent ear-pleasing note groupings.

## With attenuators / offset / CV utility modules
Very important because the manual says incoming CV is **added** to the knob position and not attenuated at the input.

You’ll want external utilities to:
- reduce pitch modulation range
- center the useful tonal area
- keep wave selection from jumping too wildly
- set playable frequency windows

## With envelopes and VCAs after the output
Since the internal sound is hit-based and snapshot-based, an external VCA/envelope chain can reshape it into more conventionally melodic note lengths.

For example:
- Taiko out → filter → VCA
- sequencer trigger multed to Taiko and external envelope
- use the VCA envelope to impose another amplitude contour

This can make it feel more “synth voice” and less “drum voice.”

## With filters
A filter after Dinky’s Taiko is great for melody.

Use filtering to:
- tame harsh upper partials
- emphasize a stable fundamental zone
- make metallic tones sit like leads or basses
- animate timbre with external modulation

Low-pass filtering especially helps transform drum timbres into bass/melodic parts.

## With reverb and delay
One of the easiest ways to push it into melodic role.

- Short delay: pseudo-melodic rhythmic doubling
- Long feedback delay: ambient pitched motifs
- Reverb: bell, mallet, and struck-object illusion

---

## Practical strategies for writing melodic parts

## Strategy 1: Build around relative pitch, not exact tuning
Instead of trying to force western equal temperament, choose 3–5 ear-tuned positions on Start Freq that sound musical together.

That gives you:
- root
- low fifth-ish
- octave-ish
- bright tension note
- low accent note

Then sequence among them.

## Strategy 2: Keep one parameter stable
For clearer melody, don’t sequence everything at once.

A strong starting point:
- sequence **Start Freq**
- keep **Wave** fixed
- keep **Speed** fixed
- keep **End Freq** near Start

Then add modulation once the line already reads as melodic.

## Strategy 3: Use Wave as “instrument change” per note
Instead of only changing pitch, step the **Wave** input on certain notes.

This can make one sequence feel like:
- note changes
- articulation changes
- register changes
- instrument-family shifts

## Strategy 4: Use Choke for rests and note shaping
If your trigger pattern is dense, use Choke to create implied rests and tighter phrasing. This keeps a pitched line from turning into a wash.

## Strategy 5: Layer with a stable oscillator
A very effective method:
- Use Dinky’s Taiko for the characterful, percussive pitched layer
- Layer a normal VCO/sub underneath for exact pitch grounding

This gives you:
- stable tonal center
- wild, animated attack from the Taiko
- stronger melodic readability in a mix

---

## What kinds of melodic roles it does best

Dinky’s Taiko is especially good for:

- **pitched percussion hooks**
- **electro tom melodies**
- **industrial bass motifs**
- **metallic ostinatos**
- **alien marimba-like lines**
- **formant percussive stabs**
- **atonal or modal melodic fragments**

It is less ideal as:

- a keyboard-tracked lead
- a traditional subtractive monosynth voice
- a harmonically exact tonal bass over multiple octaves

---

## Example “musical” patch recipes

## Patch A: Electro tom riff
- Trigger sequencer to Trigger
- CV sequencer to Start Freq
- Mix near oscillator
- Wave in sine/low-overtone region
- End Freq slightly below Start
- Speed low
- Release medium
- Accent on every 4th step

**Use for:** classic electro, breaks, machine funk.

## Patch B: Industrial tuned stab
- Trigger on 16ths with gaps
- Sequenced CV to Start Freq
- Random stepped CV lightly mixed into Wave
- End Freq above Start
- Speed medium-high
- Release short
- EQ slightly low

**Use for:** techno, EBM, warehouse patterns.

## Patch C: Bell melody
- Sparse trigger rhythm
- Start Freq high
- End Freq close to Start
- Speed medium
- Release long
- Wave bright but not noisy
- Reverb after output

**Use for:** ambient, IDM, soundtrack textures.

## Patch D: Pseudo-bass voice
- Mix fully oscillator
- Low EQ emphasis
- Start Freq in low range
- End Freq slightly below
- Speed low-medium
- Short release
- Sequence by ear over a small range
- Filter after output if needed

**Use for:** raw bassline foundations with percussive attack.

---

## Final take

Dinky’s Taiko is a **drum voice first**, but it’s one of those Eurorack modules that becomes much more interesting when treated as a **triggered, snapshot-based digital percussion oscillator**. Its melodic strength comes from:

- sequenced **Start Freq**
- contour from **End Freq** and **Speed**
- timbral identity from **Wave**
- phrase control from **Accent** and **Choke**
- external sequencing/utilities to tame the CV range

If you approach it as a source of **pitched percussive motifs** rather than exact notes, it can produce highly musical results and distinctive melodic layers that a conventional VCO often wouldn’t.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)