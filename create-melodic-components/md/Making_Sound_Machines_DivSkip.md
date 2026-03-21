# Making Sound Machines — DivSkip

- [Manual PDF](../../manuals/SKORPION_Manual.pdf)

---

[Manual PDF / Source](about:blank)

# WMD Skorpion — using it to create melodic components

Skorpion is not just a wavefolder. Reading the manual as a musician, it’s really a **pitch-aware waveform animator / comparator-driven melodic modulation source**. That means it can contribute to melody in several ways at once:

- as a **timbre voice processor** for pitched oscillators
- as a **self-generated stepped CV source**
- as a **wave-sequenced target generator**
- as a **rhythmic/melodic modulator** derived from the harmonic movement of an incoming note
- as a **stereo melodic texture maker** with controllable width/delay

Since only this module/manual is provided, I’ll focus on how the **internal sections of Skorpion work together** to make melodic material.

---

## Big picture: why Skorpion is musically melodic

The core idea is:

1. Your input signal at **IN** is analyzed by **8 thresholds**.
2. Each threshold crossing changes the behavior of the **vector core**.
3. The vector core moves toward a **target voltage** at a speed set by **SLOPE**.
4. The selected target can come from:
   - fixed **5V**
   - the **input/CLIP**
   - or the **8-step TRGT slider sequencer**
5. Several outputs expose internal states:
   - **TRGTs**
   - **COUNT**
   - **DAC**
   - **DIFF**
   - **±G(DIR)**
   - **ABS(IN)**
   - **G(IN>0)**

So the module naturally turns one pitched signal into:
- a folded audio result
- multiple related CV streams
- step-sequence-like control voltages that can be patched back into pitch, timbre, dynamics, or other voices

That’s exactly the kind of thing that creates **melodic components**, not just distortion.

---

# The most important melodic use cases

## 1. Use Skorpion as a pitch-consistent timbre shaper for a melodic oscillator

If you feed a VCO melody into **IN**, Skorpion can keep the timbre behavior more consistent across notes because:

- **1V/OCT controls SLOPE**
- The manual explicitly says this is “necessary for equal timbre across different notes”

### Patch concept
- Melodic VCO → **IN**
- Same pitch CV used for that oscillator multed to **1V/OCT** on Skorpion
- Skorpion **OUT L/R** → mixer

### Why this matters
Normally, wavefolding changes character a lot as pitch changes. Skorpion compensates by linking pitch to slope. That means:
- bass notes and high notes retain a more similar folded identity
- melodic phrases sound intentional rather than random
- you can treat it like a playable voice processor

### Best controls for melody
- **FOLD**: harmonic intensity
- **SLOPE**: brightness / articulation / overtone density
- **SHIFT**: asymmetry; can make alternate-note color changes feel melodic
- **SHAPE**: curve character and dynamic contour

### Musical result
This is the most straightforward “melodic” role: Skorpion becomes the **expressive oscillator-shaper** in a tuned lead, bass, or arp line.

---

## 2. Use the TRGT sliders as an internal 8-step melodic contour sequencer

The **TRGTs** are one of the most melodic features in the module.

The manual says:
- the 8 targets form an **8-step voltage controlled sequencer**
- they can control the vector core destination
- they are also available directly at the **TRGTs output jack**

So even if you ignore Skorpion’s audio output, you can use it as a kind of **threshold-addressed melodic sequencer**.

### Two target order modes
- **SEQ**: target selected by the **count of active thresholds**
- **TIED**: target selected by the **most recently crossed threshold**

These are musically very different.

#### SEQ mode
Feels more like:
- a staircase melody
- contour linked to input amplitude/shape
- orderly stepped progression

#### TIED mode
Feels more like:
- event-driven melody
- edge-sensitive movement
- more angular / reactive / gestural

### Patch concept
- Audio oscillator or complex LFO → **IN**
- Set **TARGET** toward **SLIDERs**
- Program TRGT sliders to a melodic contour
- Use **TRGTs output** to modulate:
  - another oscillator’s pitch input
  - filter cutoff
  - FM index
  - VCA level
  - waveshape of another voice

