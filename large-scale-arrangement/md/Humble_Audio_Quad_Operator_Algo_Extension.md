# Humble Audio — Quad Operator Algo Extension

- [Manual PDF](../../manuals/Quad Operator Manual.pdf)

---

[Quad Operator Manual PDF](https://www.dropbox.com/paper/doc/print/JsIQoU7GbeAboEJku9ZgE?print=true)

# Humble Audio Quad Operator: using it to build full-length songs in Eurorack

The **Humble Audio Quad Operator** is much more than “a 4-op FM voice.” Read as a songwriter’s module, it is really a **small network of 4 oscillators plus one external FM bus**, with:

- global pitch control
- per-operator ratio/free tuning
- per-operator timbre shaping
- per-operator gain VCAs
- a full FM modulation matrix
- independent outputs for each operator
- optional **Algo expander** for saving/crossfading FM routings

That combination makes it unusually strong for the exact problem you described: getting beyond a nice loop and into **sectional development**, **arrangement**, and **long-form variation**.

---

## The key mindset shift: don’t treat it as one patch, treat it as a song engine

A lot of Eurorack patches stall because the sound is amazing but too static structurally. The Quad Operator helps because it can be treated as:

1. **One playable macro voice** for lead/bass/chords
2. **A bank of four related oscillators** for layered arrangement
3. **A modulation source** in LFO mode
4. **A scene morphing timbre system** via gains, matrix changes, and Algo crossfades
5. **A “song continuity” source** where multiple parts share a harmonic DNA

That last one matters. Full songs often need contrast, but they also need coherence. Quad Operator gives you both.

---

# What the manual suggests musically

From the manual, the most song-relevant features are:

- **4 operators with independent outputs**
- **Lock mode** for harmonic integer-ratio FM
- **Free mode** for independent oscillators
- **Shape crossfade** from sine → triangle → square → saw
- **Gain CV per operator**, which affects both:
  - output volume
  - how strongly that operator modulates others
- **Mod 1–4 sends per source**
- **External AR FM input** with its own gain and sends
- **LFO mode**
- **Reset input** for phase reset
- **Algo expander** with 3 saved algorithms + Live, and **crossfading between matrix states**

This means the module is especially good at songmaking through:

- **controlled harmonic FM**
- **voice stacking**
- **timbral automation**
- **algorithm morphing**
- **reusing one sound architecture across multiple sections**

---

# The big strategy: use Quad Operator for arrangement, not just tone

To make full songs, you need recurring tools for:

- **intro**
- **groove establishment**
- **verse / main A section**
- **lift / pre-chorus**
- **chorus / peak**
- **breakdown**
- **return**
- **ending**

Quad Operator can support all of those if you think in terms of **state changes over time**:

- different operator gains
- different FM depths
- different ratio relationships
- different shapes
- switching lock/free roles
- changing what is heard directly at the outputs
- using the Algo expander as “scene recall”
- crossfading algorithms gradually instead of hard switching

In other words, it excels at **evolving arrangement states**.

---

# 1. Use it as a “multi-role voice” across song sections

One of the strongest song techniques is to let the **same patch play different musical roles** over the course of a track.

## Example role progression

### Intro
- Use only **Op 1 output**
- All operators in **lock mode**
- Low FM depth
- Sine/triangle shapes
- Slow modulation of gain CV on one modulator
- Sparse melody or drones

### Verse
- Add **Op 2 as a hidden modulator**, not directly audible
- Introduce slight FM on Op 1
- Sequence a bass line from 1V/Oct
- Use a VCA/envelope on Gain 2 so the timbre has note articulation

### Pre-chorus
- Increase FM sends from Op 2 and Op 3
- Shift one shape toward square/saw
- Bring in **Op 2 output** mixed quietly beneath Op 1
- Add subtle LF FM for instability/tension

### Chorus
- Mix **Op 1 + Op 2 + Op 4 outputs**
- Increase operator gains and modulation sends
- Use broader envelopes, more harmonics
- If using Algo, crossfade to a brighter, denser algorithm

### Breakdown
- Drop back to only one operator output again
- Or switch one operator to **free mode** for unstable, drifting inharmonic texture
- Feed in external AR FM from a noise source or filtered drum loop

### Final chorus
- Return to lock mode harmonic clarity
- Use the most complex algorithm and widest output layering
- Open shape and gain CV more fully

This is how one voice becomes a full arrangement element rather than a static loop.

---

# 2. Exploit the independent outputs as separate arrangement layers

The manual notes **independent output per operator**. This is huge for song construction.

Instead of hearing the module as only one mixed FM result, treat each output as a separate recorded/processed layer.

## Patch concept: one source, multiple stems

Send:
- **Op 1** → main melodic voice chain
- **Op 2** → wavefolder / filter / VCA for a midrange counter-layer
- **Op 3** → bass-focused LPG or lowpass path
- **Op 4** → long reverb / shimmer / ambience

Even if the operators are cross-modulating internally, the separate outputs give you **parallel arrangement channels**.

### Why this helps for songs
You can mute/unmute or automate each layer across sections:
- intro: only Op 4 ambient wash
- verse: Op 1 + Op 3
- chorus: Op 1 + Op 2 + Op 3 + Op 4
- bridge: Op 2 alone through heavy delay
- outro: Op 4 reverb tail

This creates song form without repatching the core voice.

## Best companion modules
- **Mixer with mutes**: Happy Nerding Mix, WMD Performance Mixer, Befaco Hexmix
- **VCAs** for automation: Veils, Quad VCA, A-135-2
- **Stereo effects**: Mimeophon, FX Aid, Desmodus Versio, Magneto
- **Filters/LPGs**: QPAS, Three Sisters, Ripples, Optomix

---

# 3. Use lock mode for “musical sections,” free mode for “transition sections”

The manual makes a strong distinction:

- **Lock state** = integer frequency ratios relative to master pitch, good for harmonic FM
- **Free state** = independent oscillators, more inharmonic and flexible

This maps beautifully to song structure.

## Lock mode = stable musical identity
Use for:
- bass lines
- tonal hooks
- choruses
- sequenced riffs
- pads with harmonic stability

## Free mode = tension, transitions, atmosphere
Use for:
- intros
- bridges
- fills
- breakdowns
- risers
- noisy interludes

## Songwriting trick
Keep the “main song” mostly in lock mode. Then, for transitions:
- flip one operator to free
- modulate its ratio CV independently
- send it heavily into one or more locked operators
- fade it up only during transitions

That gives you section contrast without destroying the harmonic center of the piece.

### Example
- Ops 1–3 in lock mode for a stable chord/bass ecosystem
- Op 4 in free mode as a chaos/tension operator
- During verse: Gain 4 low or zero
- During build: raise Gain 4 and Mod sends into Ops 1–3
- At chorus drop: abruptly mute Gain 4, returning clarity

That’s a classic arrangement move in modular form.

---

# 4. The Gain CV inputs are your secret arrangement controls

One of the most important details in the manual:

> Gain CV affects both output level and how intensely the operator modulates other operators via its modulation sends.

This means each operator’s gain is effectively a **macro for presence + timbral influence**.

That is incredibly useful for long-form composition because one envelope or automation lane can:
- bring in a layer
- increase harmonic density
- raise perceived intensity
- reshape the whole FM network

## Practical use
Patch each operator’s Gain CV to:
- an envelope for note articulation
- a sequencer lane for section changes
- a slow CV source for long-form evolution
- a manual controller for live performance

## Song arrangement use cases

### A. Verse vs chorus
- Verse: low Gain on modulators, high Gain on carrier
- Chorus: higher Gain on modulators for brightness/complexity

### B. Build-up
- Slowly raise Gain 2 and Gain 3 over 16 or 32 bars
- FM complexity naturally increases with tension

### C. Breakdown
- Drop all modulator gains to near zero
- Leave one carrier output audible as a pure sine/triangle line

### D. “Human arrangement”
- Use random stepped CV, attenuated, into one Gain input
- Creates recurring but non-repetitive note-to-note brightness differences

This is one of the best anti-loop tools in the whole module.

---

# 5. Build songs from FM “scenes” with the Algo expander

The manual describes the **Algo expander** as a way to:
- save modulation send positions
- recall them
- crossfade between saved algorithms and live knob positions

This is perhaps the most direct “song mode” feature in the whole ecosystem.

Think of the saved states not as “algorithms” in a DX7 sense, but as:

- **Scene A** = intro/verse
- **Scene B** = chorus
- **Scene C** = breakdown
- **Live** = improvised fill / transition state

## How to use it for song sections

### Save:
- **A** = simple harmonic FM, mostly one carrier and one modulator
- **B** = denser cross-modulation for chorus energy
- **C** = self-mod and feedback-like wild texture for breakdown/noise bridge

Then:
- start on A
- crossfade slowly toward B over 8–16 bars
- snap to C for breakdown
- fade from C back to A for reset
- final chorus lives between B and Live with manual tweaks

## Why it matters
In many modular systems, changing FM routing for a new section means repatching or lots of hand movement. Here, you can make **repeatable, recallable arrangement transitions**.

That is exactly what helps turn ideas into songs.

## Great pairings
- performance CV source into crossfade input
- pressure/joystick controller
- preset sequencer
- automation lane from a DAW/CV interface

Examples:
- **Planar 2**
- **Tetrapad/Tête**
- **Pressure Points + Brains**
- **OXI One / Hermod / Metropolix modulation lanes**
- **DAW via ES-8 / FH-2**

---

# 6. Use external AR FM as a “section glue” input

The manual includes a dedicated **AR FM external modulation input** with:
- gain knob
- clipping LED
- gain CV
- modulation sends to all 4 operators

This is gold for arrangement because it lets an outside signal act like a shared energy source for the entire voice network.

## Best external sources for AR FM in songs

### Drums or percussion bus
Patch a percussion oscillator or even a full drum submix into AR FM.
- Low amount in verse
- More in chorus
- Result: the melodic voice feels rhythmically fused with the drums

### Another oscillator
Patch a fifth oscillator into AR FM.
- Tune it to root/fifth/octave
- Use it as a section-dependent “super modulator”
- Great for builds and choruses

### Noise or filtered noise
Use noise bursts or bandpassed noise into AR FM.
- Makes transitions, intros, and breakdowns more animated

### Resampled material
Patch a sampler loop, granular source, or radio/noise texture into AR FM.
- The song acquires a shared texture identity across sections

## Songwriting insight
This input helps solve a common Eurorack problem: the melody patch, bass patch, and drums often feel like separate islands. AR FM can make the Quad Operator react to another musical layer, creating **interdependence**.

That’s very song-like.

---

# 7. Make one operator the bass, another the lead, another the pad skeleton

Because operators can be **unlocked and tuned independently**, the module can act like a small oscillator bank.

That means you can create **interrelated parts** from a single module.

## Example “mini ensemble” patch

### Op 1: bass
- Free mode
- Sequenced by dedicated pitch CV
- Sine/triangle shape
- Lowpass filter after output
- Short envelope

### Op 2: lead
- Free mode
- Separate sequencer lane
- More complex shape
- Delay/reverb chain

### Op 3: drone/pad
- Free mode or locked to master
- Slow VCA envelope or sustained level
- Heavy reverb

### Op 4: hidden modulator
- Locked or free
- Not heard directly, or heard quietly
- FM source for others

## Why this works for songs
Even if these parts are separate, they share a sonic fingerprint. That helps with:
- coherence across sections
- natural transitions
- a “signature sound” for the track

This is especially useful in minimal techno, ambient, IDM, electro, soundtrack, and experimental song forms.

---

# 8. Use LFO mode to generate section automation from inside the same module

The manual says **VCO/LFO switch** changes the base frequency range and that LFO mode can generate phase-locked complex modulation signals.

This makes the Quad Operator capable of being not just the sound source but also part of the arrangement automation system.

## Approach
Dedicate one operator output in LFO mode as a modulation source for:
- filter cutoff
- VCA level
- effect send
- panning
- delay time modulation
- wavefolder symmetry

Because the operators can be related, you can create **musically synchronized internal modulations**.

## Song use
- In intro, use Quad Operator as modulation generator only
- In main section, switch back to VCO mode for audio use
- Or keep one operator in free-state LFO role while others are musical voices elsewhere in the patch ecosystem

If your surrounding system supports it, one great long-form strategy is:
- one Quad Operator operator = audible
- one = modulation source
- one = bass oscillator
- one = transition/noise FM source

That kind of multifunction patching is ideal for complete songs in small systems.

---

# 9. Use reset for repeatable phrasing and section starts

The manual notes a **Reset CV** input that resets all operators’ phase.

This is especially useful if:
- the module is being used as a modulation source
- you want consistent transient behavior
- you want section starts to feel intentional

## Song applications
Trigger reset:
- on the first step of every bar
- only at phrase boundaries
- only at section changes

This creates audible “re-centering,” which can make modular patches feel more composed and less drift-prone.

## Good uses
- percussive FM plucks where attack consistency matters
- synchronized bass re-entry after breakdown
- restarting an LFO-based timbral cycle at chorus downbeat

It’s subtle, but structure often comes from subtle repeatability.

---

# 10. Create full songs by sequencing timbre as much as pitch

The module’s design encourages a crucial compositional principle:

> Don’t just sequence notes. Sequence the FM relationships.

To get from loop to song, automate:
- operator gains
- matrix sends
- shape CVs
- ratio CVs
- external FM amount
- Algo crossfade

## Suggested modulation architecture
Use separate modulation sources on different time scales:

### Fast scale: note articulation
- envelopes into Gain CV
- accents into shape/gain
- per-step modulation from sequencer

### Medium scale: phrase variation
- 8 or 16-step CV lane into one ratio or shape input
- clocked random into one mod send via VCA
- occasional reset changes

### Long scale: section structure
- manual fader or joystick controlling Algo crossfade
- slow envelope over 32 bars into AR FM gain
- mute/unmute separate outputs through VCAs

That time-scale layering is how songs emerge.

---

# 11. Pair it with a sequencer that supports song form, not just loops

To turn Quad Operator into a song instrument, combine it with a sequencer that can handle:
- chained patterns
- per-track modulation lanes
- probability/mutation
- mutes
- fills
- scene changes

## Excellent partners
- **Intellijel Metropolix**: great for evolving hooks, transpositions, and phrase changes
- **Five12 Vector**: strong song structure and modulation lanes
- **Squarp Hermod+**: arrangement-friendly, multiple CV tracks
- **OXI One**: excellent for pattern chaining and performance
- **Winter Modular Eloquencer**: modular-friendly structured sequencing
- **NerdSEQ**: best if you want explicit tracker-style song arrangement

## How to patch with Quad Operator
Use the sequencer for more than pitch:
- 1V/Oct to master pitch
- separate modulation lanes to Gain CVs
- lanes to Shape CV
- triggers to reset
- slow CV to Algo crossfade
- gate patterns to external VCAs on operator outputs

This turns the module into a song-responsive instrument rather than a static voice.

---

# 12. Build verse/chorus contrast with processing chains, not only oscillator changes

Because Quad Operator has separate outputs, you can route each operator into a different post-processing voice.

## Example processing layout

- **Op 1** → lowpass filter → VCA → center mono
- **Op 2** → wavefolder → stereo delay
- **Op 3** → LPG → spring reverb
- **Op 4** → distortion → bandpass filter → sidechain VCA

Then use mutes/VCAs/effect sends to define sections.

### Section map
- intro: Op 3 + Op 4 only
- verse: Op 1 + subtle Op 2
- chorus: all operators
- bridge: Op 2 distorted alone
- final chorus: all operators plus increased FM and wider FX

This is a powerful way to get “produced track” structure from one synthesis source.

---

# 13. Use one operator as a sidechain-like dynamic modulator

A smart modular song trick: use one operator output as a control signal elsewhere.

Since outputs are audio/CV capable and run at 48kHz according to the manual, you can:
- rectify/filter one output to become an envelope-ish motion source
- use it to duck another layer
- use it to animate filter cutoff in another voice
- use it to modulate effect depth

This can create internal relationships that make a song feel arranged and glued together.

## Example
- Op 4 in LFO or low audio range
- Route Op 4 through envelope follower / rectifier / slew
- Use that CV to duck the Quad Operator lead reverb send during busy phrases
- Result: evolving arrangement dynamics without external DAW automation

---

# 14. Make transitions deliberately: risers, fills, breakdowns, and returns

Songs live or die on transitions. Quad Operator is very good at transitions because FM can move from clean to chaotic smoothly.

## Transition recipes

### Riser
- slowly increase Gain on one modulator
- sweep Shape from sine toward saw
- increase AR FM gain from noise or another oscillator
- add reverb send

### Fill
- briefly switch one operator to free mode
- raise self-modulation or cross-modulation
- route only that operator through delay
- mute it on the next downbeat

### Breakdown
- kill all modulator gains
- leave only one operator output
- move to LFO range or low register
- use reset sparsely

### Return/drop
- restore lock mode harmonic ratios
- reset phase on downbeat
- crossfade Algo into the denser scene
- unmute bass-focused output chain

This gives you the macro-movement full songs need.

---

# 15. Use harmonic restraint for the body of the song, save chaos for punctuation

The manual specifically recommends for harmonic FM results:
- VCO mode
- all operators in lock state
- detune at 12 o’clock
- shape fully CCW (sine)
- modulation sends at zero to start

This is excellent songwriting advice, not just synthesis advice.

## Translation into arrangement
For most of the track:
- keep the patch restrained
- make changes gradually
- use one or two modulator relationships at a time

For special moments:
- increase detune
- add overtone-rich wave shapes
- increase multiple modulation sends
- feed AR FM externally
- introduce free-mode instability

If everything is extreme all the time, it’s harder to make a song. The manual’s “sane beginning” approach is actually a recipe for arrangement headroom.

---

# 16. Example complete song workflows

## Workflow A: techno / electro track

### Modules to pair
- kick + percussion voices
- sequencer with pattern chaining
- mixer with mutes
- filter
- stereo delay/reverb
- 2–4 VCAs
- utility envelopes/LFOs

### Quad Operator role
- Op 1 = bass/lead carrier
- Op 2 = hidden harmonic modulator
- Op 3 = metallic top layer output
- Op 4 = transition modulator / noise-adjacent texture

### Song form
- **Intro**: Op 3 through delay, no kick
- **Groove in**: kick + Op 1 bass riff
- **Verse/A section**: restrained FM, low harmonic density
- **Build**: bring Op 4 gain up, increase AR FM from hi-hat bus
- **Drop/chorus**: crossfade to denser Algo, open Op 3 top layer
- **Breakdown**: bass muted, only Op 2/4 FX tails
- **Final section**: full mix, more shape brightness, wider effects
- **Outro**: return to Op 3 ambience

This works because the Quad Operator handles both hook and development.

---

## Workflow B: ambient / soundtrack piece

### Pair with
- slow sequencer or quantizer
- random voltage source
- large reverb
- delay
- matrix mixer
- LPG
- joystick/controller

### Quad Operator role
- All operators mostly in lock mode
- Very low FM depth initially
- Independent outputs to separate spatial paths

### Song form
- **Intro**: Op 4 alone, slow shape modulation
- **A section**: Op 1 enters with root drone, Op 2 quietly modulates
- **B section**: Algo crossfades to denser overtones, chords implied by ratio changes
- **Bridge**: one operator in free mode with drifting pitch CV
- **Climax**: external AR FM from another oscillator or tape loop
- **Resolution**: return to clean sine-leaning ratios

This creates a genuine narrative arc from one coherent sonic source.

---

## Workflow C: melodic IDM / experimental pop skeleton

### Pair with
- sequencer with multiple melodic tracks
- sampler/drums
- envelope follower
- multimode filter
- performance mixer
- clocked modulation source

### Quad Operator role
- Op 1 = lead voice
- Op 2 = bass support or hidden modulator
- Op 3 = pluck or countermelody output
- Op 4 = utility modulation or transition voice

### Song structure
- **Verse**: dry plucky lead, bass light
- **Pre**: shape and FM intensify
- **Chorus**: multiple outputs layered, wider FX, Algo scene B
- **Middle 8**: free-mode drifting operator and external FM from sampler loop
- **Final chorus**: return to harmonic lock with maximum gain complexity

This is a strong use case because FM can sound both percussive and lyrical.

---

# 17. A practical “song patch template” to try

Here is a concrete patch plan that should help produce a real full-length track.

## Core setup
- All operators in **lock**
- Start with all shapes at **sine**
- Start with all modulation sends at **0**
- Sequence master **1V/Oct**
- Use **Op 1** as the main audible output

## Add structure
- **Gain 2 CV** from envelope with moderate decay
- **Op 2 → Mod 1** raised slightly
- **Op 3 output** to a separate VCA/effect path, muted at first
- **Op 4** either:
  - hidden modulator for builds, or
  - free-mode transition oscillator

## Add arrangement control
- slow CV or manual control to:
  - Gain 3
  - Shape 1
  - AR FM Gain CV
  - Algo crossfade if available

## Song sections
### Intro
- only Op 3 effected output
- no Op 1 bass/melody yet

### Verse
- bring in Op 1
- slight Op 2 modulation

### Pre-chorus
- increase Gain 2 and Shape 1
- unmute a little Op 3

### Chorus
- unmute Op 3 fully
- bring Op 4 modulation in
- crossfade to brighter Algo

### Breakdown
- mute Op 1
- leave Op 3/4 with reverb and reduced pitch density

### Final chorus
- reset phase on downbeat
- full Op 1 + Op 3 + stronger Op 2 modulation
- external AR FM from percussion or another oscillator

That’s a full song architecture from one module.

---

# 18. Best supporting module categories for making songs with Quad Operator

If your goal is specifically long-form composition, these are the most useful companions:

## 1. Song-capable sequencer
For pattern chaining and modulation lanes.

## 2. Performance mixer
For bringing independent operator outputs in and out by section.

## 3. VCAs
Critical because Gain CV is central to this module’s musicality.

## 4. Envelopes and function generators
To animate operator gain and timbre per note and per phrase.

## 5. Effects
Especially stereo delay/reverb to turn outputs into distinct arrangement layers.

## 6. Filters / LPGs
Helpful for making operator outputs occupy different song roles.

## 7. Modulation recorder or controller
Joystick, faderbank, pressure controller, preset manager, CV recorder.

## 8. External audio source
To exploit the AR FM input musically.

---

# 19. The most effective songmaking techniques with this module

If I had to boil it down as a Eurorack musician, I’d say the Quad Operator becomes a song machine when you use it for these five things:

## 1. Sectional timbre states
Different FM networks for intro/verse/chorus/breakdown.

## 2. Parallel output arrangement
Each operator output as a separate stem or layer.

## 3. Gain-CV-driven orchestration
Since gain changes both loudness and FM influence.

## 4. Harmonic vs inharmonic contrast
Lock mode for song body, free mode for transitions and tension.

## 5. External interaction
AR FM lets outside material animate the whole patch.

Those are the levers that move you from “great loop” to “track with form.”

---

# 20. Final advice: compose the arrangement first, then deepen the patch

With a module this flexible, it’s easy to get lost in FM complexity. For full-length songs, I’d recommend this workflow:

1. Start with a **simple locked patch**
2. Define **3 or 4 song sections**
3. Decide which operators are audible in each section
4. Program **Gain CV changes** first
5. Add **one FM relationship per section**
6. Then add:
   - shape motion
   - external AR FM
   - free-mode transitions
   - Algo morphing

That keeps the patch musical and lets complexity serve structure.

The Quad Operator is especially strong for full songs because it can provide:
- a consistent sonic identity
- multiple arrangement layers
- evolving harmonic complexity
- recallable/morphable structural states

In short: it’s not just a sound design module. It’s a **form-building module** if you patch it with VCAs, a good sequencer, a mixer, and a plan for section changes.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)