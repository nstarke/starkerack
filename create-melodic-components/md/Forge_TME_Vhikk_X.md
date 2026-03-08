# Forge TME — Vhikk X

- [Manual PDF](../../manuals/vhikk x.pdf)

---

[Manual PDF / Source](https://forge-tme.com/vhikk-x/)

# Using FORGE-TME VHIKK X to create melodic components in music

Based on the attached manual, **VHIKK X** is a **multi-algorithm sound source and processor** for Eurorack that can function as both a voice and an effects block. Even though the detailed per-algorithm pages are external to this PDF/manual, there is still enough here to explain how to use it musically for **melodies, basslines, tuned drones, and evolving tonal parts**.

## What the module is, musically

VHIKK X is not a conventional “VCO + filter + VCA” voice. It is a **self-contained experimental synthesis voice/processor** with:

- internal synthesis/generation
- stereo audio processing
- internal VCA
- voltage control over most major parameters
- encoder-controlled macro parameters:
  - **BASIS**
  - **TIME**
  - **SEED**
  - **SCAN**
- multiple algorithms selected by two toggle switches
- 4 banks × 9 algorithms = **36 total algorithms** (with firmware support)

That means, in a patch, VHIKK X can serve as:

- the **main melodic voice**
- a **bass voice**
- a **textural counter-melody**
- a **pitched stereo processor** for external oscillators/samplers
- a **drone source** that can still track pitch

The manual explicitly mentions it is good for:

- complex drones/basses
- rich textures
- dynamic SFX
- warped signal processing

For melody-making, the key idea is: **use BASIS as your pitch anchor**, then use the other parameters to shape articulation, timbre, movement, and phrase evolution.

---

## Important melodic features from the manual

## 1. BASIS is the pitch-oriented control

The manual strongly implies that **BASIS** is the parameter used for tuning and pitch tracking:

- it has a dedicated **BASIS CV input**
- it supports **calibration**
- calibration is explicitly described using **1V and 3V** from a **V/Oct source**
- the manual discusses “tracking” in calibration mode

So for melodic work, **BASIS is your 1V/oct-style pitch destination**.

### Practical takeaway
Patch a sequencer, keyboard CV, quantizer, or precision adder into:

- **BASIS CV input**

Then set the **BASIS attenuverter fully clockwise** when you want accurate melodic tracking.

This is the single most important setup step for tonal playing.

---

## 2. There is an internal VCA for note articulation

VHIKK X includes a **VCA input** controlling an **internal stereo VCA**.

From the manual:

- with nothing plugged in, a **+5V offset** is present, so the VCA is open
- applying external CV controls amplitude
- a **+5V external CV opens the VCA fully**
- voltages above that can overdrive later stages

### Why this matters melodically
This means you do **not necessarily need an external VCA** to make notes. You can patch an envelope, gate-derived envelope, or function generator into:

- **VCA input**

This gives you actual note shapes instead of a continuous drone.

So the simplest melodic patch is:

- pitch CV → BASIS
- envelope → VCA
- output → mixer/audio interface

That turns VHIKK X into a playable voice.

---

## 3. It can be calibrated for pitch tracking

Firmware v003 and above provides **BASIS calibration**.

This is crucial if you want:

- proper melodic intervals
- basslines that stay in tune
- sequences over several octaves
- layered tuning with other oscillators

### Recommended workflow
Before serious melodic use:

1. Put the **BASIS attenuverter fully clockwise**
2. Enter calibration mode
3. Send known calibration voltages from your sequencer or keyboard CV source
4. Save calibration

This makes VHIKK X much more reliable as a tonal voice.

---

## 4. TIME, MORPH, FIELD, FORM, etc. can all become musical phrase shapers

Even if BASIS handles pitch, the other controls are where the module becomes expressive.

Panel controls/CV destinations include:

- WARP
- SPAN
- MORPH
- FUSE
- BASIS
- FIELD
- MIX
- FEED
- TIME
- FORM
- CELL
- SCAN
- VCA

For melodic use, these should be thought of as **secondary dimensions of a note**:

- **TIME**: rhythmic tail, delay scale, temporal smear, articulation length
- **MORPH**: spectral/architectural transition between tonal states
- **FORM**: structure/complexity modifier
- **FIELD**: likely energy/distribution/positioning behavior depending on algorithm
- **SCAN**: movement through internal states or timbral zones
- **SEED**: manual reseeding of wave/timbre/random architecture
- **WARP / SPAN / FUSE / MIX / FEED / CELL**: algorithm-specific voicing and behavior controls

Even without the external algorithm pages, the manual makes clear these parameters are meant to create **coherent but unusual musical transformations**.

---

# Best ways to use VHIKK X for melody

## 1. As a complete melodic voice

This is the most direct use.

### Patch
- Sequencer pitch CV → **BASIS**
- Envelope → **VCA**
- Optional slow LFO → **MORPH**
- Optional random stepped CV → **SCAN**
- Optional performance knob moves on **SEED**
- Outputs L/R → mixer

### Result
A playable stereo melodic voice with:
- proper note articulation
- tuned pitch control
- timbral variation per note or per phrase
- evolving stereo character

### Good for
- leads
- basslines
- arpeggios
- eerie plucked tones
- unstable but tonal melodies

---

## 2. As a melodic drone source

Because VHIKK X seems very strong at dense and spectrally rich output, it can be used as a **drone voice that still follows musical pitch**.

### Patch
- Quantized CV or slow sequencer → **BASIS**
- Leave **VCA unpatched** for constant sustain
- Very slow modulation → **TIME**
- Slow triangle LFO → **MORPH**
- Manual or stepped CV → **SCAN**
- Manually adjust **SEED** occasionally

### Result
Instead of discrete notes, you get:
- sustained harmonic centers
- slow pitch changes
- modal or ambient movement
- evolving melodic beds

### Good for
- ambient
- soundtrack work
- intros
- harmonic pads
- one-note riffs that bloom internally

---

## 3. As a bass voice

The manual specifically mentions **complex drones/basses**, which suggests bass-capable algorithms.

### Patch
- Bass sequencer CV → **BASIS**
- Snappy envelope → **VCA**
- Short modulation envelope or CV accent → **FORM** or **FIELD**
- Optional accent CV → **MIX**, **FEED**, or **WARP** depending on response
- Mono out from **R** jack (manual says L is normalled to R for mono sum)

### Result
You can get:
- unstable basses
- acidic/metallic low-end
- animated sub-mid structures
- distorted melodic bass sequences

### Tip
Because output and input gain are generous and designed to soft-clip, you can push the sound into more aggressive territory for bass parts.

---

## 4. As a processor for another pitched voice

VHIKK X is also a **stereo processor**, so it can add melody indirectly by processing an external oscillator, synth voice, sampler, or chord source.

### Patch
- External oscillator or full mono/stereo voice → **audio input L/R**
- Sequencer CV → **BASIS** (if algorithm uses pitch-related internal structure)
- Envelope → **VCA**
- Modulation → **TIME / MORPH / FORM / FIELD**
- Audio out → mixer

### Result
Instead of generating all tone internally, VHIKK X can:
- harmonically reshape external melodic material
- granulate/warp lines into new phrases
- add internal pitch-aware coloration
- create call-and-response versions of an original melody

### Good for
- making simple oscillator lines more alive
- stereoizing mono melodies
- transforming sequences into hybrid acoustic/electronic textures
- generating “shadow melodies” from existing material

---

## 5. As a phrase-evolving sequenced voice

One of the strongest musical uses here is to let pitch remain stable while timbre evolves under CV.

### Core idea
Use:

- **BASIS** for the actual melody
- **SCAN** for phrase-to-phrase variation
- **MORPH** for macro transitions
- **TIME** for rhythmic density or delay scale
- **SEED** manually or occasionally randomized for larger section changes

### Patch
- Quantized sequence → **BASIS**
- Gate/envelope → **VCA**
- Clocked stepped random → **SCAN**
- Slow CV → **MORPH**
- Divided clock modulation or envelope → **TIME**
- Manual SEED tweaks between song sections

### Result
The notes stay musical, but the tone behaves like a living organism.

This is especially useful if you want:
- repeating melodies that don’t sound repetitive
- techno sequences with internal mutation
- soundtrack pulses
- post-industrial melodic figures

---

# Using the encoder system musically

The center encoders can target:

- **BASIS + TIME**
- **SEED + SCAN**
- **VOL** mode for input/output levels

This suggests a strong performance workflow.

## Performance strategy

## Encoder mode 1: BASIS + TIME
Use this for:
- tuning the voice to the track
- transposing riffs
- changing delay/temporal scale live

This is ideal during composition when defining key center and rhythmic feel.

## Encoder mode 2: SEED + SCAN
Use this for:
- changing timbral family
- moving through alternate internal states
- introducing new phrase identities

This is ideal during arrangement and live performance.

## Press both buttons (firmware v003+)
This randomizes:
- **SEED**
- **SCAN**

For melodic work, this can act like:
- instant variation
- phrase mutation
- “new preset” within the same algorithm

Useful when a melodic pattern is already running and you want a new tone without changing the sequence.

---

# CV normalling makes it easy to animate melodies

One of the smartest features in the manual is the **software-controlled CV normalling**.

## Normalled behavior

### If CV is patched into VCA:
That CV is normalled to:
- MORPH
- BASIS
- FIELD
- TIME
- FORM

through the attenuverters.

### If CV is patched into MORPH:
That CV is normalled to:
- BASIS
- FIELD
- TIME
- FORM

overriding the above behavior.

### If nothing is patched to VCA and MORPH:
A small offset is normalled to those inputs so the attenuverters can be used as fine controls.

---

## Why this is useful for melody

This means one envelope or one modulation source can animate multiple note dimensions at once.

### Example: one-envelope pluck behavior
Patch:
- envelope → **VCA**

Then use attenuverters for:
- a bit of **TIME**
- a bit of **FORM**
- a bit of **MORPH**

Now every note changes not just in loudness, but also in:
- brightness
- duration feel
- spectral contour

This is a huge shortcut for making melodic phrases sound expressive.

### Example: one LFO animating a melodic line
Patch:
- slow LFO → **MORPH**

Then attenuvert into:
- BASIS
- FIELD
- TIME
- FORM

Now one modulation source creates coordinated movement across the whole voice.

That can make static sequences sound composed rather than looped.

---

# Melodic patch recipes

## Patch 1: Basic tuned lead

**Goal:** playable melodic lead

- Quantizer/sequencer CV → **BASIS**
- Envelope → **VCA**
- Set BASIS attenuverter fully CW
- Small slow LFO → **MORPH**
- Outputs L/R → stereo mixer

**What to do:**
- choose an algorithm that self-generates
- calibrate BASIS first
- keep SCAN low at first for stable timbre
- adjust TIME to control temporal character

**Result:** a tuned stereo lead with subtle motion

---

## Patch 2: Experimental bassline

**Goal:** dirty but musical bass

- 8-step sequencer CV → **BASIS**
- Fast decay envelope → **VCA**
- Accent envelope or velocity CV → **FORM**
- Slow modulation → **FEED** or **WARP**
- Mono out from **R**

**What to listen for:**
- low-end weight
- attack character
- internal saturation
- note-to-note instability that still feels controlled

**Result:** aggressive evolving bass with real melodic identity

---

## Patch 3: Generative melody

**Goal:** semi-random melodic figure

- Random source → quantizer → **BASIS**
- Triggered envelope → **VCA**
- Clocked stepped CV → **SCAN**
- Slow random CV → **MORPH**
- Manual tweaks to **SEED**
- Optional second slower envelope to **TIME**

**Result:** changing but coherent melodic phrases

---

## Patch 4: Tonal drone / harmonic bed

**Goal:** background tonal movement

- Slow sequencer or precision adder changes → **BASIS**
- Leave VCA open
- Slow CV → **TIME**
- Slow LFO → **FIELD**
- Manual SCAN movement
- Stereo out to reverb or directly to mixer

**Result:** tuned atmospheric layer that supports the harmonic center of a track

---

## Patch 5: Process external melody

**Goal:** turn a simple melody into a transformed stereo line

- External oscillator/voice → input L (or stereo L/R)
- Melody pitch source also sent to external oscillator as usual
- Optional duplicate pitch CV → **BASIS**
- Envelope → **VCA**
- Modulation → **MORPH**, **FORM**, or **TIME**
- Output L/R → mixer

**Result:** the original melody gains strange internal animation and spatial depth

---

# How to make VHIKK X behave more musically in a tonal track

Because this module is intentionally abstract, the trick is to impose a few musical constraints.

## 1. Quantize the pitch going to BASIS
This keeps the melody anchored even if the timbre is wild.

## 2. Use small modulation amounts first
Especially on:
- BASIS
- SCAN
- MORPH
- FORM

Tiny amounts can produce musical liveliness. Large amounts may become atonal or highly unstable.

## 3. Let one parameter carry the melody and others carry expression
A good default:
- BASIS = notes
- VCA = note articulation
- MORPH = timbre evolution
- TIME = rhythmic tail
- SCAN = phrase variation
- SEED = section-level mutation

## 4. Save per-algorithm states
The manual says:
- SEED and SCAN are saved per algorithm
- VOL is saved globally
- BASIS/TIME can be global or per-algorithm

For composition, **per-algorithm save** is very useful because each algorithm can become its own melodic preset.

## 5. Use global BASIS/TIME save if switching algorithms live
If you want to browse algorithms without losing your tuning center or time base, set BASIS/TIME to **global saving**.

That makes live melodic performance more manageable.

---

# Stereo considerations for melodic use

VHIKK X is stereo throughout, with:

- stereo inputs
- stereo outputs
- true stereo improvements
- level LEDs for L/R
- mono sum available by patching only the **R** output

## How this helps melodically
Melodies can feel larger and more finished without additional modules.

Use stereo when you want:
- wide lead lines
- immersive arpeggios
- animated drones
- melodic effects returns

Use mono sum when you want:
- centered bass
- simpler mix placement
- layering with other stereo voices

---

# Gain staging tips for musical patches

The module has:

- input gain from silence to **+30 dB**
- output up to **18 Vpp**
- soft clipping at gain stages
- ability to handle line level in/out as well

## For melody:
- keep output moderate if going into another resonant/filter stage
- push output harder for saturated bass or lead
- if processing external line-level synths, use input gain to bring them up
- use the encoder **VOL** mode to balance external vs internal energy

This matters because melodic clarity can disappear if the internal saturation is too heavy.

---

# Limitations to be aware of

Because the provided PDF does not include the actual algorithm descriptions, a few things remain algorithm-dependent:

- whether an algorithm is self-generating or processor-focused
- where the VCA sits in that specific signal path
- how BASIS behaves in every algorithm
- exactly what TIME / FORM / FIELD / CELL do in each algorithm

So in practice, the best melodic workflow is:

1. choose an algorithm
2. verify it has pitched/self-oscillating behavior or useful pitch interaction
3. calibrate BASIS
4. patch pitch CV to BASIS
5. patch envelope to VCA
6. use MORPH / TIME / SCAN for expression

That is the reliable “musical core” across the module.

---

# Best musical roles for VHIKK X in a Eurorack system

## Excellent at
- lead voice with complex timbre
- bass voice with internal movement
- generative melody source
- tuned drone
- stereo melodic processor
- evolving arpeggios
- unstable but repeatable riffs

## Probably less ideal for
- ultra-precise vanilla subtractive melodies
- transparent bread-and-butter analog lines
- immediate one-knob-per-function conventional synthesis

This module is best when you want the melody to feel:
- strange
- alive
- haunted
- dynamic
- textural
- characterful

---

# Recommended “used together” signal chains in a rack

If by “used together” you mean how the functions of VHIKK X work together with typical Eurorack modules, here are the strongest pairings:

## VHIKK X + sequencer
For:
- basslines
- riffs
- leads

Patch sequencer CV to BASIS, gates to envelope, envelope to VCA.

## VHIKK X + quantizer + random source
For:
- generative tonal music
- ambient melodies
- shifting motifs

Random to quantizer to BASIS, clocked triggers to envelope/VCA.

## VHIKK X + envelope/function generator
For:
- expressive notes
- plucks
- swells
- animated timbre via CV normalling

A single envelope patched to VCA can animate multiple parameters through normalled routing.

## VHIKK X + clocked modulation
For:
- per-step phrase variation
- tempo-linked movement
- evolving motifs

Patch stepped or synced modulation to MORPH, TIME, or SCAN.

## VHIKK X + external oscillator or sampler
For:
- processing existing melodies
- making cleaner sources more alien
- stereo melodic enhancement

Patch audio in, then use VHIKK X as a pitch-aware or timbre-shaping transformation stage.

---

# Bottom line

**VHIKK X can absolutely be used to create melodic components**, especially if you treat it as an **experimental tuned voice** rather than a traditional oscillator.

The essential melodic patch is:

- **Pitch CV to BASIS**
- **Envelope to VCA**
- **Calibrate BASIS**
- Use **MORPH / TIME / SCAN / FORM** for expression
- Use **SEED** for larger identity changes

Its strengths for melody are:

- stereo output
- internal VCA
- pitch calibration
- rich algorithmic sound generation
- easy coordinated modulation through CV normalling
- strong potential for evolving but still playable tones

In other words:  
**VHIKK X is best for melodies that are not merely notes, but events.**

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)