### Musical result
The input waveform becomes an **addressing mechanism** for the 8 programmed voltages. This can create:
- pseudo-sequences
- note ornaments
- harmonic shifts
- repeated melodic motifs tied to the oscillator’s own motion

If attenuated and quantized downstream, this becomes very strong melodic CV.

---

## 3. Use threshold crossings to derive melody from timbre

Because threshold states are based on the incoming waveform, Skorpion turns the shape and amplitude of a note into stepped control information.

The most useful melodic outputs here are:

- **COUNT**: 0–4V staircase, each active threshold adds 0.5V
- **DAC**: weighted threshold combination, a more nuanced staircase
- **TRGTs**: selected target voltage
- **DIFF**: difference between target and actual core position

### Why these are melodic
These outputs are correlated to:
- waveform shape
- fold amount
- threshold arrangement
- symmetry / shift
- note dynamics

That means your melody can produce **secondary melodies** or pitch-adjacent movement.

### Patch ideas

#### A. COUNT as a melodic sub-sequence
- **COUNT** → quantizer → oscillator pitch
- Main oscillator also feeds **IN**
- As each played note changes threshold activity, COUNT generates stepped voltages that become a secondary melody

Result:
- one played line creates a second harmonically related line

#### B. DAC as a more refined melodic CV
- **DAC** → quantizer → second voice pitch
- Program thresholds unevenly
- Modulate FOLD and SHIFT slowly

Result:
- less obvious staircase than COUNT
- more “encoded” melodic motion
- excellent for counter-melody

#### C. TRGTs as phrase contour
- **TRGTs output** → precision adder or quantizer → voice pitch
- Sliders define the phrase shape
- Threshold crossings decide which step is active

Result:
- reactive melody generator from the incoming note contour

---

## 4. Use SHIFT for pitch-like motion and melodic asymmetry

The manual states:

> Slow modulation here produces a frequency shift effect.

That’s a major musical clue.

**SHIFT** pushes the input signal up and down against the comparators, creating asymmetry. In melodic contexts this does several things:

- changes which thresholds are hit
- changes target selection behavior
- changes fold symmetry
- can create apparent pitch-drifting sideband-like motion

### Patch concept
- Send slow CV, envelope, or TRGT-derived CV to **SHIFT**
- Keep **SHIFT** near noon for centered behavior, then animate around it

### Musical result
This gives:
- vowel-like note animation
- note-to-note asymmetry
- subtle melodic inflection
- unstable “bent pitch” timbral motion without retuning the oscillator

This is great for:
- leads
- acid-like lines
- evolving drones with melodic perception
- expressive bass articulation

---

## 5. Use the Macro section to animate melody over time

The **MACRO SETUP & MACRO ENVELOPE** section is very strong for phrase-based melodic evolution.

It provides:
- macro attack/release
- threshold LFO amount/rate
- per-parameter modulation normals for:
  - **FOLD**
  - **SLOPE**
  - **SHIFT**
  - **SHAPE**

These can be set as either:
- **LFOs**
- **ENVs**

and all LFO amplitude is controlled by the **Macro Envelope**.

### Why this matters melodically
A melody often needs:
- note articulation
- phrase evolution
- repeated but non-static timbre
- gradually opening/closing complexity

Skorpion can do this internally.

### Patch concept: “animated melodic lead”
- Pitch CV → oscillator and Skorpion **1V/OCT**
- Oscillator → **IN**
- Enable **MACRO ENV**
- Set:
  - FOLD normal modulation as ENV
  - SLOPE normal modulation as ENV
  - SHIFT as slow LFO
  - SHAPE as slow ENV or LFO
- Trigger Macro Env per note or per phrase

### Result
Each note or phrase can:
- start clean
- bloom into more complex fold states
- shift symmetry during sustain
- release back to simpler tone

That’s extremely musical, especially when the melody is simple and the timbre does the expressive work.

---

## 6. Use equalized thresholds for classic melodic wavefolder behavior

The **EQUALIZE THLDs** switch forces equal threshold intervals and makes the timbre more like a classic wavefolder.

### Musically:
- more predictable harmonic development
- easier to tune by ear across a melody
- better for traditional leads/basses/arps
- threshold sliders no longer define irregular breakpoints

### Good use
If you want:
- a melodic line with stable “folder” behavior,
- less chaotic stepping,
- more classic West Coast folding,

