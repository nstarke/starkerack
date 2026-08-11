# xaoc Devices — Sopot

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Fractaos Manual PDF](sandbox:/mnt/data/Fractaos_User_Manual_v1.5.pdf)

# Kaona Fractaos: creative patch ideas and module pairing suggestions

Fractaos is not “just another digital oscillator.” It’s really a **4-voice fractal synthesis engine** with:

- 4 polyphonic voices
- 8 oscillators total in driver/follower pairs
- internal ADSR per voice
- internal fractal/LFO modulation behavior
- resonant fractal filter per voice
- MIDI, 1V/oct, and trig per-voice control
- Drone mode
- Multitimbral preset-per-voice mode

That means it can function as:

- a **polyphonic voice module**
- a **4-part multitimbral sound source**
- a **self-contained drone orchestra**
- a **hybrid tonal/noise/percussion generator**
- a **complex modulation-responsive digital texture machine**

Below are practical and creative ways I’d use it in a Eurorack system.

---

# 1. First: what Fractaos seems best at musically

From the manual, Fractaos excels in these zones:

- **Animated harmonic complexity** rather than static timbres
- **Organic drift and unstable spectra**
- **Stereo drones and chord clouds**
- **Percussive models blended with pitched geometry**
- **Preset-driven performance setups**
- **Multitimbral MIDI voice allocation**
- **Audio that rewards slow CV movement**

This suggests pairing it with modules that provide:

- nuanced CV animation
- spatialization
- filtering outside its internal fractal filter
- voice management
- performance macro control
- rhythmic note/gate generation
- rich effects, especially delay/reverb/granular

---

# 2. Important practical takeaways from the manual

These matter for patch planning:

## CV inputs and ranges
Fractaos has 8 CV inputs with attenuators:

- **bipolar ±5V** for:
  - Texture
  - Pitch
  - Spread
  - Morph

- **unipolar 0–5V** for:
  - Speed
  - Amount
  - F-Chaos
  - P-Chaos

So if you feed it modulation from Eurorack sources, it helps to have:

- attenuverters
- offset generators
- voltage processors
- slew limiters
- utilities for converting bipolar to unipolar

## Parameters that seem especially performance-sensitive
The most musically exploitable controls look like:

- **Morph**
- **Spread**
- **Texture**
- **Chaos / Primitive Chaos**
- **Speed / Amount**
- **Fractal Type / Primitive Type** by hand

## One limitation to exploit intelligently
- **Depth / Primitive Depth are stepped and not CV-modulatable**
  
So for live use, treat Depth like a **scene change** or timbral range selector rather than an animated modulation destination.

---

# 3. Best companion module categories

## A. Modulation utilities
Probably the best category to pair with Fractaos.

### What to use
- Make Noise Maths
- Frap Tools 321
- Happy Nerding 3xMIA
- Intellijel Triplatt
- Befaco A*B+C
- Joranalogue Select 2 / Contour 1
- After Later/Doepfer attenuators and offsets

### Why
Fractaos already has deep internal behavior, but **external modulation scaling** will make it far more playable. Especially because some inputs want 0–5V and others want ±5V.

### Great use
- Send a slow random CV into **Chaos**, but attenuate heavily
- Offset an LFO into **Amount** so it lives in the “sweet spot”
- Crossfade between two modulation sources before **Morph**

---

## B. Slow organic modulation sources
Fractaos sounds like it loves long-form movement.

### Good options
- Make Noise Wogglebug
- Mutable Marbles
- Xaoc Batumi
- DivKid Ochd / Ochd Expander
- Instruō øchd-style multi-LFOs
- Joranalogue Orbit 3
- Verbos Random Sampling
- Nonlinear Circuits chaotic modulators

### Why
The manual repeatedly points toward:
- drift
- chaos
- texture evolution
- slow filter movement
- animated detune

### Great patch targets
- **P-Chaos** for primitive instability
- **F-Chaos** for driver instability
- **Speed** for changing fractal envelope speed
- **Spread** for living detune/chord behavior
- **Texture** for evolving resonance/formant content

### Patch idea
Use 3 independent slow LFOs:
- LFO 1 → Morph
- LFO 2 → Texture
- LFO 3 → P-Chaos

Then manually adjust:
- Fractal Type
- Primitive Type
- Depth

