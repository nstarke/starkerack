# Schlappi Engineering — Angle Grinder

- [Manual PDF](../../manuals/angle_grinder_manual_20181022.pdf)

---

[Angle Grinder Manual PDF](#)

# Schläppi Engineering Angle Grinder — melodic use analysis

The attached manual is for **one module**: **Schläppi Engineering Angle Grinder**.  
So rather than “how these modules can be used together,” the useful framing here is:

- how the **internal sections** of Angle Grinder work together
- how to patch it with the rest of a Eurorack system to create **melodic material**
- what kinds of **pitched roles** it can play in a musical patch

---

## What Angle Grinder is, musically

Angle Grinder is not just a weird distortion/filter. It is really **three melodic-capable tools in one**:

1. **Quadrature sine VCO / LFO**
2. **State-variable-ish filter**
3. **Voltage-controlled waveshaper / nonlinear feedback processor**

That makes it useful for melody in several different ways:

- as a **primary oscillator** with 1V/oct tracking
- as a **companion oscillator** for phase-related voices
- as a **harmonic animation source** for otherwise plain waveforms
- as a **filter voice** that can be “played” by resonance/feedback behavior
- as a **subtle or aggressive timbral layer** that follows melodic pitch

The big concept of the module is the interaction between:

- **SPIN** = the oscillator/filter core
- **GRIND** = comparator + VCA + subtractive waveshaping/feedback network

This interaction is what turns a simple pitched tone into something alive and musically rich.

---

## Key manual takeaways for melodic patching

From the manual:

- **Tracks 4+ octaves at the V/OCT input**
- **High range:** about **10 Hz to over 20 kHz**
- **Low range:** about **0.3 Hz to over 600 Hz**
- **Four phase-related outputs**:
  - in oscillator mode: **0°, 90°, 180°, 270°**
  - in filter mode: **Low Pass, Band Pass, High Pass, Inverted Band Pass**
- **Sine outputs** are **5 Vpp**
- **GRIND/filter outputs can get much hotter**, up to around **22 Vpp**
- **FM1** can be linear or exponential via rear jumper
- **FM2** is additional exponential pitch CV
- **INJECT** can feed SPIN directly, bypassing GRIND
- **FM1 is normalled to GRIND OUT**, which matters a lot for tuning

That last point is especially important for melodic use:  
if you want clean pitch tracking, **turn FM1 down unless you intentionally want self-modulated chaos**.

---

# How the two sections work together for melody

## 1. SPIN as the pitch source

SPIN is a **quadrature sine oscillator**, which means it produces four sine waves at the same frequency but shifted by 90° relative to each other.

For melody, this gives you:

- a **clean fundamental tone**
- four related outputs that can be:
  - mixed for different timbres
  - sent to different VCAs/filters
  - used as phase-offset modulation sources
  - treated as separate “voices” that still feel unified

Because it tracks 1V/oct over several octaves, SPIN can absolutely serve as a **pitched melodic oscillator**.

### Strong melodic use cases
- lead voice
- bass voice
- tuned FM source
- chord-ish layered sine stack through further processing
- quadrature modulation source for animated stereo melodic patches

---

## 2. GRIND as harmonic sculptor

GRIND compares the SPIN phases against an input, creates square-ish control shapes, and subtracts them from the input. In plain musical terms:

- it can turn simple tones into **edgy, metallic, vocal, pyramidal, stepped, or tearing waveforms**
- it can create **harmonic complexity that still follows pitch**
- it can act like a **voltage-controlled timbre engine**

This is exactly the kind of thing that makes a melody feel expressive rather than static.

For melodic composition, GRIND is especially good at:

- adding controllable overtone motion to a pitched oscillator
- creating brighter transients on note attacks
- evolving a bassline from sine to snarling shape
- producing unstable but repeatable timbres when under CV control

---

## 3. GRIND→SPIN as “playable instability”

The **GRIND -> SPIN** control feeds the GRIND output back into the oscillator/filter core.

This is the musical magic zone.

At low amounts:
- subtle enrichment
- dynamic asymmetry
- controlled growl

At medium amounts:
- animated harmonic movement
- unstable but still pitch-centered tones
- pseudo-resonant behavior

At high amounts:
- the oscillator can be overwhelmed and shift toward **filter-like behavior**
- tones can become noisy, percussive, or semi-chaotic
- pitch may become less stable, but this can be musically great for accents and transitions

For melody, this means you can treat GRIND->SPIN as a **timbre-performance control**:
- lower for stable notes
- higher for choruses, fills, or dramatic phrases

---

# Best melodic roles for Angle Grinder

## A. Primary melodic oscillator

This is the most straightforward use.

### Patch idea
- Sequencer 1V/oct → **V/OCT**
- Envelope → VCA controlling audio level downstream
- Take **0° output** or **GRIND OUT** as main audio
- Keep **FM1 down**
- Tune with **SPIN** and **FINE**
- Use **GRIND sliders** for timbre shaping

### Musical result
- Clean sine-based melodies if you use SPIN outputs directly
- Rich, animated leads or basses if you use GRIND OUT

### Why it works
You get pitch stability from SPIN and character from GRIND.

---

## B. Melodic oscillator with animated timbre

Because each GRIND lane has its own slider and CV input, you can move the harmonic structure over time.

### Patch idea
- Sequencer → **V/OCT**
- Slow envelope/LFO/sequence rows → one or more **GRIND CV inputs**
- Main audio from **OUT**
- Optionally use a separate envelope to control final VCA

### Musical result
Each note can have:
- different brightness
- different edge
- different attack contour
- timbral movement across a phrase

This is ideal for:
- acid-adjacent leads
- morphing basslines
- synthetic plucks with internal animation

---

## C. Dual-role melody + modulation source

Since SPIN has four phase outputs, you can use one as audio and others as modulation tied to the same pitch.

### Patch idea
- 1V/oct → V/OCT
- **0° output** → audio path
- **90° / 180° / 270° outputs** → modulate:
  - panning
  - wavefolder symmetry
  - filter cutoff
  - VCA level on parallel voice

### Musical result
The melody itself drives its own movement.  
This creates very coherent patches where:
- every note has internal motion
- stereo shifts feel locked to the pitch
- supporting modulation feels musically related rather than arbitrary

This is one of the most special melodic uses of Angle Grinder.

---

## D. Melodic filtering / pingable timbre voice

When SPIN is damped or sufficiently disrupted by GRIND feedback/input, it behaves more like a filter core.

With the right external oscillator, Angle Grinder becomes a very unusual **melodic filter voice**.

### Patch idea
- Send a tuned VCO or harmonically rich source into **IN**
- Turn **GRIND -> SPIN** clockwise
- Add some **DAMPING**
- Use the SPIN outputs as:
  - low pass
  - band pass
  - high pass
  - inverted band pass

### Musical result
- moving resonant tones
- formant-like melodic filtering
- unstable but expressive spectral shifts
- pseudo-physical or vocal textures

This works great when the melody is carried by another oscillator and Angle Grinder becomes the **character voice**.

---

## E. Soft-sync melodic voice with INJECT

The **INJECT** jack directly hits the SPIN core and can be AC- or DC-coupled.  
The manual says AC mode is default and acts like a **soft sync-like effect**, especially with square or saw input.

### Patch idea
- Sequencer → V/OCT on Angle Grinder
- Another oscillator’s saw or square → **INJECT**
- Main audio from SPIN output or GRIND OUT

### Musical result
- stable pitch with reset-like articulation
- animated sync-ish harmonics
- sharper melodic presence without standard hard-sync harshness

This is excellent for:
- leads
- sync bass
- aggressive arpeggios

---

# Practical melodic patch recipes

## 1. Clean sine lead
**Goal:** pure, stable melodic line

**Patch**
- Sequencer → V/OCT
- 0° output → VCA → mixer
- Envelope → VCA CV
- FM1 fully down
- GRIND sliders down or unused
- DAMPING low / oscillator mode active

**Result**
- very pure sine lead or bass
- good for sub lines, FM carrier duty, or minimal melodies

---

## 2. Animated bass voice
**Goal:** bassline that moves harmonically while staying pitch-centered

**Patch**
- Sequencer → V/OCT
- OUT → lowpass filter or LPG → VCA
- One envelope or sequencer lane → GRIND CV 1
- Another modulation source → GRIND CV 2
- Keep GRIND->SPIN low to medium
- Use one or two sliders up

**Result**
- bass with evolving edge
- can move from rounded to biting across a phrase
- especially good for techno, EBM, industrial, electro

---

## 3. Phase-based stereo melody
**Goal:** wide melodic voice from one oscillator

**Patch**
- Sequencer → V/OCT
- 0° output → left voice chain
- 180° output → right voice chain
- Or 90° and 270° to two VCAs/panners
- Use same envelope for both, or offset them slightly

**Result**
- natural stereo spread
- strong mono relationship but lively width
- beautiful for drones, ambient melodies, and glassy tuned textures

---

## 4. Four-note articulated patch from one pitch source
**Goal:** one melodic line driving a complex ensemble feel

**Patch**
- Sequencer → V/OCT
- Send 0°, 90°, 180°, 270° to four different destinations:
  - four VCAs
  - four filters
  - four wavefolders
- Modulate each destination differently
- Mix them back together

**Result**
- one pitch source, but layered motion
- pseudo-ensemble or rotating timbre cloud
- excellent for melodic ostinatos

---

## 5. Harmonic melody processor
**Goal:** use Angle Grinder to transform another melodic oscillator

**Patch**
- External oscillator carrying the melody → IN
- Set SPIN to LFO or audio rate depending desired effect
- Listen to OUT
- Modulate GRIND sliders/CV
- Keep GRIND->SPIN low for processing, higher for feedback complexity

**Result**
- supersaw-like shimmer at low internal rates
- metallic sidebands and tearing overtones at audio rates
- melody remains recognizable but gets a distinct synthetic personality

This is especially powerful when you already have a favorite VCO but want a more original melodic timbre.

---

## 6. Filtered melody with nonlinear resonance
**Goal:** melodic line with unstable resonant animation

**Patch**
- External VCO → IN
- Use GRIND->SPIN at medium-high setting
- Add DAMPING to move away from pure oscillation
- Take LP/BP/HP outputs from SPIN
- Sequence/filter the external VCO as normal

**Result**
- animated filtering that feels halfway between a filter, resonator, and feedback network
- great for leads that need movement without adding many extra modules

---

## 7. Self-voicing chaotic melody
**Goal:** unstable but tunable lead voice

**Patch**
- Sequencer → V/OCT
- No input patched, or experiment with IN turned up as manual suggests
- Use OUT as audio
- Raise one or more GRIND sliders
- Explore GRIND->SPIN and DAMPING carefully
- FM1 down unless intentionally using self-feedback FM

**Result**
- highly characterful, almost broken-waveform tones
- can sound like sync, folding, PWM, and comparator distortion all at once
- great for aggressive hooks and industrial melody lines

---

# How to keep it melodic instead of chaotic

Angle Grinder can go wild quickly. If your goal is melody, these practices help a lot.

## 1. Turn FM1 down for pitch tracking
The manual explicitly warns that **FM1 is normalled to GRIND OUT**.  
So if nothing is plugged in and FM1 is up, the oscillator is self-modulating.

That is fun, but not ideal if you want:
- precise tuning
- consistent intervals
- stable bass

So for melodic work:
- **start with FM1 fully CCW**

---

## 2. Start from SPIN outputs, then add GRIND
If you need a reliable melodic basis:

1. get the pitch right on 0° output
2. confirm tracking
3. then bring in GRIND OUT or feedback

This prevents losing the musical center too early.

---

## 3. Use fewer sliders first
The manual’s oscilloscope examples show that each slider introduces a distinct shaping contribution, and combinations get more complex.

For melody:
- begin with **one slider**
- then try **two adjacent sliders**
- only then go to all four

This keeps the overtone structure more readable.

---

## 4. Use GRIND->SPIN like a macro performance control
Instead of setting it high all the time, automate or perform it.

Best use:
- lower during verse
- rise during fill
- spike for transitions
- pull back for pitch clarity

---

## 5. Separate “pitch CV” from “timbre CV”
Use:
- **V/OCT / FM2** for pitch-related control
- **GRIND CV inputs** for timbre-related control

This makes the module much easier to compose with.

---

# Where Angle Grinder shines in melodic genres

## Excellent for
- industrial techno
- EBM
- electro
- dark ambient
- experimental pop
- IDM
- cinematic tension music
- acid-adjacent bass and lead work
- noise-informed but tonal music

## Less naturally suited for
- very pristine traditional subtractive lead patches
- ultra-precise tonal polyphony
- delicate, perfectly repeatable analog sweet-spot patching

It can still do subtler work, but its personality is in **animated nonlinearity**.

---

# Best musical pairings in a wider Eurorack system

Even though only one module manual was attached, Angle Grinder pairs especially well with:

## Sequencers
For obvious melodic use:
- 1V/oct lines
- sequenced timbre CV to GRIND lanes
- transposition and accent tracks

## VCAs / LPGs
Essential to shape notes dynamically after the often-hot outputs.

## Envelopes
Very useful for:
- note articulation
- per-note grind animation
- feedback depth changes

## Filters
If using GRIND OUT as a main oscillator, a downstream filter can tame or spotlight specific overtones.

## Wavefolders / distortion
Angle Grinder already shapes heavily, but subtle extra processing can create very rich leads.

## Delays / reverbs
The phase outputs into stereo effects can sound huge and highly musical.

## Precision adder / quantizer
Helpful if you want to keep complex Angle Grinder patches locked into tonal material.

---

# Most musically useful outputs for melody

## 0° output
- best starting point for pitch
- cleanest reference
- ideal for tuning and stable melodic work

## 90° / 180° / 270°
- alternate voices
- stereo companions
- modulation tied to pitch
- parallel processing

## OUT / GRIND OUT
- most characterful melodic audio output
- best for aggressive basses and leads
- can get very hot; attenuate if needed

## Filter outputs when in filter behavior
- best for spectral melodies
- unusual formants
- feedback-rich tonal coloration

---

# Three high-value melodic workflows

## Workflow 1: Stable melody, unstable timbre
- Pitch from V/OCT
- Audio from GRIND OUT
- FM1 off
- Moderate slider use
- GRIND CV animated by envelopes/LFOs

This is probably the most generally useful mode.

## Workflow 2: One oscillator, many related voices
- Use multiple SPIN outputs in parallel
- Different processing per phase
- Common pitch sequence

This is excellent for stereo and layered arrangements.

## Workflow 3: External melody into Angle Grinder processor
- Use another VCO for the main melody
- Feed it to IN
- Use Angle Grinder as wave-transformer/filter-feedback network

This is the best option if you want Angle Grinder’s character without relying on it as the only pitch source.

---

# Bottom line

**Angle Grinder is absolutely capable of creating melodic components**, but it is most rewarding when treated as a **performance-oriented timbral oscillator/filter hybrid** rather than a plain voice.

Its strongest melodic uses are:

- **quadrature sine VCO** for tuned melodic lines
- **animated waveshaper** for expressive bass and lead timbres
- **phase-related multi-output source** for stereo or layered melodic structures
- **soft-sync / injected oscillator** for sharper harmonic articulation
- **nonlinear filter/resonator** for spectral melodic processing

If you want clean melody, start simple:
- V/OCT in
- FM1 down
- monitor 0° output
- add GRIND gradually

If you want memorable melody, lean into what makes Angle Grinder special:
- CV the GRIND lanes
- exploit the four phases
- perform GRIND->SPIN
- use INJECT and feedback as compositional tools

It is a module that can make a sequence sound less like “notes from an oscillator” and more like a **living mechanical voice**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)