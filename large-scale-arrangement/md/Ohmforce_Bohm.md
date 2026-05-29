# Ohmforce — Bohm

- [Manual PDF](../../manuals/Bohm documentation.pdf)

---

[Manual PDF / Bohm Documentation](https://ohmforce.com/wp-content/uploads/2025/03/Bohm-documentation.pdf)

# Using Ohm Force Bohm to build full-length Eurorack songs

Bohm is not just a kick module. It is really a **performance-oriented kick system** with:

- a main kick voice (**Bohm**),
- an optional secondary rhythm/rumbler layer (**Groove**),
- an optional sidechain/effects/performance mixer (**Performer**),
- **snapshots, programs, and live modes** for arranging,
- **CV-driven model randomization and step changes**.

That means it can function as a **structural anchor** for full tracks, not just a single drum sound.

The big idea is this:

> Use Bohm as the module that defines **sections, transitions, energy, and groove**, while other modules provide melody, bass, hats, percussion, drones, and harmonic movement.

In many Eurorack systems, the loop sounds great but never becomes a song because there is no strong mechanism for:
- changing sections,
- recalling states,
- introducing contrast,
- creating fills and transitions,
- controlling tension/release over time.

Bohm directly helps with that.

---

# What Bohm contributes to song-making

From the manual, the most important song-building features are:

## 1. Snapshot-based recall
You can save kicks as **snapshots** containing:
- model variations,
- and in live contexts, knob positions too.

This is huge for arrangement. Instead of one kick for the whole patch, you can prepare:
- verse kick,
- chorus kick,
- breakdown kick,
- bridge kick,
- fill kick,
- outro kick.

That alone gives you **section identity**.

---

## 2. Programs with up to 16 steps
Bohm has:
- **32 programs**
- each with **1–16 steps**
- each step stores a full kick snapshot.

So one program can effectively act like a **song section timeline** or a library of scene recalls.

---

## 3. Song mode
In **Live Song mode**, the FUNCTION trigger advances through a sequence of stored kick states.

This means Bohm can become a **section sequencer**:
- Step 1 = intro
- Step 2 = verse
- Step 3 = chorus
- Step 4 = verse variation
- Step 5 = breakdown
- Step 6 = build
- Step 7 = drop
- Step 8 = outro

Because the next step is cued and becomes active on the next HIT, this is ideal for musically clean transitions.

---

## 4. Jam mode
In **Live Jam mode**, you can freely cue the next snapshot from a program.

This is perfect if your songs are not rigidly linear. You can improvise:
- extend a breakdown,
- jump back to a groove,
- bring in a harder kick,
- move to a transition state when the room feels ready.

---

## 5. Groove as a second rhythmic energy layer
The optional **Groove** expander is extremely important for turning beats into arrangements.

It is not just a copy of the kick:
- it can produce repetitions,
- reverb-based rumbles,
- noise,
- grit + sub,
- tap envelopes,
- stereo shaping,
- filtering/distortion.

That gives you section changes without repatching:
- tight dry verse,
- wider rumble chorus,
- noisier breakdown,
- minimal kick-only intro,
- dense techno drop.

---

## 6. Performer as sidechain mixer / transition processor
The **Performer** expander can:
- duck external stereo input on every kick,
- process either kick, input, or both,
- apply DJ filter / LP / HP / beat roll / slip roll,
- toggle effects instantly or synced to HIT,
- split low frequencies for more transparent ducking.

This is one of the strongest “make it a song” tools in the whole system.

It lets Bohm become the center of:
- sidechain pumping,
- breakdown filtering,
- transition rolls,
- live drop effects,
- balancing external stems or voices against the kick.

---

# Core strategy: use Bohm as the arrangement brain for rhythm and energy

A full-length song in Eurorack usually needs these musical layers:

1. **Pulse** – kick and timing backbone  
2. **Groove** – secondary percussion / swing / rumble / syncopation  
3. **Bass** – repeating or evolving low-frequency motif  
4. **Harmony or texture** – pads, drones, chords, sampled atmospheres  
5. **Lead or hook** – melody, riff, vocal sample, acid line, etc.  
6. **Transitions** – fills, mutes, filters, drops, crescendos  
7. **Section control** – intro / verse / chorus / breakdown / drop / outro

Bohm mainly handles **1, 2, 6, and part of 7**, and it can strongly influence 3 and 4 through pitch tracking, ducking, and audio routing.

---

# The most useful song-building workflows

## Workflow 1: Bohm as the “section-changing kick arranger”

This is the most obvious and effective use.

### Patch concept
Use other modules for:
- melody sequencer,
- bass voice,
- hats/percussion,
- pads/drone.

Use Bohm to store a different kick+Groove+Performer state for each section.

### Example song map
Program 1:
1. Intro – soft kick, low FX, no Groove
2. Verse – tighter kick, mild Groove taps
3. Chorus – bigger kick, wider stereo, more rumble
4. Verse 2 – slightly brighter transient
5. Breakdown – minimal kick, Performer HP filter on external audio
6. Build – rising FX, stronger ducking, beat roll
7. Drop – full kick + Groove + wide stereo
8. Outro – reduced sustain and FX

Advance steps using:
- a manual button,
- a trigger sequencer,
- an end-of-cycle pulse from a clock divider,
- a gate pattern from a song controller module.

### Good companion modules
- **ALM Pamela’s Pro Workout** for section-length trigger control
- **Make Noise Tempi** for master clock and divisions
- **Intellijel Steppy** for section change triggers
- **Malekko Varigate 8+** or **Winter Modular Eloquencer** for song-level rhythm control
- **Five12 Vector Sequencer** for coordinated song structure

### Why it works
Even if the rest of the patch loops, the song feels arranged because the **drum identity and pumping behavior** evolve by section.

---

## Workflow 2: Use Bohm Song Mode as a “macro-arrangement spine”

Because Song Mode can queue the next step and follow program logic, it can act like the backbone of the performance.

### How to build it
Create one program per song section family:
- Program 1 = intro/verse states
- Program 2 = chorus/drop states
- Program 3 = breakdown/build states

Or one whole song in a single program with up to 16 steps.

Use another module to synchronize larger changes:
- sequential switch for bass pattern changes,
- preset manager for oscillator/filter states,
- clocked sequential trigger switch for drums,
- CV recorder or automation source for timbral shifts.

### Best partner modules
- **Make Noise Rene** or **Verbos Sequence Selector** for pattern changes
- **Erica Synths Sequential Switch** or **Doepfer A-151** for switching melodic CV sources
- **Noise Engineering Mimetic Digitalis** for section-specific modulation offsets
- **Acid Rain Maestro** or **Xaoc Devices Zadar** for evolving modulation per section
- **Rossum Assimil8or** or **1010 Bitbox** for section-specific samples/stems

### Song trick
Send the same “section advance” pulse to:
- Bohm FUNCTION input,
- a sequential switch,
- a reset input on your melodic sequencer,
- a logic module that opens/closes percussion VCAs.

Then one event changes the whole song section.

---

## Workflow 3: Use Groove to create arrangement contrast without adding more drum modules

The Groove expander is ideal for creating the illusion of a much larger drum arrangement.

It can do:
- techno rumble,
- kick tops,
- repeated taps,
- noise envelope movement,
- sub grit,
- stereo width changes,
- effect changes.

### Section uses
- **Intro**: Bohm only, Groove volume down
- **Verse**: Groove as subtle tap pattern
- **Pre-drop**: Groove noise source, HP-filtered
- **Drop**: full repetition/rumble
- **Breakdown**: Groove drone using GRV ENV = SUSTAIN
- **Outro**: remove Groove again

### Why it is musically important
A full song usually needs the low-end density to change over time. Groove gives you:
- “small” section vs “big” section,
- “dry” vs “washy”,
- “tight” vs “club-wide”.

That is arrangement.

### Smart external patching
Use the **TAPS output CV** to animate other modules:
- open a VCA on a noise hat layer,
- modulate a filter on a bass drone,
- drive sidechain-like envelope on pads,
- hit an LPG for percussive textures.

Since TAPS can output Groove, inverted Bohm, Performer, or Bohm envelopes depending on system setting, it becomes a **song-wide dynamics control source**.

---

## Workflow 4: Use Performer as the glue mixer for full tracks

The Performer expander is maybe the most underrated part of Bohm for songwriting.

You can route external stereo audio into it and then:
- duck it from the kick,
- filter it,
- beat roll it,
- slip roll it,
- process only the kick, only the input, or both.

### This means you can run into it:
- a stereo submix from your whole patch,
- a stereo sampler stem,
- a chord voice,
- drones/atmospheres,
- a melodic bus,
- even an external groovebox.

### Song-building uses
#### A. Breakdown generator
Send your whole melodic/percussion mix into Performer.
- In full sections: mild ducking, no filter
- In breakdown: high-pass the input
- In build: increase resonance or beat roll
- On drop: return to full-range audio

That is a classic song arc.

#### B. Live sidechain architecture
Instead of separately patching envelope followers and VCAs, let Bohm do:
- kick,
- ducking,
- performance FX,
- output summing.

Then your song instantly gets the “record-like” pumping and transitions that help loops feel finished.

#### C. DJ-style transitions
Use:
- **DJ FILTER** for opens/closes,
- **BEAT ROLL** for fill energy,
- **SLIP ROLL** for stuttered transitions before a drop.

You can perform these by hand or snapshot them as states.

---

# Use Bohm’s pitch tracking to create bass lines and song hooks

The manual says Bohm can track pitch at **1V/oct** if configured properly:
- set PITCH knob fully CCW,
- PITCH attenuverter fully CW,
- choose the correct voltage range in settings.

This means Bohm is not only a kick. It can become a **tuned bass percussion voice**.

## Musical applications

### 1. Kick-bass hybrid line
Sequence pitch CV into Bohm so the kick follows the root note of the section:
- verse on C,
- pre-chorus on F,
- chorus on G,
- breakdown on A minor variation.

This alone makes a loop feel like a song because the low end now reflects harmonic structure.

### 2. Sustained gated bass notes
Since HIT can behave as a gate, you can create longer sustained bass/kick notes for:
- breakdown bass drones,
- pitched sub accents,
- tom-like phrases,
- pseudo-bassline hooks.

### 3. Call and response with another bass oscillator
Layer Bohm as the transient/low-end thump and use another VCO/filter voice for sustained bass tone.

Good companion modules:
- **Instruō Ts-L**
- **Intellijel Dixie II+**
- **AJH MiniMod VCO**
- **Mutable Plaits**
- **SSF Zephyr / steady utility oscillators**
- any LPG/filter/VCA chain

Use a precision adder or sequential switch to change bass transposition by section.

---

# Use presets and switches with Bohm for complete song scenes

Bohm can store its own internal states, but full songs become easier when other modules also change state with it.

## Best matching module types

### Preset managers
- **Tiptop Audio ART-oriented preset tools**, if present in your ecosystem
- **Flame Memory Joystick / preset-style modules**
- **MIDI-to-CV with preset recall**
- modules with internal patch memory

### Sequential switches
- **Doepfer A-151**
- **Boss Bow Two / Joranalogue Switch 4 / similar utilities**
- **Verbos Sequence Selector**
- **Worng Soundstage ecosystem with switched submixes**
- **Shakmat modular switching utilities**

### CV storage / macro control
- **Frap Tools USTA**
- **Mimetic Digitalis**
- **Voltage Block**
- **Tetrapad/Tete**
- **Planar 2** as a performance macro source

### Why this matters
The classic reason a Eurorack patch doesn’t become a song is that too many parameters are static.  
If Bohm changes section but your bass/filter/harmony don’t, it still feels loop-based.

So make Bohm the center of a **scene-change ecosystem**.

---

# Practical song templates using Bohm

## Template 1: Techno full-length performance patch

### Modules
- Bohm + Groove + Performer
- Master clock: Pamela’s Pro Workout
- Bass sequencer: Metropolix or Vector
- Bass voice: analog VCO + filter + VCA
- Hats/percussion: sample module or noise voices
- Texture: stereo sample player or wavetable voice
- Mixer / VCAs / filter / delay / reverb

### Patch
- Pam’s clock to Bohm HIT and Groove CLOCK-related timing sources
- Section-advance trigger to Bohm FUNCTION
- Bass voice into its own mixer channel
- Full melodic/percussion submix into Performer IN
- Performer output to master output
- TAPS CV out to modulate hat VCA or pad filter
- Bohm pitch CV from sequencer for tuned kick in selected sections

### Arrangement
- Intro: filtered texture into Performer, no Groove
- Verse: kick + bass only
- Add hats after 16 bars
- Add Groove rumble at chorus/drop
- Use Performer DJ filter for breakdown
- Use beat roll before drop
- Cue harder kick snapshot for final drop
- Remove Groove and lower kick sustain for outro

This can easily become a full 5–8 minute live techno structure.

---

## Template 2: Electro / IDM structured song

### Use Bohm for:
- multiple kick models per section,
- transient variation,
- pitch tracking for melodic drum phrases,
- Groove as top/rhythm texture rather than rumble.

### Companion modules
- melodic sequencer with song mode
- logic module for conditional triggers
- random source for fills
- sampler for one-shots and transitions
- wavefolder/FM voice for lead elements

### Song method
Save snapshots with:
- dry compact kick for verses,
- glitchier FM kick for fills,
- brighter transient for chorus,
- Performer slip roll for transitions.

Use Jam Mode instead of Song Mode if you want to choose alternate phrase endings live.

---

## Template 3: Ambient / experimental long-form piece

Bohm is still useful here, but not just as a four-on-the-floor kick.

### Use:
- PM-K1 model for acoustic physical drum gestures
- gated HIT for long resonant shapes
- pitch tracking for tuned low percussion
- Groove drone behavior with **GRV ENV = SUSTAIN**
- Performer ducking as subtle dynamic breathing

### Companion modules
- resonator voices
- granular sampler
- stereo reverb
- slow CV generators
- clock divider for sparse event timing
- sequential switch for evolving trigger sources

### Structure
- start with sparse PM-K1 impacts and drones
- gradually bring Groove textures
- route ambient stereo bed through Performer for subtle kick-synced breathing
- switch to FM-2X or WT-4 for more synthetic middle section
- return to sparse acoustic model in outro

This is a good example of using Bohm for **narrative evolution**, not just a dance kick.

---

# How to solve the “loop that never becomes a song” problem with Bohm

Here are the main strategies.

## 1. Give each section a different low-end identity
Most Eurorack jams fail structurally because the kick never changes enough.

With Bohm, change:
- model,
- transient type,
- distortion,
- stereo width,
- Groove presence,
- ducking amount,
- Performer effect state.

Even small changes make sections feel intentional.

---

## 2. Use mutes and density control
A song develops by **adding and removing layers**.

With Bohm:
- remove Groove for reduced sections,
- reduce Sustain/Length for tighter moments,
- use Performer VOL and ducking to rebalance the full patch,
- cue snapshots with less FX and less stereo width for verses,
- restore full-width/rumble on drops.

Pair with:
- mute modules,
- VCAs under sequencer control,
- trigger mutes,
- switched clocks.

---

## 3. Create transitions, not just pattern changes
A song needs connectors between ideas.

Bohm can supply these with:
- beat roll,
- slip roll,
- DJ filter sweeps,
- FX on/off synced to HIT,
- transient tone changes,
- pitch drops/rises,
- randomization for fills.

You can dedicate one or two snapshots per program just to transitions.

For example:
- Step 7 = “build”
- Step 8 = “fill”
- Step 9 = “drop”

---

## 4. Use external audio through Performer
This is one of the clearest ways to make your modular patch feel like a finished track.

Instead of letting all other voices float separately, submix them and send them into Performer.
Now the kick can:
- carve space,
- create pumping,
- filter the whole mix for breakdowns,
- apply roll effects for transitions.

That kind of integrated dynamics is often what makes a loop become a track.

---

## 5. Make one control event change many things
To build songs, think in **scene changes**.

A single trigger or gate can:
- advance Bohm to next step,
- switch melodic sequence,
- reset clock divider,
- open a VCA for pads,
- mute hats,
- transpose bass.

This is how modular starts behaving like a compositional instrument instead of a perpetual loop.

---

# Excellent module pairings for full-song creation

## Sequencers and song controllers
Best with Bohm:
- **Five12 Vector Sequencer**
- **Winter Modular Eloquencer**
- **Metropolix**
- **Hermod+**
- **Varigate 8+**
- **Pamela’s Pro Workout** as timing brain

These can send:
- clock,
- reset,
- section-advance triggers,
- pitch CV for tuned kick,
- modulation tied to song sections.

---

## Mixers / VCAs / performance control
- **Happy Nerding 3xVCA / 4x Stereo Mix**
- **Befaco Hexmix / Hex VCA**
- **WMD Performance Mixer**
- **Frap Tools CGM**
- **Mute modules** and **sequential switches**

Bohm becomes much more song-capable if you can mute and submix other layers around it.

---

## Modulation
- **Acid Rain Maestro** for hands-on section modulation
- **Voltage Block** for timeline automation
- **Zadar** for complex envelopes
- **Pam’s** for synchronized modulation
- **Batumi** for LFO-based movement

Use them to vary:
- filter opening,
- bass tone,
- delay send,
- drone level,
- percussion density.

---

## Switching / logic / utilities
- **Doepfer A-151**
- **Joranalogue Compare 2**
- **Klavis Logica XT**
- **Mutable Branches / logic equivalents**
- **Sequential switches**
- **clock dividers**

These are essential for full-song architecture. Bohm provides the section concept; utilities distribute it.

---

## Samplers and texture modules
- **1010 Bitbox**
- **Rossum Assimil8or**
- **Morphagene**
- **Squid Salmple**
- **stereo loopers or sample players**

These pair extremely well with Performer’s ducking/filtering.  
You can run:
- pads,
- vocals,
- noise beds,
- percussion loops,
- field recordings
through Performer and make them “breathe” with the kick.

---

# Concrete patch recipes

## Recipe 1: 6-minute techno arrangement
### Goal
A full track with intro, build, drop, breakdown, second drop, outro.

### Bohm setup
Create snapshots:
1. Intro minimal kick
2. Verse kick
3. Verse + light Groove
4. Drop kick + full Groove
5. Breakdown filtered input only
6. Build with beat roll
7. Main drop with harder FX
8. Outro reduced kick

### Other modules
- bassline sequencer with two patterns
- hats/percussion on mutes
- stereo pad/sample into Performer input
- master clock + section trigger module

### Performance
Advance FUNCTION every 16 or 32 bars.
Use manual mutes for hats and percussion.
Let Performer handle the big transitions.

---

## Recipe 2: Song with harmonic movement
### Goal
Make the kick support chord changes.

### Patch
- pitch sequencer multed to bass voice and Bohm PITCH CV
- Bohm configured for 1V/oct tracking
- long HIT gates in some sections for bass-like sustain
- Groove only during choruses

### Result
The kick root follows the song harmony.  
This is subtle but extremely effective for making the arrangement feel composed.

---

## Recipe 3: Live improvisational set
### Goal
A non-linear performance where you can extend sections as needed.

### Setup
- Use Jam Mode
- Store 8–12 snapshots in one program:
  - 2 intros
  - 3 groove states
  - 2 breakdowns
  - 2 build states
  - 3 drops

### Pair with
- manual mute mixer
- joystick macro controller
- trigger pads or pressure controller
- stereo texture source into Performer

### Result
You can respond to the room while still having structured, recallable section changes.

---

# Best practices for turning Bohm into a song tool

## Prepare snapshots as musical roles, not just sound presets
Don’t save 10 random kick tones. Save:
- intro,
- verse,
- verse lift,
- chorus,
- build,
- breakdown,
- fake-out,
- final drop,
- outro.

Name them accordingly.

---

## Use programs as songs or song banks
A practical approach:
- Program 1 = track 1
- Program 2 = track 2
- Program 3 = track 3

Or:
- Program 1 = intros
- Program 2 = main grooves
- Program 3 = transitions
- Program 4 = drops

Depends whether your live set is fixed or improvised.

---

## Set knob behavior intentionally
The manual gives:
- **Latch**
- **Relative**
- **Override**

For full-song work:
- use **Override** for knobs you want live control over all the time,
- use **Latch** when you want snapshot accuracy first,
- use **Relative** when you want safe morphing from stored states.

For example:
- Bohm COLOR in Override = always playable
- Performer FX in Latch = recall exact transition states
- Groove VOL in Relative = easy live balancing

---

## Use Performer Exclude/Include wisely
If you want the same global performance FX setup across many steps, leave Performer **excluded** from step recalls.
If each section needs specific filtering/ducking/FX states, set it to **include**.

That is very useful for deciding whether Performer acts like:
- a global performance bus,
or
- a per-section arrangement processor.

---

## Build transitions into your clocking
A full song is often just:
- 16 bars groove,
- 8 bars variation,
- 8 bars build,
- 16 bars drop,
- 8 bars breakdown.

Use clock dividers or song sequencers to send FUNCTION triggers at those boundaries.

This avoids the endless-loop trap.

---

# Limitations to keep in mind

Bohm is powerful, but it is not a full song workstation by itself.

It does **not** replace:
- a melodic sequencer,
- a voice allocator,
- a full mixer,
- VCAs and mutes,
- utility logic,
- dedicated harmonic control.

Its strength is that it gives your patch:
- **section recall**
- **rhythmic identity**
- **dynamic glue**
- **performance transitions**
- **low-end evolution**

That is exactly the set of things many modular systems lack when trying to become full songs.

---

# My recommended “full song” mindset with Bohm

If I were building songs around Bohm, I would think of it in these roles:

## Bohm = arrangement kick instrument
Use saved states to define sections.

## Groove = energy and density control
Bring it in and out to scale the arrangement.

## Performer = master movement processor
Sidechain, filter, and transition the rest of the patch.

## External modules = notes, harmony, color
Let sequencers, oscillators, samplers, and mixers provide the musical content around Bohm’s structure.

When used like that, Bohm becomes less of a drum module and more of a **song-form engine for live modular performance**.

---

# A strong practical setup for full-length songs

If you want one concrete recommendation, here is a very effective architecture:

## Core
- Bohm + Groove + Performer
- Pamela’s Pro Workout
- one bass sequencer + bass voice
- one melodic/sample voice
- one hat/percussion source
- submixer
- a few VCAs/mutes
- reverb/delay

## Routing
- Bohm is master kick
- Groove adds sectional density
- all non-bass melodic material goes into Performer IN
- Performer OUT goes to main output
- bass stays partly separate or mixed carefully to preserve low-end clarity
- section triggers from Pam’s or sequencer go to Bohm FUNCTION
- TAPS CV modulates hats or melodic amplitude/filtering

## Musical result
You get:
- kick evolution,
- automatic pumping,
- breakdown filters,
- fill effects,
- song sections,
- room for improvisation.

That is enough to make genuinely full-length modular tracks.

---

# Final takeaway

The key to using Bohm for full songs is not just “making a better kick.”  
It is using its **snapshots, programs, Song/Jam modes, Groove layer, and Performer bus processing** as a framework for:

- section changes,
- tension and release,
- transition effects,
- mix movement,
- low-end evolution,
- and coordinated performance control.

If you combine Bohm with:
- a clock/song trigger source,
- melodic/bass sequencers,
- mixers and VCAs,
- switches and utilities,
- and a stereo source into Performer,

then Bohm can become one of the most effective modules in a Eurorack system for turning a good loop into a full, performable song.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)