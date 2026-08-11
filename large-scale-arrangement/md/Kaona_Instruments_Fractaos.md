# Kaona Instruments — Fractaos

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Fractaos User Manual PDF](manual)

# Using Kaona Fractaos to Build Full-Length Eurorack Songs

Fractaos is not just a “cool sound source.” It is unusually well-suited to **song construction** because it combines:

- **4 voices of polyphony**
- **multitimbral operation**
- **preset recall**
- **drone/chord behavior**
- **per-voice envelopes and filters**
- **MIDI and CV polyphonic access**
- **very wide timbral range** from tonal to noisy to percussive

That means it can function as a **central composition voice** rather than only a texture oscillator.

Below is a practical musician-focused analysis of how to use it to make **complete, evolving tracks** instead of short loops.

---

## Why Fractaos is unusually good for song building

A lot of eurorack patches stall because they are excellent at one of these:

- one strong bass loop
- one interesting sequence
- one evolving drone
- one drum groove

But songs require:

- **section contrast**
- **voice management**
- **recallable states**
- **arrangement control**
- **foreground/background roles**
- **transitions**
- **variation without repatching everything**

Fractaos directly addresses several of these pain points.

### 1. It can cover multiple musical roles at once
From the manual:

- 4 polyphonic voices
- each voice = driver + follower oscillator
- one resonant fractal filter per voice
- geometric, texture, and drum fractals
- multitimbral mode with different presets per voice

So one module can be:

- bass
- chord bed
- lead
- metallic percussion
- noise wash
- drone layer

That reduces the need to repatch entire systems between sections.

### 2. It has presets and LIVE mode
A big problem in eurorack song writing is inability to return to a previous “scene.” Fractaos stores presets on SD card and also supports **MULTI** voice assignment plus **LIVE** operation.

This means you can structure songs around:

- intro preset
- verse preset
- chorus preset
- breakdown preset
- outro preset

Or assign different voices to fixed roles while keeping one or two voices “live” for performance.

### 3. Drone mode and Spread can create harmonic sections
Drone mode is not just a sustain button. It changes Spread into:

- unison
- octave spread
- predefined chords/microtunings

This is very powerful for arrangement because one knob can create:

- tension build
- harmonic widening
- transition from monophonic focus into massive chordal wash
- breakdown drones
- ending pads

---

# Best ways to use Fractaos in full-song composition

## 1. Use Fractaos as the harmonic center of the track

Because it is 4-voice polyphonic and multitimbral, Fractaos can carry the **harmony** of a whole song.

### Patch idea
Use:
- a MIDI-to-CV/polyphonic sequencer or keyboard
- Fractaos as the central harmonic voice
- external drums and utility modules around it

### Song role assignment
Example:

- **Voice 1:** bass preset
- **Voice 2:** chord/pad preset
- **Voice 3:** lead/pluck preset
- **Voice 4:** texture/noise or percussion preset

In MULTI mode each voice can be on its own MIDI channel, so a sequencer like:
- Squarp Hermod+
- OXI One
- Intellijel Metropolix with MIDI/CV helpers
- Five12 Vector Sequencer
- Polyend Tracker/Play via MIDI
- Elektron box sending MIDI

can sequence each Fractaos voice independently.

### Why this helps songs
Instead of making one loop and trying to “expand” it later, you can compose:

- a bass line on one channel
- chord progression on another
- hook melody on another
- fills/noise accents on another

That is already the skeleton of a full arrangement.

---

## 2. Build songs by sections using presets

Fractaos’s preset system is one of its most song-friendly features.

Each preset stores:
- the main panel values
- switch states
- envelope settings

So rather than repatching for every section, create a **bank of section timbres**.

### Recommended preset strategy
Create groups such as:

- `01_INTRO_PAD`
- `02_VERSE_BASS`
- `03_VERSE_CHORD`
- `04_CHORUS_WIDE`
- `05_BREAK_GLASS`
- `06_DROP_KICK`
- `07_OUTRO_DRONE`

Then use:
- LOAD mode for whole-module recall in performance
- MULTI mode to assign different presets per voice

### Song workflow
For instance:

