# Kaona Instruments — Fractaos

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Fractaos Manual PDF](#)

# Creative patch ideas for **Kaona Fractaos**

Fractaos is not just “a polyphonic oscillator.” It’s really a **4-voice fractal sound engine** with:

- 8 real-time oscillators in 4 driver/follower pairs
- per-voice ADSR and fractal filter
- CV over key timbral axes
- polyphony via MIDI or 4x trig + 4x 1V/oct
- drone mode
- multitimbral preset-per-voice mode
- geometric, texture, and drum fractal models
- a special primitive/LFO/FM architecture

That means it works especially well when treated as one of these:

1. **A polyphonic voice block**
2. **A drone orchestra**
3. **A timbral percussion generator**
4. **A multitimbral digital ensemble**
5. **A modulation destination for slow, coordinated CV ecosystems**

Below are practical and creative ways I’d use it in a Eurorack system.

---

## First: what Fractaos seems to want around it

Because Fractaos already contains so much synthesis internally, the most useful companion modules are less “another oscillator” and more:

- **polyphonic CV/gate sources**
- **MIDI-to-CV / polyphonic sequencers**
- **macro modulation sources**
- **VCAs / mixers / stereo processors**
- **character filters / resonators / wavefolders**
- **granular / delay / reverb**
- **performance controllers**
- **clocked modulation / random**
- **quadraphonic or polyphonic utility modules**

It appears especially strong when you modulate:

- Texture
- Morph
- Spread
- Pitch
- Chaos / Primitive Chaos
- Speed / Amount

Depth and Primitive Depth are stepped and not CV controllable, so those are better treated like “structural scene changes” set by hand or preset.

---

# Core strengths to exploit

## 1. Polyphonic fractal timbre with external sequencing
Fractaos has 4 separate trig inputs and 4 separate 1V/oct inputs. That opens up **true modular polyphony** without requiring MIDI.

### Pair it with:
- **Quad sequencers / polyphonic sequencers**
  - Winter Modular Eloquencer with expander
  - Frap Tools USTA
  - Intellijel Metropolix with supporting utilities
  - Five12 Vector Sequencer
  - OXI One via MIDI or CV
- **4-channel quantizers**
  - Intellijel Scales + utilities
  - Shakmat Bard Quartet
  - ADDAC quantizer options
- **4-channel gate generators / trigger routers**
  - Mutable Grids-style trigger generators
  - ALM Pamela’s Pro Workout
  - vpme Euclidean Circles
  - Steppy / Varigate style modules

### Creative result:
Use Fractaos as a **polyphonic “ensemble oscillator”** where each voice gets slightly different pitch rhythm and trigger phrasing. Since each voice has its own oscillator pair and filter, even simple note sets can bloom into dense harmony.

**Patch idea:**  
Send four related but non-identical pitch lines into the 1V/oct inputs. Use a shared slow CV into Morph and Texture. This creates the impression of a living chamber ensemble rather than 4 identical voices.

---

## 2. Drone machine with harmonic spread
Drone mode is one of the most unique features here. In Drone, all 8 oscillators run continuously, and Spread becomes either:

- near-unison cluster
- progressive octave spreading
- or one of **13 chord / microtuning maps**

This is huge.

### Pair it with:
- **Slow modulation generators**
  - Make Noise Maths
  - Xaoc Batumi
  - Frap Tools Falistri
  - Joranalogue Orbit 3 / Contour 1
- **Random / chaotic CV**
  - Make Noise Wogglebug
  - SSF Ultra-Random Analog
  - Mutable Marbles
  - Chaos modules like NLC Triple Sloths
- **Stereo ambience**
  - Mimeophon
  - Magneto
  - XAOC Timiszoara
  - Strymon Starlab
  - Desmodus Versio
  - Data Bender for digital fracture
- **Resonators / spectral processors**
  - Mutable Rings (as processor/exciter destination)
  - 4ms Spectral Multiband Resonator
  - Xaoc Koszalin / Minsk style stereo processing
  - fixed filter banks

### Creative result:
Fractaos becomes a **self-contained generative drone orchestra**. The chorded Spread zone is especially good for long-form harmonic evolution.

**Patch idea:**  
- Enable Drone mode  
- Set a texture fractal like Cloud, Cluster, or Ensemble  
- Send ultra-slow CV to Texture and Chaos  
- Send stepped random CV to Spread, attenuated so it glides between chord zones  
- Run stereo outs into a long feedback delay and reverb  
This gives shifting harmonic weather rather than a static drone.

---

## 3. Multitimbral “4-module-in-1” setup
MULTI mode is very powerful: each voice can load a different preset and respond on separate MIDI channels.

This means Fractaos can act like:

- voice 1 = bass
- voice 2 = pad
- voice 3 = percussion
- voice 4 = lead

### Pair it with:
- **MIDI sequencers / grooveboxes**
  - Elektron Digitakt / Syntakt
  - Squarp Hapax
  - OXI One
  - Cirklon
  - Deluge
  - Keystep Pro
- **MIDI controllers with aftertouch**
  - Osmose
  - Hydrasynth
  - Keystep 37 / 49 / Pro
  - expressive MPE-adjacent controllers if channel pressure is usable
- **Performance mixer**
  - WMD Performance Mixer
  - Toppobrillo / Tex Mix systems
  - Befaco Hexmix
  - Happy Nerding PanMix
  - Cosmotronic mixer utilities

### Creative result:
Use Fractaos as a **complete digital multitimbral synth brain inside Eurorack**, then process its stereo output with analog modules.

**Patch idea:**  
Create four presets:
- kick/snare percussion fractal
- bass using Rule30 or Cantor
- shimmering pad using Koch/Julia
- unstable lead using Lorenz/Hénon

Sequence over separate MIDI channels from Hapax or OXI One. Then route Fractaos through a stereo filter, compressor, and effects chain for an entire track voice in one module.

---

# Excellent companion module types

## A. Polyphonic or quad envelopes / VCAs after Fractaos?
Since Fractaos outputs stereo mix rather than per-voice audio outs, external VCAs won’t give per-voice control unless you’re controlling another downstream layer. Still useful for:

- global tremolo
- sidechain dynamics
- voltage-controlled send effects
- performance muting

### Good pairings:
- Happy Nerding 3xVCA / 4x Stereo Mix
- Intellijel Quad VCA
- Xaoc Tallin
- stereo VCAs and crossfaders

### Creative use:
Put a stereo VCA after Fractaos and animate whole textures rhythmically with envelopes or an envelope follower from drums elsewhere in the patch.

---

## B. Character filters after the stereo output
Fractaos already has internal fractal filters, but external filtering can radically reshape its digital edge.

### Try:
- **Warm analog stereo filter**
  - Rossum Linnaeus
  - Bastl Ikarie
  - QPAS
  - Morgasmatron
  - Stereo Dipole
- **Fixed filter bank / resonator**
  - Frap Tools Fumana
  - ADDAC fixed filter bank
  - Resonant EQs

### Why this works:
Fractaos can generate very dense upper partials, resonant noise, and complex digital motion. Analog filtering after it can “frame” the complexity into musically controllable bands.

**Patch idea:**  
Use a bright fractal like Mandelbrot or Dragon, moderate Texture, then into QPAS with slow stereo modulation. It turns the already animated tone into a wide moving spectral sculpture.

---

## C. Wavefolders and distortion
Even though Fractaos is already harmonically rich, external nonlinearity can turn its cleaner geometric models into monstrous material.

### Great companions:
- Instruō tanh[3]
- Intellijel Bifold
- Frap Tools Brenso folder section
- Schlappi Interstellar Radio
- Noise Engineering Ruina modules
- Retro Mechanical Labs / Metasonix if you want brutal coloration

### Creative use:
- Feed **smoother fractals** like Julia, Rössler, or Fibonacci into wavefolding
- Keep internal Texture lower
- Use external saturation for dynamics instead of internal density

This gives more separation between “source complexity” and “post-harmonic aggression.”

---

## D. Granular / buffer / glitch processors
Fractaos’ evolving output is perfect for capture-and-refracture modules.

### Strong pairings:
- Make Noise Morphagene
- Qu-Bit Nebulae
- 1010 Bitbox / granular-capable samplers
- Instruō Lubadh
- Mutable Clouds descendants / Monsoon / Typhoon
- Data Bender

### Why:
The module already produces complex unstable shapes and quasi-organic motion. Granularizing that can create material that sounds much deeper than either module alone.

**Patch idea:**  
Set Fractaos in Drone mode with microtonal Spread. Feed stereo out into Morphagene. Splice tiny fragments and modulate gene size and slide slowly. Result: alien choir / bowed-metal fog.

---

## E. Resonators and physical-model style processing
Some Fractaos timbres are noisy or impulsive enough to be excellent excitation sources.

### Pair with:
- Mutable Rings / clones
- Intellijel Rainmaker
- 4ms Spectral Multiband Resonator
- feedback delay networks
- Karplus-capable delays

### Creative use:
Use drum fractals or Rule30/Collatz as exciters for resonators. Or send a narrow, transient-rich Fractaos patch into Rings in external input mode for hybrid “fractal acoustic instruments.”

---

## F. Sequential switches and preset-oriented performance modules
Because Fractaos uses presets and clear state changes, it rewards structured performance systems.

### Good matches:
- sequential switches
- scene controllers
- voltage-addressable CV routers
- clocked switch matrices
- macro controllers like:
  - Faderbanks
  - Planar 2
  - Tetrapad/Tête
  - Pressure Points
  - 16n external controller via MIDI/CV ecosystem

### Creative result:
You can treat Fractaos as the “main sound brain” and animate all CV destinations from one playable control surface.

---

# Specific creative patch concepts

## 1. Fractal percussion lab
Fractaos includes 5 drum fractals: Kick, Tom, Snare, HiHat, Cymbal.

### Combine with:
- trigger sequencer
- probability/skipping trigger processor
- transient shaper / compressor
- analog filter
- distortion
- reverb send

### Patch:
- Use four trig inputs for independent drum hits
- Route tuned CV into the 1V/oct inputs to shift tonal drums like Kick/Tom
- Modulate Chaos lightly with random CV for hit variation
- Morph drum curves with a geometric primitive for hybrid pitched percussion
- Follow with compression and a transient processor if available

### Result:
A **synthetic percussion section** with more life than static drum modules, especially if you sequence note pitch into Kick and Tom.

---

## 2. Polyphonic swarm strings
Use one of the texture models like String or Ensemble.

### Combine with:
- polyphonic MIDI keyboard or sequencer
- slow aftertouch-capable controller
- stereo chorus / ensemble
- lush reverb

### Patch:
- Use MIDI poly mode
- Texture high, Morph at medium
- Primitive as Koch, Fibonacci, or Julia for harmonic glue
- Slow CV to Speed and Amount so internal modulation breathes
- Play with aftertouch to animate “organic drift”

### Result:
A **digital string ensemble / swarm pad** that can sit between wavetable and physical-model territory.

---

## 3. Chord-memory drone cathedral
This takes advantage of Drone Spread chord zones.

### Combine with:
- slow random CV
- precision offset
- stereo filter
- shimmer reverb
- feedback mixer

### Patch:
- Drone mode ON
- Pick a texture or geometric fractal with rich overtone content
- Set Spread in upper zone for chord scanning
- Modulate Spread very slowly through a tiny attenuated range so chord families morph
- Add gentle modulation to Morph and Primitive Chaos
- Send to long reverb and subtle feedback path

### Result:
A **self-evolving harmonic installation patch**.

---

## 4. Fractal FM lead voice
The manual describes a simplified FM mode:
- Loop OFF
- Trig OFF
- Morph ON
- Spread OFF
- Chaos OFF

Then Amount becomes bipolar around center.

### Combine with:
- expressive keyboard
- portamento source
- LPG or external filter
- delay

### Patch:
- Use a geometric main fractal, not a texture or drum
- Choose a primitive with contrasting contour: e.g. Rössler, Koch, Hilbert
- Sweep Amount around center carefully
- Modulate Pitch with a subtle vibrato source
- Use external LPG or VCF for articulation

### Result:
A very unusual **fractal FM monosynth lead**, less predictable than classic two-op FM.

---

## 5. Four-voice algorithmic counterpoint
Since Fractaos accepts 4 pitch CVs and 4 trigs, you can treat it like 4 voices of independent composition.

### Combine with:
- four channels of generative pitch
- clock dividers
- logic
- quantizer
- gate delay / burst

### Patch:
- Generate four related melodic streams
- Quantize them to a scale
- Send each to one Fractaos voice
- Use a common CV into Texture or Morph to unify the timbre
- Slightly offset trigs for staggered attacks

### Result:
A **fractal chorale machine** where separate note logic meets shared timbral evolution.

---

## 6. Hybrid digital-analog bass engine
Fractaos can do strong bass tones, especially with:
- Cantor
- Rule30
- Logistic
- Fibonacci
- some lower-depth Mandelbrot settings

### Combine with:
- analog lowpass filter
- drive/saturation
- envelope follower or sidechain compressor
- sub-octave if desired

### Patch:
- Use a geometric fractal with moderate Chaos
- Keep Spread low
- Use Morph for subtle animation
- Run into a strong analog lowpass and saturator
- Sequence mono or paraphonic bass intervals

### Result:
Tight but alive basses with unusual overtone movement.

---

## 7. Microtonal harmony generator
Drone mode includes:
- Just intonation
- 7-limit flavor
- 19-TET slice
- Bohlen-Pierce subset

This is rare and very musically useful.

### Combine with:
- drones
- sine-rich external voices
- resonators
- spectral analyzers / tuners
- long-form ambient effects

### Patch:
Use Fractaos as the **harmonic reference bed**, then improvise other oscillators or acoustic instruments against it. The chord spread system gives you instant microtonal harmonic contexts.

### Result:
An easy entry point into **microtonal modular composition** without needing a dedicated tuning ecosystem.

---

## 8. Fractaos as “exciter” into huge effects
Because Fractaos can generate sharp attacks, noise-like textures, and complex formants, it is an ideal front-end for effects-heavy systems.

### Best with:
- spring reverb
- shimmer
- spectral freeze
- delay networks
- convolution / resonant IR modules
- granular freeze

### Patch:
- Use Storm, Aliasing, Cluster, or drum models
- Animate Chaos and Texture
- Feed into a freeze/granular/delay module
- Reinject a bit of the processed signal via external mixer feedback

### Result:
Massive cinematic textures from a single source.

---

# Modules that particularly make sense with Fractaos

## Sequencing / control
- **OXI One** — amazing if you want polyphonic, multitimbral, MIDI + CV flexibility
- **Squarp Hapax** — ideal for MULTI mode and separate channel control
- **Pamela’s Pro Workout** — clocks, envelopes, LFOs, Euclidean gates for four trig inputs
- **Mutable Marbles** or equivalent — beautiful semi-random pitch/gate for fractal timbres
- **Planar 2** — hands-on Morph/Texture/Spread performance control
- **Batumi** — four related LFOs for multiple CV targets
- **Maths** — classic for slew, envelopes, attenuversion, weird modulation shaping

## Audio shaping
- **QPAS** — great stereo animation after Fractaos
- **Ikarie** — stereo character and panning movement
- **Mimeophon** — particularly good with drone textures
- **Morphagene** — turns Fractaos into a soundworld generator
- **Data Bender** — complements the digital instability beautifully
- **Fumana** — spectral sculpting of dense fractal output
- **Desmodus Versio / Starlab** — lush space for drones and pads

## Utility support
- attenuverters
- offset generators
- CV mixers
- matrix mixers
- stereo mixers
- precision adders
- slews / lag processors

These are important because Fractaos has several high-impact CV inputs. Fine control matters more than raw modulation quantity.

---

# Best CV strategies

## 1. Use attenuation aggressively
Fractaos has many “macro” parameters where tiny movement matters.

Especially for:
- Spread
- Chaos
- Primitive Chaos
- Texture
- Morph

A matrix mixer or attenuverter lets you find the sweet spot between subtle animation and total collapse.

---

## 2. Separate “structural” from “gestural” modulation
Use:
- **slow CV** for Texture, Chaos, Primitive Chaos
- **performance/manual CV** for Morph and Spread
- **rhythmic CV** for Amount and Speed

This tends to produce more musical results than modulating everything at once.

---

## 3. Let Fractaos handle complexity, let external modules handle space
Often the best patch is:
- internal timbral complexity from Fractaos
- external stereo field and ambience from other modules

Instead of stacking more oscillators, give it:
- filters
- delays
- reverbs
- matrix-controlled modulation

---

# Preset strategy ideas

Because presets store:
- 11 main pot values
- 5 switch states
- envelope parameters

You can build performance sets around categories like:

- **A:** percussive fractals
- **B:** harmonic geometric tones
- **C:** unstable chaotic leads
- **D:** drone textures
- **E:** multitimbral “kits”

In MULTI mode, one killer approach is:

- Voice 1: LIVE for hands-on tweaking
- Voice 2–4: preset locked roles

This gives you one “improvisation voice” while the others hold down structure.

---

# Some especially promising fractal pairings

## For tonal melodic work
- Fibonacci + Koch
- Julia + Rössler
- Sierpinski + Mandelbrot
- Rössler + Hilbert

## For unstable experimental work
- Lorenz + Hénon
- Rule30 + Dragon
- Logistic + Collatz

## For hybrid percussive-pitched work
- Kick + Koch primitive
- Snare + Cantor primitive
- Tom + Fibonacci primitive
- Cymbal + Hilbert primitive

## For drone/pad work
- Cloud + Julia
- String + Koch
- Cluster + Rössler
- Ensemble + Fibonacci

---

# A few performance-minded patch recipes

## “Fractal Choir”
- Drone mode
- Ensemble or Cloud
- Spread in Just Intonation or Major 7
- slow CV to Morph
- aftertouch from MIDI keyboard
- stereo reverb after output

## “Broken Digital Tabla”
- Snare/Tom/Kick fractals
- Euclidean trigger sequencing
- random CV into Chaos
- analog bandpass filter after output
- delay send on selected hits

## “Evolving Glass Organ”
- Koch or Mandelbrot main fractal
- Julia primitive
- slow looping primitive modulation
- external resonant stereo filter
- shimmer reverb

## “Alien FM Brass”
- simplified FM mode
- Fibonacci or Cantor main
- Dragon or Rössler primitive
- Amount above center
- external VCA and LPG articulation

## “Microtonal Black Metal Pad”
- Drone mode
- BP subset or 19-TET slice Spread
- high Texture
- saturated stereo filter
- huge reverb
- slow random modulation into Chaos

---

# Final take

Fractaos seems most rewarding if you **don’t treat it like a conventional oscillator**. It’s better viewed as:

- a **polyphonic fractal timbre engine**
- a **drone harmony computer**
- a **multitimbral digital ensemble**
- a **hybrid percussion synthesizer**

So the best companion modules are not necessarily more sound sources, but modules that provide:

- elegant control
- modulation scaling
- sequencing structure
- stereo processing
- spectral framing
- spatialization

If you want, I can also turn this into:

1. a **“best companion modules by budget” list**,  
2. a **small / medium / large rack integration plan**, or  
3. **10 concrete patch sheets** with knob suggestions and signal flow diagrams.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)