then enable **EQUALIZE THLDs** and use:
- 1V/OCT to stabilize timbre across pitch
- SLOPE and FOLD to sculpt brightness
- SHAPE for articulation

### Contrast
If you want a more sequenced / melodic-CV-generating behavior, disable equalization and use irregular threshold positions.

---

## 7. Use SYNC for cleaner pitch-centered notes

The **SYNC** switch resets the vector core at zero crossings of the input.

Modes:
- **SOFT**
- **X** = off
- **HARD**

### Melodic implications
For pitched material, sync often makes notes:
- cleaner
- more repeatable
- more stable in attack
- less smeared

#### HARD sync
- best for percussive, articulate melodies
- sharper note identity
- more aggressive harmonic reset

#### SOFT sync
- smoother
- more organic
- still pitch-coherent

### Good patch
For melodic bass or plucked sequences:
- oscillator → IN
- pitch CV → oscillator and 1V/OCT
- SYNC = SOFT or HARD
- Macro envelope opening FOLD or SHAPE per note

Result:
- consistent attacks
- strong note centers
- more playable behavior

---

## 8. Use HALT and HALT IF TARG=0 to create pitched, square-like melodic segments

This is one of the coolest musical features.

- **HALT jack** stops the vector core from moving
- **HALT IF TARG=0** lets any target slider at 0 create a halted segment

That means you can deliberately insert **flat held segments** into the folded waveform. The manual says this creates “squares in the timbre.”

### Why melodic?
Square-like held segments emphasize:
- pitch center
- odd harmonics
- note articulation
- digital/stepped phrasing

### Patch idea
- Set **TARGET** to use **SLIDERs**
- Put some TRGT steps at 0
- Enable **HALT IF TARG=0**
- Feed a melodic oscillator into IN
- Use **TIED** or **SEQ** target ordering

### Result
Some waveform segments freeze while others slope. This can produce:
- speech-like note shapes
- stepped timbral accents
- pseudo-PWM melodic tones
- phrase-dependent harmonic punctuation

This is especially effective for:
- electro leads
- square-ish basses
- sequenced techno lines

---

## 9. Use CLIP and TRGT MOD to impose another melody onto the current one

The module allows the target voltage to be influenced externally:

- **CLIP** can replace the normal input-clipping reference
- **TRGT MOD** directly influences the output of the TARGET pot
- TRGT MOD can be **SYM** or **ASYM**

This is a huge “use together” point internally: input audio, target selection, and external modulation can all interact.

### Musical uses

#### A. Overlay one melody onto another
- Voice A audio → **IN**
- Voice B audio or CV → **CLIP** or **TRGT MOD**
- Set TARGET toward CLIP or slider region

Result:
- melody A’s timbre is shaped by melody B
- harmonic contour of one line imprints onto another

#### B. Symmetric modulation for stable melodic richness
- **TRGT MOD = SYM**
- Feed an LFO, envelope, or another oscillator

Result:
- more balanced timbral animation
- less asymmetric weirdness
- better for tonal leads

#### C. Asymmetric modulation for phrase accents
- **TRGT MOD = ASYM**
- Feed sequence CV or envelope

Result:
- note-dependent skewing
- expressive accenting
- unstable, animated melodic contour

---

## 10. Use the stereo output and delay to widen melodic voices without losing the center

The **OUTPUT** control blends:
- **DRY ↔ WET** on lower half
- **WET ↔ WIDE** on upper half

The **WIDE** section introduces:
- ultra-short delay
- optional **mid/side** network
- optional filtering below/above 240 Hz to keep lows centered

### Melodic value
For lead and arp parts:
- mono center retains pitch solidity
- high frequencies spread wide
- movement feels bigger without detuning

### Best practice
- melodic bass: keep output lower / centered, maybe FILTER mode for mono lows
- melodic lead: move OUTPUT into upper half for width
- sequence or arp: use FILTER mode so low fundamentals stay focused and highs spread

### Delay output
The **DELAY** jack exposes the delayed waveform:
- no output below 12 o’clock
- fades in around 12–12:30
- longer delay up to 3 o’clock
- beyond 3 o’clock adds more delay time and slow modulation