#### Intro
- Voice 1 LIVE texture
- Voice 2 preset pad
- Voice 3 muted
- Voice 4 noise/cluster preset

#### Verse
- Voice 1 bass preset
- Voice 2 chord preset
- Voice 3 subtle counterline
- Voice 4 percussion accent

#### Chorus
- same pitch material, but:
  - raise Texture
  - different preset with brighter fractal
  - wider Spread
  - more Morph movement
  - longer ADSR

#### Breakdown
- Drone mode on
- chord Spread in microtuning area
- no external drums
- long reverb
- slow modulations

#### Final chorus/outro
- return to note-triggered mode
- bring back drums
- open texture/noise voices
- slowly move to drone chord ending

This preset-based workflow is much closer to how songs are actually arranged.

---

## 3. Use Fractaos as a “band in a box” inside eurorack

Because it includes tonal fractals, textures, and drum models, you can treat it as a mini ensemble.

### Internal role possibilities
From the manual:

- **Geometric fractals** = stable musical tones, basses, leads, harmonics
- **Texture fractals** = pads, ambiences, noisy beds
- **Drum fractals** = kick, tom, snare, hihat, cymbal

That means Fractaos can contribute both **pitched** and **percussive** material.

### Practical use
In MULTI mode:

- Voice 1 = Kick or Tom
- Voice 2 = Snare/metallic percussion
- Voice 3 = Bass geometric fractal
- Voice 4 = Chord or pad

Then surround it with:
- external VCAs
- mutes
- effects
- sequencers
- drum reinforcement

This gives you a song-ready core very quickly.

### Caveat
I would not rely on Fractaos alone for an entire drum section in every genre. But its drum models are excellent for:
- synthetic percussion
- fills
- transitions
- hybrid drum layering
- glitch rhythm beds

A dedicated kick/snare module or sample drum module can provide the anchor while Fractaos adds character.

---

# Specific full-song patch strategies

## Strategy A: Techno / IDM arrangement engine

### Supporting modules
Pair Fractaos with:
- a multi-track sequencer: Hermod+, Vector, OXI One
- drum modules: Basimilus, BIA, WMD-style drum voices, sample player, or Squid Salmple
- mixer with mutes: Performance Mixer, Cosmix Pro, Befaco Hexmix
- effects: Mimeophon, FX Aid, Desmodus Versio, beads/granular, delay/reverb
- modulation: Pam’s Pro Workout, Batumi, Zadar, Stages
- utilities: VCAs, switches, sequential switch, logic, clock divider

### Arrangement method
#### Intro
- texture fractal like Cloud, Storm, Cluster
- very slow Speed
- moderate Texture
- Drone mode ON
- external high-pass filter slowly opening
- send to large reverb

#### Groove enters
- bring in external kick
- Fractaos voice 1 plays bass on MIDI/CV channel 1
- voice 2 adds metallic stab on offbeats
- voice 3 stays drone/pad
- voice 4 sporadic hihat-like Drum fractal hits

#### Mid-section development
Use switches:
- enable Chaos LFO modulation
- then Spread modulation
- then Morph/FM mode on selected section

This creates strong section changes without changing notes.

#### Breakdown
- mute kick and bass
- Drone mode
- Spread into chord zone
- use Just intonation, 7-limit flavor, or 19-TET slice for alien harmony
- feed into long delay and reverb
- modulate Pitch slowly with attenuated CV for rising instability

#### Drop
- exit drone
- restore rhythmic envelopes
- preset load to brighter/aggressive bass tone
- reintroduce kick and percussion
- tighten release

This produces a real song arc: density, removal, rebuild, release.

---

## Strategy B: Ambient / drone / longform evolving composition

Fractaos may be even stronger here.

### Supporting modules
Ideal companions:
- slow CV generators: Batumi, Quadrax, Maths, Zadar
- random with memory: Marbles, Sapèl, Source of Uncertainty
- matrix mixer: A-138m, AI Matrix Mixer
- spectral or resonant processing: QPAS, Ikarie, Three Sisters, Morpheus
- lush effects: reverb, shimmer, granular, looping delay
- manual performance tools: Planar 2, joysticks, mute mixer, faders