This should turn Fractaos into an evolving, semi-self-composing digital ecosystem.

---

## C. Polyphonic sequencers / MIDI-CV tools
Fractaos is unusually capable as a poly voice in Eurorack.

### Strong matches
- Expert Sleepers FH-2
- Endorphin.es Shuttle Control
- Hexinverter Mutant Brain
- Tubbutec uTune / MIDI-CV ecosystems
- OXI Coral/One ecosystem if integrated externally
- Squarp Hermod+
- Winter Modular Eloquencer + MIDI/CV helpers

### Why
Fractaos can take:
- TRS MIDI
- 4x trig
- 4x 1V/oct

That opens multiple workflows:
- keyboard polyphony
- DAW-driven chord sequencing
- per-voice modular sequencing
- multitimbral routing by MIDI channel

### Best use
Use a MIDI-CV interface that can send:
- four pitch CVs
- four gates
- velocity or aftertouch via MIDI

Then let Fractaos be a **complete polyphonic synth voice** while the rest of the modular provides modulation and effects.

---

## D. External filters
Fractaos has internal filtering/texture behavior, but external filtering can turn it into something much larger.

### Great pairings
- Stereo filter: QPAS, Ikarie, Dual Dagger
- Character filter: Belgrad, Three Sisters, Morgasmatron
- Clean poly-ish shaping: ADDAC, Doepfer dual filters
- LPGs: Optomix, LxD, Natural Gate

### Why
Fractaos can be spectrally dense, noisy, and formant-rich. External filtering gives you:
- macro sculpting
- contrast against the internal fractal texture filter
- animation between digital complexity and analog restraint

### Patch ideas
1. **Drone mode into stereo filter**
   - Fractaos in Drone
   - Spread in chord zone
   - external slow CV to Morph/Texture
   - stereo filter sweeping slowly
   - big reverb after

2. **Percussion model into LPG**
   - Use Kick/Snare/Tom
   - external trig
   - route audio through LPG for woodier transient behavior
   - especially nice for turning digital drums into more acoustic-feeling hits

---

## E. Effects: delay, reverb, granular, spectral
This is maybe the biggest payoff category.

### Strong matches
- Make Noise Mimeophon
- Strymon Magneto / Starlab
- XAOC Timiszoara
- Desmodus Versio
- Noise Engineering electus/Imitor style delays
- Mutable Clouds/Beads-inspired modules
- Qu-Bit Aurora / Nautilus / Prism
- Arbhar, Morphagene
- Eventide/H90 external send-return if using line conversion

### Why
Fractaos naturally produces:
- internal detail
- spectral movement
- noisy tails
- pseudo-acoustic and digital textures

Effects turn those into:
- cinematic pads
- generative ambience
- metallic dub echoes
- granular swarms
- glitched harmonic clouds

### Specific patch
**Fractal ensemble wash**
- Main fractal: Ensemble or Cluster
- Primitive: Hilbert or Fibonacci
- Slow modulation to Morph and Texture
- Drone mode chord spread
- Into Mimeophon with moderate Halo and Color
- Then huge reverb

Result: shimmering evolving orchestra-from-another-planet.

---

## F. VCAs and macro performance mixers
Fractaos is deep enough that you’ll want gesture control.

### Recommended types
- Quad VCA
- Stereo VCA
- performance mixer
- CV-controlled crossfader
- macro controller

### Good modules
- Intellijel Quad VCA
- ALM Tangle Quartet
- Happy Nerding PanMix / 3xVCA
- WORNG Soundstage / vector mixers
- Planar 2
- Tetrapad + Tête
- Faderbank modules
- Befaco Hexmix ecosystem

### Why
Since Fractaos can be:
- 4 voices
- 2 stereo outs
- preset/live hybrids in MULTI

You’ll want to control:
- level
- CV depth externally
- wet/dry effect blends
- transitions between calm and chaos

### Performance trick
Use a joystick or macro fader to simultaneously control:
- external VCA on Fractaos audio
- CV amount sent to Chaos
- effect send level
- filter cutoff

One gesture can move from “stable glass pad” to “fractured storm noise.”

---

# 4. Creative patch strategies

## Patch 1: Four-voice polyphonic “alien string machine”
**Goal:** lush playable poly synth

