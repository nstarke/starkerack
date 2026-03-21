# WMD — Skorpion

- [Manual PDF](../../manuals/SKORPION_Manual.pdf)

---

[Manual PDF](https://wmdevices.com/cdn/shop/files/Skorpion_Manual_Rev1.00.pdf)

# WMD Skorpion: creative patch ideas and module pairing guide

Skorpion is not just a wavefolder. It’s really a **comparator-driven waveform animator**, a **voltage-addressed target sequencer**, a **self-modulation ecosystem**, and a **stereo sound widener** with lots of patch points exposed. The most interesting use cases come from treating it as:

- a wavefolder
- a strange oscillator/chaotic function block
- a modulation source
- a threshold-driven event extractor
- a stereo timbre processor
- a self-patching voice core

Below are practical and creative ways to use it with other modules.

---

## What makes Skorpion special in a system

A few manual details matter a lot for patching:

- **8 thresholds** determine where folds happen.
- The **vector core** moves toward a **target voltage** and reverses when thresholds are crossed.
- **SLOPE** is effectively the movement speed / brightness control and tracks **1V/oct**.
- **TARGET** can be:
  - fixed **5V**
  - **CLIP** input / IN waveform
  - the **8-step TRGT slider sequencer**
- **SHAPE** applies feedback to slope from many sources: `IN`, `OUT`, `DELAY`, `COUNT`, `DIFF`, `TRGTs`, `DAC`, `DIR`
- Useful outputs: `ABS(IN)`, `G(IN>0)`, `TRGTs`, `DIFF`, `±G(DIR)`, `COUNT`, `DAC`, `DELAY`
- Stereo output can be **dry/wet/wide**, with optional filtered mid/side behavior
- Macro system adds internal **LFOs/envelopes** to thresholds and the four main controls

That means Skorpion pairs especially well with:

- clean oscillators
- envelope followers
- random/CV sequencers
- VCAs
- matrix mixers
- comparators / logic
- resonant filters
- delay/reverb/granular processors
- stereo utilities
- clocked modulation
- LPGs and VC panners

---

# Best companion module types

## 1. Precision oscillators / simple VCOs
Skorpion loves harmonically simple material and rewards stable tracking.

### Why
A plain sine, triangle, or saw at `IN` lets the threshold network create complex spectra very predictably. Since **1V/oct controls slope**, you can get more consistent timbre across pitches than many wavefolders.

### Great pairings
- Intellijel Dixie II+
- Joranalogue Generate 3
- AJH Minimod VCO
- Doepfer A-110 variants
- Verbos Foundation Oscillator
- any clean analog triangle/sine VCO

### Patch idea
- VCO sine → `IN`
- keyboard/sequencer pitch → VCO pitch and Skorpion `1V/OCT`
- `EQUALIZE THLDs` ON
- `TARGET` near 5V
- `SYNC` SOFT or HARD depending desired stability

Result: a more “playable” folded voice with consistent character over a melodic line.

---

## 2. Complex modulation sources
Because thresholds, target behavior, shape, and output width all respond beautifully to CV, Skorpion thrives with rich modulation.

### Good sources
- Make Noise Maths
- Frap Tools Falistri
- Xaoc Zadar
- Batumi / Pamela’s Pro Workout
- Mutable Tides / clones
- Joranalogue Orbit 3
- random + stepped voltages

### Why
Slow modulation on:
- **SHIFT** gives asymmetry and even frequency-shift-like movement
- **FOLD** changes fold density
- **SHAPE** changes the actual curvature/behavior of the vector core
- **OUTPUT** animates stereo width and delay behavior

### Patch idea
Use four different CVs:
- envelope → `FOLD`
- slow triangle LFO → `SHIFT`
- random stepped CV → `TARGET`
- attenuated chaotic CV → `SHAPE`

Keep `TARGET` in `SLIDERs` mode, then set TRGT sliders to a melodic contour. The result is a timbre-sequenced voice that morphs as if the folding engine were “re-composing” itself.

---

## 3. Matrix mixers / feedback routers
This is one of the most powerful pairings.

### Why
Skorpion already has internal feedback concepts via SHAPE sources. External feedback lets you create highly tuned recursive systems while keeping level control and polarity manageable.

### Great pairings
- AI Synthesis Matrix Mixer
- Doepfer A-138m
- Instruō lion + attenuators
- Happy Nerding 3xMIA / 6xMIA
- Befaco A*B+C
- Frap 321
- Joranalogue Select 2 + Mix 3

### Patch ideas

#### External feedback sculpture
- `OUT L` or `DIFF` → matrix mixer
- matrix outputs to `SHIFT`, `SHAPE CV`, `TRGT MOD`, or even back to another processor before `IN`

Add inversion on one path. This gives controlled instability: vocal, metallic, tearing, almost PLL-like behaviors.

#### Parallel control network
Send:
- `COUNT` → filter cutoff
- `DAC` → VCA CV
- `±G(DIR)` → switch or crossfader
- `DIFF` → FM on a second oscillator

Now Skorpion becomes the center of a whole ecosystem, not just a timbre effect.

---

## 4. Filters and fixed filter banks
Skorpion generates rich harmonics, but the more interesting pairing is when a filter is used as a *dynamic partner*, not just a tone control.

### Good pairings
- Serge / Random*Source VCFQ
- Three Sisters
- Xaoc Belgrad
- WMD C4RBN
- Frap Tools Fumana
- ADDAC fixed filter banks
- Bastl Ikarie for stereo movement

### Patch ideas

#### Post-Skorpion spectral spotlight
- `OUT L/R` → stereo filter
- modulate filter cutoff with `COUNT` or `DAC`

Because `COUNT` reflects active threshold quantity, the filter follows Skorpion’s internal state.

#### Pre-Skorpion contour shaping
- oscillator → filter → Skorpion `IN`

Use resonance to emphasize frequencies that trigger threshold crossings in more dramatic ways. Sweeping a pre-filter changes not just tone but the fold topology.

#### Band-splitting
Split oscillator:
- lowpass path dry
- highpass path into Skorpion
- mix back together

This keeps low-end intact while Skorpion destroys the top end beautifully.

---

## 5. VCAs, LPGs, and dynamics processors
Skorpion can be very alive dynamically, especially with `DIFF`, `COUNT`, and `TRGTs` affecting downstream VCAs.

### Great pairings
- Optomix / LxD
- Tallin
- Veils
- Blinds
- Tangle Quartet
- any bipolar VCA

### Patch ideas

#### Direction-based articulation
- `±G(DIR)` → comparator or rectifier/splitter
- use positive and negative direction to open two different VCAs

One VCA passes dry signal, the other passes filtered or wet Skorpion output. Upward vs downward vector motion becomes an articulation language.

#### Dynamic harmonic emphasis
- Skorpion output → LPG
- `DIFF` or `COUNT` → LPG CV

As the internal target/core difference increases, the note opens up. It feels like a self-accenting, self-exciting voice.

---

## 6. Sequencers and voltage-addressed control
The TRGT system makes Skorpion much deeper than a normal folder.

### Why
The **TRGT sliders form an 8-step voltage sequencer** selected by threshold activity. This is huge. It means the waveform itself can address sequences.

### Good pairings
- Metropolix
- René
- Mimetic Digitalis
- Voltage Block
- Moskwa / Tirana
- Bard Quartet
- any precision adder / quantizer

### Patch ideas

#### Timbre-sequenced oscillator
- VCO → Skorpion `IN`
- `TARGET` = `SLIDERs`
- set 8 target voltages as a contour
- `TARGET ORDER` = `SEQ`

Now each active-threshold count chooses a different destination voltage for the vector core. This can sound like wave sequencing inside the fold path.

#### Threshold-addressed external sequence
- `TRGTs` output → quantizer → second oscillator pitch or filter cutoff

Now Skorpion’s threshold crossings generate a CV melody tied directly to timbre shape.

#### Most-recent threshold mode
Set `TARGET ORDER` to `TIED`. This makes the most recently crossed threshold select the target. The response becomes more “gesture-sensitive” and less staircase-like. Great for expressive audio-rate modulation.

---

## 7. Comparators, logic, and switches
Skorpion already contains event logic, and its outputs are perfect for driving external logic structures.

### Useful outputs
- `G(IN>0)` = polarity gate of input
- `±G(DIR)` = direction gate of vector core
- `COUNT` = staircase event density
- `DAC` = weighted threshold state

### Good pairings
- Joranalogue Compare 2
- Doepfer logic modules
- Klavis Logica XT
- switched multiples
- sequential switches
- Bernoulli gates

### Patch ideas

#### Direction-controlled routing
- `±G(DIR)` → logic / comparator
- route between two effects chains:
  - rising vector motion = phaser
  - falling vector motion = ring mod

#### Threshold density as a logic clock
- `COUNT` into comparator
- generate triggers whenever threshold count exceeds a chosen amount

This creates rhythm from harmonic complexity.

#### Audio-derived percussion gates
- percussion loop → `IN`
- `G(IN>0)` and `COUNT` → logic AND/OR with clock streams

Now Skorpion becomes an audio event extractor.

---

## 8. Envelope followers and transient shapers
The threshold architecture reacts extremely well to dynamic material.

### Good pairings
- Mutable Ears / clones
- Instruō tràigh or other envelope followers
- ADDAC 601 / 603 style modules
- transient shapers
- compressors

### Patch ideas

#### Percussion reanimator
- drum loop or single drum voice → Skorpion `IN`
- use envelope follower from same audio to modulate `FOLD` or `SLOPE`
- `SYNC` HARD for strong transient reset behavior

This can turn simple percussion into articulated metallic bursts while remaining locked to transients.

#### Dynamic asymmetry
- envelope follower → `SHIFT`
- audio to `IN`

Harder hits shift the threshold relationship, so louder transients produce more asymmetrical folds.

---

## 9. Delay, reverb, and granular modules
Skorpion already has a tiny stereoizing delay internally. Pairing it with external spatial modules gets very rich.

### Good pairings
- Mimeophon
- Starlab
- Magneto
- Beads / granular processors
- Desmodus Versio
- FX Aid
- Data Bender
- stereo reverbs and diffusers

### Patch ideas

#### Internal/external delay interaction
- turn `OUTPUT` into `WIDE` region so `DELAY` jack is active
- send `DELAY` output to external reverb or granular module
- mix with main `OUT L/R`

This creates a split image: the main tone remains coherent while the delayed side energy blooms separately.

#### Shape from delayed self
- use internal `SHAPE SOURCE = DELAY`
- also patch `DELAY` output into another modulation destination externally, like `SHIFT` or filter cutoff

The patch links stereo smear and fold behavior in a musical way.

#### Granular excitation
- Skorpion `OUT` or `DIFF` → granular input
- `COUNT` or `DAC` → grain density / position

The granular engine follows threshold complexity.

---

## 10. Ring mod, wave multipliers, and distortions
Skorpion stacks brilliantly with other nonlinear processors.

### Good pairings
- ring modulators
- folder-before-folder chains
- analog distortion
- rectifiers
- resonators

### Patch ideas

#### Before Skorpion
- oscillator → ring mod → Skorpion

This creates more unusual comparator-crossing patterns than a pure waveform.

#### After Skorpion
- Skorpion `OUT` → subtle saturation / tube / diode clipper

Useful when Skorpion is set to cleaner or equal-threshold “classic folder” behavior and you want body afterward.

#### Parallel nonlinearities
Split one oscillator:
- path A → Skorpion
- path B → another wavefolder / ring mod / bit crusher
- crossfade using `±G(DIR)` or `COUNT`

Excellent for animated hybrid timbres.

---

# Self-patching ideas using Skorpion’s own outputs

These are especially strong because the manual exposes many internal states.

## 1. `DIFF` to `SHAPE`
`DIFF` is the difference between target voltage and actual vector-core position, and it naturally slopes toward zero.

- Patch `DIFF` → `SHAPE CV`
- Set SHAPE source to something complementary like `OUT` or `DIR`

Result: sharper, aggressive, spiky timbres that feel self-correcting and unstable in a good way.

---

## 2. `COUNT` to `FOLD`
As more thresholds become active, increase fold amount.

- `COUNT` → attenuator → `FOLD CV`

Result: recursive complexity scaling with threshold activity. Can create self-intensifying textures.

---

## 3. `DAC` to `SHIFT`
`DAC` is a weighted threshold-state output, subtler than `COUNT`.

- `DAC` → attenuated `SHIFT CV`

Result: asymmetry evolves according to threshold pattern, often more nuanced than using `COUNT`.

---

## 4. `TRGTs` out to `TRGT MOD`
- `TRGTs` output → `TRGT MOD`
- try `SYM` and `ASYM`

Result: the target sequencer modulates the target path itself, creating nested stepped movement and highly animated segment behavior.

---

## 5. `ABS(IN)` as a sidechain control
- `ABS(IN)` → VCA CV / filter CV / another module’s FM attenuator

This lets input amplitude control another path without needing a separate follower.

---

## 6. `±G(DIR)` to a bipolar VCA or panner
Use `±G(DIR)` as a switching or polarity signal.

- `±G(DIR)` → bipolar VCA CV
- process `DIFF` or `DELAY` through it

Result: alternating positive/negative modulation synchronized to vector direction.

---

# Particularly strong patch recipes

## Patch 1: Precision melodic wavefolder voice
**Modules:** clean VCO, VCA/LPG, envelope, sequencer, optional filter

- VCO triangle → Skorpion `IN`
- pitch CV → VCO and Skorpion `1V/OCT`
- envelope → VCA
- Skorpion `OUT L/R` or mono from one side → VCA
- `EQUALIZE THLDs` ON
- `TARGET` toward `5V`
- `SYNC` SOFT or HARD
- subtle LFO to `SHIFT`

**Why it works:** gives a playable voice with more pitch consistency and less “random fold drift” than many folders.

---

## Patch 2: Audio-driven modulation lab
**Modules:** another oscillator/filter voice, VCA, attenuators

- main sound source → Skorpion `IN`
- `COUNT` → second voice filter cutoff
- `DAC` → second voice FM amount or wave index
- `G(IN>0)` → clock reset / switch
- `DIFF` → VCA CV for noise or sub layer

**Result:** one audio source drives an entire modulation network.

---

## Patch 3: Percussion-to-metal machine
**Modules:** drum source, reverb, LPG, random CV

- snare or tom loop → Skorpion `IN`
- `SYNC` HARD
- `TARGET` = CLIP or SLIDERs
- random CV → `SHIFT`
- `DIFF` → LPG CV controlling a parallel noise burst
- `OUT` → reverb

**Result:** snare attacks become alien struck-metal tones with animated decay.

---

## Patch 4: Chaotic stereo lead
**Modules:** stereo reverb/delay, modulation source, filter

- VCO → Skorpion
- set `OUTPUT` into upper half toward `WIDE`
- `OUTPUT SWITCH` = FILTERS
- SHAPE source = `DELAY`
- slow LFO → `OUTPUT CV`
- `DELAY` out → shimmer reverb
- `OUT L/R` → stereo mixer

**Result:** moving stereo field where internal delay actively participates in timbre formation.

---

## Patch 5: Threshold-addressed wavetable-ish oscillator
**Modules:** quantizer, clocked modulation, VCA

- VCO sine → Skorpion `IN`
- `TARGET` = `SLIDERs`
- set TRGT sliders to a non-linear contour
- `TARGET ORDER` = `SEQ`
- `TRGTs` out → quantizer → second oscillator pitch
- `COUNT` → modulate first oscillator PWM or filter

**Result:** Skorpion acts like a threshold-addressed waveform sequencer and CV source simultaneously.

---

## Patch 6: Harmonic gate extractor
**Modules:** comparator/logic, trigger sequencer, envelopes

- complex audio or full mix stem → Skorpion `IN`
- `COUNT` → comparator threshold
- comparator output → trigger envelope
- `G(IN>0)` → logic gate input
- logic out → percussion voice or VC switch

**Result:** event extraction based on harmonic/threshold activity, not just amplitude.

---

## Patch 7: Dual-core recursive voice
**Modules:** second wavefolder / function generator / VCO, mixer, attenuation

- oscillator → Skorpion `IN`
- `DIFF` → second oscillator FM
- second oscillator → `CLIP`
- `TRGT MOD` from attenuated second oscillator
- mix second oscillator with Skorpion output

**Result:** cross-coupled timbral system where another oscillator defines Skorpion’s target clipping behavior.

---

# Best modules to pair by role

## Excellent “specific module” pairings

### Joranalogue Generate 3
Fantastic into Skorpion because:
- clean but rich source
- through-zero and dynamic waveform options
- can provide modulator and carrier duties

### Make Noise Maths / Falistri
Ideal utility companions:
- envelopes for FOLD/SLOPE
- slewed modulation
- mixing/inversion
- feedback management

### Pamela’s Pro Workout / Batumi
Great for:
- clocked modulation into SHIFT/OUTPUT
- synchronized macro-like movement
- subtle periodic scanning of thresholds and shape

### Xaoc Zadar
Excellent for highly sculpted CV to:
- SHAPE
- TARGET
- OUTPUT
- HALT

Short complex envelopes produce very articulate results.

### Mimeophon / Starlab / Data Bender
Natural spatial extensions:
- emphasize Skorpion’s stereo/delay personality
- great from `DELAY`, `DIFF`, or full stereo out

### Frap Tools Fumana or fixed filter banks
Amazing after Skorpion:
- isolate moving bands
- animate with `COUNT` and `DAC`
- turns folded output into spectral choreography

### Matrix mixers and attenuverters
Honestly maybe the most important category after a VCO.
Without attenuation and routing, you’ll miss a lot of Skorpion’s depth.

---

# Less obvious but very musical pairings

## 1. Quantizers
Quantize `TRGTs`, `DAC`, or even attenuated `DIFF` for melodic side effects.

## 2. Sequential switches
Use `±G(DIR)` or `G(IN>0)` to switch sources into `CLIP`, `TRGT MOD`, or `SHAPE`.

## 3. Resonators / physical modeling
`DIFF` into a resonator can sound incredible—sharp, bright excitation with internal movement.

## 4. PLLs / frequency trackers
Because Skorpion has sync and threshold logic, it can sit nicely in pitch-reactive systems.

## 5. Samplers / loopers
Feed loops into `IN`; use `COUNT` and `G(IN>0)` to derive modulation from sampled material.

---

# Performance tips from the manual behavior

## Use `EQUALIZE THLDs` when you want “classic” wavefolder behavior
This makes the threshold spacing regular and more predictable.

## Use `DRY IF NO THLDs` when heavily modulating `FOLD`
This prevents signal dropout and can produce lowpass-like behavior when the core follows the input.

## Use `SHIFT` for animation, not just asymmetry
The manual notes slow SHIFT modulation can produce a frequency-shift effect. That makes it a prime target for LFOs or envelopes.

## Don’t sleep on `TARGET`
This is one of the most unique controls. Moving between `5V`, `CLIP`, and `SLIDERs` changes the whole engine philosophy:
- `5V`: squarer, more classic destinations
- `CLIP`: overlays/follows another waveform
- `SLIDERs`: segment-by-segment programmed behavior

## `HALT` is compositionally useful
Stopping the vector core mid-motion can create flat, square-like held segments. Excellent with gates, bursts, or rhythmic logic.

## `OUTPUT` is not just wet/dry
Past noon it introduces the stereo delay/wide behavior. Modulating this slowly can make the stereo image feel alive without needing external effects.

---

# If I were building a “best friends for Skorpion” mini-system

A very strong small setup would be:

- **Clean VCO**
- **Function generator** (Maths/Falistri)
- **Matrix mixer / attenuverters**
- **Stereo filter or resonant filter**
- **Clocked modulation source**
- **Stereo delay/reverb**
- **Quantizer**
- **A few VCAs**

That combination unlocks nearly everything the manual suggests.

---

# Summary

Skorpion excels when treated as a **wavefolder plus control-voltage ecosystem**. The real magic is not only the main output, but the interaction between:

- threshold crossings
- target sequencing
- direction sensing
- difference/error voltage
- internal/external feedback
- stereo delay-derived behavior

The best partners are modules that let you:
- feed it stable or dynamically rich source material
- attenuate and route self-patching carefully
- derive structure from its outputs
- exploit its stereo and target architecture

If you want, I can also give you:
1. **10 genre-specific Skorpion patches**  
2. **a “best modules to pair with Skorpion under different budgets” list**  
3. **a signal-flow cheat sheet for self-patching Skorpion**  

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)