This means the stereo widening engine is also a modulation/audio source.

### Musical patch
- Skorpion processed voice at OUT L/R
- **DELAY** output patched elsewhere:
  - into another filter
  - into FM index
  - into another voice’s wavefolder
  - into a VCA for “echo melody” timbral doubling

---

# Internal combinations that work especially well for melody

## A. Clean melodic voice
Use when you want a playable lead/bass.

- Oscillator → **IN**
- Pitch CV → oscillator and **1V/OCT**
- **EQUALIZE THLDs ON**
- **SYNC SOFT**
- **TARGET = 5V** or slight blend toward **CLIP**
- Moderate **FOLD**
- SHAPE at noon or slight **OUT** feedback
- OUTPUT in wet zone, not too wide

Result:
- classic-ish folded melodic voice
- stable across pitch
- expressive but controlled

---

## B. Sequenced melodic timbre
Use when the melody should also generate internal steps.

- Oscillator → **IN**
- Pitch CV → oscillator and **1V/OCT**
- Uneven threshold slider settings
- **TARGET = SLIDERs**
- Program TRGT sliders as a phrase contour
- **TARGET ORDER = SEQ**
- **COUNT** or **TRGTs** output → quantizer → second oscillator pitch

Result:
- primary melody plus derived counter-melody
- tightly related harmonic movement

---

## C. Reactive counterpoint generator
Use for evolving melodic systems.

- Main voice → **IN**
- **DAC** output → quantizer → second voice pitch
- **DIFF** output → filter FM or VCA CV
- **G(IN>0)** or **±G(DIR)** → trigger envelopes or switch events
- Skorpion output as stereo main voice

Result:
- one source creates:
  - audible melody
  - counter-melody
  - dynamic articulation
  - timbral rhythm

This is one of the strongest “single source to melodic ecosystem” uses.

---

## D. Phrase-evolving lead
Use for expressive lines without needing extra modulation modules.

- Oscillator → **IN**
- Pitch CV → oscillator and **1V/OCT**
- Macro Env gate per note or per phrase
- Macro setup:
  - **FOLD** = ENV
  - **SLOPE** = ENV
  - **SHIFT** = slow LFO
  - **SHAPE** = slow LFO or ENV
- **SYNC HARD** for punch or SOFT for smoother tone

Result:
- notes open and close like acoustic articulation
- repeated sequences feel alive
- strong for melodic hooks

---

## E. Harmonic melody mutation
Use for aggressive or experimental tonal music.

- Voice A oscillator → **IN**
- Voice B oscillator or melodic CV → **TRGT MOD**
- Optionally percussion or another synth line → **CLIP**
- **TARGET** toward CLIP/SLIDER region
- **TRGT MOD = ASYM**
- **TARGET ORDER = TIED**

Result:
- one line mutates another
- harmonic “cross-synthesis” feel
- unstable but still trackable melodic content

---

# Best outputs for building melodic systems

If your goal is “melodic components,” these are the most useful outputs ranked by likely usefulness:

## 1. TRGTs output
Best for:
- programmed step contours
- repeatable melodic patterns
- quantized pitch sequencing

Why:
- directly represents your 8 programmed target voltages

---

## 2. DAC output
Best for:
- nuanced melodic CV
- encoded harmonic movement
- subtle second-voice pitch control

Why:
- weighted threshold combination gives richer variation than simple count

---

## 3. COUNT output
Best for:
- obvious staircase sequences
- simple transposition patterns
- rhythmic melodic stepping

Why:
- easy to hear and patch musically

---

## 4. DIFF output
Best for:
- edgy melodic modulation
- FM amount
- filter movement
- aggressive upper-voice pitch experiments

Why:
- always slopes toward 0 and is rich in harmonics

---

## 5. ±G(DIR) and G(IN>0)
Best for:
- note subdivision logic
- alternating melodic articulations
- switching between two pitch offsets or timbres

Why:
- they provide reliable state/gate signals tied to the waveform’s motion

---

## 6. ABS(IN)
Best for:
- octave-ish or rectified contour modulation
- re-using melody energy as modulation
- creating pitch-related envelopes or CV shapes

---

# Practical melodic patch recipes