### Patch concept
Use Fractaos as four simultaneous layers:

- Voice 1: stable low drone
- Voice 2: midrange evolving harmonic body
- Voice 3: high shimmering crystalline partials
- Voice 4: intermittent noisy texture or cymbal-like breath

### How to make it a full-length piece
A longform ambient piece needs macro-structure.

Use external modulation to define 4 large phases:

1. **Arrival**  
   - low Morph
   - low Chaos
   - low Texture
   - little Spread

2. **Bloom**  
   - slowly increase Depth
   - open filter externally
   - increase LFO Amount
   - more movement in primitive

3. **Disorientation**  
   - switch to Lorenz, Hénon, Rule30, Cluster, Storm
   - introduce aftertouch or CV gestures
   - move Spread into nonstandard chord/microtuning zone

4. **Resolution**  
   - reduce Chaos
   - reduce Texture
   - move to unison cluster or just intonation
   - longer release / lower density

### Powerful trick
Put one or two voices in fixed MULTI presets and leave another in LIVE mode.  
That way:

- fixed voices = continuity across the entire piece
- LIVE voice = your active improvisational foreground

That balance is excellent for keeping a long piece coherent.

---

## Strategy C: Polyphonic song writing with external sequencer

If you want actual verse/chorus songwriting, Fractaos becomes much more useful when driven by a sequencer capable of separate tracks or polyphonic MIDI.

### Best pairing
- OXI One
- Squarp Hapax or Hermod+
- Five12 Vector
- NerdSEQ with expanders
- external DAW via MIDI
- Elektron Digitakt/Digitone/Syntakt sending MIDI

### Recommended role split
#### Voice 1
Bass line

#### Voice 2
Chord progression root/inversion note

#### Voice 3
Chord extension or melody

#### Voice 4
Lead, arpeggio, or FX accent

### Song form example
#### Verse
- minimal bass
- short envelope on chord voices
- low Morph
- low Texture
- narrow Spread

#### Pre-chorus
- increase Release
- increase primitive Speed
- automate Morph switch/LFO behavior
- add tension with Chaos modulation

#### Chorus
- wider Spread
- brighter fractal selection
- more Texture
- longer ADSR
- layered delay/reverb

#### Bridge
- switch one voice to Drum or Texture fractal
- keep bass sparse
- move chords to Drone mode
- use alternate chord/microtuning spread

#### Outro
- remove trig-based motion
- keep only drone/chord voices
- reduce amplitude and harmonic density

The reason this works is that Fractaos can retain a unified sonic identity while still changing enough between sections.

---

# Best module combinations for song-building with Fractaos

## 1. Sequencers: the arrangement brain
To make full songs, Fractaos wants a sequencer that can do more than 16-step looping.

### Strong pairings
- **Squarp Hermod+**: excellent for MIDI/poly sequencing and section changes
- **OXI One**: ideal for multitrack song mode and polymetric composition
- **Five12 Vector**: great for arranged phrases and per-track control
- **NerdSEQ**: tracker-style composition, excellent for full structures
- **DAW + MIDI**: easiest if you want formal songs fast

### Why
Fractaos provides timbral complexity; the sequencer must provide:
- section recall
- clip changes
- transposition
- mutes
- probability variation
- phrase lengths

Without that, you may still end up in loop-land.

---

## 2. Performance mixers and VCAs: essential for sections
Full songs come from **bringing parts in and out**.

Pair with:
- WMD Performance Mixer
- Befaco Hexmix
- Toppobrillo Stereo Mix
- Cosmix / Cosmix Pro
- multiple VCAs and mute modules

### Use
Send Fractaos voices or processed copies to separate channels if possible:
- dry Fractaos
- delayed Fractaos
- reverb return
- filtered resample
- bass-specific processing lane

Then create sections by:
- muting layers
- changing send levels
- automating VCA levels
- fading percussion layers up/down

Even if Fractaos is internally rich, external level control is what turns ideas into arrangements.

---

## 3. Effects: make sections feel larger than timbre changes
Fractaos naturally produces complex spectra. Effects turn those timbres into **section identities**.

