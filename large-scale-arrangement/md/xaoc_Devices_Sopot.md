# xaoc Devices — Sopot

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Fractaos Manual PDF](#)

# Using Kaona Fractaos to Build Full-Length Eurorack Songs

Fractaos is not just a “weird oscillator.” It is much closer to a **4-voice fractal sound engine** with:

- 4 polyphonic voices
- 8 total oscillators arranged as driver/follower pairs
- per-voice ADSR and fractal filter
- preset loading/saving
- Drone mode
- true multitimbral operation
- MIDI and CV polyphony
- drum/percussion models
- geometric tonal fractals
- noisy texture generators

That combination is unusually important for songwriting, because the biggest obstacle in Eurorack is often not making *a good sound*, but making **enough contrast, structure, recall, and arrangement states** to sustain a track for 4–8 minutes.

Fractaos is one of the rare Eurorack modules that can help with that directly.

---

## What Fractaos is best at in a song context

From the manual, Fractaos can cover multiple musical roles:

- **Bass voice**
- **Lead voice**
- **Chord/pad voice**
- **Drone bed**
- **Percussion voice** via Kick/Tom/Snare/HiHat/Cymbal fractals
- **Atonal/noise/texture layer**
- **Multitimbral preset-based sound source** for multiple parts at once

That means you can use it in at least three different “songmaking” roles:

1. **As the main sound source for most of the track**
2. **As a specialized texture/chord/drone/percussion voice alongside other modules**
3. **As a scene-based arrangement module using presets and MULTI mode**

The third point is the most important for full-length songs.

---

# Why Fractaos is unusually good for arrangement

A lot of Eurorack patching gets stuck in loop-land because:

- one oscillator patch does one thing well
- changing sections requires repatching
- there is no memory
- there is no multitimbral separation
- transitions are too abrupt or too risky live

Fractaos addresses that with:

- **preset storage on SD card**
- **automatic EEPROM saving**
- **MULTI mode** where each voice can load a different preset
- **LIVE + preset coexistence**
- **Drone mode** for section changes and sustained harmonic beds
- **Spread behavior** that can move from unison to chords/microtuning
- **different fractal categories** that naturally create section contrast

So instead of thinking of it as “an oscillator,” think of it as a **song-state generator**.

---

# The central strategy: use Fractaos for contrast across sections

A full song needs contrast across time:

- intro
- groove entry
- bass drop
- verse
- chorus
- breakdown
- rebuild
- outro

Fractaos gives you several dimensions of contrast without repatching:

- **Fractal Type** changes the core spectral identity
- **Primitive Type** changes modulation behavior
- **Morph** shifts between main and secondary behavior
- **Texture** changes resonance/formants/filtering/organic detuning
- **Spread** changes detune or harmonic voicing
- **Drone mode** changes role from played voice to sustained environment
- **Preset recall** changes many parameters at once
- **MULTI mode** turns one module into several arranged parts

So a song on Fractaos should not be thought of as “one patch evolving forever.”  
Instead, treat it as a **small cast of reusable characters**.

Example:

- **Intro:** texture fractal in Drone mode, sparse
- **Verse:** poly bass + restrained lead
- **Pre-chorus:** increased chaos and morph motion
- **Chorus:** MULTI mode with chord spread and extra voices
- **Breakdown:** drum fractal + filtered drone only
- **Final chorus:** all voices active, wider spread, more texture, more LFO amount

That is how you get from a loop to a song.

---

# Best companion modules for turning Fractaos into songs

To make full-length tracks, Fractaos benefits from modules that provide:

## 1. Sequencing and song structure
Use with:

- **Metropolix**
- **Hermod+**
- **Five12 Vector Sequencer**
- **NerdSEQ**
- **Oxi One** via MIDI/CV
- **Torso T-1** via MIDI
- **Winter Modular Eloquencer**

What you want from a sequencer:

- pattern chaining
- mute states
- probability
- transposition
- multiple tracks
- song mode or scene mode
- MIDI output if using Fractaos polyphonically or multitimbrally

Fractaos becomes much more song-capable when driven by a sequencer that can change sections deliberately.

## 2. Mixers and VCAs
You need arrangement control outside the module:

- **performance mixer**: WMD Performance Mixer, Befaco Hexmix, Tesseract Tex Mix
- **VCAs**: Intellijel Quad VCA, Mutable Veils, Happy Nerding 3xVCA
- **mute/performance tools**: Befaco Mutes, WMD SSM, noise engineering mute modules

Even though Fractaos has output levels, external VCAs and mutes are how you stage entries/exits over time.

## 3. Effects for section differentiation
Fractaos wants space-processing:

- **reverb**: Strymon Starlab, Make Noise Erbe-Verb, Desmodus Versio
- **delay**: Mimeophon, Sealegs, Chronoblob
- **modulation FX**: FX Aid Pro, Timiszoara, Beads, Aurora
- **filtering/saturation** downstream: Ikarie, QPAS, Ghost, Analog Heat externally

Different effects sends help turn the same core timbre into intro/verse/chorus variations.

## 4. Clocking and event generation
For transitions:

- **Pamela’s Pro Workout**
- **Tempi**
- **Shakmat clock tools**
- **logic/event modules** like Compare 2, Branches, Joranalogue Compare 2, Klavis Logica XT

These let you automate section changes and rhythmic density.

## 5. Modulation sources
Fractaos already has internal motion, but full songs benefit from macro modulation:

- **quad envelopes/LFOs**: Quadrax, Zadar, Batumi
- **random but controlled**: Marbles, Chance, Wogglebug, Sapel
- **slow CV scenes**: Maestro, Planar 2, Tetrapad/Tête

Especially useful for Morph, Texture, Spread, Chaos, and Pitch CV inputs.

---

# Best ways to use Fractaos in a full song

## 1. Use it as a self-contained “band” in MULTI mode

This is probably the strongest songwriting use.

In **MULTI mode**, each of the 4 voices can have:

- a different preset
- a separate MIDI channel
- its own volume
- LIVE or preset status

That means one Fractaos can behave like:

- Voice 1: bass
- Voice 2: lead
- Voice 3: chord stab
- Voice 4: percussion or texture

### Example full-song patch
- **Voice 1:** Kick or bass fractal, MIDI channel 1
- **Voice 2:** melodic lead, MIDI channel 2
- **Voice 3:** pad/chord preset, MIDI channel 3
- **Voice 4:** noise/texture or hi-hat/snare model, MIDI channel 4

Run Fractaos stereo out into:
- mixer
- compressor/saturation
- delay/reverb sends

Use a sequencer like Hermod+, Oxi One, or Vector to:
- sequence each MIDI channel independently
- mute/unmute channels by section
- transpose chord channels
- trigger different note densities

### Why this works for songs
Now the arrangement is not one loop. It is **four coordinated roles** with separate entry/exit control.

---

## 2. Build sections by saving intentionally different presets

Preset memory is key.

Do not save random sounds. Save **section-function presets**.

For example:

- `BASS_A_TIGHT`
- `BASS_B_OPEN`
- `LEAD_VERSE`
- `LEAD_CHORUS`
- `PAD_INTRO`
- `PAD_BIG`
- `DRONE_BREAK`
- `SNARE_NOISE`
- `KICK_DIRTY`

Then use:

- LOAD mode for auditioning
- MULTI mode for assigning roles
- LIVE mode for expressive manual variation after matching the knobs

### Smart preset strategy for songs
Create preset families where only a few dimensions change:

#### Bass family
- same pitch range
- same envelope
- different Texture and Chaos
- one tighter, one wider, one more aggressive

#### Lead family
- same fractal pair
- different Morph/Spread/LFO settings
- verse, chorus, breakdown versions

#### Pad family
- one geometric and stable
- one texture-based and diffuse
- one Drone-oriented chordal version

That gives you repeatable section changes without losing musical identity.

---

## 3. Use Drone mode as your arrangement glue

Drone mode is one of the best tools here for turning patterns into songs.

In Drone mode:
- the sound is continuous
- all 8 oscillators can be spread
- Spread goes from unison to octave spread to predefined chords/microtunings
- MIDI/CV can still transpose individual pairs

This is perfect for:

- intros
- breakdowns
- ambient bridges
- tension risers
- harmonic beds behind sequenced parts
- outros

### Song idea
- Start with Drone mode and a red texture fractal like Cloud or Storm
- Slowly increase Texture and Speed
- Fade in external percussion
- Bring in sequenced bass from another module
- Exit Drone mode for a verse with note-triggered lines
- Re-enter Drone mode in breakdown for a suspended chord wash
- Use Spread chord scanning to bloom into final section

Drone mode helps solve the “what happens between loops?” problem.

---

## 4. Use Spread as a section macro

Spread behaves very differently depending on mode:

- **normal mode**: detunes driver/follower per voice
- **Drone mode**: becomes unison → octave spread → chord/microtuning selector
- **MULTI + Drone**: global Spread can affect all 8 oscillators, including preset voices

This is huge for arrangement.

### Practical song uses of Spread

#### In normal mode
Use Spread for:
- widening choruses
- making bass rougher in later sections
- moving a lead from focused to unstable

#### In Drone mode
Use Spread for:
- intro unison -> chorus chord expansion
- transitions from one harmonic color to another
- microtonal interludes
- tension by moving through denser tunings

### Excellent performance trick
Patch a slow CV source or manually ride Spread during transitions while the sequencer keeps the same notes.  
The harmony and perceived size can change dramatically without changing the sequence itself.

That is a classic full-song trick: **same pattern, new orchestration**.

---

## 5. Use drum fractals for transitional percussion, not just full drums

The manual makes clear that Kick, Tom, Snare, HiHat, and Cymbal are **real-time percussion models**, not samples.

They are available only as the main fractal, and Morph can blend them with a geometric primitive.

This makes them especially good for:

- fills
- accent layers
- industrial percussion tails
- hybrid percussive melodies
- breakdown percussion
- transitional impacts

### Not the best use
Trying to make Fractaos your entire drum machine all the time.

### Better use
Use it for:
- one signature kick layer
- metallic snare tail
- fractal cymbal wash
- tuned tom motif
- percussive lead that appears in one section

Pair with dedicated drum modules:
- BIA / Basimilus
- Queen of Pentacles
- WMD Crucible / Fracture / Chimera
- sample players like Assimil8or, Bitbox, Squid Salmple

This gives you stable drums from other modules and **signature transitional percussion** from Fractaos.

That is much more song-useful.

---

## 6. Use Fractaos as the harmonic center, and simpler modules as support

Because Fractaos is spectrally rich and animated, it works best when other voices are more function-specific.

A strong song-oriented rack pairing would be:

- **Fractaos** = chords / lead / drones / special percussion
- **analog VCO + filter voice** = simple bassline
- **sample drum voice** = kick/snare backbone
- **hi-hat/noise voice** = rhythmic energy
- **sampler or looper** = spoken word / texture / transitions

This solves a common problem: if everything in the rack is equally complex, the track becomes dense but not structured.

Let Fractaos be the color, and let simpler modules be the skeleton.

---

# Song-building patch recipes

## Recipe 1: Fractaos as full track core

### Modules
- Fractaos
- MIDI sequencer with 4 tracks/song mode
- stereo mixer
- reverb/delay
- external kick/snare/hat modules
- master clock
- VCAs or mute module

### Patch concept
- MIDI ch1 -> Fractaos bass preset
- MIDI ch2 -> Fractaos lead preset
- MIDI ch3 -> Fractaos chord preset
- MIDI ch4 -> Fractaos texture or drum preset
- Fractaos stereo out -> mixer/effects
- drums on separate channels
- use sequencer scenes for arrangement

### Song form
- **Intro:** ch3 and ch4 only, lots of reverb
- **Verse:** add ch1 bass
- **Pre-chorus:** increase Texture/Chaos manually or with CV
- **Chorus:** unmute ch2 lead, widen Spread
- **Breakdown:** mute bass/drums, enable Drone mode on chord preset
- **Final chorus:** restore sequence, more Spread and Morph motion
- **Outro:** remove drums, leave texture drone

This is likely the most direct way to make full tracks.

---

## Recipe 2: Fractaos as evolving chord/drone machine

### Modules
- Fractaos
- melodic mono synth voice
- drum machine modules
- slow modulation source
- performance mixer
- effect sends

### Patch concept
Use Fractaos almost entirely in:
- Drone mode
- chord-scanning Spread region
- texture/geometric blend presets

Then let the rest of the rack handle:
- kick/snare/hat
- bassline
- lead melody

### Why this works
One of the hardest parts of Eurorack arrangement is making tracks feel like they have a **world** around the groove.

Fractaos can be that world:
- shifting harmonic cloud
- wide stereo bed
- evolving resonant pad
- tuned tension layer
- microtonal bridge between sections

This is especially effective in ambient techno, IDM, soundtrack, industrial, experimental pop, and cinematic electronica.

---

## Recipe 3: Fractaos as “chorus machine”

Keep verses relatively dry and minimal using other modules.  
Bring Fractaos in only when you need the track to “open up.”

### Verse
- mono bass
- drum groove
- minimal pluck

### Chorus
- Fractaos enters with:
  - wider Spread
  - richer Morph
  - more Texture
  - multivoice harmonic preset

This gives you a reliable large-scale contrast with a single mute/unmute move.

---

## Recipe 4: Fractaos for transitions and fills

A full song lives or dies on transitions.

Use Fractaos for:
- risers
- chord blooms
- spectral swells
- tom fills
- chaos bursts
- filtered noise bridges
- metallic impact tails

### Patch
- trigger one Fractaos voice from a fill track
- use drum fractal or aggressive geometric fractal
- modulate Chaos and Texture with envelopes
- run through long delay/reverb
- mute/unmute around section boundaries

This gives you recognizable “song punctuation.”

---

# How to structure a full-length song with Fractaos

Here is a practical arrangement workflow.

## Step 1: define 4 roles
Before patching, assign roles:

- Voice A = bass
- Voice B = lead
- Voice C = pad/chords
- Voice D = percussive texture

Or if using other voices in your rack:

- Fractaos = pad/drone/lead only
- external modules = drums/bass

Do not leave it open-ended. Role clarity is how songs get finished.

## Step 2: design 2–3 presets per role
Not 20 presets. Just enough for sections.

For example:
- Bass intro
- Bass main
- Bass aggressive

- Lead sparse
- Lead hook
- Lead wide

- Pad thin
- Pad lush
- Drone dark

## Step 3: map sections to roles
Example:

| Section | Bass | Lead | Pad | Texture |
|---|---|---|---|---|
| Intro | off | off | drone thin | yes |
| Verse 1 | main | sparse | low | subtle |
| Chorus 1 | main | hook | lush | yes |
| Breakdown | off | off | drone dark | big |
| Chorus 2 | aggressive | hook wide | lush | yes |
| Outro | off | fragments | drone thin | fade |

This is essentially your arrangement chart.

## Step 4: automate mutes and transpositions
Use sequencer scenes, mute modules, or VCAs.

You do not need huge parameter automation if:
- voices enter/leave
- harmony shifts
- density changes
- effects sends change

## Step 5: reserve manual gestures for major moments
Use your hands for:
- Spread
- Morph
- Texture
- switching Drone on/off
- effect send amount
- mixer mutes

These are better performance gestures than constant micro-tweaking.

---

# Specific Fractaos controls that are best for musical development

## Fractal Type
Best used for:
- preset-defined section changes
- major identity swaps
- intro vs chorus contrast

Usually not the first thing to wiggle constantly in a song unless you want drastic changes.

## Primitive Type
Great for changing the behavior of motion and timbral interaction.  
Better as a composition choice or preset family difference than a frequent performance move.

## Chaos / Primitive Chaos
Excellent for:
- tension build
- making later sections rougher
- increasing instability before a drop
- transitioning from tonal to noisy

Use slow CV or manual rides.

## Depth / Primitive Depth
These are stepped and not CV-modulated.  
Better used as preset-level structural choices.

## Morph
One of the best performance/song controls.
Use it for:
- verse restraint vs chorus richness
- attack/tail blend on drum models
- gradually revealing the primitive influence

## Texture
Another top-tier macro control.
It affects:
- resonance
- formants
- filter intensity
- organic micro-detunings

This is excellent for making sections feel more “alive” without rewriting patterns.

## Speed / Amount
Great for:
- motion density
- rhythmic breathing
- LFO-based development
- adding animation in later sections

## Pitch
Useful for global transposition or live octave shifts.

---

# Great module combinations with Fractaos

## Fractaos + Hermod+
Very strong if you want:
- MIDI sequencing
- polyphony
- multitimbral channel management
- song sections
- automation lanes

Hermod+ can turn Fractaos into a compact song workstation.

## Fractaos + Oxi One
Excellent for:
- multiple MIDI channels
- poly sequencing
- generative but recallable structures
- performance scenes

## Fractaos + Pamela’s Pro Workout
Use Pam’s for:
- synced modulation into CV inputs
- trigger generation for CV/gate voices
- macro ramps during transitions
- clock division for slower structural movement

## Fractaos + Planar 2
A very musical pairing.
Map joystick-recorded motion to:
- Morph
- Texture
- Spread
- Chaos

This creates replayable section gestures.

## Fractaos + a sampler/looper
Pair with:
- Morphagene
- Lubadh
- Bitbox
- Assimil8or

Use sampler for:
- vocals
- field recordings
- transitional audio markers

Fractaos then becomes the harmonic/timbral engine while the sampler adds identifiable song moments.

---

# Genre-specific ways to use it

## Techno
- Drone mode intros and breakdowns
- percussion fractals for metallic fills
- MULTI mode bass/chord split
- texture blooms into drops
- external steady kick for anchor

## Ambient
- long Drone mode sections
- chord scanning with Spread
- slow modulation of Texture and Chaos
- sparse melodic voices over evolving bed

## IDM / experimental
- drum fractals morphing into pitched lines
- chaotic preset switching between sections
- multitimbral independent MIDI sequencing
- microtonal chord use in Drone mode

## Synth pop / soundtrack
- stable bass from another oscillator
- Fractaos for chorus pads and hook leads
- preset-based recallable sections
- aftertouch-enabled expressive lines

---

# Limitations to be aware of for songwriting

To use Fractaos well in full songs, note these constraints from the manual:

## 1. Single stereo output
Even though it is multivoice internally, it is not giving you four separate outs.  
That means internal balances matter, and external arrangement via per-voice processing is limited.

So for songs:
- use MULTI voice volumes carefully
- complement with other modules that have separate outputs
- treat Fractaos as a grouped instrument, not a full mixer replacement

## 2. Some parameters are stepped or less CV-friendly
Depth is stepped and not CV modulatable.  
So not every parameter is ideal for smooth live morphing.

## 3. Preset voices in MULTI share output space
You can’t fully isolate every part for different external effects chains unless using external role separation elsewhere in the rack.

## 4. Texture/drum models are constrained as primitives
That’s fine musically, but means some combinations are intentionally limited.

These are not dealbreakers; they just suggest the best strategy is:
- use Fractaos as a powerful grouped voice system
- use other modules for independent stems and structural anchors

---

# A very practical full-song workflow

## Workflow A: compose first, patch second
1. Decide song sections on paper
2. Assign Fractaos roles by section
3. Save/load presets intentionally
4. Program sequencer scenes
5. Rehearse transitions using Spread, Morph, Texture, Drone

This works better than exploratory patching if your goal is finished songs.

## Workflow B: capture sections as live takes
1. Patch a strong groove
2. Record 5–10 minute improvisation
3. Use Fractaos controls to create clear section changes
4. Edit best moments later in DAW or tape-style recorder workflow

Fractaos excels at this because its macro controls create audible large-form changes.

---

# Example full-length song blueprint

## Intro
- Fractaos in Drone mode
- Texture fractal: Cloud or Storm
- Spread near unison, then slowly into Maj triad spread
- external reverb heavy
- no drums yet

## Groove entry
- external kick enters
- Fractaos voice 1 bass preset starts via MIDI
- keep lead muted
- texture layer reduced

## Verse
- bass + drums + restrained Fractaos chord voice
- Morph low
- Texture moderate
- lead absent or sparse

## Pre-chorus
- increase Chaos
- modulate Speed/Amount for more movement
- automate filter/effects send externally
- maybe transition to Add9 or Minor7 chord behavior in Drone section

## Chorus
- MULTI lead voice active
- Spread widened
- Texture increased
- reverb send up
- chord voice louder

## Breakdown
- drums mostly muted
- Fractaos drone returns
- use microtonal Spread chord
- slow manual Morph sweep
- maybe bring in cymbal drum fractal accents

## Final chorus
- return to stable chord spread
- bring full drums back
- more aggressive bass preset
- lead preset wider/brighter

## Outro
- bass and drums drop out
- leave drone/pad and texture
- reduce Speed and Amount
- collapse Spread back toward unison

That is a complete song arc using Fractaos as the core dramatic engine.

---

# Best mindset for making songs with this module

The best way to succeed with Fractaos is:

- **don’t treat it as just an oscillator**
- **treat it as a recallable 4-part instrument**
- **design presets for sections, not just sounds**
- **use Drone mode for non-loop transitions**
- **use MULTI mode for role separation**
- **use other modules for anchors: drums, bass, mixer, sequencing**
- **perform macro changes, not endless knob drift**

In other words:

Fractaos helps solve the full-song problem because it provides **memory, multitimbrality, harmonic spread, percussion options, and dramatic timbral contrast** inside one module. Those are exactly the things most Eurorack patches lack when they get stuck as great 16-bar loops.

If you want, I can also turn this into any of these:

1. a **“Fractaos song patch cookbook”**  
2. a **recommended companion module list by budget**  
3. a **step-by-step techno/ambient/full-song patch plan**  
4. a **cheat sheet of the best Fractaos settings for bass, pads, leads, and drums**

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)