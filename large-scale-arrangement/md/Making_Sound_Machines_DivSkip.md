# Making Sound Machines — DivSkip

- [Manual PDF](../../manuals/SKORPION_Manual.pdf)

---

[Manual PDF](https://www.wmddevices.com/products/skorpion)

# WMD Skorpion: using one wild wavefolder to build full-length songs

Skorpion is not just a “make sound gnarly” module. Reading the manual closely, it’s really a **wavefolder + dynamic comparator network + target sequencer + modulation source bank + stereo widener + self-patch lab**. That means it can do much more than timbral sweetening inside a loop. It can become a **section-generator**, **arrangement pivot**, and **performance instrument** for turning a cool 8-bar patch into an actual track.

Below is a practical song-focused analysis.

---

## Why Skorpion is unusually good for song structure

A lot of Eurorack wavefolders are “set and forget” tone modules. Skorpion is different because it has:

- **8 thresholds (THLDs)** that define where folds happen
- **8 targets (TRGTs)** that act like a voltage sequencer tied to threshold activity
- **macro modulation** with attack/sustain/release behavior
- multiple **aux outputs** that can drive the rest of your system:
  - `TRGTs`
  - `COUNT`
  - `DAC`
  - `DIFF`
  - `ABS(IN)`
  - `G(IN>0)`
  - `±G(DIR)`
  - `DELAY`
- an **OUTPUT** control that morphs:
  - dry → wet
  - wet → wide
- **sync**, **halt**, and **dry if no thresholds** behavior

That means Skorpion can control:
1. **Timbre**
2. **Dynamics of timbral change over time**
3. **Stereo width / perceived scale**
4. **Modulation exported to other modules**
5. **Section contrast**

Those five things are exactly what’s usually missing when a patch sounds cool but doesn’t become a song.

---

# Core song-making concept

Think of Skorpion as a **scene transformer**:

- same pitch sequence in
- same rhythm in
- but different **threshold maps**, **targets**, **shape feedback**, **stereo width**, and **macro envelope states**
- output feels like a new verse, chorus, breakdown, or bridge

So instead of asking:
> “How do I make a whole song from one riff?”

Ask:
> “How do I use Skorpion to create 4–6 clearly different states of the same source material?”

That is where it shines.

---

# What Skorpion contributes in a full arrangement

## 1. Sectional timbre evolution
Use Skorpion to make one line evolve from:
- nearly dry intro
- lightly folded verse
- aggressive harmonically rich chorus
- halted/square-ish breakdown
- wide stereo outro

Because `FOLD`, `SLOPE`, `SHIFT`, `SHAPE`, `TARGET`, `OUTPUT`, `SYNC`, and threshold behavior interact, you get much more than “more distortion.”

## 2. Arrangement modulation source
The bottom-row outputs are perfect for sending “what Skorpion is doing” into:
- filters
- VCAs
- delay feedback
- reverb size
- sequential switches
- clock dividers / logic
- transposition
- percussion accents

So one lead voice processed by Skorpion can also drive the movement of your drums, bass, and ambience.

## 3. Contrast without repatching
The sliders store threshold and target profiles. Since settings are saved, and the spring toggle exposes different contexts, Skorpion can act like a **performable timbral score**. You can build recurring section identities.

## 4. Stereo expansion for bigger choruses
The `OUTPUT` control and delay/wide circuitry are very useful for song form:
- mono-ish verse
- wider pre-chorus
- big chorus
- dry breakdown
- wide return

This is huge for making sections read as “song sections” instead of just parameter changes.

---

# Best roles for Skorpion in a song

## A. Main lead voice transformer
Patch a VCO or complex melody through it and let Skorpion define section changes.

Best when you want:
- evolving hooks
- recurring motif with different emotional states
- performance-oriented transitions

## B. Bass enhancer that becomes a section marker
With restraint, Skorpion can make bass go from:
- round and dry
- clipped and articulate
- folded and aggressive
- asymmetrical and unstable

Use `OUTPUT SWITCH` in `FILTERS` mode to keep low end centered while widening upper harmonics.

## C. Drum bus or percussion mangler
Feeding percussion into `IN`, especially with `SYNC`, `CLIP`, `DIFF`, and `COUNT` outputs, can create sections ranging from tight and punchy to metallic and chaotic.

## D. Modulation hub
Even if the audio output is secondary, Skorpion can generate rich control voltages tied to audio activity. This is powerful for arrangement because audio-derived modulation feels musically coherent.

---

# Modules that pair especially well for making songs

Skorpion becomes much more “song-capable” when paired with:

## Sequencers
- melodic sequencer
- trigger sequencer
- CV recorder
- sequential switch

Use these to create recurring forms and recallable sections.

## VCAs / mixers
Essential for:
- automating dry/wet blends externally
- muting voices for arrangement
- sidechaining modulations
- fading Skorpion-derived aux outputs in and out

## Clock and logic
Use Skorpion outputs like `G(IN>0)` or `±G(DIR)` with:
- logic modules
- clock dividers
- comparators
- trigger routers

This creates section-dependent rhythmic variation.

## Filters
Skorpion is harmonically dense; pairing it with a filter lets you:
- restrain verses
- open choruses
- create breakdowns by emphasizing different bands

## Envelopes / function generators
Skorpion’s internal macro section is great, but external envelopes can:
- reshape transitions
- control output VCA
- sweep filter cutoff
- animate `FOLD`, `SHIFT`, or `OUTPUT`

## Samplers / loopers
Excellent for full-song construction:
- sample a Skorpion texture
- use that sample as a recurring motif
- reintroduce transformed versions across the arrangement

## Reverb / delay
Skorpion already adds width, but external spatial FX are crucial for section contrast:
- dry verse
- long reverb in bridge
- feedback bloom in outro

## Performance mixer
A proper mixer is where songs happen. Skorpion can create section identity, but the mixer makes it read as composition.

---

# Important manual features that matter for songwriting

## 1. OUTPUT knob: dry ↔ wet ↔ wide
This is one of the most song-useful controls on the module.

- lower half: blend dry and processed
- upper half: blend processed into stereo widened version

### Song use:
- **Intro:** mostly dry
- **Verse:** a little wet
- **Pre-chorus:** more wet, start widening
- **Chorus:** wide
- **Breakdown:** pull back toward dry
- **Final chorus:** full wide

This single control can act like an arrangement macro.

---

## 2. Macro envelope
The macro envelope controls the amplitude of internal LFOs. It can be gated from the toggle or `MACRO ENV` jack. Attack and release can be very long.

### Song use:
This is ideal for **section transitions**:
- long attack into chorus
- long release into outro
- slow morph over 16 or 32 bars
- repeated swells tied to phrase boundaries

Because it globally fades internal modulation, it feels like the patch “comes alive” or “calms down” over time.

---

## 3. THLDs and TRGTs
These are the heart of Skorpion’s compositional potential.

### THLDs
Control where folds occur.

### TRGTs
Define destination voltages for the vector core; essentially a threshold-driven voltage sequence.

### Song use:
You can create different timbral identities by changing:
- threshold distribution
- target order (`SEQ` vs `TIED`)
- target mode (`5V`, `CLIP`, `SLIDERs`)

This means one melody can behave like:
- smooth and stable in verse
- jagged and sequenced in chorus
- frozen/square-like in breakdown

---

## 4. SHAPE sources
The `SHAPE` control can modulate slope from:
- `IN`
- `OUT`
- `DELAY`
- `COUNT`
- `DIFF`
- `TRGTs`
- `DAC`
- `DIR`

### Song use:
Different shape sources can define section mood:

- `OUT`: more self-interacting, organic, “alive”
- `DIFF`: harsh, spiky, intense
- `TRGTs`: segmented, sequence-like, structured
- `COUNT`: rhythmic staircase feel
- `DELAY`: smeared, animated stereo motion

You can reserve specific shape-source choices for specific sections.

---

## 5. DRY IF NO THLDs
If no thresholds are active, output becomes dry signal tracking input.

### Song use:
This is excellent for **safe performance modulation**. You can heavily animate `FOLD` or thresholds without risking dead sections. It helps transitions stay musical.

---

## 6. HALT IF TARG=0 and HALT jack
This can stop the vector core for portions of the waveform or entirely.

### Song use:
This is a breakdown tool.
Use it to create:
- gated, square-ish static timbres
- dramatic holds
- rhythmic freezes
- “drop” moments before chorus re-entry

At audio rate modulation it can get very aggressive.

---

## 7. SYNC soft/hard
Resetting at input zero crossings changes the behavior significantly.

### Song use:
- **SOFT sync**: smoother, more controlled phrase sections
- **HARD sync**: more abrupt, aggressive, chorus/drop sound
- **No sync**: freer, more unstable intros/bridges

Changing sync mode between sections is underrated.

---

# Five concrete full-song strategies

## Strategy 1: One riff, four sections
This is the most direct way to turn a loop into a song.

### Patch
- VCO → Skorpion `IN`
- Skorpion `OUT L/R` → mixer
- Sequencer → VCO pitch
- Envelope/VCA after Skorpion or before depending on taste
- External clock to your sequencer
- Optional filter after Skorpion

### Build 4 section states

#### Intro
- `OUTPUT` near dry
- `FOLD` low
- `SHAPE` near noon
- `TARGET` toward `CLIP` or mild setting
- `SYNC` soft or off
- `WIDE` low

#### Verse
- moderate `FOLD`
- asymmetry via slight `SHIFT`
- modest `SHAPE` from `OUT`
- threshold pattern sparse
- narrow stereo

#### Chorus
- increase `SLOPE`
- increase `FOLD`
- `TARGET` toward `SLIDERs`
- richer TRGT values
- `SHAPE` from `TRGTs`, `COUNT`, or `DIFF`
- `OUTPUT` into wide region

#### Breakdown
- `HALT IF TARG=0` enabled
- some TRGT sliders at zero
- less width
- maybe `SYNC` hard
- more square/static segments

Now the same melodic line yields a full arrangement.

---

## Strategy 2: Use Skorpion as the song’s modulation brain
Instead of only using the audio output, use the aux outputs to animate the whole patch.

### Very useful outputs
- `COUNT`: 0–4V staircase, each active threshold adds 0.5V
- `DAC`: weighted threshold count
- `TRGTs`: target sequencer CV
- `DIFF`: difference between target and actual vector position
- `ABS(IN)`: full-wave rectified input
- `G(IN>0)`: polarity gate
- `±G(DIR)`: direction gate
- `DELAY`: delayed stereo signal source

### Example system patch
- `COUNT` → filter cutoff on pads
- `DAC` → reverb decay or send amount
- `TRGTs` → transpose a bassline or modulate oscillator FM depth
- `DIFF` → percussion VCA for metallic accents
- `G(IN>0)` → clock a switch between hi-hat patterns
- `±G(DIR)` → pan modulation or alternate drum voices

### Song result
Your lead voice and the rest of the arrangement evolve together. This is how patches stop sounding like isolated loops.

---

## Strategy 3: Verse/chorus via stereo width and harmonic density
A classic arrangement trick is:
- verse = narrow and less bright
- chorus = wide and harmonically rich

Skorpion is excellent for that by itself.

### Patch
- Bass voice through Skorpion or lead through Skorpion
- `OUT SWITCH` to `FILTERS` mode
- `OUT L/R` to main mix

### Arrangement
- **Verse:** output just below noon, mostly wet but not wide
- **Pre:** cross noon and start introducing delay-based width
- **Chorus:** 1–3 o’clock or more, wide engaged
- **Bridge:** pull width down, change shape source
- **Final chorus:** return to widest setting

This gives very obvious macro song form.

---

## Strategy 4: Make a bridge by changing what clips to what
The `CLIP` input is very interesting: input normally clips to itself, but another signal can replace it.

### Patch
- Main melody oscillator → `IN`
- Percussion loop / second oscillator / noise source → `CLIP`
- Modulate `TARGET` and/or `TRGT MOD`

### Song use
For a bridge or middle section:
- use a different `CLIP` source than the main voice
- your lead becomes overlaid/interrupted by another rhythm or melodic contour
- feels like a new harmonic environment without changing the sequencer drastically

This is excellent for:
- industrial
- techno
- experimental
- electro-acoustic transitions

---

## Strategy 5: Build long-form evolving sections with Macro Env
The internal modulation system is probably the most song-specific feature in the manual.

### Macro setup ideas
- slider 1: long attack, e.g. 16–64 bars
- slider 2: long release, e.g. 8–32 bars
- slider 3: threshold LFO amount moderate
- slider 4: threshold LFO rate slow
- sliders 5–8:
  - FOLD = LFO
  - SLOPE = ENV
  - SHIFT = slow LFO
  - SHAPE = ENV

Then trigger `MACRO ENV` from:
- a manual gate for performance
- an end-of-phrase trigger
- a song sequencer section pulse

### Result
A section can slowly “open up” over minutes, then collapse back. This is extremely useful for ambient, techno, kosmische, and soundtrack structures.

---

# Specific song roles by genre

## Techno
Skorpion can carry a lot of the arrangement alone.

### Good uses
- acid/bassline wavefolding with increasing `SLOPE`
- percussion through `CLIP` for industrial transitions
- `COUNT` or `DAC` controlling filter or send levels
- `OUTPUT` widening for drops/returns
- `DIFF` into FM amount on another oscillator for tension

### Song form
- 32-bar intro: dry/minimal
- 32-bar groove: mild folding
- 16-bar build: macro env opens SHAPE and thresholds
- drop: hard sync, wide output, high fold
- break: halt segments + reduced kick
- return: same riff, new target profile

---

## Ambient / drone
Skorpion is more than capable of slow-form composition.

### Good uses
- slow `MACRO ENV`
- sparse thresholds, equalized thresholds on/off
- `SHAPE` from `DELAY` or `OUT`
- `TRGTs` output to modulate reverb or filter banks
- `ABS(IN)` and `DIFF` for subtle motion elsewhere

### Song form
- establish clean tone
- gradually animate threshold motion
- widen output over long time
- introduce asymmetry via `SHIFT`
- bridge through alternate `CLIP`
- resolve back to dry-ish center

---

## IDM / experimental
This module was born for this.

### Good uses
- switch `TARGET ORDER` between `SEQ` and `TIED`
- use `HALT IF TARG=0`
- self-patch `DIFF`, `COUNT`, `TRGTs`
- feed rhythmic signals into `CLIP`
- use `G(IN>0)` or `±G(DIR)` as pseudo-rhythm generators

### Song form
- repeat motif
- mutate by target order
- bridge with halt or hard sync
- recontextualize same sequence with different threshold maps
- make returns feel earned by pulling back to a simpler state

---

## Pop / melodic electronic
Skorpion can still work, but with restraint.

### Good uses
- use as controlled harmonic sweetener
- automate `OUTPUT` for chorus size
- use `FILTERS` mode to preserve center low end
- keep `SHIFT` moderate
- use `TRGTs` for subtle phrase variation rather than chaos

### Song form
- intro: nearly dry pluck
- verse: slight fold
- pre-chorus: shape starts moving
- chorus: wider, richer harmonics
- post-chorus hook: use `DELAY` output separately
- bridge: more asymmetry or alternate clip source
- final chorus: widest and brightest

---

# Self-patching ideas that help with arrangement

Skorpion’s outputs make it especially suitable for self-patching. These often create section-changing behavior.

## 1. `COUNT` → `SHAPE CV`
More active thresholds create more shape modulation.
- section effect: density grows with fold complexity

## 2. `TRGTs` → `SHIFT CV`
Each threshold-crossing state changes symmetry.
- section effect: verse/chorus phrasing becomes more vocal-like

## 3. `DIFF` → `FOLD CV`
Aggressive unstable feedback.
- section effect: use only for builds or climaxes

## 4. `ABS(IN)` → external filter cutoff
Amplitude-following brightness.
- section effect: makes part sit forward without extra envelopes

## 5. `±G(DIR)` → switch between two effects sends
- up direction sends to delay
- down direction sends to reverb
- section effect: moving stereo phrases and responsive ambience

## 6. `DELAY` output → another voice’s FM or wavefolder input
- section effect: chorus-like interdependence across voices

---

# Building an actual full song: practical templates

## Template 1: “Single-voice song”
Great when you want to compose with minimal modules.

### Modules
- 1 oscillator
- 1 sequencer
- 1 envelope
- 1 VCA
- Skorpion
- reverb
- mixer

### Structure
1. **Intro**  
   Dry or near-dry oscillator through Skorpion, low fold.
2. **Verse**  
   Add moderate fold, slight shift asymmetry.
3. **Pre-chorus**  
   Bring in Macro Env, slowly increase threshold motion.
4. **Chorus**  
   Wider output, higher slope, shape from `OUT` or `TRGTs`.
5. **Breakdown**  
   Lower wet, enable halting behavior with zero targets.
6. **Final chorus**  
   Return to widest, richest state.
7. **Outro**  
   Long Macro Env release, pull output toward dry.

This works because the timbral arc itself becomes the song.

---

## Template 2: “Skorpion-centered trio”
A classic full arrangement with bass, lead, and drums.

### Modules
- Bass voice
- Lead voice
- Drum system
- master sequencer
- Skorpion
- filter
- mixer with sends
- delay/reverb

### Patch
- Lead voice → Skorpion
- `COUNT` → bass filter cutoff
- `TRGTs` → drum accent CV or percussion pitch
- `DIFF` → FX send level
- `G(IN>0)` → trigger logic for percussion variation
- `OUT L/R` → stereo mix

### Why this works
Now the lead timbre drives bass articulation and drum movement. That creates “arranged coherence,” which is often missing in modular jams.

---

## Template 3: “Bass through Skorpion, melody elsewhere”
Useful if you want stronger section contrast while keeping lead stable.

### Patch
- Bass oscillator/filter/VCA → Skorpion
- Melody voice straight to mixer
- `DAC` or `COUNT` from Skorpion → melody filter or FM index
- `DELAY` out → send FX or sidechain modulation destination

### Song result
The bass becomes the emotional engine of the arrangement:
- dry/tight verse bass
- distorted chorus bass
- halted breakdown bass
- wide harmonic final section

Meanwhile the melody provides continuity.

---

## Template 4: “Skorpion as bridge machine”
Sometimes a patch already has a great verse and chorus, but no bridge.

### Bridge recipe
- change `TARGET ORDER` from `SEQ` to `TIED` or vice versa
- feed a new signal into `CLIP`
- switch `SHAPE SOURCE` to `DIFF` or `DELAY`
- reduce `OUTPUT` width temporarily
- engage `HALT IF TARG=0`
- use macro env to slowly restore previous state

This gives a middle section that feels related but distinct.

---

# How to avoid “cool modular loop syndrome” with Skorpion

## 1. Assign one parameter per section identity
Do not wiggle everything at once. Decide:
- verse = target mode
- chorus = width
- breakdown = halt
- bridge = clip source
- outro = macro release

Section meaning becomes clearer.

## 2. Use recurrence
A full song needs return. If chorus 1 used:
- `TARGET` toward sliders
- `OUTPUT` wide
- `SHAPE` from `OUT`

then chorus 2 should recall that, even if bigger.

## 3. Exploit dry/wet contrast
People underestimate how musical it is to simply reduce processing. A dry return after complexity feels like composition, not just less modulation.

## 4. Let Skorpion modulate other voices
This is one of the biggest takeaways from the manual. The aux outs are not extras; they are your arrangement glue.

## 5. Use long times
Macro attack/release up to 600 seconds is enormous. That’s an invitation to think in phrases, sections, and movements, not just bar loops.

---

# A few especially strong patch ideas for songwriting

## Patch idea: Chorus opener
- lead voice → Skorpion
- Macro Env triggered every 16 bars
- FOLD LFO enabled
- SHAPE ENV enabled
- OUTPUT CV from a slow rising envelope
- `FILTERS` mode on output switch

Effect: each chorus blooms wider and brighter while lows stay centered.

---

## Patch idea: Breakdown freeze
- some TRGT sliders set to zero
- `HALT IF TARG=0` enabled
- lower `OUTPUT` toward wet but not wide
- `SYNC` hard
- `DIFF` → external LPG or VCA for clicks/textures

Effect: waveform stalls in certain segments, making a rigid broken shape perfect for a stripped-down breakdown.

---

## Patch idea: Bass-to-lead handoff
- bass through Skorpion in verse
- `TRGTs` output modulates a second oscillator’s timbre
- in chorus, mute bass processing down and raise second oscillator
- both are linked because the lead inherits the bass’s threshold-driven motion

Effect: continuity across sections without repetition.

---

## Patch idea: Skorpion-generated percussion accents
- percussive audio to `IN`
- `G(IN>0)` and `COUNT` used for logic/comparator-triggered accents
- `DIFF` to strike resonant filter ping or LPG
- `OUT L/R` lightly mixed under drums

Effect: the drum bus generates related percussion events, creating arranged fills and transitions.

---

# Limitations and how to work around them

## Limitation: easy to get lost in complexity
Skorpion can do so much that sections may blur together.

### Workaround
Use a notebook or patch sheet:
- Intro settings
- Verse settings
- Chorus settings
- Bridge settings

Treat it like recallable performance composition.

## Limitation: can overpower a mix
It produces lots of harmonics and width.

### Workaround
- use `OUTPUT SWITCH` in `FILTERS` mode
- keep bass centered
- use external EQ/filter
- automate dry/wet rather than leaving it full

## Limitation: modulation can become constant motion
Too much internal LFO activity can flatten the arrangement because everything is always “active.”

### Workaround
Use `MACRO ENV` strategically so modulation appears only in selected sections.

---

# Best overall mindset

The big compositional lesson from this manual is:

**Don’t use Skorpion only as a sound enhancer. Use it as a section designer and modulation narrator.**

If you do that, it can help solve one of the hardest Eurorack problems: making a patch tell a story over several minutes.

A strong approach is:

- choose one core riff or motif
- route it through Skorpion
- define 4–5 recognizable Skorpion “states”
- export Skorpion aux CVs to move the rest of your system
- use OUTPUT width and Macro Env for transitions
- return to earlier states for song-level repetition

That turns “cool loop” into “full-length piece.”

---

# Quick song-building checklist with Skorpion

## Use Skorpion for:
- **intro/chorus width contrast**
- **verse/chorus timbral contrast**
- **bridge via alternate CLIP source**
- **breakdowns via HALT / zero targets**
- **builds via Macro Env**
- **arrangement glue via COUNT / DAC / TRGTs / DIFF**
- **returns via saved threshold/target identities**

## Pair with:
- sequencer
- VCAs
- filter
- effects
- logic/switching
- mixer
- sampler/recorder if you want structure beyond live patching

---

If you want, I can also turn this into:
1. a **10-patch cookbook for full-song composition with Skorpion**, or  
2. a **section-by-section techno / ambient / IDM patch plan**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)