### Setup
- MIDI keyboard or sequencer into Fractaos
- Polyphonic mode on a single MIDI channel
- Choose:
  - main fractal: Fibonacci / Koch / Julia
  - primitive: Rössler / Hilbert / Sierpinski
- Moderate Texture
- Slow Speed
- Amount medium-low
- Slight Spread
- ADSR with soft attack and long release

### Add modules
- Stereo chorus, ensemble, or reverb
- Optional stereo analog filter
- Slow LFO into Morph

### Why it works
Fibonacci/Koch/Hilbert-like shapes should give harmonically rich but playable tones; Fractaos’s internal motion avoids the static feel of ordinary digital polys.

---

## Patch 2: Drone cathedral
**Goal:** giant harmonic drone installation

### Setup
- Activate Drone mode
- Put Spread in upper chord zone
- Try:
  - main fractal: Cloud / Cluster / String / Lorenz
  - primitive: Dragon / Hilbert / Hénon
- Very slow modulation on:
  - Texture
  - Morph
  - F-Chaos
  - Speed

### Add modules
- stereo filter
- reverb
- very slow panner
- submixer for parallel dry/wet

### Bonus
Use one of the microtonal Drone chords:
- Just intonation
- 7-limit flavor
- 19-TET slice
- Bohlen-Pierce subset

### Why it works
Fractaos’s Drone mode treats all 8 oscillators individually, which is much more like a small drone ensemble than a regular detuned oscillator.

---

## Patch 3: Fractal percussion laboratory
**Goal:** weird percussion that still feels “played”

### Setup
- Use Drum fractals:
  - Kick
  - Tom
  - Snare
  - HiHat
  - Cymbal
- Trigger voices separately with modular gates
- Primitive set to a geometric fractal
- Use Morph to blend percussion body with pitched/harmonic tail

### Add modules
- trigger sequencer
- probability trigger source
- logic modules
- LPG or transient shaper
- delay on snare/cymbal only if you can route externally

### Creative use
Because Drum fractals still respond to MIDI pitch or CV pitch coloration, you can sequence tuned toms or electro-percussion lines instead of just static drums.

### Patch expansion
Use:
- Euclidean trigger module
- random skip/probability
- sequential switch for changing incoming pitch CV patterns

Result: hybrid kit / melodic percussion voice.

---

## Patch 4: FM-ish metallic machine
**Goal:** exploit simplified FM mode

The manual says simplified FM mode is:
- Loop OFF
- Trig OFF
- Morph ON
- Spread OFF
- Chaos OFF

Then **Amount** becomes bipolar around center:
- below center = internal feedback
- above center = primitive 2 modulates main fractal frequency

### Setup
- Use geometric main fractals, not textures/drums
- Try:
  - main: Mandelbrot, Sierpinski, Koch, Dragon
  - primitive: Rössler, Logistic, Hilbert, Julia
- Sweep Amount slowly around center

### Add modules
- precision offset/attenuverter
- envelope follower or manual CV controller
- wavefolder or analog filter after Fractaos

### Why
This should create metallic, unstable, operator-like digital timbres unlike classic DX/FM voices.

### Advanced move
Use a CV recorder or joystick to “play” the Amount region around the FM center point. That zone is likely extremely expressive.

---

## Patch 5: Multitimbral modular “band”
**Goal:** 4 independent characters from one module

### Setup
Use MULTI mode with separate MIDI channels per voice.

Example layout:
- Voice 1: bass preset
- Voice 2: chord pad preset
- Voice 3: percussion preset
- Voice 4: lead/live voice

### Add modules
- MIDI sequencer with multitrack channel output
- external mixer
- stereo FX bus
- clocked modulation synced across all voices

### Why
Fractaos can effectively become a **tiny self-contained digital ensemble**.

### Creative angle
Leave one voice in **LIVE** while the others use presets. Then perform the live voice from the panel while the preset voices remain stable.

This is one of the most unique features in the manual.

---

## Patch 6: CV-addressed chaos sculpture
**Goal:** let modular CV “play the fractal”

### Setup
Use CV sources into:
- F-Chaos
- P-Chaos
- Morph
- Texture

### Add modules
- stepped random
- slewed random
- voltage-addressable sequencer
- sample & hold
- clock divider

### Trick
Clock a sample-and-hold slowly and send it to Primitive Chaos while a slewed random moves Morph. Keep the base sound simple. You’ll get a consistent identity with evolving internal fracture.

