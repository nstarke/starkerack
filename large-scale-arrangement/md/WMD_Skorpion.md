# WMD — Skorpion

- [Manual PDF](../../manuals/SKORPION_Manual.pdf)

---

[Manual PDF](https://www.wmddevices.com/products/skorpion)

# Using the WMD Skorpion to Build Full-Length Songs

Skorpion is not just a wavefolder. It is a **gesture-rich, self-modulating timbre sequencer, stereo widener, modulation source, and structure tool**. If you only use it as “audio in, folded audio out,” you’ll get excellent tones. But if your goal is **full-length songs**, the real power is that Skorpion can create **evolution over time**: section changes, timbral motifs, rising tension, drops, transitions, call-and-response, and arrangement-level modulation.

That is exactly the missing link in many Eurorack systems: not how to make a good sound, but how to make a sound **develop across minutes**.

---

## What Skorpion contributes to song structure

From the manual, these are the features that matter most for composition and arrangement:

- **Voltage-controlled wavefolding with multiple dimensions**
  - FOLD
  - SLOPE
  - SHIFT
  - SHAPE
  - TARGET behavior
  - threshold layout via sliders

- **8 thresholds and 8 targets**
  - This means the timbre can be treated almost like a **sequence of internal events**
  - The sound can change differently depending on which threshold crossings are active

- **Macro system with envelope-gated internal LFOs/envelopes**
  - This is huge for song form
  - You can bring modulation in and out over long timescales
  - Attack/release can be from **50 ms to 600 s**
  - That’s not just modulation; that’s **arrangement timing**

- **Aux outputs**
  - ABS(IN)
  - G(IN>0)
  - TRGTs
  - DIFF
  - ±G(DIR)
  - COUNT
  - DAC
  - DELAY
  - These can drive other modules, making Skorpion a **central composition brain**

- **Stereo output behavior**
  - Dry/wet/wide blending
  - Delay-based stereo widening
  - Optional filtered mid/side treatment
  - This helps with section contrast and mix placement over a song

So the key idea is:

> Skorpion can function as a **song-evolution engine**, not just a sound shaper.

---

# Core strategy: use Skorpion on the “arrangement axis”

In a full song, you need some or all of these:

1. **A stable identity**
2. **Gradual development**
3. **Clear section changes**
4. **Variation without losing coherence**
5. **Transitions**
6. **Mix-space contrast**
7. **A way to return to motifs**

Skorpion is especially strong at points 2–6.

Use it in one or more of these roles:

- **Main voice timbre animator**
- **Bass voice enhancer**
- **Percussion mangler**
- **Stereo transition processor**
- **Arrangement modulation hub**
- **Self-playing texture layer**
- **Cross-modulation source for the whole patch**

---

# Best full-song use cases

## 1. Make Skorpion the lead voice’s “arrangement performer”

Patch a melodic oscillator into **IN**, then send **OUT L/R** to your mixer or final VCA.

### Good pairings
- Analog VCO or complex oscillator
- Sequencer with transposition
- Envelope + VCA
- Filter after or before Skorpion
- Delay/reverb after Skorpion

### Why this works
A melody often gets stale because only pitch changes while timbre stays fixed. Skorpion gives you:
- different harmonic density via **SLOPE**
- different fold event behavior via **THLDs**
- asymmetry and frequency-shift-like movement via **SHIFT**
- section-specific contour via **TARGET**
- feedback personality via **SHAPE**

### Song workflow
- **Intro:** dry-ish output, low fold, equalized thresholds on for a classic wavefolder feel
- **Verse:** moderate fold, subtle macro-LFO on SHIFT or SHAPE
- **Pre-chorus:** start opening threshold modulation amount and increase output width
- **Chorus:** more wet, more slope, more target modulation, wide stereo on
- **Breakdown:** dry-if-no-thlds and sparse threshold settings so the voice almost collapses back to a filtered near-dry core
- **Final chorus:** reintroduce modulation with greater macro attack/release and wider stereo

This preserves the same melodic material while changing the emotional intensity.

---

## 2. Use Skorpion as a “section morph” processor for bass

Basslines often sound great in a loop but need arrangement variation without losing weight. Skorpion is useful because:
- it can remain centered if you use the **FILTERS** output switch with the mid/side network
- low frequencies under 240 Hz stay centered
- higher harmonics widen

This is ideal for full songs because you can make the bass:
- mono and restrained in verses
- brighter and wider in choruses
- aggressive and broken in fills
- filtered and reduced in breakdowns

### Patch
- Bass oscillator or submix -> Skorpion IN
- OUT L/R -> mixer
- Optionally blend a dry sub bass in parallel outside Skorpion

### Good controls to automate over a song
- **OUTPUT** from dry to wet to wide
- **SLOPE** for harmonic growth
- **SHIFT** for asymmetry and motion
- **TARGET** set toward 5V for more squared/aggressive character in louder sections
- **SYNC** hard or soft depending on desired tightness

### Arrangement trick
Use **COUNT** or **DAC** output to modulate:
- filter cutoff on a parallel bass filter
- VCA for a subtle dynamic brightness change
- compressor sidechain threshold CV if your system supports it

This ties the bass timbre’s internal folding activity to the rest of the mix.

---

## 3. Turn Skorpion into a percussion scene-transformer

Skorpion should be thought of as excellent for **drum bus processing** or **single percussion voice mutation**.

### Best input material
- Hats
- Claps
- Toms
- FM percussion
- Entire drum submix
- Noise bursts
- Loops from a sample player

Because Skorpion responds to threshold crossings and slope behavior, percussive material can become:
- metallic
- splattered
- gated
- sequenced in timbre
- pseudo-granular
- stereo animated

### Song application
Instead of changing the drum pattern, change the **drum character per section**.

### Example arrangement
- **Verse:** hats through Skorpion with low fold, slight delay width
- **Pre-chorus:** increase SHAPE using DIFF or OUT feedback source
- **Chorus:** widen output, increase SLOPE and THLD LFO amount
- **Bridge:** use HALT and TRGT = 0 segments for glitchy frozen slices
- **Transition fill:** hard sync and rapid modulation of FOLD and SHIFT

This creates the impression of new drum sections while the actual pattern may remain almost unchanged.

---

# The macro envelope is the song form secret weapon

The manual’s **Macro Setup / Macro Envelope** section is the most compositionally important part of the module.

You can:
- fade in/out the amplitude of threshold LFOs
- assign LFOs or envelopes to FOLD, SLOPE, SHIFT, SHAPE
- gate the whole internal modulation ecosystem with the toggle or MACRO ENV input
- use attack/release times up to **600 seconds**

That means Skorpion can evolve over **10-minute timescales**.

## Why this matters for songs
A full song needs macro-time movement. Most modular patches only move on:
- note timescale
- bar timescale
- maybe 8-bar timescale

Skorpion can move on:
- **section timescale**
- **whole-song timescale**

## Practical uses
### Long build
- Set macro attack to 60–180 seconds
- Gate macro on at the beginning of the track
- Let threshold LFO amount and SHAPE modulation slowly emerge
- Your lead or drone gradually becomes more alive over the first half of the track

### Chorus bloom
- Trigger macro gate only during chorus sections
- Use medium attack and release
- FOLD and OUTPUT widen together
- Chorus gets a consistent “opened up” identity

### Breakdown fade
- Turn macro off entering breakdown
- Long release allows motion to decay naturally
- Texture simplifies without abruptness

### Outro decomposition
- Send sparse gates to MACRO ENV while reducing source sequence complexity
- Let Skorpion become the main thing still moving
- Great for ambient and techno endings

---

# Build song sections with threshold and target states

The **THLDs** and **TRGTs** are where Skorpion becomes compositional rather than merely timbral.

## THLDs = where folds happen
The thresholds determine the “terrain” the incoming signal interacts with.

### Section idea
Use different threshold configurations for:
- intro
- verse
- chorus
- bridge

If you can’t automate the slider positions directly, create section changes with:
- **EQUALIZE THLDs** switch/jack
- **THLDs/** CV input
- **THLD1** input
- macro threshold LFO amount/rate
- switching between static settings with external CV or manual performance

### Musical effect
- Equalized thresholds: classic, more predictable, more “instrument-like”
- Unequal thresholds: more animated, quirky, phrase-like, unstable

That is a perfect contrast between:
- **verses = tighter**
- **choruses = richer or more chaotic**

## TRGTs = an internal 8-step voltage sequence
The targets can act like a mini sequencer affecting the vector core’s destination voltage.

This is powerful because it can impose **internal phrase contour** on the wavefolding.

### Song use
Create one target profile for a restrained section and another for a more dramatic section.

Also:
- Use **TARGET ORDER** = SEQ for more orderly progression
- Use **TARGET ORDER** = TIED for more event/reactivity based behavior

### Musical interpretation
- **SEQ** feels more patterned, stable, song-like
- **TIED** feels more gestural, responsive, live, chaotic

You can use this distinction structurally:
- intro/verse = SEQ
- fill/bridge/noise section = TIED

---

# Use the auxiliary outputs as composition signals

This is where Skorpion becomes truly valuable in larger patches.

---

## 1. COUNT output for arrangement-linked modulation

COUNT outputs a staircase from 0–4V, each active threshold adding 0.5V.

### Use it to modulate
- filter cutoff on another voice
- decay time of a percussion envelope
- VCA level for a texture layer
- clock divider probability
- wave index on a wavetable oscillator
- effect send amount

### Song value
COUNT lets another voice “follow” the density of Skorpion’s activity. This makes the song feel coordinated even if only one voice is directly processed.

Example:
- Lead voice through Skorpion
- COUNT modulates hi-hat decay and noise brightness
- As the lead becomes more harmonically active, hats become brighter too
- Instant chorus lift without changing the drum pattern

---

## 2. DAC output for subtler coordination

DAC is a weighted version of threshold count, more nuanced than COUNT.

### Use it for
- nuanced filter FM
- morph CV on digital oscillators
- scan position on a sampler
- stereo field control
- reverb size or tone
- LPG response

### Song use
If COUNT feels too stair-steppy, DAC can provide more “musical continuity.” It’s excellent for:
- background pad brightness
- send effects that bloom with the lead
- gentle movement in accompaniment

---

## 3. DIFF output as a high-energy transition source

DIFF is the difference between the target voltage and the vector core’s current position. It tends to be harmonically rich and always slopes toward 0V.

This is fantastic as a **transition CV** or even as audio.

### Use it to modulate
- resonant filter cutoff
- LPG strike amount
- distortion amount
- sample rate / bit depth
- reverb send
- burst generator density

### Song use
Patch DIFF into:
- a second oscillator’s FM index
- a filter on noise/percussion
- a VCA opening a riser layer

Then when Skorpion becomes more active, the transition layer naturally intensifies.

This is ideal for:
- pre-drop risers
- bridge noise tension
- chorus entry impact

---

## 4. TRGTs output as a phrase source

The TRGTs jack outputs the target sequencer directly.

### Use it to control
- another oscillator pitch, quantized
- filter cutoff sequence
- effect send sequence
- panning sequence
- switch matrix selection

### Song use
Let the same target sequence that shapes the lead timbre also shape:
- chord inversion changes
- percussion accents
- bass cutoff motion

That creates a deep sense of **motivic unity** across the arrangement.

---

## 5. G(IN>0), ABS(IN), and ±G(DIR) for rhythmic logic

These are excellent utility outputs for generative song structure.

### G(IN>0)
A gate high when input is above 0V.

Use it for:
- rhythmic gates tied to waveform polarity
- clocking switches
- pseudo-subdivision generation
- opening a VCA on another layer

### ABS(IN)
Full-wave rectified input.

Use it for:
- envelope-like modulation from any bipolar source
- dynamic reverb or delay send
- ducking signals
- deriving motion from a melodic line without polarity issues

### ±G(DIR)
+5V when vector core rises, -5V when it falls.

Use it for:
- bipolar panning
- alternating modulation destinations
- switching between two VCAs or effects
- creating call/response between left/right or A/B voices

### Song-level application
These outputs are excellent for making accompaniment voices derive their rhythm and phrasing from the main Skorpion voice, which helps a patch feel like a composed piece instead of disconnected loops.

---

# Song-building patch recipes

## Patch 1: Techno arrangement engine

### Modules
- Kick
- Hat/perc voice
- Bass oscillator + VCA/filter
- Lead oscillator + quantizer + envelope
- Sequencer
- Mixer
- Reverb/delay
- One or two VCAs
- Skorpion

### Patch
- Lead oscillator -> Skorpion IN
- Skorpion OUT L/R -> mixer
- COUNT -> hat decay CV
- DAC -> bass filter cutoff
- DIFF -> effect send VCA CV
- Macro ENV gate from sequencer section trigger

### Performance
- Verse: low macro, narrow output, equalized thresholds
- Build: increase macro env attack, open OUTPUT toward WIDE
- Chorus: increase FOLD/SLOPE and turn on threshold modulation
- Breakdown: lower fold and use DRY IF NO THLDs so melody remains but texture thins
- Rebuild: use DIFF to drive noise riser
- Drop: hard sync, wide output, stronger SHAPE feedback

Result: one melodic voice drives the evolution of several parts of the track.

---

## Patch 2: Ambient/drone long-form piece

### Modules
- Two oscillators or one oscillator + sampler
- Slow random or function generator
- Reverb
- Stereo mixer
- Skorpion
- Optional filterbank or resonator

### Patch
- Rich oscillator/drone source -> Skorpion IN
- DELAY output -> resonator or filterbank
- TRGTs output -> slow quantizer -> second oscillator pitch
- ABS(IN) -> reverb send amount
- ±G(DIR) -> stereo panning CV or crossfader
- Macro ENV gate manually toggled for section entrances

### Structure
- Start mostly dry and centered
- Slowly fade in macro modulation over 3–5 minutes
- Shift THLD LFO amount upward for increasing internal complexity
- Midway, use TRGTs and TARGET selection to alter contour
- End by reducing macro and leaving only delay/wide residue

Result: Skorpion becomes the central organism that evolves the entire piece.

---

## Patch 3: Bass-focused song with evolving top harmonics

### Modules
- Bass VCO
- Sub oscillator
- Filter
- VCA
- Drum machine / drum voices
- Sequencer
- Mixer
- Skorpion

### Patch
- Bass VCO -> Skorpion IN
- Sub oscillator bypasses Skorpion and stays mono
- Skorpion OUT -> mixer
- OUTPUT switch on FILTERS
- OUTPUT CV from section CV source
- G(IN>0) -> trigger accent envelope for percussion
- COUNT -> subtle overdrive amount on drum bus

### Arrangement
- Keep sub constant through the whole song
- Use Skorpion only for harmonic/top bass layer
- Verses: low wet, less width
- Choruses: more wet/wide and more target activity
- Fills: use HALT or target-zero squaring to make stuttering bass texture

This avoids losing low-end consistency while still getting major sectional changes.

---

## Patch 4: Drum bus mutation for transitions

### Modules
- Drum mixer/submix
- Skorpion
- Compressor
- FX send
- Noise source
- Envelope follower or function generator

### Patch
- Drum submix -> Skorpion IN
- Skorpion OUT -> parallel mixer channel
- DELAY out -> FX chain or feedback chain
- DIFF -> VCA controlling noise burst layer
- ABS(IN) -> compressor sidechain CV or ducking logic
- Macro ENV triggered only on fills and transitions

### Song use
Keep the clean drums always present, and bring in Skorpion as a parallel mutation layer:
- small in verses
- louder in fills
- huge before drops
- cut away after the drop

This is one of the most direct ways to make a loop become a full arrangement.

---

# How to use Skorpion for intro, verse, chorus, bridge, outro

## Intro
Best approaches:
- Dry/wet low
- Equalized thresholds on
- Low SLOPE
- Little to no macro modulation
- OUTPUT near dry or just entering wet
- DELAY/wide subtle

Goal: establish motif without giving away maximum intensity.

## Verse
- Moderate fold
- Controlled threshold activity
- SEQ target order for predictability
- FILTERS mode for stable stereo image
- Gentle SHAPE modulation

Goal: rhythmic and tonal clarity.

## Pre-chorus / build
- Increase macro envelope or trigger it on
- Increase THLD LFO amount
- Raise SLOPE
- Add DIFF-driven motion elsewhere
- Increase width slowly

Goal: growing complexity and anticipation.

## Chorus
- Wider output
- Higher fold and/or slope
- More asymmetry via SHIFT
- More active SHAPE source such as OUT, DIFF, or DELAY
- Potentially use TIED target order for livelier feel

Goal: maximal harmonic and spatial bloom.

## Breakdown
- Reduce active thresholds or use DRY IF NO THLDs
- Pull back width
- Simplify target behavior
- Let a single aux output modulate another minimal voice
- Long macro release to gracefully decay complexity

Goal: contrast and reset.

## Bridge / experimental middle section
- Use CLIP input from another signal
- Use TRGT MOD asymmetrically
- Use HALT creatively
- Switch sync modes
- Repatch SHAPE source

Goal: a truly distinct section without changing your main voice inventory.

## Outro
- Slowly reduce macro
- Pull OUTPUT back from wide to wet to dry
- Reduce target complexity
- Let DELAY or DIFF continue modulating support layers
- Thin the arrangement while preserving motion

Goal: decomposition instead of abrupt stopping.

---

# Combining Skorpion with specific module types

## With sequencers
Use sequencers not just for pitch, but for:
- section CV to OUTPUT, FOLD, or TARGET
- gates to MACRO ENV
- switching sync modes
- transposition while timbre remains continuous

Best song trick:
- one sequencer row for notes
- one row for section intensity
- that intensity row controls Skorpion

## With switches / sequential switches
Excellent for:
- swapping audio sources into CLIP
- changing CV source into SHAPE
- routing TRGTs output to different destinations per section
- alternating between equalized and custom threshold states

Switches are one of the easiest ways to turn Skorpion from “good sound” into “arranged composition.”

## With VCAs
Use VCAs everywhere around Skorpion:
- to control modulation depth from aux outputs
- to fade parallel dry/wet structures
- to automate transition layers driven by DIFF or COUNT

If you want full songs, VCAs are mandatory.

## With filters
Skorpion plus filter is very strong in either order:
- **Oscillator -> filter -> Skorpion** = cleaner and more controlled fold events
- **Oscillator -> Skorpion -> filter** = more sculpted, mix-ready aggression

For arrangement, a post-Skorpion filter helps you:
- reveal harmonics in choruses
- tame them in verses
- automate dramatic sweeps in builds

## With effects
Skorpion’s stereo output and delay behavior make it ideal before:
- reverb
- tempo delay
- granular processor
- shimmer
- resonator

Its aux outputs can also animate effect parameters so the effects “track” the timbral intensity.

## With samplers / loopers
Patch loops into IN or CLIP:
- vocal phrases
- drum loops
- field recordings
- chords

Then use Skorpion to create section mutations without changing the source sample.

This is especially effective for full songs because a familiar sample can remain identifiable while still evolving.

---

# Advanced full-song concepts

## 1. Use Skorpion as a recurring motif transformer
Have one melody or one texture recur in multiple song sections, but change Skorpion’s:
- threshold mode
- target behavior
- width
- shape source
- sync mode

This gives classic songwriting cohesion: **same theme, new emotional framing**.

## 2. Use aux outputs to make the whole patch “breathe together”
Instead of random unrelated modulations, derive motion from Skorpion:
- COUNT to percussion
- DAC to pads
- DIFF to FX sends
- G(IN>0) to rhythmic accents
- ±G(DIR) to panning or A/B switching

This makes the patch feel orchestrated.

## 3. Reserve Skorpion’s most extreme settings for only one section
A common mistake in modular is starting too intense. Because Skorpion can get very rich, save these for your biggest section:
- high SHAPE feedback
- hard sync
- TIED target order
- asymmetrical TRGT MOD
- maximum wide output
- active halt tricks

That creates a real arc.

## 4. Use manual performance as arrangement
Skorpion invites performance:
- move OUTPUT through dry/wet/wide
- flip EQUALIZE THLDs
- change TARGET mode
- hold spring toggle left/right to alter TRGTs or Macro Setup
- tap macro gate live

A full song in modular often emerges from a combination of:
- pre-patched relationships
- a few planned manual gestures

Skorpion is excellent for that.

---

# Practical “song mindset” with Skorpion

Instead of asking:

- “How do I make this sound cooler?”

Ask:

- “How does this same voice behave in section A vs B?”
- “What CV from Skorpion can animate another part of the arrangement?”
- “What parameter can evolve over 32 or 64 bars?”
- “How can I reduce complexity after increasing it?”
- “What is the chorus version of this timbre?”
- “What is the breakdown version of this timbre?”

That is the difference between a patch and a song.

---

# A simple template for writing a full track with Skorpion

## Voice roles
- Kick: stable
- Bass: mostly stable pitch/rhythm, moderate Skorpion-linked brightness
- Lead: main Skorpion-processed voice
- Texture/pad: modulated by Skorpion aux outs
- FX/riser: driven by DIFF or DELAY

## Section plan
### Intro
- lead dry-ish
- little macro
- no width

### Verse
- moderate wet
- equalized thresholds
- stable target behavior

### Build
- macro on
- threshold LFO amount rising
- output widening
- DIFF opens FX

### Chorus
- widest output
- highest slope/fold
- more active target behavior

### Breakdown
- dry-if-no-thlds
- lower modulation
- maybe only TRGTs output controls a secondary voice

### Final chorus
- return with wider stereo and stronger macro than first chorus

### Outro
- release macro
- narrow stereo
- fade to dry or delay residue

This alone can turn a loop into a complete form.

---

# Best companion modules for full-song use

Skorpion pairs especially well with:

- **A strong sequencer**  
  for notes, section gates, and intensity CV

- **VCAs / modulation VCAs**  
  to scale aux outputs into arrangement-level changes

- **Sequential switches**  
  for section-dependent routing and variation

- **A mixer with mutes or scenes**  
  to bring Skorpion in as parallel processing

- **A filter or EQ module**  
  for section contrast and mix control

- **A stereo reverb/delay**  
  because Skorpion already creates width and complex harmonics

- **A sampler or loop source**  
  for long-form mutation of repeated phrases

- **Logic / comparators / clock utilities**  
  to translate Skorpion’s gates into song events

If you’re trying to make full songs, don’t just patch Skorpion as a single insert effect. Patch it as a **network node**.

---

# Final takeaway

The WMD Skorpion is unusually well-suited to full-length Eurorack songwriting because it bridges three things at once:

1. **Sound design**
2. **Modulation architecture**
3. **Arrangement-scale evolution**

Most modules do one or two of these. Skorpion does all three.

Its strongest song-level uses are:

- evolving a lead or bass voice across sections
- making percussion or loops transform without changing patterns
- using macro attack/release for long-form movement
- deriving arrangement CV from COUNT, DAC, DIFF, TRGTs, and gate outputs
- creating stereo expansion as a compositional event
- letting one patch produce multiple section identities

If you approach it as a **section morphing instrument** rather than just a wavefolder, it can absolutely help turn a compelling loop into a compelling song.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)