### Good matches
- **Delay:** Mimeophon, Chronoblob, Rainmaker
- **Reverb:** Desmodus Versio, MercuryX, FX Aid, Erbe-Verb
- **Granular/texture:** Arbhar, Beads, Morphagene
- **Stereo imaging:** anything widening/panning/modulating
- **Saturation/distortion:** Ruina Versio, tanh modules, wavefolders, analog drive

### Song use
- verse = dry and centered
- chorus = wide stereo delay and reverb
- breakdown = granular freeze/resample
- outro = filtered feedback trails only

This can be more musically effective than changing fractal type every section.

---

## 4. Filters and dynamics processors: shape role separation
Since Fractaos can fill a lot of spectral space, external processing helps it sit in a mix.

### Pair with
- LPGs for plucky lines
- multimode filters for bass/chords separation
- compressors/sidechain tools
- transient shapers if using drum fractals
- EQ/saturation modules

### Example
- bass voice → low-pass filter + saturation
- pad voice → stereo high-pass + reverb
- percussion voice → band-pass + transient accent
- lead voice → delay and moderate compression

This makes one module feel like several distinct instruments.

---

# Practical song-building methods with Fractaos

## Method 1: One module, four song functions
Assign:

- Voice 1 = bass
- Voice 2 = chords
- Voice 3 = lead
- Voice 4 = FX/percussion

Then build arrangement only by:
- sequencer mutes
- Fractaos preset changes
- external mixer fades
- Drone mode for breaks
- effects sends

This is probably the fastest route to full songs.

---

## Method 2: Fixed backbone + live improvisation
A very strong eurorack songwriting approach is:

- 2 voices in fixed MULTI presets
- 1 voice in LIVE mode
- 1 voice for percussion or texture events

The fixed voices provide:
- harmonic continuity
- repeatable identity
- reliable structure

The live voice provides:
- performance gestures
- transitions
- fills
- improvisation

This avoids the common modular problem of “everything changes, so nothing feels like a song.”

---

## Method 3: Build sections with envelope and modulation logic
Fractaos changes character a lot depending on:

- ADSR
- Morph
- Spread
- Chaos
- Texture
- primitive-trigger behavior

So instead of always changing notes, change **behavior per section**.

### Example section map
#### Intro
- long attack/release
- Loop ON
- Trig OFF
- low Amount

#### Verse
- short attack
- medium decay
- Triggered primitive
- low Spread
- modest Texture

#### Chorus
- more Morph
- more Spread
- higher Texture
- brighter fractal
- more external reverb

#### Bridge
- FM mode
- more Chaos
- weird fractal
- less bass
- more microtonal spread

The notes may remain similar, but the song still evolves.

---

## Method 4: Use Drone mode for transitions, not just ambient pieces
A lot of users will think Drone mode is only for drone music. It is actually fantastic for **transitions**.

### Transition examples
- verse ends on held chord
- turn Drone ON
- widen Spread into chord zone
- mute drums
- send to reverb
- slowly adjust Morph and Texture
- bring in a new sequencer pattern
- switch Drone OFF into the next section

That creates a musically convincing bridge between sections.

### Especially useful chord choices
From the manual:
- Maj triad spread
- Min triad spread
- Major 7th
- Minor 7th
- Add 9
- Add 11
- Add 13
- Just intonation
- 7-limit flavor
- 19-TET slice
- Bohlen-Pierce subset

These are not just tuning novelties. They are **arrangement devices**:
- triads/7ths for stable chorus moments
- add9/add11/add13 for lush expansions
- just intonation for consonant resolution
- 19-TET/Bohlen-Pierce for alien interludes or breakdowns

---

# Genre-specific ideas

## Techno
Use Fractaos for:
- bass
- metallic percussion
- dub chords
- break drones

Best companions:
- kick module
- sequencer with mutes
- delay/reverb
- sidechain compressor

Song tactic:
- keep bass and kick constant
- use Fractaos presets for section identity
- use Drone mode for breakdowns
- use texture/drum fractals for risers and fills

---

## Ambient
Use it as:
- the whole harmonic and atmospheric core

Best companions:
- slow modulation
- stereo processing
- random voltages
- field recording or granular support