### Best partner modules
- Marbles
- Turing Machine + expanders
- Ornament & Crime
- Klavis Twin Waves as modulation source
- stochastic sequencers

---

## Patch 7: Chord machine with external quantized modulation
**Goal:** harmonic motion without changing played notes

### Setup
In Drone mode, Spread accesses predefined chord sets. But outside Drone, Spread handles detune. So exploit both states performatively.

### Add modules
- gate utility or manual switch
- CV generator into Pitch
- precision adder
- quantizer
- sequential switch

### Idea
Use Pitch CV to transpose the drone chords while manually moving Spread through the chord section. Then process with reverb and filtering.

### More advanced
Use 4 pitch CVs differently per voice even in Drone mode, so each pair gets independent transposition while the global Spread still organizes the overall 8-oscillator structure.

This should create shifting harmonic fields rather than fixed chords.

---

## Patch 8: External resonator or physical-model hybrid
**Goal:** turn Fractaos into an exciter for resonant systems

### Pair with
- Mutable Rings / Resonator modules
- 2hp Pluck-style resonators
- feedback resonators
- Karplus/comb filters
- spring reverb tanks

### Why
Fractaos has:
- noisy textures
- percussive models
- harmonically jagged waveforms
- unstable transients

Those can act as fantastic excitation sources.

### Patch examples
- HiHat fractal into resonator for synthetic metallic tuned percussion
- String/Cloud texture into comb filter for haunted bowed ambience
- Kick/Tom into resonant lowpass for huge cinematic booms

---

## Patch 9: Audio-rate modulation ecosystem
**Goal:** brutal digital complexity

Fractaos doesn’t expose raw oscillator internals, but you can still build an ecosystem around it.

### Pair with
- wavefolder
- analog distortion
- bitcrusher
- sample rate reducer
- PLL
- frequency shifter
- ring modulator

### Recommended types
- wavefolder: Serge-style, Intellijel Bifold, Bastl Timber
- frequency shifter: Xaoc Koszalin, Doepfer A-126-2
- distortion: Ruina Versio, Data Bender, Industrial Music Electronics style processors

### Why
Fractaos already creates rich spectra. Nonlinear post-processing can reveal hidden motion and sidebands.

### Great sounds
- Mandelbrot + FM mode into wavefolder
- Cloud/Storm into frequency shifter
- Rule30 bass into saturation and LPG
- Cymbal into bitcrusher and reverb

---

## Patch 10: Fractaos as the “digital top layer” of a larger patch
**Goal:** use it as a spectral contrast voice

### Pair with
- analog VCO bass voice
- sample-based drum voice
- west-coast bongo voice
- field recording/granular layer

### Why
Fractaos shines when contrasted against simpler materials.

### Example arrangement
- Analog mono bass underneath
- Fractaos poly pad above
- Fractaos percussion voice in MULTI
- noise/snare elsewhere
- long stereo FX send only on Fractaos

This keeps the mix intelligible while preserving Fractaos’s complexity.

---

# 5. Best module pairings by musical role

## For ambient / drone
- Ochd or Batumi for slow modulation
- QPAS / Ikarie / stereo filter
- Mimeophon / Magneto / Desmodus
- Planar 2 for macro gestures
- Clouds/Beads/Arbhar for granular diffusion

## For techno / industrial
- trigger sequencer
- Euclidean sequencer
- logic modules
- distortion / wavefolder / bitcrusher
- LPG or snappy VCA
- performance mixer

Use Rule30, Drum fractals, Logistic, Collatz, Hénon, and simplified FM mode.

## For generative / experimental
- Marbles
- Turing Machine
- Ornament & Crime
- chaotic CV source
- quantizer
- resonator
- granular effect

Use Lorenz, Dragon, Hilbert, Cluster, Storm, and microtonal Drone chords.

## For keyboard poly synth use
- FH-2 / Shuttle Control / Mutant Brain / Hermod+
- stereo chorus/reverb
- external filter
- expression controller or aftertouch-capable controller

Use Fibonacci, Julia, Koch, Sierpinski, Rössler.

---

# 6. Specific high-value modulation targets

If I were patching Fractaos, these would be my priority CV destinations:

## 1. Morph
Probably the richest continuously playable parameter.

