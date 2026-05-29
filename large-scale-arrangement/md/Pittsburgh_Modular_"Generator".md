# Pittsburgh Modular — "Generator"

- [Manual PDF](../../manuals/Generator - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF / source](https://pittsburghmodular.com/generator)

# Pittsburgh Modular Generator: using an FM monster to build full-length songs

The **Pittsburgh Modular Generator** is not a conventional precision melodic oscillator. It is a **dual oscillator FM voice / modulation source** built for **complex timbre, internal cross-functionality, and animated instability**. That makes it especially good for the part of eurorack songwriting that often feels hardest:

- turning a loop into an arrangement
- making sections feel different without replacing the whole patch
- creating transitions, fills, breakdowns, rises, and textural contrast
- deriving multiple related musical layers from one core sound source

## What the module is, musically

From the manual:

- **Two triangle-core oscillators**
- **Wide frequency range**
- **Exponential CV inputs**, but **not 1V/oct** and **not temperature compensated**
- **Generator 2 is internally FM’d by Generator 1 Index Out**
- **Shape control** morphs the waveform relationship between the two oscillators
- **External FM input** can target either oscillator
- **Index section** is effectively a VCA on Generator 1’s output, and that post-VCA signal both:
  - appears at **Index Out**
  - drives the **internal FM amount to Generator 2**

So musically, Generator is best understood as:

1. a **dual raw oscillator voice**
2. a **self-patched FM network**
3. a **timbral percussion and noise engine**
4. a **modulator generator**
5. a **section-making machine**

That last point matters for songs. A lot of modules help you make a sound. Generator helps you make **states** of a sound:
- dry vs internally FM’d
- low vs mid vs high ranges
- triangle-ish vs square-ish spectral balance
- oscillator 1 foreground vs oscillator 2 foreground
- external modulation routed to oscillator 1 or 2

Those state changes are exactly what help produce verses, choruses, intros, breakdowns, and endings.

---

# Key behaviors from the manual that matter for arranging

## 1. It is not a precision pitch voice
The manual explicitly says the EXP inputs are exponential but **do not track 1V/oct**.

That means:

- do **not** rely on Generator as your only “traditional” tuned melody source across multiple octaves
- do use it for:
  - drones
  - bass riffs in narrow ranges
  - percussion
  - FM stabs
  - tension layers
  - atonal or semi-tonal hooks
  - tuned-by-ear motif voices
  - transitions and sound design

It can still be musical; it’s just better approached like an **expressive performance oscillator** than a keyboard synth VCO.

## 2. Oscillator 2’s FM depth is tied to the Index section
This is huge. The manual says Generator 2 is internally FM’d by **Generator 1 Index Out**, and the **Index pot / Index CV** control that amount.

So one CV destination changes both:

- the amplitude of Generator 1 at **Index Out**
- the internal FM intensity sent into Generator 2

That means one envelope or sequence can create **simultaneous loudness + timbral development**.

This is excellent for full-song composition because it lets one control gesture create a “bigger” section automatically.

## 3. Shape is a section-defining macro control
The **Shape pot** changes both oscillators at once:

- full left:
  - Gen1 = square
  - Gen2 = triangle
- full right:
  - Gen1 = triangle
  - Gen2 = square

That means the harmonic role of each oscillator swaps as you turn one knob/CV source. This is extremely useful for:

- verse vs chorus tone shifts
- intro dullness to chorus brightness
- evolving drones
- fills and transitions

## 4. External FM destination switch is arrangement gold
External modulation can be routed to **Generator 1 or Generator 2**.

That means the exact same modulation source can produce two different musical results. In a song context, that gives you a simple “section switch”:
- route modulation to Gen1 for one section
- route to Gen2 for another

---

# Best role for Generator in a song-oriented modular system

Generator is usually strongest as one of these:

## A. Main “feature voice”
Use it as the memorable lead texture or bass/percussion signature that defines the track.

Good if your song wants:
- industrial FM bass
- metallic hook
- unstable lead
- tuned percussion motif
- game-console-ish weirdness
- noisy drum voice

## B. Secondary motion layer
Let a more stable voice handle exact pitch duties, while Generator adds:
- grit
- attack layer
- FM shimmer
- fills
- background tension
- call-and-response accents

## C. Transition engine
Use it mostly for:
- risers
- drops
- noise bursts
- self-FM drum fills
- section cues
- breakdown textures

## D. Self-contained percussion / bass hybrid
One of the best strategies: use Generator to blur roles. In different sections, the same patch can become:
- kick-like thump
- tom pattern
- bassline
- metallic hat wash
- FX burst

That “same DNA, different function” is very powerful for cohesive songwriting.

---

# What other modules pair best with it for full songs

To make songs rather than loops, Generator benefits from a support cast that provides **structure**.

## Essential partners

### 1. A sequencer with multiple lanes or scenes
Examples:
- Make Noise Rene
- Intellijel Metropolix
- Five12 Vector
- Winter Modular Eloquencer
- NerdSEQ
- OXI One controlling the rack externally

You want:
- pitch/CV lanes
- gate lanes
- pattern switching
- mutes
- probability
- song mode or chained patterns

Since Generator isn’t strict 1V/oct, sequencer lanes are still useful for:
- narrow-range pitch gestures
- transposition offsets
- FM amount automation via CV tracks
- range-changing logic

### 2. Function generators / envelopes
Examples:
- Maths
- Zadar
- Quadrax
- Stages
- Delta-V
- Contour 1

These are crucial because Generator comes alive when:
- Index CV is animated
- external FM comes in bursts
- filter/VCA after it shape phrases
- section envelopes move timbre over many bars

### 3. VCAs
You will want more VCAs than you think.

Use them for:
- controlling external FM depth before it hits Generator
- dynamically modulating Shape or frequency inputs
- ducking Generator under drums
- automating transitions
- crossfading between outputs 1 / 2 / Index Out

### 4. A filter or spectral shaper
Even though Generator already does lots of timbral work, filtering helps define song sections.

Useful pairings:
- LPG for percussive phrasing
- multimode filter for bass/lead shaping
- wavefolder for more aggression
- fixed filter bank for arranged tone colors

### 5. Mixer with mutes / sends
For songs, this matters more than another oscillator.

A performance mixer lets you:
- mute Generator layers in/out by section
- send it to reverb only in breakdowns
- dub in feedback delays for transitions
- create arrangement live

### 6. Clocked modulation / logic / switches
Examples:
- sequential switch
- clock divider
- burst generator
- logic module
- clocked random
- compare / sample and hold

These help Generator change role every 4, 8, 16, or 32 bars without repatching.

---

# How to think about full-length songs with this module

The mistake many modular users make is asking a patch to stay interesting by itself for 6 minutes.

Instead, with Generator, think in terms of **reusable arrangement states**.

## Build 4 states, not 1 patch

For example:

### State 1: Intro / sparse
- low Index amount
- slow or no external FM
- Shape biased toward triangle-heavy behavior
- long reverb
- low register
- maybe just output 2

### State 2: Verse / groove
- moderate Index CV from envelopes
- external FM from a synced modulation source
- tight VCA articulation
- dry mix
- controlled pitch range

### State 3: Chorus / impact
- larger Index modulation
- shape shifted brighter
- more external FM
- doubled with another oscillator or sample voice
- accent pattern opens filter or increases distortion

### State 4: Breakdown / transition
- frequency ranges switched
- external FM rerouted to other oscillator
- use output 1 or Index Out alone
- more delay/reverb
- less rhythmic gating, more wash or texture

Then use sequencer scenes, mute automation, switches, and envelope changes to move between them.

That is how you get a song.

---

# Important outputs and how to exploit them for arrangement

From the manual:

- **1** = Generator 1 output, pre Index VCA
- **2** = Generator 2 output
- **OUT** = post Index VCA Generator 1 output

These are very useful as three related but distinct signals.

## Practical use of the three outputs

### Output 1: stable raw oscillator source
Use for:
- a constant bass/drone layer
- pre-VCA recording path
- clean signal to process separately

### Output 2: the internally FM-affected partner
Use for:
- your main complex timbre voice
- metallic lead/percussion source
- layered voice against output 1

### Index Out: the “arrangement output”
Use for:
- dynamically shaped phrases
- envelope-driven accents
- the main voice for sections with stronger motion

Because Index Out also influences Gen2’s internal FM behavior, this output is especially good for creating “alive” sections.

## Song trick: use all three as separate arrangement layers
Patch:
- **1** to a lowpass filter for bass body
- **2** to a VCA + delay for top texture
- **OUT** to a distortion or LPG for rhythmic phrases

Now one module becomes a mini-ensemble. Across a full song you can mute/unmute or emphasize different paths.

---

# Full-song patch strategies

## 1. Generator as the central song voice

### Patch concept
- Output 2 = main voice
- Index Out = accent layer
- Output 1 = sub/low body or parallel distortion feed
- Sequencer sends slow pitch CV to both EXP inputs
- Envelope to Index CV
- Another oscillator/LFO/sample source into External FM input
- External destination switch set per section

### Arrangement use
- **Intro:** only output 1, filtered, low register
- **Verse:** bring in output 2 with modest FM
- **Pre-chorus:** increase Index CV depth with a longer envelope
- **Chorus:** mix output 2 + Index Out together
- **Breakdown:** mute output 2, leave delayed Index Out tail
- **Final chorus:** external FM deeper + shape brighter + parallel distortion

This works because the same timbral family persists through the whole song.

---

## 2. Generator as a percussion engine for evolving drums

The manual even gives a percussion patch idea:
- patch **Generator 2 output** into **External CV Input**
- set external switch to modulate **Generator 1**
- patch an **envelope generator** into **Index CV**
- listen to **Index Out**
- Gen1 low range, Gen2 mid range gives nice percussion

That can be expanded into a full drum architecture.

### Build a full drum role
- Trigger short envelopes into Index CV for struck timbres
- Sequence pitch offsets narrowly for different drum hits
- Use range switches manually or through external switched CV setups between sections
- Process with LPG, transient shaper, distortion, or compressor

### Full-song use
- **Verse:** Generator acts like tom/snare metallic hits
- **Chorus:** faster trigger density and more FM = industrial hats/rides
- **Breakdown:** long envelope into Index CV = resonant booms
- **Outro:** sparse percussive pings with heavy delay

One module can carry a whole drum subplot through the track.

---

## 3. Generator as bassline + fill machine

Since it doesn’t track perfectly, keep it in a narrow range and write bass parts by ear.

### Patch
- Output 2 through a lowpass filter and VCA
- Sequencer CV to Gen2 EXP in a limited range
- Envelope to VCA
- Index CV from accents or a second sequencer lane
- External FM from a synced LFO or from a percussion trigger converted to CV

### Why this works for songs
Bass arrangement often needs:
- stable root motion
- occasional fills
- section-dependent aggression

Generator can do all three if you separate:
- pitch motion = modest, constrained
- timbral motion = large, evolving

### Song map
- **Verse bass:** low Index, rounded shape, filtered
- **Chorus bass:** brighter shape, more internal FM, slight saturation
- **Turnaround fill:** brief burst of external FM on last bar
- **Bridge:** same bass rhythm but waveform shape reversed and lowpassed less

This keeps harmonic continuity while timbre tells the arrangement story.

---

## 4. Generator as a lead that evolves across sections

A strong modular song lead often needs to change identity while staying recognizable.

### Patch
- Output 2 into wavefolder or filter
- Index Out to a separate VCA/delay path
- Sequencer provides stepped CV motifs
- Slow envelope or LFO to Shape
- Performance control over Index amount
- External FM from another oscillator tuned to a consonant or dissonant interval by ear

### Section design
- **Intro motif:** dry output 2, triangle-leaning
- **Verse lead:** sparse notes, low FM
- **Pre-chorus:** increase FM and delay send
- **Chorus:** layer output 2 and Index Out, wider stereo FX
- **Solo/bridge:** reroute external FM destination to the other oscillator for a “same lead, new personality” change

That one destination switch can feel like a new instrument entering.

---

## 5. Generator as a drone/textural bed that supports song development

Generator is fantastic at long-form movement.

### Patch
- Output 1 and 2 to separate channels
- Very slow CV into one or both EXP inputs
- Slow random or looping envelope to Shape
- Sparse gates to Index CV for intermittent blooming
- External FM from a sub-audio LFO, another drone oscillator, or filtered noise

### Song use
- **Intro:** establish atmosphere
- **Verse:** keep low in mix as harmonic tension bed
- **Chorus:** open filter / add FM / widen stereo
- **Breakdown:** remove rhythmic instruments, let Generator carry continuity
- **Outro:** reduce motion until nearly static

This is a very effective way to make a modular track feel composed rather than merely looped.

---

# Techniques specifically for turning loops into songs

## 1. Use Generator as a macro-variation source
If your rhythm/melody is already working, don’t rewrite it immediately. Instead, use Generator to create sectional contrast over the loop.

For every 8 or 16 bars, change one of:
- Index amount
- Shape position
- external FM source depth
- external FM destination
- which output is prominent in the mix
- filter processing after the outputs

This creates musical development without losing the groove.

## 2. Create “energy lanes”
Assign separate control sources to:
- **pitch lane**
- **brightness lane**
- **FM intensity lane**
- **density lane** via VCA/gates
- **space lane** via effects send

Generator is strongest on the **brightness / FM intensity** lanes. Let another module handle exact harmony if needed.

## 3. Write section changes with CV, not only notes
A modular song often becomes full-length when section changes are driven by:
- different envelope times
- different FM amounts
- different wave shape balances
- switched modulation routing

With Generator, those changes are more dramatic than merely changing a note sequence.

## 4. Record long performances of timbre, then compose from them
Because Generator is gestural, it’s excellent for live takes:
- manually perform Shape
- ride Index
- switch modulation destination
- tweak frequency ranges between sections

Record 10 minutes, then edit into a song structure. This is often more effective than trying to sequence every change.

---

# Concrete arrangement recipes

## Recipe A: Verse / Chorus industrial electro track

### Supporting modules
- drum machine or drum voices
- sequencer with 2–4 CV lanes
- one filter
- 3 VCAs
- delay/reverb
- mixer with mutes

### Generator role
Main bass-lead hybrid

### Patch
- Output 2 → filter → VCA → mixer
- Index Out → distortion → VCA → mixer
- Output 1 → sub mixer channel or compressor input
- Accent envelope → Index CV
- Sequencer lane → Gen2 EXP
- Slow offset CV → Gen1 EXP
- Clocked LFO or another oscillator → External FM input

### Arrangement
- **Intro:** only filtered output 1 + delay send
- **Verse:** output 2 enters, low FM
- **Chorus:** Index Out distortion layer added
- **Post-chorus:** mute drums briefly, let Generator scream with more external FM
- **Bridge:** switch external FM destination, lower drum density
- **Final chorus:** all three outputs blended in different amounts

---

## Recipe B: Melodic techno with Generator as tension layer

### Supporting modules
- precise VCO for main melody
- quantizer
- sample-based drums
- stereo effects
- sequential switch
- utility mixer/VCAs

### Generator role
Counter-melody and textural riser source

### Patch
- Main melodic VCO handles accurate pitch
- Generator receives related but narrow CV movement
- Output 2 → bandpass filter → reverb
- Index Out → short delay ping path
- External FM from the main VCO or a divided clock LFO

### Arrangement
- **Verse:** subtle Generator texture underneath main line
- **Build:** increase Index CV every 4 bars
- **Drop:** mute main melody briefly; Generator carries lead tension
- **Chorus:** restore main melody while Generator becomes higher, noisier sparkle
- **Breakdown:** only Generator + kick + FX remain

This is very song-effective because Generator provides emotional motion without forcing tonal precision.

---

## Recipe C: Experimental ambient full-length piece

### Supporting modules
- random voltage source
- slews
- quad VCA
- stereo reverb
- looper or sampler
- LPG or resonant filter

### Generator role
Primary sound ecosystem

### Patch
- Output 1 → LPG → left channel
- Output 2 → filter → right channel
- Index Out → shimmer reverb
- Very slow random CV to Shape
- Sparse triggers to Index CV
- External FM from noise or another slow oscillator
- Manual changes of range switches every few minutes

### Arrangement
- **Part I:** nearly static drone
- **Part II:** introduce slow pulse through Index envelope
- **Part III:** external FM grows harsh and active
- **Part IV:** sampled loops of earlier material layered back in
- **Part V:** remove modulation, return to sparse harmonic residue

Generator can absolutely carry a long-form composition in this context.

---

# Advanced techniques for song structure

## Crossfade between outputs instead of changing patches
Because outputs 1, 2, and OUT are related, a crossfader can create smooth arrangement transitions.

Examples:
- verse = mostly output 1
- chorus = mostly output 2
- fill = momentary emphasis on OUT

This preserves continuity while still sounding arranged.

## Use switched modulation sources every 8 or 16 bars
Run a sequential switch into the External FM input:
- source 1 = slow LFO
- source 2 = envelope bursts
- source 3 = noise
- source 4 = another oscillator

Now Generator becomes a section-varying instrument automatically.

## Send drums or bass envelopes into Index CV
This is especially effective for track cohesion.
If the same envelope family controlling drums also controls Index dynamics, the Generator part “breathes” with the rhythm section.

## Parallel process the outputs
Try:
- Output 2 dry and centered
- Index Out distorted and compressed
- Output 1 lowpassed for sub/body

Mute combinations of these channels to produce structure.

## Use the range switches as arrangement markers
The 3-way range switch on each oscillator is not just setup; it is compositionally important.

Possible section logic:
- intro: Gen1 low, Gen2 low-mid
- verse: Gen1 low, Gen2 mid
- chorus: Gen1 mid, Gen2 high
- breakdown: Gen1 low, Gen2 high for extreme FM contrast

Even if done manually during recording, this is a powerful formal device.

---

# What kind of songs this module excels at

Generator is especially strong in:

- industrial
- electro
- EBM
- IDM
- experimental techno
- noise
- dark ambient
- sci-fi soundtrack
- broken beat
- abstract percussion music
- game-sound-inspired music
- drone-based composition

It can still work in melodic genres, but usually best when paired with a more precise pitch voice.

---

# A practical songwriting workflow with Generator

## Method 1: Build the arrangement first
1. Patch Generator into 2–3 parallel outputs.
2. Create four timbral states for sections.
3. Program or perform mutes and modulation changes.
4. Only after that, write detailed note content.

This avoids getting trapped in a perfect 4-bar loop.

## Method 2: Let Generator define transitions
If your drums and bass are already static:
1. keep the groove unchanged
2. automate Generator’s Shape / Index / FM routing over 16–32 bars
3. use it as the emotional curve of the track

## Method 3: Record stems from different outputs
Record:
- output 1 stem
- output 2 stem
- Index Out stem
- effects return stem

Then arrange those stems as if they were separate instruments. This is one of the easiest ways to get a “full song” from modular material.

---

# Limitations to plan around

## Not ideal as your only tuned voice
Because it is not 1V/oct and not temp compensated, use it by ear, in limited ranges, or as a secondary/expressive voice.

## FM can get chaotic quickly
That’s part of the appeal, but for song use:
- control depth with VCAs
- save the wildest settings for transitions and climaxes
- keep at least one layer more restrained

## Macro controls are powerful
Small movement can create large change. This is good for arrangement but means you should:
- attenuate incoming CV
- use offset generators
- rehearse performance gestures

---

# Best “song building” pairings by role

## If Generator is your bass voice
Add:
- precise sequencer
- lowpass filter
- envelope
- compressor
- parallel distortion
- accent CV lane to Index

## If Generator is your lead
Add:
- stereo delay
- reverb
- wavefolder or multimode filter
- clocked modulation
- crossfader for output blending

## If Generator is your percussion source
Add:
- trigger sequencer
- fast envelopes
- LPG or VCA
- transient shaping/distortion
- sample layer for consistency if needed

## If Generator is your texture bed
Add:
- slow random
- long envelopes
- stereo effects
- mixer sends
- looper/sampler for arrangement capture

---

# Simple full-song templates

## Template 1: 6-minute techno track
- 0:00–1:00 intro drone from output 1
- 1:00–2:00 beat enters, output 2 low in mix
- 2:00–3:00 bass pattern emerges via narrow EXP sequencing
- 3:00–4:00 increase Index CV and external FM for peak section
- 4:00–4:45 breakdown using Index Out + delay only
- 4:45–6:00 full groove returns with brighter Shape setting

## Template 2: electro song form
- intro
- verse A: Generator bass
- chorus A: Generator bass + distorted Index Out hook
- verse B: external FM destination changed
- bridge: Generator as percussion only
- final chorus: all layers return
- outro: output 1 alone fades

## Template 3: ambient narrative
- scene 1: low static pair
- scene 2: slight shape movement
- scene 3: internal FM bloom
- scene 4: external FM disruption
- scene 5: decaying residue

---

# Bottom line

The Pittsburgh **Generator** is excellent for full-length songs because it is not merely an oscillator—it is a **timbral relationship instrument**. Its real songwriting strength is that it lets you derive many related musical identities from one patch:

- raw voice
- FM voice
- percussion voice
- modulation source
- transition effect
- drone layer

To make songs with it, don’t treat it only as “the sound.” Treat it as a **section engine**:
- use **Index** for energy
- use **Shape** for character
- use **External FM routing** for contrast
- use its **multiple outputs** as separate arrangement layers
- pair it with **sequencers, envelopes, VCAs, filters, and a performance mixer**
- design **4–5 states** and move between them over time

That’s how this module can go from making a great loop to carrying a complete composition.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)