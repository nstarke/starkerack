# Ohmforce — Bohm Multimodal Kick Drum Voice

- [Manual PDF](../../manuals/Bohm_Eurorack_Manual_Compiled.pdf)

---

[Manual PDF / source](https://bohm-eurorack-manual.readthedocs.io/en/latest/index.html)

# Using Bohm to build full-length songs in Eurorack

Bohm is not just a kick module in the usual “one trigger in, one thump out” sense. Based on the manual, it is really a **stereo dual-voice kick system** with **multiple drum models**, **performance modes**, and optional **Groove** and **Performer** expanders. That makes it useful as a **structural anchor** for a full track, not just a drum voice.

In a Eurorack song-building context, that matters a lot: the kick often defines **section changes, energy levels, drops, transitions, arrangement cues, and sidechain behavior**. Bohm seems designed to help with exactly that.

---

## What Bohm brings to song creation

From the manual, the important features for arrangement are:

- **Stereo dual-voice kick architecture**
- **Multiple kick “models”** with different behavior
- Controls for:
  - HIT
  - VELOCITY
  - LENGTH
  - SUSTAIN
  - ATTACK
  - PITCH
  - CURVE
  - TRS DECAY
  - COLOR
  - FX
  - TRS TONE
- **Groove expander** for:
  - secondary kick voice
  - techno rumbles
  - layered percussion
- **Performer expander** for:
  - DJ-style effects
  - ducking
  - stereo processing
- **Studio / Live Song / Jam modes**

That means Bohm can cover several arrangement roles:

1. **Main kick**
2. **Layered low percussion**
3. **Rumble / tail / reverb-style energy bed**
4. **Stereo movement and transitions**
5. **Section-by-section kick program changes**
6. **Mix glue via ducking**

For full songs, these are all crucial.

---

# The key idea: use Bohm as the arrangement spine

A lot of modular patches fail to become songs because everything is equally active all the time. Bohm can help solve that if you think of it as the **arrangement spine**:

- Verse: lighter kick model, shorter decay
- Pre-chorus/build: more pitch curve, more sustain, more velocity movement
- Drop/chorus: heavier model, layered Groove rumble, wider Performer stereo processing
- Breakdown: remove main kick, keep only rumble or filtered tail
- Outro: simplify to dry kick with less sustain and less FX

Instead of making one good kick patch and leaving it static for 8 minutes, use Bohm to create **distinct sections**.

---

# Why Bohm is especially good for full songs

## 1. Different models can act like different “drummers” or “machines”
The manual says each model represents a different drum-machine architecture, and the controls behave differently depending on the model.

That is powerful for arrangement because changing models can create:

- classic verse/chorus contrast
- old-school vs modern section contrast
- tighter club section vs looser breakdown section
- dry intimate groove vs huge rave section

In practical song terms:

- **Intro**: select a simpler, tighter kick model
- **Main section**: choose a punchier, fuller model
- **Breakdown**: switch to a softer or boomier model with reduced attack
- **Final drop**: return to the most aggressive model

Even if the melodic content stays the same, these changes make the track feel like it evolves.

---

## 2. The secondary voice from Groove can become your arrangement engine
The Groove expander adds a **secondary kick voice** for **techno rumbles and layered percussion**.

This is huge for full-length tracks because a second low-frequency rhythmic layer can function as:

- a **rumble bus**
- an **offbeat bass-percussion layer**
- a **transitional texture**
- a **chorus energy boost**
- a **breakdown tail or ghost pulse**

This means Bohm + Groove can support song sections like this:

- **Intro**: dry main kick only
- **Verse**: add subtle Groove layer every few bars
- **Build**: automate Groove decay/tone/color for rising energy
- **Drop**: full main kick + Groove rumble
- **Breakdown**: mute main kick, keep only filtered Groove tail
- **Outro**: remove Groove, leave dry kick again

That alone is often enough to turn a loop into a track.

---

## 3. Performer gives you transitions, not just tone
Performer adds:

- DJ-style effects
- ducking
- stereo processing

This is exactly the kind of thing many modular systems lack when trying to become “song-capable.”

A great loop becomes a full track when you have:

- transitions
- tension/release
- mix-space management
- controlled widening/narrowing of sections

Performer seems designed for that.

You can use it for:

- **build-ups** with widening or FX emphasis
- **drops** by snapping from effected/wide to dry/centered
- **breakdowns** with ducking reduced or transformed
- **returns** where the kick regains authority in the mix

---

# Practical full-song strategies with Bohm

## Strategy 1: Use Bohm programs as section presets
The manual mentions memory for **system settings and up to 32 programs**.

That suggests one of the best song workflows:

Create separate programs for sections such as:

1. Intro
2. Verse A
3. Verse B
4. Build
5. Drop
6. Breakdown
7. Final drop
8. Outro

For each program, change things like:

- kick model
- pitch curve feel
- decay/sustain amount
- color/tone
- FX intensity
- Groove layer presence
- Performer stereo width or ducking behavior

This is one of the cleanest ways to make a modular song feel intentional.

### Example program map
- **Program 1 – Intro**
  - short kick
  - low sustain
  - minimal FX
- **Program 2 – Main groove**
  - medium sustain
  - stronger attack
  - moderate color
- **Program 3 – Build**
  - brighter tone
  - longer tail
  - increased stereo processing
- **Program 4 – Drop**
  - full sustain
  - heavier model
  - Groove rumble active
- **Program 5 – Breakdown**
  - softer attack
  - reduced velocity
  - tail-heavy or filtered layer
- **Program 6 – Final**
  - strongest hit
  - widest stereo
  - aggressive ducking

If Live Song Mode allows sequenced kick changes as the manual suggests, this becomes even more powerful.

---

## Strategy 2: Build the song around density, not just note changes
In Eurorack, people often focus on changing pitch sequences to make a song. But often what works better is changing **rhythmic density and envelope weight**.

Bohm’s controls support that directly:

- **LENGTH** and **SUSTAIN**: control how much space the kick occupies
- **ATTACK**: changes punch and front-edge definition
- **VELOCITY**: changes groove and emphasis
- **PITCH** and **CURVE**: shape perceived impact and style
- **COLOR / TRS TONE / FX**: define mix placement and character

For sections:

- **Sparse section**
  - shorter length
  - reduced sustain
  - lower velocity variation
  - less FX
- **Big section**
  - stronger velocity
  - longer sustain
  - more pitch curve snap
  - more color and stereo emphasis

This creates arrangement contrast even if the trigger pattern stays mostly the same.

---

## Strategy 3: Use Bohm to define the drop
A full song needs at least one moment where the energy clearly lands. Bohm can make that happen through controlled contrast.

### Build technique
Over 8 or 16 bars:

- gradually increase:
  - FX
  - COLOR
  - TRS TONE
  - SUSTAIN
- optionally bring in Groove rumble
- narrow or remove main kick in the final bar
- then reintroduce full, dry, punchy kick at the drop

This is a classic dance arrangement trick.

### Modules to pair with
- **Sequential switch**: route different CV sources to Bohm section by section
- **CV recorder / automation module**: record knob movements for build-ups
- **Clock divider / multiplier**: trigger transitions every 8/16/32 bars
- **Mute module**: drop the kick briefly before impact
- **Filter or EQ module** after Bohm: automate low-pass/high-pass sweeps on the rumble layer

---

# Combining Bohm with other modules for complete songs

## 1. With sequencers
Bohm becomes much more song-capable when paired with a sequencer that can handle:

- pattern chaining
- probability
- mutes
- CV automation
- song mode

Ideal pairings are modules that can:
- send kick triggers
- send accent/velocity CV if available in your system
- send section-change CV or gates
- sequence mutes for Groove and Performer behaviors

### Use cases
- Trigger Bohm with a main 4/4 pattern
- Use a second sequencer lane for occasional missing kicks in breakdowns
- Use another lane to modulate velocity or tone every 8 bars
- Chain patterns into a full arrangement

If you have a sequencer with song mode, let the sequencer drive:
- triggers
- resets
- section changes
- mutes on bass, melody, and hats

Then Bohm’s section programs define the drum architecture while the sequencer defines timing.

---

## 2. With bass voice modules
The kick and bass relationship is usually the main obstacle in turning a loop into a track. Bohm’s **ducking** via Performer is especially relevant here.

### Good approach
Patch:
- Bohm as your kick anchor
- a separate bass oscillator/filter/VCA chain
- use ducking from Performer or an external envelope follower/VCA setup

Then design sections like:

- **Intro**: kick only, no bass
- **Verse**: bass enters on reduced notes
- **Drop**: full bass with ducking
- **Breakdown**: bass becomes more tonal, kick reduced
- **Final drop**: both return, tightly ducked

This lets the song breathe.

### Bass modules that work well conceptually
Any:
- mono synth voice
- wavetable bass voice
- FM bass voice
- acid-style voice
- resonant filter ping bass

The key is not the module type, but **arrangement discipline**:
don’t let bass play the same density in every section.

---

## 3. With melodic voices
Bohm helps songs because strong kick arrangement gives melody something to arrange against.

Use Bohm section changes to cue melodic changes:

- shorter drier kick = melody can be busier
- heavier sustained kick = melody should simplify
- breakdown kick reduction = melody can expand harmonically
- drop kick return = melody should become hook-like and repetitive

### Great patching concept
Use one master sequencer or clocked logic system to control:
- Bohm triggers
- bass sequence variation
- melodic transpositions
- mute states
- effects sends

That way the whole patch shifts together in sections.

---

## 4. With clock, logic, and utility modules
This is where songs really emerge.

### Useful module types
- clock divider
- logic
- Bernoulli gate / probability router
- sequential switch
- CV mixer / attenuator
- offset generator
- sample & hold
- precision adder
- mute matrix

### Why they matter
They let you change Bohm over longer timescales:
- every bar
- every 4 bars
- every 8 bars
- every 16 bars

Instead of random moment-to-moment variation, you get **structured variation**.

### Example
- main trigger every quarter note
- every 8 bars, a sequential switch changes Bohm modulation source
- every 16 bars, a gate activates Groove layer
- every 32 bars, a programmed switch changes to another Bohm preset or mode

That is song architecture.

---

## 5. With modulation sources
Bohm’s many parameters suggest it benefits from selective modulation rather than constant hands-on tweaking.

### Best modulation targets for song progression
- **VELOCITY** for groove evolution
- **PITCH/CURVE** for style shift between sections
- **SUSTAIN/LENGTH** for energy scaling
- **COLOR / TONE** for spectral growth in builds
- **FX** for transitions

### Best modulation source types
- slow synced LFOs
- stepped CV sequencers
- envelope followers
- random with attenuation
- manual CV controller / fader bank
- pressure/touch controller for live arrangement

### Important tip
Use **small, section-aware modulation**, not constant chaos.
For songs, subtle and intentional beats interesting-but-stagnant every time.

---

# Song forms Bohm can support well

## 1. Techno arrangement
Bohm + Groove is especially suited for this.

### Example form
- **0:00–1:00 Intro**
  - dry kick
  - hats/noise slowly enter
  - occasional Groove tail
- **1:00–2:00 Main groove**
  - bass enters
  - moderate kick sustain
- **2:00–2:30 Build**
  - open hats
  - more FX/stereo
  - rising rumble density
- **2:30–3:30 Drop**
  - full kick + rumble + bass
- **3:30–4:15 Breakdown**
  - remove main kick
  - leave rumble texture and melodic pad
- **4:15–5:30 Final drive**
  - strongest Bohm model
  - full ducking
  - wider stereo
- **5:30–6:00 Outro**
  - return to dry kick
  - elements drop away

Bohm’s model changes and dual-voice design map naturally to this.

---

## 2. Electro / IDM arrangement
Here the kick can vary more in attack, pitch curve, and timing emphasis.

Use:
- tighter, shorter models in detailed sections
- more dramatic pitch curves in fills
- selective Groove layering for odd phrase endings
- Performer effects for glitch-style transitions

Pair with:
- trigger sequencer with pattern memory
- probability logic
- sample voice for percussion accents
- melodic voice with phrase switching

---

## 3. Industrial / EBM arrangement
Bohm looks very suitable because **color, tone, attack, and stereo processing** can define aggression.

Arrange through:
- increasingly distorted or sharpened kick tone per section
- secondary voice as pounding low-mid percussion
- abrupt mute-based transitions
- ducked synth stabs and bass sequences

---

## 4. Ambient / cinematic rhythm tracks
Even here Bohm can work if used more texturally.

- use softer attack
- longer sustain
- reduced trigger density
- Groove as sub movement rather than obvious rumble
- Performer stereo processing for width and space

This supports a “slow-blooming” full track rather than club arrangement.

---

# A practical patch recipe for making an actual full song

Here is a concrete modular setup.

## Core modules
- **Bohm**
- **Groove expander**
- **Performer expander**
- master clock
- sequencer with pattern chaining/song mode
- bass voice
- melodic voice
- hi-hat / percussion modules
- mixer with mutes
- filter or EQ
- reverb/delay
- utility modules for logic, attenuation, switching

## Patch concept
### Bohm
- main kick on quarter notes
- Groove voice layered only in selected sections
- Performer handling ducking/stereo/transition effects

### Bass voice
- sequence tied to section changes
- ducked against Bohm
- simpler in drops, more melodic in breakdowns

### Melody voice
- sparse hook in main sections
- expanded harmonic content in breakdown

### Percussion
- hats and claps increase through arrangement
- use mutes to sculpt sections

### Utilities
- sequential switch changes modulation destination every 16 bars
- clock divider activates fills every 8 bars
- manual fader controls FX amount and rumble intensity

## Section plan
### Intro
- Bohm only
- short decay
- no bass
- filtered hats slowly fade in

### Verse / Groove A
- bass enters
- moderate kick sustain
- melody absent or very minimal

### Groove B
- add clap/percussion
- increase velocity variation
- subtle Groove rumble

### Build
- raise FX and tone brightness
- automate longer tails
- reduce melodic content
- maybe mute kick for half a bar before drop

### Drop
- strongest Bohm program
- full bass
- full ducking
- wider stereo image
- main hook returns

### Breakdown
- remove main kick or shorten it drastically
- leave Groove tail or processed sub pulse
- melody/pads move to foreground

### Final drop
- biggest kick model
- highest contrast
- additional percussion layers

### Outro
- strip back to kick and one texture
- return to original dry sound

This is a complete track architecture.

---

# How to avoid the common “great loop, no song” trap

## Problem 1: everything sounds equally big all the time
**Fix with Bohm:** reserve your longest sustain, biggest model, fullest stereo, and strongest rumble for only one or two major sections.

## Problem 2: kick never changes across the track
**Fix with Bohm:** create multiple programs with distinct attack, pitch curve, and color.

## Problem 3: breakdowns feel empty instead of intentional
**Fix with Bohm:** use Groove rumble or Performer stereo processing as a “ghost rhythm bed” when the main kick drops out.

## Problem 4: bass and kick fight each other
**Fix with Bohm:** use Performer ducking and reduce bass density in kick-heavy sections.

## Problem 5: transitions are weak
**Fix with Bohm:** automate FX, tone, stereo width, and temporary kick removal before returns.

## Problem 6: modular variation is too random
**Fix with Bohm:** use structured timing from dividers, switches, and programmed CV changes rather than free random modulation.

---

# Best module pairings for Bohm in a song-focused rack

If your goal is full tracks, Bohm pairs especially well with:

- **Song-capable trigger/pitch sequencer**
- **Mute/performance mixer**
- **Bass voice with easy pattern recall**
- **Stereo processor / delay / reverb**
- **Clock dividers and phrase counters**
- **Sequential switches**
- **CV recorder or automation module**
- **Manual performance controller**
- **Filter/EQ for section filtering**
- **Looper or sampler** for capturing and reintroducing material

A very effective system is:

- Bohm = arrangement/drum spine
- sequencer = section timeline
- bass voice = weight
- melodic voice = hook
- mixer/mutes = entry/exit of parts
- utilities = phrase-level change logic

That combination gets you from pattern-making to song-making.

---

# Live use vs studio use

The manual mentions three modes:

- **Studio Mode**
- **Live Song Mode**
- **Jam Mode**

## Studio Mode
Best for:
- designing several section-specific kick programs
- dialing exact envelope/tone differences
- recording automation or multitrack takes

## Live Song Mode
Best for:
- chaining section changes
- predictable arrangement progression
- performance with deliberate transitions

This is probably the mode to lean on if your issue is “I can improvise grooves but not finish songs.”

## Jam Mode
Best for:
- finding ideas
- improvising transitions
- discovering alternate section shapes

A smart workflow is:
1. Jam to discover interesting section contrasts
2. Rebuild them as saved programs
3. Arrange them in Live Song Mode
4. Record the full performance

---

# Final takeaway

Bohm can help create full-length songs because it appears to be more than a kick voice: it is a **section-defining rhythmic architecture module**.

Its strongest song-making uses are:

- creating **distinct kick identities for different sections**
- layering a **secondary low percussion/rumble voice** with Groove
- using **ducking, stereo processing, and FX transitions** through Performer
- saving **multiple programs** and treating them like arrangement scenes
- pairing it with sequencers, switches, mutes, bass voices, and utility modules to create **bar-scale and phrase-scale evolution**

If you use Bohm as the **center of energy management** in the patch, it can absolutely help turn a compelling loop into a full arrangement.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)