Use:
- slow triangle LFO
- joystick
- pressure CV
- envelope follower

## 2. Texture
Likely the fastest route to “alive” timbral animation.

Use:
- slow random
- ADSR from external keyboard dynamics
- accent CV from sequencer

## 3. F-Chaos / P-Chaos
Use carefully scaled CV here. Small moves probably matter more than large ones.

Use:
- attenuated random
- stepped CV with slew
- burst envelopes

## 4. Spread
Especially powerful in Drone mode.

Use:
- macro controller
- manually performed offset voltage
- slewed stepped random for slow chord migration

## 5. Amount / Speed
These govern the internal fractal envelope/LFO behavior and FM intensity contexts.

Use:
- synced LFOs
- manual offset
- envelope control for per-note articulation changes

---

# 7. Patches that exploit manual-specific quirks

## A. Preset surfing performance patch
Because LOAD mode applies presets immediately for auditioning, you can use Fractaos almost like a performance preset instrument.

### Setup
- sequence running into Fractaos
- go into LOAD
- audition presets in time with the music
- use manual “match the knobs to arrows” method to recover live control

This is ideal if you want morphing between predesigned scenes during a set.

---

## B. LIVE + preset hybrid in MULTI
Because LIVE voices in MULTI still respond to the panel, you can do this:

- Voice 1: preset bass
- Voice 2: preset pad
- Voice 3: LIVE lead
- Voice 4: LIVE FX/percussion

Then the front panel becomes a shared live sculptor for only the LIVE voices while other voices stay fixed.

That’s unusually powerful for a Eurorack oscillator.

---

## C. Sustain = 0 envelope trick
The manual notes that Release still matters when Sustain is 0.

Use this for:
- pseudo-plucks with variable tail
- disappearing notes if held
- expressive early note release gestures from keyboard/sequencer

It’s especially useful for:
- Drum + geometric Morph patches
- mallet-like plucks
- sparse generative melodies

---

# 8. Suggested “dream systems” around Fractaos

## Small system
- Fractaos
- Quad modulation source
- utility attenuverter/offset
- stereo filter
- delay/reverb
- small mixer

This is enough for ambient, drones, and performance textures.

## Poly performance system
- Fractaos
- MIDI-CV/poly controller
- macro controller
- stereo chorus/filter
- reverb
- performance mixer

This makes Fractaos the centerpiece synth voice.

## Experimental lab system
- Fractaos
- random/chaotic CV generator
- resonator
- bitcrusher/distortion
- granular processor
- logic and trigger sequencer

This gets the most out of its fractal/noise/percussion identity.

---

# 9. Concrete module recommendations

If you want especially synergistic pairings, I’d shortlist:

## Utilities
- Happy Nerding 3xMIA
- Intellijel Triplatt
- Make Noise Maths

## Modulation
- DivKid Ochd
- Xaoc Batumi
- Mutable Marbles

## Poly/MIDI control
- Expert Sleepers FH-2
- Squarp Hermod+
- Endorphin.es Shuttle Control

## Filtering
- Make Noise QPAS
- Bastl Ikarie
- XAOC Belgrad

## Effects
- Make Noise Mimeophon
- Desmodus Versio
- Strymon Magneto
- Mutable/clone Clouds or Beads
- Instruō Arbhar

## Performance control
- Intellijel Planar 2
- 4ms Catalyst Controller style macro tools
- tetrapad/fader-style controllers

---

# 10. Final creative takeaway

The most interesting way to use Fractaos is **not** as a static oscillator replacement.

It becomes special when you treat it as:

- a **fractal ensemble**
- a **preset/live hybrid instrument**
- a **drone chord engine**
- a **digital percussion + harmonic blend source**
- a **polyphonic texture organism** that needs carefully curated modulation

My personal favorite uses based on the manual would be:

1. **Drone mode + chord Spread + slow CV + huge reverb**
2. **MULTI mode with 2 preset voices and 2 LIVE voices**
3. **Drum fractals morphed into geometric tails**
4. **Simplified FM mode with a joystick controlling Amount**
5. **Microtonal drone chords through stereo filtering and granular effects**

If you want, I can also turn this into:

- a **“best companion modules by budget” list**
- a **genre-specific patch guide** for ambient/techno/industrial
- or a **10-patch recipe sheet** with exact signal flow diagrams.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)