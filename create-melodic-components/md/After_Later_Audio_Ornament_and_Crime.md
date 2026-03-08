# After Later Audio — Ornament and Crime

- [Manual PDF](../../manuals/ornament and crime.pdf)

---

[Ornament & Crime v1.3 User Manual](https://ornament-and-cri.me/user-manual-v1_3/)

# Using Ornament & Crime apps together to create melodic components

Ornament & Crime is best understood not as one module, but as a **toolbox of pitch and rhythm logic**. From the manual, the apps most directly useful for melodic work are:

- **Quantermain** — quad quantizer
- **Meta-Q** — dual quantizer with scale-slot sequencing
- **Sequins** — dual pitch sequencer
- **Acid Curds** — chord sequencer / harmonic quantizer
- **Harrington 1200** — triadic chord transformation generator
- **Automatonnetz** — Tonnetz vector sequencer for chords and melodies
- **CopierMaschine** — quantizing ASR / melodic delay / CV recorder
- **Piqued** — envelopes and Euclidean trigger filtering
- **Quadraturia / Low-rents / Dialectic Ping Pong / Viznutcracker** — modulation or semi-random CV sources that can feed the pitch apps
- **References** — tuning and calibration support

Below is a practical musician-focused analysis of how they can work together to produce **melody, harmony, variation, phrasing, and structure**.

---

## 1. The core melodic workflow in O_C

A useful mental model is:

1. **Generate CV**
   - sequenced
   - random
   - chaotic
   - sampled
   - chord-derived

2. **Quantize or harmonize it**
   - Quantermain
   - Meta-Q
   - Acid Curds
   - CopierMaschine

3. **Add timing and phrasing**
   - Piqued
   - trigger delays
   - Euclidean masks
   - sample-and-hold clocks

4. **Create harmonic relationships**
   - Harrington 1200
   - Automatonnetz
   - Acid Curds
   - Sequins in parallel channels
   - CopierMaschine shifted taps

That means O_C can cover:
- lead melody
- bassline
- countermelody
- chord roots
- triads / chord voicings
- arpeggios
- transposed repeats
- probabilistic note streams

---

# 2. Best apps for melody creation

## Quantermain: turning any voltage into melody

Quantermain is the most universal melodic app in the manual.

### Why it matters musically
It takes external or internal CV and turns it into notes in a chosen scale. Since each of the four channels is independent, it can do:

- 4 voices from 4 CV sources
- 1 CV source quantized differently across 4 outputs
- 4 related melodic lines sharing clock or scale
- quad sample-and-hold melodies

### Strong melodic uses
- Quantize slow LFOs into stepped melodies
- Quantize sequencer rows from another module
- Use continuous quantization for glide-like melodic movement
- Use clocked quantization for rigid rhythmic notes
- Use internal sources:
  - **Turing/LFSR** for looping pseudo-random melodies
  - **Logistic map** for chaotic melodic movement
  - **Byte beats** for strange note patterns
  - **Integer sequences** for mathematically structured melodies

### Melodic patch ideas
- **Bass / lead pair:** same CV into two channels, different scales or note masks
- **Pedal + melody:** one channel with narrow range, another with wider transpose
- **Canon:** same trigger and source, different transposition per channel
- **Modal morphing:** use different active note masks per channel

### Especially useful feature
You can set scale to **Off** and use it as a pure S&H or unquantized CV source, then quantize elsewhere later.

---

## Meta-Q: melody plus harmonic sequencing

Meta-Q is like Quantermain, but more compositional.

### Why it matters musically
Each channel has **four scale slots**, and each slot stores:
- scale
- mask
- root
- transpose

These slots can be sequenced by trigger or CV. So instead of just quantizing notes, Meta-Q can quantize notes while changing the harmonic frame over time.

### Musical result
This is excellent for:
- chord progression-aware melodies
- modal interchange
- phrase-based scale changes
- melody lines that recontextualize the same incoming CV

### Typical uses
- Feed one evolving CV into Meta-Q
- Sequence scale slot changes with TR2/TR4
- Result: same contour, different harmonization over time

This is a powerful way to get:
- “verse / chorus” pitch language shifts
- ii–V–I style movement
- melodic repetition with harmonic evolution

### Best role in a system
Meta-Q is ideal as a **high-level musical brain** that imposes harmonic structure on otherwise simple CV.

---

## Sequins: direct note writing

Sequins is the most straightforward melodic source in the manual.

### Why it matters musically
It provides:
- 2 channels
- 4 patterns per channel
- up to 16 steps per pattern
- chaining up to 64 notes
- scale quantization
- direction modes
- clock mult/div
- CV addressing

### Musical strengths
- Write exact melodies
- Create bassline + lead together
- Use different pattern lengths for polymelody
- Sequence pattern changes externally
- Use CV address mode for non-linear phrase access

### Great compositional features
- Sequence chaining: `SEQ+1` to `SEQ+3`
- Trigger-based switching: `TR+1` to `TR+3`
- Brownian direction
- Random direction
- Pendulum movement
- Reset/mute behavior

### Musical applications
- **Bassline engine**
- **Theme generator**
- **Motif sequencer**
- **Counterpoint** if both channels drive separate voices
- **Live variation** by editing “offline” patterns while another plays

### Very useful pairing
Use **channel A** as root melody and **channel B** as related harmony, or use B to modulate A through CV assignments.

---

## Acid Curds: chord progression to melodic framework

Acid Curds is a harmonic sequencer, but it is deeply useful for melody.

### What it does
It outputs chord tones across 4 outputs:
- output A = root / base note
- B/C/D = chord tones

You can set chord qualities, voicing, inversion, base note, and octave.

### Why it matters for melody
A melody often works best when anchored to harmony. Acid Curds gives you:
- explicit chord progressions
- quantized chord outputs
- harmonic motion that other melodic voices can follow

### Musical uses
- Use **A** as bass/rootline
- Use **B** as topline melody source
- Use **C/D** as harmonized voices or secondary melodies
- Clock progression separately from S&H/root sampling for flexible harmonic rhythm

### Best use in a patch
Acid Curds can be the **harmonic skeleton**:
- bass voice from A
- pluck arpeggio from B/C/D
- another O_C app or external quantizer uses the same scale/root for melody

---

# 3. Chord-transform apps as melody engines

## Harrington 1200: harmonic motion from simple triggers

Harrington 1200 is nominally a chord app, but it’s very strong for melody generation if you think in terms of **voice-leading**.

### What it outputs
- A = quantized root
- B/C/D = triad notes

### Why it’s melodic
Neo-Riemannian transforms (P, L, R, or N, S, H) create smooth movement between triads. This means the voices on B/C/D move by small intervals, which is exactly what makes melodic lines sing.

### Musical use cases
- Send B/C/D to 3 oscillators for triads
- Or treat just one output, say **B**, as the melody voice
- As transformations happen, B becomes a voice-led melody line

### Euclidean trigger mode
One of the strongest features from the manual:
- a single clock can generate complex patterns of chord transformations
- each transform type has Euclidean masks

That means you can create:
- harmonic progression
- melodic voice-leading
- repeating-but-shifting musical phrases

### Best musical role
Harrington 1200 is a **harmonic progression machine that also emits melodies for free**.

---

## Automatonnetz: vector melody / harmony sequencer

Automatonnetz is one of the most compositionally rich apps in the manual.

### Why it matters
It moves through a 5x5 grid, each cell containing:
- a transform
- an offset
- inversion
- mutation

On each clock, the current position moves by dx/dy. The active cell modifies the chord.

### Musical result
This is not a conventional step sequencer. It creates:
- melodic drift
- recurring harmonic regions
- self-modifying patterns
- structured unpredictability

### Key melodic trick from the manual
If every cell transform is set to `*` and only the **offset** values are used, it can function as a melody sequencer. Output B can become a melodic line, with C and D as transposed variants.

### Use cases
- evolving melody over a fixed tonality
- harmonic wandering with smooth voice leading
- self-mutating melodic cells
- root plus strummed or arpeggiated chords

### Very strong for
- generative ambient melodies
- minimalism
- post-tonal or quasi-tonal harmonic exploration

---

# 4. CopierMaschine as a melody processor

## CopierMaschine: melodic delay, canon, and phrase memory

Originally an ASR, CopierMaschine is extremely useful for melodic writing.

### Core behavior
- sample a CV on a clock
- output current and previous sampled values across A/B/C/D
- quantize the results to a scale

### Why it matters musically
This creates:
- delayed melodic copies
- harmonically constrained echoes
- canons
- stepwise phrase memory

### Very musical features
- **buffer index** as delay
- **freeze** to loop a recorded phrase
- **mask rotation**
- assignable CV for transpose/root/buffer size
- internal CV sources

### Musical roles
- turn one melody into 4 staggered melodic voices
- freeze a captured phrase and transpose it
- use delay indexing to create pseudo-counterpoint
- use as a CV looper for motif repetition

### Strong patch idea
Take a melody from Sequins or Quantermain into CopierMaschine:
- A = current note
- B/C/D = delayed voices
- each voice to a different oscillator or timbre

This gives instant canon/polyphony.

---

# 5. Rhythm and phrasing tools for melodic lines

## Piqued: make melodies articulate

Piqued is “just” envelopes on paper, but for melody it is crucial.

### Why
Melody is not just pitch. It needs:
- articulation
- note length
- accent
- phrasing
- rhythmic filtering

Piqued provides:
- quad envelopes
- mappable triggers
- trigger delays
- looping envelopes
- Euclidean trigger filters

### How this helps melodic components
Use Piqued to drive:
- VCAs for note articulation
- filters for accent
- FM depth per note
- wavefolder amount
- LPGs for plucks

### Especially important feature
The **Euclidean trigger filter** can gate which melodic notes actually sound. So even if a pitch sequence is regular, articulation can become polyrhythmic.

### Great pairings
- Sequins + Piqued = classic sequenced melody with contour
- Quantermain + Piqued = random notes with intentional rhythm
- Harrington 1200 + Piqued = triads with changing attack shapes
- Acid Curds + Piqued = chord stabs / plucks / pulses

---

# 6. Modulation sources that become melodies

## Quadraturia as quantized melody source

Quadraturia is a quadrature wavetable LFO, but if you route its outputs into a quantizer, it becomes a melodic contour generator.

### Patch concept
- Quadraturia output -> Quantermain CV input
- trigger Quantermain with clock
- scale chosen in Quantermain

### Musical result
The smooth cyclic motion becomes:
- scalar melodies
- repeating phrases
- 4 related phase-shifted melodies

### Why it’s powerful
Because the four outputs are phase/frequency-related, you can get:
- melody
- bass variation
- countermelody
- canon-like relationships

---

## Low-rents as generative melody source

Lorenz and Rössler attractors are excellent for “alive” melodic motion.

### Patch concept
- one Low-rents output -> Quantermain
- another Low-rents output -> transposition / mask / range modulation
- clock Quantermain externally

### Musical result
- unstable but bounded melodic behavior
- non-repeating contour
- natural-feeling wandering pitch

Especially effective for ambient, generative, and Berlin-school-adjacent patches.

---

## Dialectic Ping Pong as stepped melodic CV

Though intended as bouncing envelopes, at slower rates and with retriggering, it can provide CV that a quantizer turns into melodies.

### Musical behavior
- arcing pitch contours
- repeated bouncing interval shapes
- pseudo-physical melodic gestures

This is especially nice for:
- mallet lines
- descending rebound motifs
- “gravity-shaped” melodic behavior

---

## Viznutcracker as stepped CV source

The bytebeat app can run slowly and output stepped voltages. The manual explicitly notes this can be used as a source of control voltages.

### Patch concept
- Viznutcracker output -> Quantermain or Meta-Q
- external trigger clocks stepping or resetting phase
- optional loop mode

### Musical result
- highly idiosyncratic note sequences
- digital/mechanical melodic motifs
- repeatable weirdness

Best for experimental and IDM-style melodic fragments.

---

# 7. Multi-app musical strategies

Here are the most useful combinations from a musician’s perspective.

---

## Strategy A: Conventional melodic voice + bass + harmony

### Patch
- **Sequins ch.1** -> lead oscillator
- **Sequins ch.2** -> bass oscillator
- **Piqued** -> envelopes for both VCAs
- **Acid Curds** or **Harrington 1200** -> chord voices

### Result
A complete tonal structure:
- bassline
- lead motif
- harmonic accompaniment

This is the most direct “songwriting” setup.

---

## Strategy B: One CV source, many melodic interpretations

### Patch
- external CV, Low-rents, or Quadraturia -> **Quantermain** channels A-D
- each channel uses:
  - different scale
  - different mask
  - different transpose
  - different trigger division

### Result
One shape becomes:
- bass
- lead
- harmony
- counterline

This is one of the best uses of O_C’s polymorphic design.

---

## Strategy C: Chord progression driving melody

### Patch
- **Acid Curds** creates chord progression
- use output A as bass/root
- use B or C as top-note melody
- use another quantizer or sequencer transposed around same harmonic center

### Result
Melody stays harmonically embedded because it literally comes from chord data.

---

## Strategy D: Transforming harmony into melody

### Patch
- **Harrington 1200** or **Automatonnetz**
- clock transforms with Euclidean or irregular triggers
- take one chord output as melody
- use others for supporting voices

### Result
Melodies emerge from voice-leading rather than from step sequencing.

This often sounds more “composed” and less gridlike.

---

## Strategy E: Melodic canon and echoes

### Patch
- source melody from **Sequins** or external sequencer
- feed into **CopierMaschine**
- freeze and modulate buffer index
- outputs A-D to 4 voices or 2 voices plus modulation destinations

### Result
- canon
- delayed imitation
- looping motifs
- transposed memory phrases

This is especially good for minimalist or contrapuntal music.

---

## Strategy F: Generative melody with harmonic progression

### Patch
- **Low-rents** or **Turing source in Quantermain**
- quantize with **Meta-Q**
- sequence scale slots via trigger
- articulate with **Piqued**

### Result
A melody that wanders, but inside a changing harmonic plan.

This is probably the strongest “musical generative” combination in the manual.

---

# 8. Best app roles in a melodic system

## For exact composed melody
- **Sequins**

## For harmonic-aware melody
- **Meta-Q**
- **Acid Curds**

## For voice-led melodic movement
- **Harrington 1200**
- **Automatonnetz**

## For melodic echoes / layered phrases
- **CopierMaschine**

## For random or generative note material
- **Quantermain** with:
  - Turing
  - logistic map
  - bytebeats
  - integer sequences

## For phrasing and articulation
- **Piqued**

## For source CV to be turned into melody
- **Quadraturia**
- **Low-rents**
- **Dialectic Ping Pong**
- **Viznutcracker**

---

# 9. Practical melodic patch recipes

## Patch 1: Generative lead with stable harmony
- Quantermain channel A: Turing source, clocked
- Meta-Q channel 1: same or related CV, scale slot sequencing
- Piqued: envelopes for articulation
- Acid Curds: chord bed underneath

**Sound:** a lead line that feels free, while harmony progresses intentionally.

---

## Patch 2: Minimalist canon
- Sequins channel 1 outputs motif
- route to CopierMaschine
- outputs A-D to 3 or 4 voices
- small octave/transposition differences
- Piqued or external EGs articulate each voice

**Sound:** Steve Reich / Terry Riley style layered repetition.

---

## Patch 3: Harmonic melody from transforms
- Harrington 1200 in Euclidean trigger mode
- one transform stream sparse, another dense
- output B as lead
- output A as bass
- outputs C/D as supporting harmony

**Sound:** elegant chord-driven melodic motion.

---

## Patch 4: Ambient evolving melody
- Low-rents output -> Quantermain CV in
- Quantermain channel A/B with different masks
- slow clock divisions
- Piqued with long envelopes
- Automatonnetz or Acid Curds supplies occasional harmonic shifts

**Sound:** floating, evolving melodic ecosystem.

---

## Patch 5: Plucked chord melody
- Automatonnetz with OutA set to strum or arp
- B/C/D to resonators or plucked voices
- root on A to bass
- Piqued shapes timbre or dynamics

**Sound:** animated harmonic melody with built-in gesture.

---

# 10. What these apps do especially well together

From the manual, the unique strength of O_C is not merely sequencing notes. It is the ability to combine:

- **quantization**
- **scale editing**
- **masking**
- **clocked sampling**
- **internal pseudo-random sources**
- **harmonic transforms**
- **Euclidean timing**
- **multi-channel parallel outputs**

That means the module excels at building melodic music from:
- one source interpreted many ways
- one harmony expressed across several voices
- one sequence expanded into canon, arpeggio, and counterpoint
- one random source constrained into tonal behavior

In musical terms, O_C is especially good at:
- **countermelody**
- **harmonized melody**
- **voice-leading**
- **generative tonal material**
- **algorithmic melody with strong constraints**

---

# 11. Recommended “musical architecture” using these apps

If I were building melodic components with O_C in a Eurorack patch, I’d think in layers:

## Layer 1: Harmonic frame
Use:
- Acid Curds
- Harrington 1200
- Meta-Q scale-slot sequencing

## Layer 2: Primary note generation
Use:
- Sequins
- Quantermain internal sources
- Automatonnetz

## Layer 3: Derived voices
Use:
- CopierMaschine
- parallel quantizer channels in Quantermain
- multiple chord outputs from Harrington / Acid Curds

## Layer 4: Phrasing
Use:
- Piqued
- Euclidean trigger masks
- trigger delays
- clock division

## Layer 5: Motion and variation
Use:
- Quadraturia
- Low-rents
- Dialectic Ping Pong
- CV mappings into scale mask, root, transpose, inversion, loops

This gives you complete melodic ecosystems rather than isolated note streams.

---

# 12. Final takeaway

From the manual, Ornament & Crime is particularly powerful for melodic music because it lets you move fluidly between:

- **written melody** (Sequins)
- **quantized modulation as melody** (Quantermain)
- **harmonized melody** (Acid Curds, Harrington 1200)
- **transform-based voice-leading** (Automatonnetz, Harrington 1200)
- **melodic memory and imitation** (CopierMaschine)
- **generative phrasing and articulation** (Piqued)

If your goal is to create melodic components, the strongest combinations are:

1. **Sequins + Piqued** for direct melodic composition  
2. **Quantermain + internal sources** for generative melodies  
3. **Meta-Q + scale-slot sequencing** for harmonic evolution  
4. **Acid Curds / Harrington 1200** for melody derived from chords  
5. **CopierMaschine** for layered melodic repetition and canon  

In practice, O_C shines most when one app supplies **pitch structure**, another supplies **rhythmic articulation**, and the outputs are used as **related musical voices** rather than isolated CV lines.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)