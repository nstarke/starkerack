# Fancyyyyy — K-Accumulator Digital Complex Oscillator

- [Manual PDF](../../manuals/K_ACCUMULATOR_Quickstart_v1.02.pdf)

---

[Manual PDF](https://fancysynthesis.net)

# Using K-ACCUMULATOR to Build Full-Length Eurorack Songs

K-ACCUMULATOR is not just a voice. From the quick-start, it is really a **self-contained composition engine** built around:

- a main stereo oscillator
- a mod oscillator
- a full-spectrum function generator (UFG)
- a delta-sigma pattern generator (Δ–∑)
- internal routing and quantized root-based tuning
- morphable timbral states

That matters for songwriting, because “full song” in Eurorack usually fails when a patch has only one good loop. K-ACCUMULATOR gives you several independent-but-related axes of change:

1. **Pitch structure** via Root, scales, and quantization  
2. **Sequence variation** via Δ–∑ Chance, Length, Smooth, and pattern editing  
3. **Timbre evolution** via Morph plus Shift/Depth/Shape/Stretch  
4. **Energy contour** via UFG loop/trigger behavior and Damped/Pulsar  
5. **Voice interaction** via Mod oscillator tracking relationships  
6. **External signal interaction** via tracking, sync, TZPM, and 1V/TZ

That makes it unusually strong for turning a patch into sections: intro, verse, lift, breakdown, climax, outro.

---

## 1. The songwriting mindset for this module

Instead of treating K-ACCUMULATOR as:

- one oscillator making one interesting sound

treat it as:

- **a central harmonic system**
- **a morphing lead/bass/pad/percussion voice**
- **a sequencer/modulator clock source**
- **a transition machine**

A full song needs three things:

- **repetition**
- **contrast**
- **return**

K-ACCUMULATOR supports all three:

- **repetition**: lock Δ–∑ at low Chance, fixed Root/Scale, stable Morph point
- **contrast**: change Morph mode, scale, sync source, UFG rate, Damped/Pulsar
- **return**: come back to “Centre” or to a saved parameter region

The manual’s emphasis on **Centre** is especially important for arrangement. Centre is your “home base.” In songwriting terms, that is gold: it gives you a way to periodically reset density and rebuild.

---

# 2. What K-ACCUMULATOR uniquely contributes to song structure

## A. Root system as global harmonic anchor
The **Root** section can quantize pitch and distribute tuning to OSC and/or UFG. That means you can define a song’s key center from one place.

Use this for:

- key-centered bass + melody relationships
- controlled modulation rates that stay musically related
- section changes by changing scale density or tuning system

### Song use:
- Verse: send Root to OSC only
- Chorus: send Root to OSC + UFG so modulation becomes harmonically locked
- Bridge: disengage Root from one destination for freer, more unstable movement

---

## B. Δ–∑ as evolving motif generator, not just a sequencer
The Δ–∑ is especially useful for “full song” writing because it is **non-destructive**. You can wander away from a pattern with Chance, then return.

That solves a huge modular problem:
- randomization often destroys the hook
- here, you can mutate the hook and recover it

### Song use:
- Keep a memorable 8-step motif at minimum Chance
- Raise Chance during transitions, fills, bridges
- Return Chance to minimum for the chorus/return section
- Modulate Length to zoom into fragments for tension
- Add Smooth for legato or filtered-audio-rate texture

This is one of the strongest tools in the module for arrangement.

---

## C. Morph as arrangement
The Morph section is not just “different sounds.” It is a **continuum of related modulation topologies**.

That means you can treat Morph positions like sections of a song:

- **FMNT** = intro / airy vocal-ish / pad-like
- **FBPM / 2OP** = stable body sections
- **XPM / XPM2** = climax, aggression, peak density
- **Asym** = unstable, broken, granular bridge/outro

Because the timbral identity stays related, a song can evolve dramatically while still sounding like one instrument.

---

## D. UFG as energy control
The UFG acts as:

- modulation source
- envelope/window for pulsar behavior
- internal clock for Δ–∑
- audio-rate oscillator when needed

This is important for arrangement because it lets you shift between:

- slow envelopes
- tempo-synced modulation
- audio-rate complexity

### Song use:
- Intro: UFG in sub-audio, single-shot or slow looping
- Main groove: UFG clocking Δ–∑ in stable looping mode
- Chorus: increase Time or change trigger mode
- Breakdown: switch to manual/single-shot triggering
- Peak: audio-rate UFG for extra harshness/animation

---

# 3. Practical strategies to make full songs with this module

## Strategy 1: Use K-ACCUMULATOR as the “main character” voice
Patch it as your central stereo voice and let other modules support it.

### Good supporting modules:
- **clock / master transport**: Pamela’s Pro Workout, Tempi
- **mixer**: Performance Mixer, TexMix, Cosmix
- **VCAs**: Quad VCA, Veils, Tallin
- **filter**: stereo filter or LPG for macro dynamics
- **reverb/delay**: Mimeophon, Magneto, FX Aid, Desmodus Versio
- **sampler/drums**: sample drum modules or dedicated drum voices
- **mute/performance module**: Mutamix, Joranalogue Switch 4, WMD SSM if available used
- **sequential switch**: Doepfer A-151, Vice Virga, Switchblade
- **recorder/looper**: Lubadh, Morphagene, Arbhar, Bitbox

### Song method:
- K-ACCUMULATOR handles melodic/timbral identity
- drum modules provide groove grid
- external mixer and mutes create entrances/exits
- FX sends define space per section

This works especially well if you commit to one voice carrying the song theme.

---

## Strategy 2: Split a song into arrangement layers
Use K-ACCUMULATOR to supply multiple roles over time:

- intro drone
- bassline
- lead
- rhythmic texture
- transition FX

Even if it only outputs one stereo signal at a time, you can **re-record**, **sample**, or **loop** sections.

### Example workflow:
1. Build an intro texture using FMNT + slow UFG
2. Record 16 bars into a looper/sampler
3. Reset to Centre
4. Create a bassline with Δ–∑ to 1V/TZ and low Morph complexity
5. Record another section
6. Use the live voice for lead/variation over the looped material
7. Resample again for breakdown textures

This is one of the best ways to turn a single rich Eurorack voice into a full track.

Modules that help:
- Morphagene
- Lubadh
- 4ms Stereo Triggered Sampler
- Bitbox
- Assimil8or
- external DAW, Octatrack, or hardware recorder

---

## Strategy 3: Use section presets by patch design, not memory
The manual doesn’t mention preset storage, so make “manual presets” using patch architecture.

For example, define:

- **Section A**: Morph CV from UFG, low Depth, quantized scale
- **Section B**: Morph CV from external sequencer, higher Damped/Pulsar
- **Section C**: external sync input active, higher Stretch, different Mod tracking

Use switches, offsets, and VCAs so a few performance gestures move between section states.

### Modules that help:
- precision adders
- voltage memories/preset managers
- switched offsets
- matrix mixers
- sequential switches
- macro controllers

Examples:
- Acid Rain Maestro
- Frap Tools 321 / 333
- Happy Nerding 3xMIA
- Joranalogue Select 2 / Step 8
- ADDAC manual CV modules
- Verbos Voltage Multistage
- Make Noise Pressure Points + Brains
- Planar 2 for macro morphing

A song becomes much easier when one gesture changes several voltages at once.

---

# 4. Best ways to use each section for arrangement

## Root section for song-scale harmonic planning

The Root system is more than tuning. It is a way to enforce harmonic coherence across a long-form patch.

### Use cases:
- **Change sections with scale selection**: narrower scale for verse, denser or more exotic scale for bridge
- **Use Root Send states as arrangement states**
  - OSC only: stable melody voice
  - OSC + UFG: modulation rhythm becomes tuned and integrated
  - UFG only: modulation changes while main voice remains freer
- **Use Just Intonation in intros/breakdowns**, 12-TET in main rhythmic sections if pairing with other tonal modules

### With other modules:
- Send the same external pitch CV to K-ACCUMULATOR Root and another voice via buffered mult
- Use a precision adder to transpose Root between sections
- Use a keyboard/sequencer for deliberate verse/chorus key centers

Great pairing modules:
- Metropolix
- Rene
- Oxi One
- Hermod+
- Sinfonion
- Bard Quartet
- Ornament & Crime (quantizer duties if external needed)

### Song trick:
Use one 8- or 16-step melodic contour externally, but transpose Root by section. The phrase stays recognizable while the harmony changes.

---

## OSC section for sectional density

The OSC controls are ideal for “same phrase, different intensity.”

### Core arrangement controls:
- **Shift**: harmonic animation without total destabilization
- **Depth**: more phase-modulation edge and density
- **Shape**: wavefolding and additional brightness/complexity
- **Stretch**: powerful for choruses/lifts because it changes harmonics while keeping fundamental stable
- **Damped/Pulsar**: huge section-defining control; goes from subtle to percussive/gated/hard-sync behavior

### How to use in songs:
- Verse: low Shift, low Depth, low Shape, no Stretch
- Pre-chorus: gradually raise Shift and Stretch
- Chorus: more Shape + moderate Damped/Pulsar
- Breakdown: back to Centre or near-Centre
- Climax: high Damped/Pulsar + aggressive Morph mode + external sync or Mod interaction

### With other modules:
Patch attenuators, VCAs, or control buses into:
- Morph CV
- Shift CV
- Depth CV
- Shape CV
- Damped/Pulsar CV

Then use one macro source to create a coordinated build.

Good helpers:
- Quad VCA as CV processor
- Stages
- Maths
- Batumi
- Maestro
- Planar 2
- Tetrapad/Tete
- voltage block style sequencer

---

# 5. Morph as verse/chorus/bridge architecture

The manual strongly suggests two paths through the morph matrix:

- **left path**: more predictable
- **right path**: more nonlinear/extended

That maps beautifully to songwriting.

## Left path for core song sections
FMNT → FBPM → 2OP → XPM

Use this path for sections where the listener needs to keep hold of the identity.

- **FMNT**: intros, pads, cleaner hooks
- **FBPM**: basses, body, foundational riffs
- **2OP**: stronger choruses or melodic leads
- **XPM**: climax, final chorus, techno peak

Because control roles stay relatively stable, this path is best for live arrangement.

## Right path for contrast sections
FMNT → FBPM2 → 2OP2 → XPM2 → Asym

Use this path for:
- breakdowns
- bridges
- transitions
- weird middle-eight moments
- outros

These modes are more likely to produce “something new happened” without needing an entirely different voice.

### Performance idea:
Use Morph manually as a section marker:
- bars 1–16: FMNT
- bars 17–32: FBPM
- bars 33–48: 2OP
- bars 49–56: XPM
- bars 57–64: back to FBPM or Centre

This is a strong live-techno arrangement approach.

---

# 6. Mod oscillator for song-scale counterpoint and tension

The Mod oscillator is one of the most underappreciated arrangement tools here.

Because it can track:
- Root
- OSC
- UFG

you can create section-specific relationships without repatching much.

## Uses in songs

### A. Stable harmonic support
Set Mod to harmonic relationships above OSC for musical PM color.

Good for:
- bass and lead sections that must stay tonal
- repeated hooks that need richness but not chaos

### B. Detuned animation for choruses
The **Detune** control affects both Mod pitch relation and harmonic wavefolder animation.

That makes it perfect for:
- chorus widening
- “bloom” during peaks
- subtle movement over repeated motifs

### C. Section-specific tracking changes
Switch Mod tracking source by section:

- **Root tracking**: most stable
- **OSC tracking**: coherent with main pitch phrase
- **UFG tracking**: can produce more unusual rhythmic/timbral coupling

### D. Harmonic/Order as arrangement
You can start with free pitch offset in intro/bridge and move toward quantized harmonic or scale-locked behavior in the main section.

That feels like:
- chaos resolving into musical order
- or order dissolving into instability

Which is exactly what long-form arrangement needs.

---

# 7. UFG for phrases, envelopes, and transitions

The UFG is a big deal for full-song writing because it can behave as:

- envelope
- LFO
- audio oscillator
- clock
- pulse/gate source

This is almost a section designer by itself.

## Use 1: Clock the Δ–∑ with phrasing in mind
Because UFG is the internal clock source for Δ–∑, you can control not just rate, but feel.

- slower UFG = sparse phrase spacing
- faster UFG = denser melodic activity
- skewed function = asymmetrical rhythmic feel

### Song technique:
Keep the same Δ–∑ pattern, but change UFG Time/Skew between sections.  
Now the motif feels different without changing notes.

---

## Use 2: Pulsar synthesis for rhythmic identity
The Damped/Pulsar control ties UFG behavior to the main oscillator.

### Use it like this:
- low in intro
- medium in groove sections for subtle motion
- high in breakdown/percussion hybrid parts
- very high in climax for almost drum-like gating/hard-sync effects

This lets K-ACCUMULATOR become partly rhythmic, not just melodic.

---

## Use 3: Trigger modes as phrase articulators
The UFG trigger response modes can shape section feel:

- hard sync with subharmonic locking
- sync reversal
- sustain + sync variants

### With other modules:
Feed UFG Trig from:
- master clock divisions
- irregular trigger sequencer
- logic outputs
- Euclidean trigger generator
- manual trigger button/performance pads

This helps create:
- periodic accents
- fill bars
- phrase resets
- alternate section shapes

Good partners:
- Pamela’s
- Numeric Repetitor
- Steppy
- Temps Utile
- Grids
- logic modules like Compare 2, Plog, Joranalogue Compare 2

---

# 8. Δ–∑ as a full-song sequencer brain

The Δ–∑ section is perhaps the single strongest full-song feature.

## Why it helps arrangement
Most Eurorack sequences become static because they are either:
- fixed and repetitive
- or too random to be memorable

Δ–∑ offers a middle path.

## Use its controls as arrangement controls

### Chance
This is basically a **variation amount** macro.

- minimum = your hook
- medium = evolving verse
- high = fill/bridge/disruption
- back to minimum = return of the hook

This is song gold.

### Length
Use Length to zoom into pieces of the phrase.

- 16 steps = full section
- 8 steps = standard groove
- 4 steps = tension build
- 2 steps = breakdown mantra / techno lock
- back to 8 or 16 = release

### Smooth
Smooth is also dual-purpose:
- sub-audio: glide/humanization
- audio-rate: filtering/softening modulation behavior

Use it to move from:
- plucky stepped bassline
to
- legato acid-ish lead
to
- smoothed modulation texture

### Pattern switch
This is excellent for live song writing:
- write a “home” pattern
- temporarily mutate
- restore old value
- double pattern length for expansion

This can form verse/chorus or A/B song parts without another sequencer.

---

# 9. Full-song patch recipes

## Patch 1: Techno full-track engine
### Goal
Create intro, groove, breakdown, peak, outro from one K-ACCUMULATOR-centered patch.

### Modules
- K-ACCUMULATOR
- drum voices + trigger sequencer
- master clock
- stereo mixer
- reverb/delay
- filter or LPG
- sequential switch or mute module
- optional sampler/looper

### Patch
- Root quantized to a minor-ish 12-TET scale
- Root sent to OSC + UFG
- Δ–∑ output to OSC 1V/TZ attenuverter
- UFG looping, synced to master clock if needed
- Main outputs to stereo mixer and FX send
- moderate Morph CV from slow external modulation
- Damped/Pulsar under CV from a build envelope

### Arrangement
- **Intro**: FMNT, low Chance, high reverb, low Damped/Pulsar
- **Groove**: FBPM, 8-step Length, moderate Chance, drums enter
- **Lift**: increase Stretch + Shape + Detune
- **Breakdown**: pull drums, return near Centre, reduce Length to 4, raise Smooth
- **Peak**: XPM/XPM2, increase Damped/Pulsar, external sync or stronger Mod relation
- **Outro**: lower Chance to restore original motif, Morph back toward FMNT

Why it works:
- melody, rhythm, and timbre all evolve in coordinated ways
- the “hook” remains recoverable via Chance minimum

---

## Patch 2: One-voice ambient song
### Goal
Turn K-ACCUMULATOR into a whole evolving piece with long-form development.

### Modules
- K-ACCUMULATOR
- reverb
- delay
- looper or sampler
- slow modulation sources
- stereo VCA or mixer
- optional resonator/filter

### Patch
- Main outputs to long stereo FX chain
- Root in JI mode for more organic harmonic relations
- UFG very slow, modulating waveshaping
- Δ–∑ clocked slowly, feeding slight pitch movement or Morph CV
- Mod set to harmonic tracking from Root
- external macro CV controls Morph and Damped/Pulsar

### Arrangement
- Start at Centre with pure sine/cosine
- introduce Shift slowly
- layer recorded loops
- move FMNT → FBPM → 2OP2 over several minutes
- use Smooth and Chance as long-term variation
- collapse back to Centre at ending

Why it works:
- the stereo sine/cosine identity gives coherence
- continuous morphing creates narrative without abrupt breaks

---

## Patch 3: Bass + lead + percussion from one module using resampling
### Goal
Create a complete song by printing sections and repurposing the module.

### Modules
- K-ACCUMULATOR
- sampler/looper
- drum voices
- mixer
- filter/VCA
- effects

### Workflow
1. **Record bassline**
   - low Morph complexity
   - quantized Root
   - Δ–∑ low Chance
2. **Record chordal/texture layer**
   - higher Smooth
   - FMNT/2OP with more stereo FX
3. **Record rhythmic/pulsar layer**
   - high Damped/Pulsar
   - sub-audio UFG triggered from rhythm source
4. **Perform lead live**
   - stronger Morph movement
   - external pitch control or live Root shifts

This is one of the most realistic ways to make full tracks in Eurorack without needing many complete voices.

---

## Patch 4: Song sections via macro CV
### Goal
Use external CV tools to turn K-ACCUMULATOR into a section-based instrument.

### Modules
- K-ACCUMULATOR
- 4-channel CV sequencer or preset manager
- quad VCA / attenuator
- master clock
- drums and mixer

### Patch idea
Program 4 macro voltages:
- Macro 1: verse
- Macro 2: pre-chorus
- Macro 3: chorus
- Macro 4: breakdown

Route these through VCAs/offsets to:
- Morph CV
- Shift CV
- Shape CV
- Damped/Pulsar CV
- Δ–∑ Chance CV if available externally via utility workaround
- filter cutoff / FX send on external modules

Now one trigger or button press can transform the whole role of the voice.

This is one of the best ways to get actual “song sections” instead of knob-fiddling.

---

# 10. Best companion modules for full songs

## A. Sequencers
Even though K-ACCUMULATOR has internal sequencing behavior, external sequencing expands arrangement.

Good options:
- **Metropolix**: phrase variation, transposition, stage control
- **Oxi One / Hermod+**: song mode and recall
- **Rene**: exploratory and performative
- **Stillson Hammer / Vector / Eloquencer**: structured long-form phrases

Use external sequencers for:
- Root transpositions
- trigger changes to UFG
- switching external sync states
- modulation scenes

---

## B. Utilities and control modules
These are essential for song structure.

Best types:
- VCAs for CV
- offsets/attenuverters
- sequential switches
- logic
- manual gates/mutes
- precision adders
- clock dividers/multipliers

These turn K-ACCUMULATOR from “complex voice” into “arrangeable instrument.”

---

## C. Sampling and looping
This may be the single biggest missing ingredient in many Eurorack songs.

K-ACCUMULATOR can make many roles, but not all simultaneously unless you:
- record layers
- loop phrases
- resample transitions

Best options:
- Morphagene
- Lubadh
- Assimil8or
- Bitbox
- external DAW / Octatrack / SP-404 style device

---

## D. Performance mixer
A real mixer is often what makes “song” finally happen.

You need:
- mute groups
- aux sends
- level riding
- panning/stereo placement

Because K-ACCUMULATOR already outputs a stereo pair, it deserves a mixer that can preserve its width.

---

# 11. Concrete arrangement templates

## Template A: 5-part live modular song
### Intro
- Centre or FMNT
- slow UFG
- Root in JI or sparse scale
- no drums or only sparse percussion

### Part 2: Establish groove
- Δ–∑ low Chance, 8-step length
- Root to OSC
- add kick/hat modules
- moderate Shift, low Shape

### Part 3: Build
- increase Chance slightly
- add Stretch
- Mod Detune rises
- more FX send
- maybe move FBPM → 2OP

### Part 4: Breakdown
- remove drums or thin them out
- lower Length to 2 or 4
- raise Smooth
- maybe disengage Root from one destination
- use right-hand morph path for more alien timbre

### Part 5: Final return/climax
- restore original Δ–∑ pattern via Chance minimum
- move to XPM or XPM2
- increase Damped/Pulsar and sync intensity
- full drums and FX
- final reduction back to Centre or FMNT for outro

---

## Template B: Verse/chorus song
### Verse
- left-hand morph path
- stable scale
- Root to OSC only
- low Chance, moderate Length
- subtle Mod harmonic relationship

### Chorus
- Root to OSC + UFG
- wider Detune
- more Shape and Stretch
- increased stereo FX
- higher Damped/Pulsar
- maybe denser scale or stronger harmonic movement

### Bridge
- switch to right-hand morph path
- increase Chance
- alter Length
- maybe use external tracking/sync input
- reduce drums, spotlight the timbre

### Final chorus
- restore recognizable motif
- maximize modulation richness while staying musical

---

# 12. How to avoid getting stuck in a loop

This is the main problem you asked about. Here are practical K-ACCUMULATOR-specific solutions.

## Problem: “The patch sounds good, but nothing changes.”
### Solution:
Assign three independent change layers:
- one for pitch: Root or Δ–∑ Length/Chance
- one for timbre: Morph or Shift/Depth/Shape
- one for energy: UFG Time / Damped/Pulsar / drum density

Never rely on only one changing dimension.

---

## Problem: “Randomization ruins the motif.”
### Solution:
Use Δ–∑ Chance as temporary departure, then return to minimum.  
This module is designed for exactly that.

---

## Problem: “The song loses tonal focus.”
### Solution:
Use Root as the master anchor and keep Mod tracking harmonic or quantized during core sections. Save the weird freer states for transitions only.

---

## Problem: “Everything is dense all the time.”
### Solution:
Return to Centre often.  
The manual’s Centre concept is musically useful. It gives you a literal arrangement reset.

Think of Centre as:
- breakdown
- reset
- sparse verse
- pre-drop tension tool

---

## Problem: “I can make a cool sound, but not a section change.”
### Solution:
Use one external macro controller to move:
- Morph
- Damped/Pulsar
- Shape
- FX send
- drum mute state

A section change should affect multiple parameters at once.

---

# 13. Best musical roles for K-ACCUMULATOR in a full song

K-ACCUMULATOR works especially well as:

## 1. Main stereo lead/bass voice
Most obvious use. Strong for techno, IDM, ambient, electro-acoustic.

## 2. Harmonic centerpiece
Use Root and scale system to keep several other voices aligned.

## 3. Transitional sound design machine
Morph and Δ–∑ can generate fills, breakdown textures, and re-entry moments.

## 4. Percussive synth voice
With Damped/Pulsar, trigger-based UFG behavior, and sync interaction, it can produce highly rhythmic events.

## 5. Resampling source
Create one role, sample it, then repurpose it for the next role.

This last role is especially valuable for full-length music.

---

# 14. My strongest recommendations

If your goal is to make complete songs with this module, I would prioritize these approaches:

## Best approach 1
**Use Δ–∑ as your recoverable motif engine**  
Write a loop you love, then use Chance/Length/Smooth as arrangement controls.

## Best approach 2
**Treat Morph positions as song sections**  
Don’t just turn Morph randomly. Give each mode a role in your structure.

## Best approach 3
**Use Root as the harmonic spine of the patch**  
Let other modules follow or contrast it in deliberate ways.

## Best approach 4
**Add a sampler/looper**  
This instantly expands K-ACCUMULATOR from “one amazing voice” into “multiple song layers.”

## Best approach 5
**Use macro control and utilities**  
A full song usually requires coordinated voltage changes, not isolated parameter tweaks.

---

# 15. Example “minimum viable full-song rack” around K-ACCUMULATOR

A very effective composition-focused setup could be:

- **K-ACCUMULATOR**
- **master clock / modulation sequencer**
- **drum voice or sampler**
- **quad VCA / CV utility**
- **performance mixer**
- **stereo FX**
- **looper or sampler**
- **sequential switch or mute controller**

With just that, you can make:
- intro textures
- bass hooks
- melodic leads
- rhythmic pulses
- transitions
- arranged returns

That is enough for full tracks if you think in sections and commit to recording/resampling.

---

# Final takeaway

K-ACCUMULATOR is unusually well-suited to making **full-length songs** because it already contains the ingredients many modular systems lack:

- a tunable harmonic center
- a built-in evolving pattern source
- a controllable modulation/envelope/clock engine
- a structured timbral morphing system
- a way to depart from and return to a core motif

The key is to stop using it as a static “complex oscillator” and instead use it as a **sectional composition instrument**.

If you want, I can next turn this into any of these:

1. a **10-patch songwriting cookbook** for K-ACCUMULATOR  
2. a **section-by-section live performance template**  
3. a **companion module buying guide** specifically for building songs around it  
4. a **sample patch sheet** with exact cable routings and knob goals

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)