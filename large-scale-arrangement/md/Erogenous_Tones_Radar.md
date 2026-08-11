# Erogenous Tones — Radar

- [Manual PDF](../../manuals/radar-instructions.pdf)

---

[Manual PDF / Manufacturer Info](http://erogenous-tones.com)

# Using Erogenous Tones RADAR to build full-length songs in Eurorack

RADAR is easy to underestimate if you think of it as “just” an 8-channel envelope generator. In practice, it can be a **song-structure engine** because it gives you:

- **8 envelopes/LFOs at once**
- **independent or phase-related motion**
- **triggered events and repeating modulation**
- **AD / AR / looping behavior**
- **analog vs digital envelope behavior**
- **composite outputs**
- **quad/oct phase relationships**

That combination makes RADAR very useful for solving the classic Eurorack problem:

> “I can make a great 8-bar loop, but I can’t make it evolve into a full song.”

The key insight is this:

## Think of RADAR as a macro-arrangement module, not only a voice utility

Instead of assigning RADAR only to VCA plucks, use its channels to control:

- section fades
- drum density
- bass entrance/exit
- melody emphasis
- filter narrative arcs
- FX sends
- modulation intensity
- clock-derived transitions
- crossfades between sequences
- phase-offset movement across multiple voices

Because there are 8 lanes, you can dedicate some to **per-note articulation** and others to **slow structural changes** over many bars.

---

# What the manual tells us, musically

From the manual, RADAR has 3 major modes:

- **Envelope Mode**: 8 independent channels
- **Quad Mode**: 2 groups of 4 phase-offset envelopes
- **Oct Mode**: 8 phase-offset envelopes

Each lane can act as:

- **Repeating** = looping envelope / LFO
- **AD**
- **AR**

Important musical behaviors:

## 1. Trigger normalization
Each channel trigger is normalized to the next channel below.

This is huge for composition because one trigger stream can create a **family of related modulations**. You can drive several envelopes from one rhythm source, then vary times/shapes to create layered structure.

## 2. AD vs AR
- **AD** gives fixed transient shapes
- **AR** lets gate length matter

That means AR is especially good for:
- longer held notes
- phrase-level swells
- section-dependent sustain
- translating sequencer gate length into musical dynamics

## 3. Repeating mode
Looping envelopes can become:
- LFOs
- asymmetrical clocks
- slow song-shape generators
- pseudo-sidechain motion
- repeating rises/falls that drive arrangement changes

## 4. Analog vs digital modeling
This is one of the most compositionally important features.

- **Digital** resets to zero on retrigger
- **Analog** can rise from current level and behaves more like capacitor charging/discharging

Musically:
- **Digital mode** is tighter, more percussive, more clock-locked
- **Analog mode** is more organic, legato, evolving, and less “start-stop”

For full songs, analog mode is often better for **continuity between sections**, while digital mode is better for **clean groove articulation**.

## 5. Envelope shape control
You can continuously vary between:
- LOG
- LIN
- EXP

And the release can be:
- equal to attack shape
- opposite shape

This matters for arrangement because shape is not just timbre—it changes **how tension and release feel over time**.

Examples:
- **EXP decay** = punchy, percussive
- **LOG rise** = gradual bloom
- **LIN** = neutral transitions
- **opposite mode** = more natural rise/fall contrast

## 6. Composite outputs on lanes 4 and 8
In Envelope Mode:
- lane 4 can output the **max** of lanes 3+4
- lane 8 can output the **max** of lanes 6+7+8

This is excellent for making:
- grouped drum accents
- “highest energy wins” control voltages
- combined section envelopes
- dynamic bus modulation

## 7. Quad and Oct phase modes
These are maybe the most powerful “songfulness” tools in RADAR.

- **Quad Mode**: 4 related envelopes 90° apart
- **Oct Mode**: 8 related envelopes 45° apart

This lets one timing structure create coordinated movement across:
- drums
- bass
- pads
- melody
- FX
- stereo image
- filter banks
- multiple sequencers

Instead of all modulation happening at once, everything can take turns.

That is exactly how you get from a loop to a song.

---

# The main full-song strategy: use RADAR at multiple time scales

A good song in modular usually needs **three time layers**:

## A. Fast layer: per-note articulation
Use RADAR for:
- voice VCAs
- filter plucks
- FM index envelopes
- wavefolder dynamics
- LPG strikes

This gives the groove its immediate character.

## B. Mid layer: phrase evolution over 1–16 bars
Use RADAR for:
- opening filter over 8 bars
- increasing reverb send during fills
- introducing ratchets or probability
- changing bass envelope amount every phrase
- changing sequence transpose depth

This creates progression.

## C. Slow layer: section arrangement over 16–64+ bars
Use RADAR in repeating mode or long AR envelopes for:
- fade in percussion bus
- slowly widen stereo field
- raise distortion on climax
- mute/unmute voices through VCAs
- crossfade between sequencers
- progressively increase modulation depth

This creates actual song form.

The beauty of RADAR is that a single module can cover all three layers at once.

---

# Patch ideas for full-length songs

## 1. RADAR as a section arranger

### Goal
Turn 2–4 voice loops into intro, verse, build, breakdown, and outro.

### Patch
Use several RADAR channels to control VCAs placed after entire voice chains or submixes:

- **Lane 1**: kick/submix level
- **Lane 2**: hats/percussion level
- **Lane 3**: bass level
- **Lane 4**: melody level
- **Lane 5**: pad/texture level
- **Lane 6**: FX send amount
- **Lane 7**: filter cutoff on full mix or bus
- **Lane 8**: reverb/delay return VCA

Trigger them from:
- a master clock divider
- a manual gate source
- a sequential switch
- a logic-derived section trigger

### Why it works
Instead of muting manually, RADAR can **fade sections in and out musically**. Different attack/release times give each part a role:
- percussion can snap in
- pads can bloom
- bass can ease in late
- FX can trail into transitions

### Best module partners
- VCAs: Intellijel Quad VCA, Veils, Mutable Shades + VCA combo
- Mixers: Performance Mixer, Befaco Hexmix, Happy Nerding PanMix
- Clock dividers: Pamela’s Pro Workout, 4ms QCD, Temps Utile
- Gate sequencing: Steppy, Varigate, Eloquencer, Metron

---

## 2. Use AR mode to make sections depend on gate length

### Goal
Create verse-length and chorus-length events rather than tiny one-shot envelopes.

### Patch
Send long gates from:
- a gate sequencer
- pressure controller
- manual buttons
- a macro sequencer
- a clock divider with reset logic

Use AR lanes to control:
- master filter opening
- melody voice VCA
- wavetable position modulation depth
- delay feedback amount
- drum send to reverb

### Why it works
A long gate can represent a musical section:
- gate high = chorus
- gate low = verse

In **analog modeling AR mode**, shorter or changing gates feel especially organic because attack may not always fully complete before release starts. This gives transitions that feel less rigid and more “performed.”

---

## 3. Build transitions with repeating mode as slow cyclic structure

### Goal
Escape static loops without needing a full song sequencer.

### Patch
Set 2–4 RADAR lanes to **Repeating** with very slow rates:
- one cycling every 8 bars
- one cycling every 16 bars
- one cycling every 32 bars
- one slightly offset in shape/time

Patch them to:
- probability amount on trigger modules
- fill density on drums
- sequence transposition CV depth
- oscillator wavefold amount
- noise level in percussion
- reverb send amount
- stereo panning CV attenuation
- clock swing amount if supported

### Why it works
If several parameters evolve at different long periods, your patch produces **song-length variation automatically**. The repeating envelopes become low-frequency arrangement curves.

### Tip
Use:
- **digital repeating** for stable exact cycles
- **analog repeating** for more fluid return behavior and more lifelike transitions

---

## 4. Crossfade between two sequencers or two patterns

### Goal
Create verse/chorus or A/B sections.

### Patch
Use one RADAR lane and an inverted copy of it to control two VCAs or a crossfader.

For example:
- Sequencer A -> VCA 1 -> quantizer/voice
- Sequencer B -> VCA 2 -> quantizer/voice
- RADAR lane opens VCA 1 while inverse closes VCA 2, or vice versa

Or use RADAR to crossfade:
- two drum submixes
- two filter outputs
- dry/wet textures
- bassline variants
- two modulation buses

### Best partners
- Happy Nerding 3xVCA / 4x Stereo Mix
- Joranalogue Morph 4
- Planar 2
- X-PAN
- any CV-controllable crossfader

### Why it works
Crossfades create real arrangement changes while preserving continuity. A long RADAR envelope over 8–16 bars can make transitions feel composed rather than abruptly switched.

---

## 5. Use Quad Mode for phased multi-voice arrangement

### Goal
Make multiple voices evolve as parts of one larger form.

### Patch
In **Quad Mode**, one group of four outputs is 90° apart.

Assign outputs to:
- bass filter
- lead VCA level
- pad timbre
- percussion density

Because each lane is phase shifted, each musical part peaks at different times.

### Result
Instead of all voices becoming brighter/louder together, they **trade focus**:
- bass dominates first
- then melody
- then percussion
- then texture

That feels like arrangement.

### Great uses
- 4 voice techno progression
- 4-part ambient ecosystem
- polyrhythmic percussion scene
- quadraphonic/stereo movement

### Manual-based extra controls
In Quad Mode, lanes 2–4 can handle:
- **Speed**
- **Gravity**
- **SDelta**

Musically:
- **Speed** = phrase tempo of the whole evolving movement
- **Gravity** = how tightly the other channels pull toward or away from the main phase reference
- **SDelta** = shape spread across voices, making each lane articulate differently

That lets you create “everyone changes together but not identically,” which is ideal for full-song development.

---

## 6. Use Oct Mode as an 8-scene evolving orchestra

### Goal
Create a whole-song modulation ecosystem.

### Patch
In **Oct Mode**, all 8 outputs are 45° apart. Patch them to 8 destinations across the patch:

1. kick decay or drum VCA
2. snare tone
3. hat density
4. bass filter
5. chordal voice amplitude
6. lead timbre
7. delay send
8. reverb return or stereo width

Now one modulation process distributes energy around the patch over time.

### Why it works
This prevents the common modular problem where every modulation peaks simultaneously and the patch feels looped. Oct Mode creates **rotating emphasis**.

### Great for
- ambient
- IDM
- generative songs
- long-form techno
- soundtrack-style progression

---

## 7. Use normalized triggers to derive entire arrangements from one rhythm

### Goal
Take one gate stream and grow a whole composition from it.

### Patch
Feed one trigger pattern into the top lane and use the normalization downward. Set each lane differently:
- Lane 1: short AD for pluck
- Lane 2: longer AD for filter
- Lane 3: AR for sustained VCA
- Lane 4: repeating for local tremolo
- Lane 5: long AD for FX send
- Lane 6: very slow envelope for transposition depth
- Lane 7: repeating for pan motion
- Lane 8: long release for mix glue

### Why it works
One rhythmic motive can generate a **hierarchy of musical consequences**:
- note attack
- timbre bloom
- ambience trail
- phrase movement
- section-level tension

That’s how a simple sequence becomes compositional material.

---

## 8. Composite outputs as “energy buses”

### Goal
Build macro control signals that reflect activity in several lanes.

In Envelope Mode:
- lane 4 can output max(lane 3, lane 4)
- lane 8 can output max(lane 6, lane 7, lane 8)

### Patch ideas
Use lane 8 composite output to control:
- master distortion amount
- global filter brightness
- sidechain ducking depth
- delay send
- compressor sidechain level
- scene lighting in a performance patch

### Why it works
The max function behaves like an **energy detector**: whichever source is most active dominates. That gives arrangement-level control without messy CV mixing.

For example:
- lane 6 = bass phrase intensity
- lane 7 = lead phrase intensity
- lane 8 = percussion accent envelope

Composite output then opens a reverb send whenever any of those become active.

That can make sections “bloom” naturally.

---

## 9. Use RADAR to automate fills and breakdowns

### Goal
Add song markers every 8 or 16 bars.

### Patch
Take a long clock division or end-of-phrase trigger and fire a RADAR lane that modulates:
- snare decay
- burst generator density
- ratchet amount
- sample player start point
- filter resonance
- mute VCA on kick for a short breakdown

### Example
Every 16 bars:
- a RADAR AD envelope opens a VCA sending noise to percussion
- another lane in repeating mode briefly increases delay send
- another lane lowers bass level
- then all return

### Best partners
- logic modules
- burst generators
- probabilistic triggers
- sample players
- sequential switches

This is one of the easiest ways to get from “loop” to “track.”

---

# Pairing RADAR with common module categories

## With sequencers
RADAR is extremely effective with:
- Metropolix
- Rene
- Eloquencer
- Hermod
- Five12 Vector
- NerdSEQ
- Pamela’s Pro Workout as a trigger brain

Use RADAR to animate:
- gate length via VCAs/logic
- sequence transpose
- modulation lane depth
- probability amount
- step selection through sequential switch addressing

### Song trick
Use one sequencer for notes and RADAR for **everything that changes the meaning of those notes** over time.

---

## With sequential switches
A sequential switch plus RADAR is a song machine.

Use RADAR to:
- fade switched sources in/out
- modulate which sequence is active
- shape the transitions between switched timbres
- control reset moments

Modules:
- Doepfer A-151
- Vice Virga
- Boss Bow Two
- Verbos Sequence Selector

### Example
4 melodic sequences feed a switch. Every 8 bars a new sequence is selected. RADAR fades filter and amplitude differently for each handoff.

---

## With VCAs and mixers
This is probably the most important pairing.

RADAR turns into an arranger when patched through lots of VCAs:
- per-voice VCA
- CV VCA
- send-return VCA
- submix VCA
- master ducking VCA

Remember: **full songs in modular often come from voltage-controlled mixing, not just more sequencing**.

---

## With filters and low pass gates
Use different RADAR shapes to make repeated phrases feel less repetitive.

Examples:
- bass: short EXP decay for punch
- chords: long LOG rise for swelling entrances
- melody: AR with held gate for expressive sustain
- percussion bus: repeating lane to animate filter opening over several bars

---

## With effects
RADAR is excellent for arrangement through FX control.

Patch lanes to:
- delay send
- reverb send
- feedback amount
- shimmer depth
- bitcrusher mix
- chorus depth
- stereo width

A full song often feels complete when space changes over sections. RADAR can automate those changes elegantly.

---

## With logic and clock utilities
This is where song structure gets serious.

Use:
- AND / OR / XOR logic
- clock dividers
- trigger delays
- comparators
- Bernoulli gates
- burst generators

to create higher-level triggers that launch RADAR envelopes only:
- every 4 bars
- on fills
- when a manual button is pressed
- after probability conditions
- when another envelope crosses a threshold

This makes RADAR behave like an arrangement director.

---

# Concrete full-song templates

## Template 1: Techno arrangement
### Voices
- kick
- percussion
- bass
- stab/lead

### RADAR assignment
- Lane 1: kick bus ducking envelope
- Lane 2: bass filter envelope
- Lane 3: stab amplitude envelope
- Lane 4: percussion bus level over phrases
- Lane 5: repeating 16-bar build into lead filter
- Lane 6: AR controlling reverb send during breakdown gate
- Lane 7: repeating slow modulation to hi-hat density
- Lane 8: composite energy output to master saturation

### Song form
- intro: percussion + filtered stab only
- verse/groove: bass enters via long AR
- build: lane 5 opens lead filter over 16 bars
- breakdown: lane 6 raises reverb, lane 1 reduces kick dominance
- drop: digital retriggered envelopes tighten everything again
- outro: long releases remove bass and percussion gradually

---

## Template 2: Ambient long-form piece
### Voices
- drone
- harmonic voice
- soft pulses
- noise texture

### RADAR assignment
Use **Oct Mode**:
- each output controls one parameter in a distributed ecosystem

Examples:
- drone filter
- drone amplitude
- harmonic timbre
- harmonic VCA
- pulse rate modulation depth
- pulse brightness
- noise level
- reverb send

### Result
The patch never feels static because emphasis rotates slowly through the system.

### Song form
Instead of rigid sections, the song becomes:
- emergence
- blooming
- density
- suspension
- dissipation

RADAR is perfect for this style.

---

## Template 3: Song-like melodic modular patch
### Voices
- drums
- bass
- chords
- lead

### Structure idea
Use one “section gate sequencer” or manual controller.

### RADAR lanes
- Lane 1: drum bus level
- Lane 2: bass VCA
- Lane 3: chord VCA
- Lane 4: lead VCA
- Lane 5: chord filter sweep
- Lane 6: lead delay send
- Lane 7: transpose modulation depth
- Lane 8: outro fade/master texture send

Use long AR gates for:
- verse
- pre-chorus
- chorus
- bridge

This gives you actual section behavior, not just pattern chaining.

---

# Best musical practices with RADAR for song writing

## 1. Reserve some lanes for arrangement only
Don’t spend all 8 channels on per-note envelopes.

A good rule:
- 3–4 lanes for articulation
- 2–3 lanes for phrase movement
- 1–2 lanes for section control

## 2. Use long times unapologetically
A lot of modular patches stay “small” because modulation cycles are too short.

Let some RADAR lanes span:
- 4 bars
- 8 bars
- 16 bars
- even 32+ bars

That’s where songs start happening.

## 3. Mix digital and analog behavior intentionally
- **Digital** for drums, tight bass articulation, hard resets
- **Analog** for pads, transitions, drones, legato changes

## 4. Use shape as narrative
- LOG rise = suspense
- EXP decay = impact
- LIN = neutrality
- opposite mode = more natural asymmetry

## 5. Build one control lane per musical question
Examples:
- “When does bass enter?”
- “When does space increase?”
- “When does melody become dominant?”
- “How does density rise before the drop?”

RADAR can answer each of these with a lane.

## 6. Let one lane modulate modulation depth
A classic full-song move:
Use one RADAR lane to open a VCA that controls another modulation source.

Example:
- LFO -> VCA -> filter FM
- RADAR controls that VCA

Now modulation itself appears only in later sections.

That’s very song-like.

---

# Especially powerful combinations

## RADAR + Pamela’s Pro Workout
Pam provides:
- clocks
- divisions
- logic-ish trigger patterns
- long gates
- synced timing

RADAR provides:
- contour
- shape
- phrase motion
- arrangement fades

Together, they can build complete evolving structures.

## RADAR + Metropolix or Vector
Sequencer handles notes and pattern switching.
RADAR handles:
- voice entrances
- timbral evolution
- transition envelopes
- buildup/release arcs

## RADAR + matrix mixer
A matrix mixer lets one RADAR lane influence several destinations in controlled amounts.

One long envelope can simultaneously:
- increase cutoff
- increase reverb
- reduce bass
- widen stereo field

That is pure arrangement power.

## RADAR + performance mixer
Use RADAR to animate what would otherwise be manual fader moves. Great for recording whole performances into coherent tracks.

---

# A practical “full song patch” recipe

If you want one immediately useful setup:

## Core modules
- RADAR
- 1 drum voice or drum system
- 1 bass voice
- 1 melodic/chord voice
- 1 sequencer
- clock source/divider
- several VCAs
- mixer
- reverb/delay
- optional sequential switch

## Patch
### Articulation
- Lane 1 -> bass VCA envelope
- Lane 2 -> melody VCA envelope
- Lane 3 -> melody filter envelope

### Phrase
- Lane 4 -> drum submix VCA or drum filter
- Lane 5 repeating slow -> bass filter modulation depth
- Lane 6 repeating slow -> melody delay send

### Section
- Lane 7 AR -> pad/chord voice level from a long gate
- Lane 8 AR or AD -> master FX bloom / outro fade

### Control
- Sequencer triggers notes
- Clock divider sends phrase triggers every 8/16 bars
- Manual gate button or sequencer track defines chorus/breakdown sections

## Result
You now have:
- note-level dynamics
- phrase-level change
- section-level form

That is the architecture of a song.

---

# Final takeaway

RADAR helps create full-length songs because it can function as:

- an **8-channel articulation source**
- a **slow modulation bank**
- a **phase-based arrangement engine**
- a **macro fade/transition controller**
- a **section-performance assistant**

The reason many modular patches remain loops is not lack of notes, but lack of **hierarchical control over time**. RADAR gives you exactly that hierarchy.

If you approach it as:
- some lanes for notes,
- some lanes for phrases,
- some lanes for sections,

then it becomes much more than an envelope generator: it becomes a **song form module**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)