## Patch 1: West-coast lead with stable pitch behavior
- VCO sine/triangle → **IN**
- Sequence CV → VCO + **1V/OCT**
- **EQUALIZE THLDs ON**
- **SYNC SOFT**
- **TARGET = 5V**
- Moderate **FOLD**
- Increase **SLOPE** until bright
- SHAPE source = **OUT**, slight amount
- OUT L/R to mixer

This gives a very playable folded lead.

---

## Patch 2: One oscillator creates two melodies
- VCO → **IN**
- Sequencer CV → VCO + **1V/OCT**
- Uneven thresholds
- TARGET toward **SLIDERs**
- Program TRGT sliders to a musical contour
- **TRGTs output** → quantizer → second oscillator pitch
- Skorpion audio out = voice 1
- Second oscillator = voice 2

You get a lead plus a derived counterline.

---

## Patch 3: Bassline with animated note attacks
- Bass VCO → **IN**
- Pitch CV → VCO + **1V/OCT**
- **SYNC HARD**
- **TARGET = 5V**
- Macro Env triggered per note
- FOLD modulation = ENV
- SHAPE modulation = ENV
- OUTPUT switch = **FILTERs**
- OUTPUT in moderate wet/wide range

This creates punchy, centered low-end with animated upper harmonics.

---

## Patch 4: Reactive melody sequencer from thresholds
- Audio-rate oscillator → **IN**
- Thresholds set irregularly
- **TARGET ORDER = SEQ**
- **COUNT** → quantizer → oscillator B pitch
- **DAC** → filter cutoff on oscillator B
- **TRGTs** → FM amount or wavefold amount on oscillator B

This produces a secondary melody and phrase-linked animation.

---

## Patch 5: Frozen-step harmonic lead
- Oscillator → **IN**
- Pitch CV → oscillator + **1V/OCT**
- **TARGET = SLIDERs**
- Set some TRGT sliders to zero
- Enable **HALT IF TARG=0**
- Moderate **SHIFT** around noon
- TIED mode for more event-driven target changes

This yields stepped, square-inflected melodic textures.

---

# What matters most for tonal results

If you want Skorpion to behave musically rather than chaotically, prioritize these:

## Use 1V/OCT
This is essential if the input is playing notes.

## Start with equal thresholds
Then disable equalization once you understand the behavior.

## Use TARGET = 5V first
That gives the most stable, square-ish, pitch-clear behavior.

## Add TRGTs later
The slider targets are powerful, but more complex.

## Use SOFT/HARD sync for notes
Especially for bass and plucks.

## Keep SHIFT near noon at first
The manual specifically hints at noon for some operations; too much shift can quickly destabilize the relation between pitch and fold behavior.

## Quantize melodic CV outputs if using them for pitch
TRGTs, COUNT, and DAC are melodic, but they’ll really shine when run through a quantizer or precision pitch path.

---

# Best musical interpretation of Skorpion

If I had to describe Skorpion’s melodic role in a rack:

> It is a **playable wavefolder voice processor plus an internal melodic CV extractor/sequencer**.

It excels when one pitched signal is allowed to generate:
- its own folded tone,
- its own phrase contour,
- its own counter-melody,
- its own articulation logic,
- and its own stereo expansion.

That makes it unusually good for:
- solo lead voices
- generative counterpoint
- animated basslines
- stereo arps
- self-modulating melodic systems

---

# Summary

## Best ways to use Skorpion for melodic components
1. **Process a tuned oscillator** and mult pitch CV to **1V/OCT** for stable melodic timbre.
2. Use **TRGT sliders** as an 8-step contour source.
3. Patch **TRGTs / COUNT / DAC** to other voices for derived melodies.
4. Use **Macro Env + internal LFO/ENV normals** to animate note phrasing.
5. Use **SYNC** to improve note definition.
6. Use **HALT IF TARG=0** for square-like, stepped melodic articulation.
7. Use **WIDE / DELAY** for stereo melodic presence.
8. Use **CLIP** and **TRGT MOD** to let one line reshape another melodically.

If you want, I can also turn this into:
- a **set of 10 specific patch recipes**
- a **beginner-friendly quickstart**
- or a **signal-flow diagram showing how to patch Skorpion as a melodic voice**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)