Song tactic:
- create 3–5 macro sections with different fractal families
- use microtonal spread as emotional turning points
- keep one repeating motif to maintain form

---

## IDM / Experimental
Use:
- Rule30, Lorenz, Hénon, Cluster, Aliasing, Drum fractals

Best companions:
- clock modulation
- probability sequencers
- logic and switches
- sample-and-hold
- glitch effects

Song tactic:
- alternate stable grooves and fractured passages
- let Fractaos handle timbral complexity
- use a strict drum backbone externally so the song remains legible

---

## Synth-pop / cinematic / melodic
Use Fractaos for:
- poly chords
- moving bass
- hook lead
- textural transitions

Best companions:
- MIDI keyboard or arranger sequencer
- reverb/delay
- mixer
- compressor
- maybe an additional analog mono lead voice

Song tactic:
- write actual chord progressions
- keep presets consistent across verse/chorus
- increase width and harmonic complexity in choruses
- use Fractaos as the identifiable “signature” sound of the track

---

# Limitations to be aware of when trying to make songs

## 1. The panel is shared
In MULTI mode, LIVE voices respond to the panel directly, while preset voices retain saved values in certain ways. That is useful, but it also means you should decide whether the module is acting more as:

- a fixed multitimbral instrument
- or a performable live voice

Trying to do both at once without planning can get confusing.

## 2. Preset transitions are timbral, not arrangement by themselves
Presets help, but they do not replace:
- mutes
- sequencer scene changes
- modulation planning
- dynamic mixing

You still need a larger performance architecture.

## 3. Fractaos is dense
Its sounds can occupy a lot of bandwidth. For full songs, leave room by using:
- filtering
- VCAs
- EQ
- sparse sequencing
- strategic muting

Don’t run all voices fully active all the time.

---

# A highly effective “full song” system around Fractaos

If I were building a song-focused rack around this module, I would pair it with:

- **Sequencer:** OXI One / Hermod+ / Vector
- **Clocking/modulation:** Pam’s Pro Workout
- **Complex envelopes/modulation:** Zadar or Quadrax
- **Mixer:** performance mixer with mutes
- **Effects:** stereo delay + big reverb
- **Utility:** VCAs, attenuverters, sequential switch
- **Drums:** one anchor kick + one sample drum module
- **Optional:** external compressor/sidechain

### Why this works
- Fractaos = harmonic/timbral identity
- sequencer = structure
- mixer = arrangement
- FX = spatial section changes
- drums = anchor
- VCAs/switches = movement and transitions

That is enough for intros, verses, choruses, drops, breakdowns, and outros.

---

# Example complete song blueprint

## Intro
- Fractaos in Drone mode
- Texture fractal + slow movement
- reverb high
- no drums
- Spread on Add9 or Just Intonation

## Verse A
- Drone off
- bass voice enters
- simple chord stabs
- minimal kick and hat
- lead muted

## Verse B
- subtle extra voice
- more Texture
- percussion fractal accents
- delay send up slightly

## Pre-chorus
- release longer
- Chaos modulation increases
- drums thin out
- pitch rise via sequencer transpose or CV

## Chorus
- wide Spread
- brighter chord preset
- full drums
- lead voice active
- stereo effects increased

## Breakdown
- mute drums and bass
- Drone mode on
- move to 7-limit or 19-TET spread
- granular or long delay processing

## Final chorus
- return to tonal spread
- strongest bass preset
- all main voices active
- manual Morph/Texture performance

## Outro
- remove rhythmic voices
- leave drone/chord wash
- reduce Chaos
- fade to unison cluster

This is a genuinely achievable eurorack song architecture using Fractaos as centerpiece.

---

# Final takeaway

Fractaos is especially good for full-length songs because it solves three core modular problems at once:

1. **not enough voices**  
2. **not enough recall**  
3. **not enough section contrast without repatching**

Its strongest songwriting uses are:

- **multitimbral voice assignment**
- **preset-based section design**
- **drone/chord transitions**
- **one module covering bass/chords/lead/textures/percussion**
- **external sequencer + mixer + effects for arrangement**

If you treat it not merely as an oscillator but as a **4-part fractal instrument with scenes**, it becomes a powerful foundation for complete tracks.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)