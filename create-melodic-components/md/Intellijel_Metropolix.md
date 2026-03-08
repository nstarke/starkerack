# Intellijel — Metropolix

- [Manual PDF](../../manuals/metropolix_manual_v1.4_2022.04.04.pdf)

---

[Metropolix Manual PDF](#)

# Using Intellijel Metropolix to Create Melodic Components in Eurorack

The **Intellijel Metropolix** is an unusually deep melodic sequencer. Even though it looks like an 8-stage pitch/gate sequencer, it’s really a **performance-oriented melodic composition system** with:

- **2 pitch/gate tracks**
- **8 modulation lanes**
- **2 assignable outputs**
- **3 assignable CV inputs**
- **scale quantization**
- **probability, ratchets, slide, accumulation**
- **preset recall and chaining**

If your goal is to create **melodic material**—basslines, leads, counterpoint, arpeggios, evolving motifs, chord movement, and modulation-driven phrasing—Metropolix is extremely capable.

---

## What this module does musically

At its core, Metropolix gives you:

- a set of **8 pitch sliders** for an initial melodic contour
- per-stage **timing and gate behavior**
- two tracks that can reinterpret the same stage data differently
- modulation lanes that can animate pitch, scale, order, length, root, probability, slide, and more

This means one programmed idea can become:

- a **main melody**
- a **harmonic partner**
- a **bassline variant**
- an **arpeggiated extension**
- a **transposing phrase**
- a **self-modulating generative line**

---

# Core melodic building blocks

## 1. Pitch sliders as melodic skeleton

The 8 pitch sliders define the basic note contour. With **scale quantization**, those slider positions become stable melodic intervals in a chosen scale.

Useful global pitch tools:

- **Scale + Root**
- **Bottom Pitch = C or Root**
- **Slider Octaves** per track (1–4 octaves)
- **Slider Direction** per track (normal or inverted)
- **Transpose** per track

### Musical use
Program a simple contour with sliders:
- up-step
- leap
- repeat
- fall
- resolve

Then let each track reinterpret it differently.

Example:
- **TRK 1** = narrow 1-octave melody in C minor
- **TRK 2** = same sliders, but transposed up a 5th, inverted, or spanning 3 octaves

That immediately creates melodic relationships without reprogramming notes.

---

## 2. Two tracks for counterpoint and harmony

A big strength of Metropolix is that **TRK 1 and TRK 2 share the main slider/switch structure**, but each track can have different:

- order
- length
- clock division
- swing
- slide time
- gate length
- transpose
- slider range/direction
- per-stage pitch/gate/ratchet/probability/accumulation/CV

### Musical use
This is ideal for melodic layering:

#### A. Melody + bassline
- **TRK 1** → lead voice
- **TRK 2** → bass oscillator

Use:
- same slider pattern
- TRK 2 lower transpose
- slower division on TRK 2
- shorter sequence length on one track for phrase cycling

#### B. Melody + counter-melody
- TRK 1 = linear forward
- TRK 2 = pendulum or odd/even
- different stage skips and lengths

This creates **interlocking melodic motion** from one shared source.

#### C. Unison variation
Send both tracks to similar voices:
- one dry
- one filtered/delayed/slid

Use subtle differences in:
- gate length
- pitch pre/post
- probability
- order

This gives “doubled lead” behavior without exact repetition.

---

# Melodic timing and phrasing tools

## 3. Pulse count creates rhythmic phrasing for notes

Each stage can last **1 to 8 pulses**. That changes how long a note occupies space.

This matters melodically because note duration shapes phrase identity as much as pitch.

### Musical use
Use long pulse counts on:
- phrase starts
- cadence tones
- pedal notes

Use short pulse counts on:
- passing notes
- ornaments
- arpeggio-like movement

For example:
- Stage 1 = 3 pulses
- Stage 2 = 1 pulse
- Stage 3 = 1 pulse
- Stage 4 = 4 pulses

This turns a plain pitch pattern into a real phrase.

---

## 4. Gate type changes articulation

Per stage you get:

- **HOLD**
- **MULTIPLE**
- **SINGLE**
- **REST**

### Melodic applications
- **HOLD** = legato tie across stages
- **SINGLE** = one articulated note even if stage lasts several pulses
- **MULTIPLE** = repeated articulation on the same pitch
- **REST** = silence, space, phrasing

This is excellent for making melodic patterns feel played rather than mechanical.

Example:
- HOLD on a note before a slide
- REST before phrase restart
- MULTIPLE for repeated tonic or dominant pulses

---

## 5. Slide for legato and acid phrasing

Per-stage **SLIDE** with global track slide settings gives expressive transitions.

Slide types:
- **Analog**
- **Tempo**
- **Acid**

### Musical use
- Add slide only on selected approach notes
- Use acid mode for classic tied melodic sequences
- Use tempo slide for synchronized lead phrasing
- Use analog for freer portamento feel

Great for:
- basslines
- legato leads
- gliding modal melodies
- synthetic vocal phrasing

---

# Advanced melodic variation

## 6. Per-stage pitch override

The sliders are only the default. Each stage can have a **pitch override**.

### Musical use
This is powerful for:
- forcing important harmonic tones
- changing just one note in a looping phrase
- creating call/response variants between tracks
- making one track diverge from the common slider pattern

A useful strategy:
- use sliders for broad melodic shape
- use pitch overrides for “composed” anchor notes

---

## 7. Skip for phrase reshaping

Skipping stages changes both rhythm and note order.

### Musical use
A melodic phrase can become:
- sparse
- syncopated
- asymmetrical
- alternate-bar variation

Very useful for:
- verse vs chorus feel
- switching between complete and reduced phrases
- turning 8-stage material into 5- or 6-note motifs

Also excellent when modulated with **Skip Invert** for phrase swapping.

---

## 8. Probability for melodic instability and life

Probability can apply at:
- **Stage**
- **Pulse**

### Musical use
Use probability to create:
- ghost notes
- variable ornaments
- occasional melodic omissions
- unstable motif repetition

Examples:
- 80% probability on passing tones
- 50% probability on a decorative upper neighbor
- 100% on structurally important notes

This keeps melodies fresh without losing identity.

---

## 9. Ratchets for ornaments and repeated notes

Ratchets subdivide pulses into repeated gates.

### Melodic use
Ratchets are not just rhythmic—they create melodic ornament when combined with:
- accumulation
- slide
- CV lane modulation
- gate stretching

Good uses:
- stuttered repeated note on a climax tone
- flutter before resolution
- pseudo-trill or mordent effect on one stage
- repeated bass pulse under moving harmony

---

## 10. Accumulation is one of the best melodic tools here

The **ACCUM** function cumulatively transposes notes over time by scale degree. This is huge for melodic development.

Per stage you can define:
- transpose amount
- trigger source (stage / pulse / ratchet)

And with **LIM** options:
- positive/negative limits
- stage vs track mode
- wrap / pendulum / random / hold
- unipolar / bipolar
- reset behavior

### Musical use

#### A. Sequence evolution
A simple 4-note melody can climb diatonically over repeats.

#### B. Arpeggiated chord motion
Use chord scales and accumulation to walk through chord tones over time.

#### C. Canon-like development
Track mode makes one stage’s accumulation affect the whole track, causing phrase-wide transposition.

#### D. Generative tonal movement
Random or pendulum accumulation creates melodic movement that stays musically constrained.

This is one of the strongest features for writing **evolving melodic material**.

---

# Scales, roots, and harmonic movement

## 11. Scale quantization keeps melodies musical

Metropolix has many scales and chord shapes, plus 100 user scales.

### Musical use
You can use scale quantization to make slider movement immediately usable for:

- tonal melodies
- modal melodies
- pentatonic riffs
- chord-tone constrained melodies
- non-Western scalar movement

---

## 12. User scales for chord progressions and melodic harmony

User scales store both:
- scale pattern
- root

And can be sequenced via CV/modulation.

### Musical use
Build a bank of custom scales representing chord tones, for example:
- Cmaj triad
- Amin triad
- Fmaj triad
- Gmaj triad

Then modulate **Scale (User)** to move through harmonic centers while the same slider pattern keeps playing.

This is an elegant way to create:
- chord-following melodies
- arpeggiated harmonic movement
- phrase transposition with harmonic constraint

This makes Metropolix unusually strong for **harmonic melodic sequencing** rather than just monophonic looping.

---

# CV lanes and MOD lanes as melodic animators

## 13. Track CV lanes add one more melodic control stream per track

Each note track includes a CV lane that can be:
- continuous voltage
- gate toggle

You can route this out through OUT A or B.

### Musical use for melodies
Use track CV lanes to animate the voice being sequenced:
- filter cutoff per note
- wavefold amount per note
- FM amount per note
- accent/velocity
- envelope decay
- oscillator timbre

This turns a melody into a phrase with articulation and timbral contour.

Examples:
- brighter notes on high melodic peaks
- accent every 4th note
- longer envelope on cadence tones
- timbral rise on phrase build

---

## 14. 8 MOD lanes can modulate melodic behavior internally

Each MOD lane has:
- 8 stages
- its own order
- its own length
- its own clock division
- assignable destination

Destinations include many melodic parameters:
- pitch pre
- pitch post
- root
- user scale
- play order
- pulse count
- probability
- ratchet
- stages length
- stage offset
- slide amount
- gate length
- loopy settings
- accumulation settings

### Musical use
This is where Metropolix becomes a full melodic ecosystem.

#### A. Internal transposition
Assign MOD lane to **Pitch Pre** for in-scale melodic motion.

#### B. Chromatic destabilization
Assign MOD lane to **Pitch Post**.

#### C. Harmonic movement
Assign MOD lane to **Root** or **Scale (User)**.

#### D. Phrase restructuring
Assign MOD lane to **Play Order**, **Stages Len**, or **Stage Offset**.

#### E. Expressive articulation
Assign MOD lane to **Probability**, **Gate Length**, or **Slide Amount**.

This allows melodies to morph over time without external modules.

---

# Performance-oriented melodic techniques

## 15. Loopy mode for live melodic improvisation

Loopy lets you temporarily loop sub-sections of the sequence or play stages manually.

### Musical use
This is outstanding for live melodic performance:
- repeat one note as a pedal
- isolate a 2–4 note motif
- create fills by looping a mid-phrase fragment
- manually “play” stages as a mini keyboard when stopped

1-finger and 2-finger loopy can create improvised melodic variation in real time.

This is great for:
- techno lead fills
- live bassline mutation
- breaking a phrase into hooks
- performance transitions

---

## 16. CTRL knobs for expressive melodic macro control

The two CTRL knobs can be assigned to melodic parameters such as:
- Pitch Pre/Post/Offset
- Root
- Scale (User)
- Probability
- Ratchet
- Slide Amount
- Swing
- Stages Len
- Clock Div
- Trk Out Swap

### Musical use
These make excellent melodic macro controls:

- **CTRL 1 → Gate Length**: articulation macro
- **CTRL 2 → Slide Amount**: expressive phrasing
- **CTRL → Root**: harmonic movement
- **CTRL → Probability**: stable to unstable melody
- **CTRL → Stages Len**: phrase contraction/expansion
- **CTRL → Play Order**: melody permutation control

Very playable.

---

## 17. AUX inputs for external melodic interaction

Three AUX CV inputs can modulate internal melodic parameters.

### Musical use
Patch external modulation into:
- root
- scale selection
- pitch pre/post
- play order
- stages length
- slide
- probability
- accumulation behavior

That lets another sequencer, LFO, envelope, random source, keyboard, or pressure CV reshape melody in real time.

Example:
- slow random CV to **Root**
- envelope to **Slide Amount**
- gate pattern to **Skip Invert**
- keyboard CV to **Octave**

Now Metropolix behaves less like a fixed sequencer and more like an interactive melodic instrument.

---

# Presets and composition workflow

## 18. Presets for melodic scenes

Metropolix stores 64 presets.

A preset can store:
- track settings
- stage settings
- scale settings
- optionally slider/switch/CTRL/AUX states

### Musical use
Treat presets as:
- verse melody
- chorus melody
- breakdown variation
- transposed harmonic section
- sparse/dense alternate states

---

## 19. Preset chaining for song-form melody

Preset chains let you sequence preset changes over time.

### Musical use
Create structured melodic arrangements:

- Preset 1 = intro motif
- Preset 2 = bass enters
- Preset 3 = full lead phrase
- Preset 4 = variation with different root/scale/order
- Preset 5 = reduced outro loop

This turns Metropolix into a **melodic song-form sequencer**, not just a phrase generator.

---

# Practical melodic patch ideas

## Patch 1: Bassline + lead from one idea
- **TRK 1 PITCH/GATE** → bass voice
- **TRK 2 PITCH/GATE** → lead voice
- Same slider contour
- TRK 1: lower transpose, acid slide, shorter gate
- TRK 2: longer gate, different order, higher octave

Result:
A coherent melodic pair from one gesture.

---

## Patch 2: Chord-following melody with user scales
- Create user scales for progression chord tones
- Lock user scale bank
- Assign MOD lane or AUX to **Scale (User)**
- Program lead phrase on sliders

Result:
One phrase follows chord changes without manually reprogramming notes.

---

## Patch 3: Evolving modal melody
- TRK 1 = melody
- MOD lane 1 → Root
- MOD lane 2 → Probability
- MOD lane 3 → Play Order
- CV lane → filter cutoff on voice

Result:
Melody stays recognizable but keeps shifting tonally and structurally.

---

## Patch 4: Ornamented generative lead
- Use a simple 4-stage motif
- Add ratchets on one or two stages
- Add stage probability to passing tones
- Add accumulation with pendulum order
- Use slide selectively

Result:
A melodic line that sounds composed but continues developing.

---

## Patch 5: Performance hook machine
- Build a strong 8-stage motif
- Use Loopy for live fragment looping
- Assign CTRL knobs to Slide Amount and Root
- Use AUX input for Skip Invert or Play Order

Result:
You can “perform” melody rather than merely start playback.

---

# Best melodic strengths of Metropolix

## Especially strong for:
- basslines
- acid sequences
- modal melodies
- counterpoint from one source
- evolving repeating motifs
- arpeggio-like melodic figures
- harmonically constrained generative phrases
- live melodic improvisation

## Less about:
- piano-roll style step entry
- explicit polyphonic chord sequencing from separate outputs alone

It excels at **musical variation from compact material**.

---

# Summary

The **Intellijel Metropolix** can be used to create melodic components by combining:

- **pitch sliders** for note contour
- **scales/root** for tonal control
- **2 tracks** for harmony/counterpoint
- **pulse counts and gate types** for phrasing
- **slide, ratchets, probability, and skip** for expression and variation
- **accumulation** for evolving melodic transposition
- **CV lanes** for note-by-note articulation
- **MOD lanes** for self-modulating melodic change
- **Loopy** for live performance manipulation
- **presets and chains** for melodic arrangement over time

In practice, Metropolix is best understood not as a simple step sequencer, but as a **melodic performance and composition engine** for Eurorack.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)