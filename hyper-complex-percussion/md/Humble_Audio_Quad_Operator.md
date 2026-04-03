# Humble Audio — Quad Operator

- [Manual PDF](../../manuals/Quad Operator Manual.pdf)

---

[Quad Operator Manual PDF](https://www.dropbox.com/paper/doc/print/JsIQoU7GbeAboEJku9ZgE?print=true)

# Using the Humble Audio Quad Operator for Dense Rhythmic and Hyper-Complex Percussion

The Quad Operator is not a drum module in the usual sense, but it is *very* well suited to percussion design because it gives you:

- 4 independent operators
- per-operator outputs
- internal FM routing via modulation matrix
- self-modulation
- external audio-rate FM input
- lock/free behavior
- reset input
- LFO mode
- CV control over ratio, shape, and gain

That combination makes it excellent for building **metallic hits, toms, kicks, zaps, digital hats, tuned percussion, pseudo-sequenced modulation networks, and interlocked polyrhythmic voices**.

The key mindset is this:

> Treat the Quad Operator less like “one FM voice” and more like a **4-node rhythm/percussion network**.

---

## What in the manual matters most for percussion

From the manual, the most useful features for your goal are:

- **Independent output per operator**  
  You can make each operator its own drum voice or layer.

- **Lock vs Free state**
  - **Lock** = integer ratios, better for harmonic/tuned percussion
  - **Free** = independent oscillators, better for inharmonic/noisy percussion and multi-voice independence

- **Gain CV per operator**
  - Controls output level
  - Also controls how strongly that operator modulates others through its modulation sends  
  This is huge: one envelope can simultaneously shape amplitude *and* FM intensity.

- **Mod 1–4 per operator**
  - Each operator can modulate any operator, including itself
  - This lets you create bursty, recursive, unstable percussion structures

- **AR FM input**
  - Lets you feed external oscillators/noise/drums back into the FM network
  - Great for chaotic accents and transient enhancement

- **Reset input**
  - Resets phase of all operators
  - Very important for tight transients and repeatable rhythmic attacks

- **LFO mode**
  - Allows phase-locked complex modulation signals
  - Great for rhythmic CV generation and cyclic FM structures

- **Algo expander**
  - Save/recall/crossfade modulation matrices
  - Perfect for switching between rhythmic FM topologies over a sequence

---

# Core strategy for complex percussion

For dense rhythmic music, use the Quad Operator in **three simultaneous roles**:

1. **Percussion voice generator**  
   Make kicks, toms, hats, pings, metallic hits.

2. **Internal modulation network**  
   Use one or more operators as modulators instead of audible voices.

3. **Rhythmic structure generator**  
   Use Reset, gain envelopes, ratio CV, and possibly LFO mode to force repeating but evolving rhythmic behavior.

The most effective approach is to assign operators like this:

- **Op 1** = low drum / kick / body
- **Op 2** = snare/tom/clang body
- **Op 3** = metallic layer / hat / click
- **Op 4** = hidden modulator or independently audible accent voice

Then patch each output to separate VCAs, LPGs, wavefolders, filters, and envelopes triggered by different clocks.

---

# Best patch architecture for polyrhythmic percussion

## 1. Use separate trigger streams per operator

Because the Quad Operator does not have per-operator trigger inputs, percussion articulation comes from **external VCAs/envelopes**.

Patch:

- **Op 1 out** → VCA 1 → mixer
- **Op 2 out** → VCA 2 → mixer
- **Op 3 out** → VCA 3 → mixer
- **Op 4 out** → VCA 4 → mixer

Then use different trigger lanes:

- VCA 1 envelope: every 5 steps
- VCA 2 envelope: every 7 steps
- VCA 3 envelope: every 11 steps
- VCA 4 envelope: every 13 steps

This instantly creates **long-cycle polyrhythms** even before you animate the FM.

### Why this works well here
Each operator can still modulate the others continuously inside the module, so even if only one operator is audible at a given moment, its timbre reflects the invisible motion of the whole FM matrix.

That means your percussion pattern can feel far denser than the number of triggers suggests.

---

## 2. Use Gain CV as your percussion “strike” control

The manual says Gain CV affects:

- output volume
- modulation intensity via modulation sends

This is one of the module’s best percussion features.

### Patch idea
For each operator:

- trigger → fast decay envelope → Gain CV

This gives you a hit whose loudness and brightness/complexity rise together.

### Result
At low envelope level:
- quieter
- cleaner
- more sine-like or lightly modulated

At high envelope level:
- louder
- more aggressive
- more sidebands
- more noise/metallic attack

That is basically ideal for percussion synthesis.

### Practical examples
- **Kick**: short envelope to Gain CV, minimal modulation
- **Tom**: medium envelope to Gain CV, modest cross-mod
- **Metal hit**: short spiky envelope to Gain CV, strong inharmonic modulation
- **Hat**: very short envelope, high ratios/free-state modulators, lots of FM

---

# Lock vs Free for rhythmic percussion

## Use Lock state for:
- tuned toms
- kicks with pitch identity
- marimba-like percussion
- harmonic bells
- sequences that need tonal center despite rhythmic complexity

Because ratios are integer relationships to the master pitch, lock state keeps things musically coherent even when rhythms are wild.

### Great rhythmic use
Set:
- all operators in lock
- detune centered
- sine shapes to start
- use integer ratios like 1, 2, 3, 5, 7, 11

This creates a family of tuned percussion voices that still feel related.

---

## Use Free state for:
- hats
- snares
- clanks
- broken digital percussion
- inharmonic accents
- polymetric noise voices

In free state, each operator becomes its own oscillator with independent tuning. This is better for drum-machine-style multi-voice behavior and for abrasive percussion.

### Hybrid recommendation
A very powerful setup is:

- **Op 1 locked** = kick/body
- **Op 2 locked** = tom/bell
- **Op 3 free** = hat/noise/metal
- **Op 4 free** = unstable modulator/accent voice

This gives both tonal coherence and rhythmic complexity.

---

# Reset input: essential for tight rhythms

The manual notes that Reset resets all operators’ phase and is great when using the module as a modulation source.

For percussion, it is also critical because it gives you **repeatable transients**.

Without reset, FM percussion can drift and produce slightly different attacks each time. That can be great, but for dense polyrhythms it may blur the groove.

## Patch ideas for Reset

### A. Reset every bar
- master bar pulse → Reset

This preserves some evolving movement inside the bar but re-aligns everything periodically.

### B. Reset on only the downbeat of an odd cycle
- 15-step or 21-step divider pulse → Reset

Now the entire FM network re-synchronizes only at long-form pattern boundaries.

### C. Reset from an irregular logic pattern
- Boolean combination of clocks → Reset

This creates a structured but unstable feeling where transients “snap into focus” at non-obvious points.

### D. Reset for specific percussion families
Since Reset affects all operators, use it as a **global phrase punctuation** tool rather than constant clocking.

---

# Building hyper-complex percussion voices

## 1. FM Kick

### Setup
- Op 1 audible
- Op 1 in **lock**
- Ratio low, likely 1
- Shape near sine
- Detune centered
- little or no modulation at first

### Add impact
- Op 2 in lock at ratio 2 or 3
- Send Op 2 → Mod 1 lightly
- Use envelope on **Gain 2 CV**
- Op 2 may be silent in mixer or mixed very low

Because Gain CV affects modulation strength, Op 2 can act like a pitch-envelope/transient source for the kick.

### Enhance
- trigger Op 1 VCA with short decay
- trigger Op 2 Gain CV with shorter, snappier envelope
- occasional reset on bar start

### Polyrhythmic variation
Trigger the kick VCA on one pattern, but trigger Op 2’s Gain CV on a different pattern.  
Now the kick body remains in one rhythm while attack brightness follows another meter.

---

## 2. Metallic snare / industrial clap body

### Setup
- Op 2 audible
- Op 2 in free state
- Shape somewhere between triangle and square
- Op 3 and Op 4 in free state at different tunings
- Send Op 3 → Mod 2
- Send Op 4 → Mod 2
- Optionally self-mod on Op 2

### Envelope use
- envelope to Gain 2 CV
- different trigger streams to Gain 3 CV and Gain 4 CV

This makes the snare body change depending on which modulators are “awake” at the moment.

### Rhythmic complexity trick
Use separate Euclidean or step lengths:

- audible snare envelope every 8
- Op 3 mod envelope every 5
- Op 4 mod envelope every 7

The snare appears on a stable pulse, but its internal texture cycles over 35 steps.

---

## 3. Hats and ticks

The Quad Operator can do excellent hats if you lean into inharmonic high-ratio or free-state FM.

### Setup
- Op 3 audible
- Op 3 free state, high frequency
- Shape toward square or saw
- Op 4 free state, also high frequency
- Op 4 → Mod 3
- maybe self-mod on Op 3

### Make closed/open variations
Use two envelope lengths into Gain 3 CV:
- short decay = closed hat
- long decay = open hat

Or:
- one trigger pattern for VCA
- another for Gain CV accenting

### Add articulation
Patch a stepped CV source into Shape 3 CV or Ratio 3 CV, with a different clock than the hat trigger.

This gives changing hat alloys over time.

---

## 4. Bell trees / tuned percussion clouds

### Setup
- all operators locked
- sine or triangle-heavy shapes
- integer ratios spread musically: 1, 2, 3, 5 or 1, 3, 4, 7
- modest modulation sends

### Rhythm design
Give each output its own envelope with different sequence lengths:
- Op 1: 9-step pattern
- Op 2: 10-step pattern
- Op 3: 12-step pattern
- Op 4: 14-step pattern

Because the voices share the same master tuning but interact through FM, the resulting cloud feels unified while the pattern lattice is very long.

---

# Use the modulation matrix like a drum network

The manual says any FM algorithm is possible via the modulation matrix, including self-modulation.

That means you should think in terms of **roles**, not just voices.

## Useful matrix topologies

### 1. Chain
- Op 4 modulates Op 3
- Op 3 modulates Op 2
- Op 2 modulates Op 1

Use Op 1 as main audible voice.  
Great for kicks, toms, and evolving strike complexity.

### 2. Parallel modulators
- Op 2 → Op 1
- Op 3 → Op 1
- Op 4 → Op 1

Great for snares and metallic percussion, especially when each modulator has separate gain envelope timing.

### 3. Cross-coupled pair
- Op 1 ↔ Op 2
- Op 3 ↔ Op 4

Then use the two pairs as two percussion families:
- low pair for body/toms
- high pair for hats/metals

### 4. Self-mod emphasis
- Op 3 → Mod 3
- Op 4 → Mod 4

Self-modulation is useful for harsher transients, distorted zaps, and noisy metallic percussion.

### 5. Shared hidden modulator
- Op 4 modulates all operators
- don’t mix Op 4 output, or mix it quietly

This is especially powerful if Op 4 is driven by its own odd-meter envelope pattern.

---

# Polyrhythm methods that work especially well

## Method 1: Different envelope clocks per operator
The simplest and strongest method.

Example:
- Op 1 amplitude envelope: every 4
- Op 2 amplitude envelope: every 5
- Op 3 amplitude envelope: every 7
- Op 4 gain envelope: every 9

Even a static tuning setup becomes a dense rhythmic engine.

---

## Method 2: Audible rhythms vs modulation rhythms
Separate the timing of what you hear from the timing of what shapes it.

Example:
- Op 1 audible hits on 4-step cycle
- Op 2 modulation bursts on 3-step cycle
- Op 3 modulation bursts on 5-step cycle
- Reset every 16 or 32 steps

This produces recurring but non-obvious accent patterns.

---

## Method 3: Different CV clocks for shape and ratio
The manual allows CV over shape and ratio.

Use:
- one slow sequencer to Ratio CV
- another stepped random or sequencer to Shape CV
- a third trigger pattern to Gain CV

Now pitch family, spectral family, and hit timing all run on different clocks.

That is ideal for music in complex meters.

---

## Method 4: VCO vs LFO mode as structural layer
LFO mode can create complex phase-locked modulation signals.

Try:
- switch to LFO mode
- use one or more operators as cyclic modulation sources
- patch outputs to external VCAs, wavefolders, filters, or clockable comparators

This can turn the module into a multi-lane rhythmic CV source, not just a sound source.

Then occasionally return to VCO mode or use a second voice path for audio percussion.

---

# Complex time signatures and metric design

If you want 5/4, 7/8, 11/8, or nested polymeters, the Quad Operator fits best when you assign different operator functions to different metric layers.

## Example: 7/8 industrial percussion patch
- **Op 1**: kick body, pattern accents on beats 1 and 5
- **Op 2**: metallic snare on beat 4 and occasional fills
- **Op 3**: hats in a 3-against-7 pattern
- **Op 4**: hidden modulator triggered every 5 pulses

Because Op 4 changes the FM state on a 5-pulse loop while the phrase is in 7/8, the apparent drum timbre rotates against the bar line.

## Example: 11-step cycle
- Op 1 audible every 11
- Op 2 audible every 4
- Op 3 modulates Op 2 every 6
- Op 4 resets phrase every 33 pulses via external logic

This creates long evolving cycles without needing a huge number of modules.

---

# The Algo expander is extremely useful for percussion composition

The manual says the Algo expander can:

- save modulation send knob positions
- load them
- crossfade between saved algorithms and live settings

This is unusually powerful for rhythmic music.

## Why it matters
Instead of just changing notes or triggers, you can change the **entire FM topology** while keeping the same rhythmic skeleton.

That means one pattern can cycle through:
- clean tuned percussion
- harsh metallic network
- sparse kick/snare architecture
- self-modulating noise cluster

## Performance ideas

### A/B contrast
- **A** = restrained harmonic FM percussion
- **B** = noisy cross-modulated industrial percussion
- crossfade between them over 16 bars

### Live morphing
- save one stable algorithm in A
- use Live as a second state
- perform the Mod knobs by hand
- crossfade between saved structure and current structure

### Phrase-level form
Use different algorithm slots for different sections:
- A = groove
- B = fill
- C = breakdown chaos
- Live = improvised mutation

For dense rhythmic music, this is gold.

---

# External AR FM for extreme percussion

The manual gives the AR FM input its own gain and sends to all operators. This is one of the best tools for creating layered percussion attacks.

## What to patch into AR FM
- noise source
- another digital oscillator
- filtered noise burst
- a feedback loop from one Quad Operator output
- a drum module transient
- ring mod or wavefolder output
- a click or impulse source

## Best uses

### 1. Attack injection
Patch a click, burst, or filtered noise into AR FM and send it lightly to one or more operators.  
This adds sharpness and complexity to percussion attacks.

### 2. Shared chaos bus
Use one external source to modulate all 4 operators at different amounts.  
Now one rhythmic source “glues” all voices together.

### 3. Controlled feedback
The manual explicitly suggests feedback-like use, especially with lock mode operators.  
Patch one operator out to external processing and back into AR FM.

This can create:
- tearing kicks
- metallic tearing snares
- unstable hats
- swarming transients

Watch the clipping LED and adjust AR FM gain accordingly.

---

# Practical patch recipes

## Patch 1: 4-voice polymetric percussion bank

### Module setup
- Op 1 lock, ratio 1, sine-ish
- Op 2 lock, ratio 3, triangle-ish
- Op 3 free, high freq, square-ish
- Op 4 free, mid-high freq, saw-ish

### FM matrix
- Op 2 → Mod 1 medium
- Op 3 → Mod 2 medium
- Op 4 → Mod 3 high
- Op 4 → Mod 1 low
- self-mod Op 3 a little

### External patching
- each op out to separate VCA
- different trigger/envelope streams to each VCA
- different envelopes to Gain CV 1–4

### Rhythms
- Op 1 on 5-step cycle
- Op 2 on 7-step cycle
- Op 3 on 11-step cycle
- Op 4 on 13-step cycle

### Result
A self-related but extremely long evolving percussion pattern.

---

## Patch 2: One voice, many hidden rhythm layers

### Goal
Use Op 1 as the only audible output, but let the other operators rhythmically reshape it.

### Setup
- mix only Op 1
- Op 2, 3, 4 used as modulators
- all send to Op 1
- Op 2 in lock
- Op 3 and 4 in free

### Timing
- Op 1 VCA envelope on main groove
- Gain 2 CV triggered every 3
- Gain 3 CV triggered every 5
- Gain 4 CV triggered every 8

### Result
One drum voice that seems to play many variations and internal subdivisions without changing its main trigger rhythm.

Excellent for dense techno, IDM, broken beat, and industrial sequences.

---

## Patch 3: Rotating meter percussion scene with Algo

### Save states
- **A** = minimal harmonic modulation
- **B** = metallic cross-mod network
- **C** = self-mod chaotic texture

### Rhythm
Use a master sequence in 7/8 or 15/16.

### Performance
Crossfade between A and B slowly, jump to C for fills, return to Live for hands-on mutation.

This gives structure to complicated rhythms without needing to resequence everything.

---

# Sound design tips from the manual, adapted for percussion

The manual’s harmonic FM advice says to start with:

- VCO mode
- all operators in lock
- detune centered
- sine waves
- modulation sends at zero

That is also the right way to build percussion deliberately.

## Workflow
1. Start from simple sine/lock setup
2. Make one voice at a time
3. Add one modulator
4. Add Gain CV envelope
5. Add shape modulation
6. Then destabilize with free state, detune, self-mod, or AR FM

For hyper-complex music, this matters.  
If you start already chaotic, you won’t know what is creating the rhythmically useful complexity and what is just noise.

---

# Advanced rhythmic tricks

## 1. Use one operator as a “ghost accent modulator”
Keep one operator mostly inaudible but send it to multiple destinations.  
Trigger its Gain CV on offbeats or tuplets.  
This creates accents across several voices at once.

## 2. Put operator outputs through comparators or logic
Because outputs are audio/CV capable and phase-resettable, in LFO mode especially you can derive gates or rhythmic pulses from them externally.

## 3. Alternate reset lengths
Reset every 16 bars in one section, then every 15 in another.  
This changes how the FM drift aligns to the meter.

## 4. CV the shape on high percussion only
Fast hats and metal sounds respond strongly to shape shifts between sine/triangle/square/saw.  
Stepped shape CV can act like changing cymbal alloy or stick position.

## 5. Sequence ratio in free state for pseudo-drum tuning changes
In free state, ratio CV becomes 1V/oct for that operator.  
Use sequenced voltages to jump between kick tunings, tom registers, or metallic clusters.

## 6. Use detune for unstable flams
Small detune between interacting operators can mimic flams, chorused attacks, or rattling surfaces.

---

# Recommended starting setups

## Clean polyrhythmic percussion starter
- VCO mode
- Op 1 and 2 lock
- Op 3 and 4 free
- detunes centered
- shapes near sine/triangle
- all modulation off
- separate envelopes to each operator’s VCA and Gain CV
- add modulation one lane at a time

## Industrial complexity starter
- Op 1 lock low
- Op 2 free mid
- Op 3 free high
- Op 4 free high or hidden
- moderate self-mod on Op 3
- Op 2, 3, 4 all send to Op 1 or 2
- AR FM fed from noise or processed feedback
- reset only occasionally

## Tuned odd-meter percussion starter
- all operators lock
- ratios 1, 2, 3, 5
- sine/triangle shapes
- minimal detune
- one saved Algo per section
- envelopes triggered in 5, 7, 9, 11-step cycles

---

# Biggest takeaway

For your goal, the Quad Operator shines when you stop thinking of it as only an FM oscillator and start treating it as:

- a **4-voice percussion synthesis engine**
- a **matrix of mutually affecting rhythmic bodies**
- a **cross-modulated polyrhythmic ecosystem**

The most important moves are:

1. **Use separate trigger/envelope streams outside the module**
2. **Exploit Gain CV for both loudness and FM intensity**
3. **Mix lock and free operators**
4. **Use Reset as phrase-level timing glue**
5. **Use saved/crossfaded algorithms to change rhythmic topology**
6. **Let some operators be modulators only**
7. **Run audible rhythms and modulation rhythms on different cycle lengths**

That is how you get percussion that feels:
- dense
- alive
- mathematically interlocked
- still performable

If you want, I can also give you:
- a **set of 10 concrete patch recipes**
- a **techno-focused patch plan**
- an **IDM/glitch patch plan**
- or a **“what to connect to what” system-specific patch sheet** for the modules you already own.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)