# Humble Audio — Quad Operator Algo Extension

- [Manual PDF](../../manuals/Quad Operator Manual.pdf)

---

[Quad Operator Manual PDF](https://www.dropbox.com/paper/doc/print/JsIQoU7GbeAboEJku9ZgE?print=true)

# Humble Audio Quad Operator: creative patch ideas and companion modules

The **Humble Audio Quad Operator** is much more than a 4-op FM voice. Based on the manual, it’s really a **4-oscillator digital FM matrix**, where each operator can be:

- a **carrier**
- a **modulator**
- **self-modulating**
- **locked** into harmonic integer ratios
- or **freed** into independent oscillators

Plus, it has:

- per-operator **variable waveshape**: sine → triangle → square → saw
- per-operator **gain CV** acting like a built-in modulation VCA
- an **external audio-rate FM input** with its own modulation sends
- **independent outputs** for each operator
- **reset input** for phase sync / repeatable modulation
- **LFO mode**
- optional **Algo expander** for storing/crossfading FM matrices

That combination makes it useful as:

- a classic FM voice
- a chord/drone bank
- a complex modulation generator
- a feedback lab
- a pseudo-additive oscillator
- a quad synced LFO source
- a hybrid digital/analog cross-modulation hub

---

# What stands out musically from the manual

A few important behaviors define how to patch it creatively:

## 1. Lock vs Free is the big structural choice
In **lock state**, operators stay in strict integer ratios to the master tuning. This is where you get:

- stable harmonic FM
- Yamaha-style operator stacks
- controllable bells, plucks, basses, electric pianos, metallic but tonal sounds

In **free state**, each operator becomes an independent oscillator, and the ratio control becomes coarse tuning with 1V/oct via ratio CV. This opens up:

- 4-voice paraphonic or pseudo-poly use
- beating drones
- cross-modulated oscillator clusters
- inharmonic and chaotic FM

## 2. Gain CV is secretly very powerful
Per the manual, **Gain CV affects both output level and how much that operator modulates others via its sends**.

This means Gain CV is effectively an **operator index VCA**. That’s huge. It lets you animate FM amount dynamically without needing external VCAs for each operator.

So envelopes, LFOs, random voltages, gates, and sequenced CV into Gain can radically change timbre and dynamics at once.

## 3. Shape is continuous, not a switch
Each operator sweeps from **sine → triangle → square → saw**. That means you can morph an operator from clean FM-friendly sine into brighter overtone-rich modulators/carriers.

This is not just “tone color” — in FM it changes the sideband content dramatically.

## 4. AR FM input makes the module a system hub
The dedicated external audio-rate modulation input has:

- gain control
- clipping indication
- gain CV
- separate sends to each operator

That means any oscillator, noise source, drum voice, filtered feedback, or even a full submix can become an FM source into the Quad Operator network.

---

# Best companion module categories

Below are the most fruitful module pairings.

---

## 1. Envelope generators and function generators
These are probably the most immediately rewarding companions, because **Gain CV** is where the Quad Operator comes alive.

### Why they work
Patch envelopes to:
- operator Gain CV for dynamic FM index
- Shape CV for attack brightness
- LF FM for pitch envelopes
- Algo crossfade CV if you have the expander

### Great pairings
- Make Noise **Maths**
- Frap Tools **Falistri**
- Intellijel **Quadrax**
- Xaoc **Zadar**
- Befaco **Rampage**
- generic ADSR or AD envelopes

### Patch idea: “FM percussion lab”
- All operators in **lock**
- All shapes fully CCW (sine) to start
- Use one operator as carrier, one or two as modulators
- Send snappy envelopes to the modulator **Gain CVs**
- Send a short pitch envelope to **LF FM**
- Take just one operator output as the voice

Result:
- kicks
- toms
- woodblocks
- claves
- metallic percussion
- digital congas

If you open Shape on a modulator during the transient, the attack gets much harsher.

---

## 2. VCAs and CV mixers
Even though it has internal gain control, external VCAs and mixers let you sculpt the modulation ecosystem around it.

### Why they work
Use them to:
- control CV into Ratio / Shape / Gain
- mix multiple modulators into AR FM
- automate transitions between harmonic and unstable regions
- create feedback amount control outside the module

### Great pairings
- Intellijel **Quad VCA**
- Happy Nerding **3xVCA**
- Mutable Instruments **Veils**
- ALM **Tangle Quartet**
- any attenuverter/mixer like **Happy Nerding 3xMIA**, Frap **321**, Befaco **A*B+C**

### Patch idea: “performance macro FM”
- Mult one macro CV source into several attenuverters
- Send to:
  - modulator Gain CV
  - one operator Shape CV
  - LF FM amount
  - AR FM Gain CV
- Tune attenuators so one gesture moves the patch from mellow to explosive

This gives you a playable “meta timbre” control.

---

## 3. Sequential switches, matrix mixers, and routers
The Quad Operator is all about routing modulation, so external routing modules supercharge it.

### Why they work
You can dynamically change:
- which operator feeds AR FM feedback paths
- which outputs go to filters/waveshapers
- which external oscillator enters AR FM
- layered modulation structures over time

### Great pairings
- Doepfer **A-151**
- Joranalogue **Switch 4**
- Erica Synths **Matrix Mixer**
- Instruō **Lion**
- AI Synthesis / Livestock / generic matrix mixers

### Patch idea: “algorithm scanner without the expander”
- Patch Op 1–4 outputs into a sequential switch or matrix
- Route different operators into AR FM
- Clock the switch slowly
- Keep internal Mod sends static
- Let the external routing create evolving “new algorithms”

This effectively creates moving operator topologies.

---

## 4. Filters and resonators
The module is digital FM and can get bright, buzzy, and alias-prone in musically useful ways. Filters and resonators add contour and body.

### Why they work
Use filters:
- after individual operator outputs
- after a mix of several operators
- in feedback paths via AR FM

### Great pairings
- Mutable **Ripples**
- Rossum **Linnaeus**
- Serge / Random*Source **VCFQ**
- Bastl **Ikarie**
- Three Sisters
- fixed filter banks / resonators like **QPAS**, **Resonant EQ**, **Rings**-style resonators

### Patch idea: “FM into resonator”
- Build a bright FM tone on one operator output
- Send it through a resonator or LPG
- Modulate operator Shape and Gain with envelopes
- Use another operator output as a dry layer

This creates acoustic-ish tones:
- struck strings
- marimba-like voices
- glassy bowed timbres
- synthetic vocal resonances

### Patch idea: “filtered external FM”
- Send filtered noise, bandpassed drums, or a resonant self-oscillating filter into **AR FM**
- Use the AR FM sends selectively to one or two operators
- Sweep the filter cutoff

This produces moving, formant-like FM spectra.

---

## 5. Wavefolders, distortions, and analog nonlinearities
Because the Quad Operator already spans several waveforms, adding external nonlinear shaping can turn it into a monster.

### Why they work
FM plus wavefolding is one of the fastest ways to get:
- animated drones
- industrial basses
- vocal tearing textures
- “West Coast but digital” timbres

### Great pairings
- Intellijel **Bifold**
- Instruō **àthru**
- Serge wave multipliers
- Noise Engineering distortions
- tanh/saturation modules
- feedback mixers

### Patch idea: “operator split personality”
- Use one operator output as clean voice
- Use another operator output through a wavefolder
- Mix both
- Modulate their Gain CVs differently

Since each operator has its own output, you can layer clean and mangled versions from the same FM ecosystem.

---

## 6. Random and chaos sources
This module responds beautifully to controlled instability.

### Why they work
Random CV into:
- Gain = changing FM index
- Shape = changing overtone content
- Ratio CV in free mode = unstable interval clouds
- Algo crossfade = morphing algorithmic states

### Great pairings
- Make Noise **Wogglebug**
- Mutable **Marbles**
- Frap **Sapèl**
- Joranalogue **Orbit 3**
- Nonlinear Circuits chaos modules
- sample & hold + noise

### Patch idea: “unstable machine choir”
- Put 2 operators in lock, 2 in free
- Use slow random on free operators’ Ratio CV
- Use smooth random on Shape CV
- Mix all four outputs
- Add slight self-modulation on one free operator

This creates an evolving digital ensemble with quasi-harmonic drift.

---

## 7. Quantizers and precision CV tools
Because free-state operators can be independently tuned by Ratio CV as 1V/oct, quantizers turn the module into a compact multi-oscillator melodic system.

### Why they work
You can:
- tune free operators into chords
- sequence operators independently
- force modulation oscillators into scales
- create tonal counterpoint from internal FM relationships

### Great pairings
- Intellijel **Scales**
- ADDAC quantizers
- Ornament & Crime
- Shakmat **Bard Quartet**
- precision adder / buffered mults

### Patch idea: “4-op chord engine”
- Set all operators to **free**
- Send related quantized pitch CVs to each Ratio input
- Slightly detune some operators
- Use minimal internal modulation
- Mix outputs externally

Then slowly introduce internal FM:
- Op 2 modulates Op 1
- Op 3 modulates Op 2
- AR FM modulates Op 4 from another voice

You get chord voices that can move from clean organ-like tones to animated glassy pads.

---

## 8. LPGs, low-pass gates, and VCAs for voice articulation
The Quad Operator can sound very direct and digital; LPGs add organic contour fast.

### Why they work
Even if Gain CV shapes output internally, external amplitude articulation changes the feel:
- woody
- plucky
- acoustic-ish
- Buchla-adjacent

### Great pairings
- Make Noise **Optomix**
- Natural Gate
- LxD
- any LPG or VCA with expo response

### Patch idea: “FM bongo / marimba”
- Harmonic lock mode
- Sine carriers and modulators
- Snappy envelope to modulator Gain
- Output through LPG
- Slight pitch envelope via LF FM

Very effective for tuned percussion.

---

## 9. Delay, granular, and reverb processors
The Quad Operator can generate dense spectra that love spatial treatment.

### Why they work
Use effects to turn the module from voice into environment.

### Great pairings
- Make Noise **Mimeophon**
- Intellijel **Sealegs**
- Xaoc **Timiszoara**
- Magneto
- granular modules
- shimmer / spectral reverbs

### Patch idea: “frozen FM cloud”
- Set module in LFO mode or low VCO range
- Use slow internal modulation with multiple outputs mixed
- Process through long delay/granular/reverb
- Send one delayed tap back into AR FM at low gain

This creates self-evolving digital ambiences and unstable spectral blooms.

---

## 10. Drum modules and samplers into AR FM
The dedicated external audio-rate input is one of the coolest features.

### Why they work
Any rhythmic source can become an FM modulator.

Try:
- hats
- snare noise
- click tracks
- chopped samples
- spoken word fragments
- wavetable oscillators
- another FM voice

### Great pairings
- sample players
- noise/drum voices like Basimilus, BIA, Plaits percussion, SSF Entity, Squid Salmple, Bitbox
- analog noise + filter
- digital speech/sample modules

### Patch idea: “rhythmic sideband sculpting”
- Send hi-hats or clicks into **AR FM**
- Turn up sends only to one or two operators
- Use envelope-controlled AR FM Gain CV
- Keep one carrier clean and another heavily modulated
- Mix both outputs

This gives a rhythmic “grain” embedded into pitch.

---

# Specific musical roles for the Quad Operator

## A. As a classic 4-op FM synth voice
Best companions:
- envelopes
- VCA/LPG
- filter
- reverb

Suggested structure:
- Op 1 = carrier
- Op 2 = modulator for Op 1
- Op 3 = modulator for Op 2
- Op 4 = second carrier or parallel modulator

Use Gain CV envelopes on Op 2/3 for evolving attack and decay.

Very effective for:
- DX-ish keys
- metallic plucks
- basses
- bells
- electric piano-adjacent tones

---

## B. As a 4-oscillator drone cluster
Best companions:
- mixers
- slow random
- filters
- wavefolders
- spectral FX

Suggested structure:
- all operators in **free**
- tune to chord tones / just intervals
- mild cross-modulation between only some operators
- slow random into Shape and Gain
- mix outputs separately in stereo

This is where it becomes a drone orchestra.

---

## C. As a modulation generator
In **LFO mode**, especially with reset, it becomes a complex modulation hub.

Best companions:
- clock/reset utilities
- switches
- logic
- CV recorders
- CV-addressed effects

Suggested structure:
- lock operators for phase-related LFOs
- use different ratios for rhythmic subharmonics/polyrhythms
- patch operator outputs as modulation signals, not audio
- reset from sequencer

Because outputs are audio/CV rate and resettable, you can get repeatable complex motion.

### Patch idea: “phase-locked modulation ecosystem”
- LFO mode
- all operators locked
- different ratios
- one operator self-modulates slightly
- use outputs for:
  - filter cutoff
  - wavefolder symmetry
  - stereo panning
  - delay time

The reset input makes the whole animated pattern restart in sync with your sequence.

---

## D. As a feedback instrument
The manual explicitly suggests feedback use via **AR FM**, especially with phase-locked operators.

Best companions:
- attenuators
- filters
- VCAs
- delays
- matrix mixers
- output limiter/compressor if desired

### Patch idea: “managed digital feedback”
- Take Op 4 output
- Send through VCA or filter
- Return to AR FM
- Send AR FM only to Op 1 and Op 2
- Keep gain low initially
- Use locked operators for pitch stability

Then slowly open:
- AR FM gain
- AR FM send amounts
- filter resonance or cutoff

This can move from subtle edge to screaming unstable structures.

---

# Patch recipes

## 1. “DX bell with modern bite”
Modules:
- Quad Operator
- 2 envelopes
- VCA/LPG
- stereo reverb

Patch:
- All operators in lock
- Shapes at sine
- Op 2 modulates Op 1
- Op 3 modulates Op 2 lightly
- Op 4 as a second carrier or parallel bright layer
- Fast-decay envelope to Op 2 Gain CV
- Slower envelope to Op 3 Gain CV
- Output Op 1 (and optionally Op 4) through LPG/VCA
- Add long reverb

Variation:
- Slightly advance Shape on Op 2 or Op 3 for glassier attack

---

## 2. “Four-voice metallic chord”
Modules:
- quantizer
- chord/sequencer CV source
- stereo mixer
- delay

Patch:
- All operators in free
- Send different quantized pitches to each Ratio CV
- Tune as chord tones
- Set tiny amounts of cross-modulation in a ring:
  - Op1→Op2
  - Op2→Op3
  - Op3→Op4
  - Op4→Op1
- Mix outputs in stereo

Result:
A shimmering harmonic field that can become unstable with just small modulation-send increases.

---

## 3. “Pseudo-resynthesis”
Modules:
- envelope followers or VCAs
- filter bank or EQ
- mixer

Patch:
- Use each operator output as a partial band
- Tune in lock ratios approximating harmonic partials
- Set shape and gain per operator
- Mix externally
- Animate each Gain CV with different envelopes/LFOs

This is more additive than FM, but internal FM between selected operators adds motion impossible in static additive patches.

---

## 4. “Granular FM percussion”
Modules:
- sample player or glitch source
- envelope
- LPG
- distortion

Patch:
- Sample/glitch source into AR FM
- Triggered envelope into AR FM Gain CV
- AR FM sends to only one or two operators
- Use a locked carrier output as primary audio
- Run through LPG or distortion

This yields crunchy, sampled transient fingerprints inside a tuned voice.

---

## 5. “Complex synced LFO brain”
Modules:
- clock sequencer
- logic
- filter
- panner
- delay/reverb

Patch:
- Switch to LFO mode
- Use reset input from clocked trigger
- Operators in lock
- Ratios set to different integer values
- One slight self-mod send for one operator
- Use op outputs as CVs for multiple destinations

This is excellent for:
- synchronized evolving modulation
- repeating but non-obvious rhythmic CV patterns
- phrase-level movement

---

## 6. “Self-modulated bass engine”
Modules:
- envelope
- VCA
- lowpass filter
- saturation

Patch:
- Lock mode
- Op 1 carrier
- Op 1 self-modulates a little
- Op 2 modulates Op 1
- Envelope to Op 2 Gain CV
- Slight LF FM envelope for punch
- Op 1 output through lowpass and saturation

A little self-FM plus external saturation gives aggressive but playable bass.

---

## 7. “Dual-layer lead: tonal + noise edge”
Modules:
- noise source or oscillator
- filter
- reverb/delay

Patch:
- Build a harmonic FM tone internally
- Patch noise or another VCO into AR FM
- Send AR FM only lightly to the main carrier
- Use Gain CV to bring in external FM only during attack
- Mix a second operator output separately for body

This creates articulate leads with a noisy or vocalized edge.

---

# Recommended module pairings by goal

## For classic playable FM voices
- Quadrax / Maths / Zadar
- Optomix or Quad VCA
- a warm filter like Ripples or Ikarie
- reverb/delay

## For experimental digital chaos
- Wogglebug / Sapèl / Marbles
- matrix mixer
- feedback-capable filter
- distortion / wavefolder
- delay with feedback loop

## For chord and drone work
- quantizer
- precision adder
- stereo mixer / panner
- resonator / reverb
- slow random

## For modulation-system duties
- clock/reset utility
- logic
- sequential switch
- CV recorder
- attenuverters

## For hybridizing with other oscillators
- analog VCO into AR FM
- wavetable VCO into AR FM
- drum/sample source into AR FM
- comparator/envelope follower to derive extra control from the same source

---

# A few especially strong module recommendations

If I were building around the Quad Operator, I’d especially want:

- **Intellijel Quadrax** – perfect for animating multiple Gain CVs
- **Maths** – envelopes, slews, offsets, modulation utilities
- **Happy Nerding 3xMIA** – crucial for taming CV depth
- **Mutable Veils / Intellijel Quad VCA** – extra modulation control and macro performance
- **Doepfer A-151** – simple but powerful for re-routing outputs into AR FM
- **Bastl Ikarie** or **QPAS** – stereo filtering for digital timbres
- **Mimeophon** – Quad Operator loves spacious, smeared echoes
- **Marbles** – melodic and timbral uncertainty
- **Ornament & Crime** – quantizer, envelope, modulation brain
- **an LPG** like Optomix – gives digital FM a more organic front end

---

# Practical advice from the manual that matters in patching

## Start harmonic, then destabilize
The manual explicitly recommends for harmonic results:

- VCO mode
- all operators in lock
- detune at noon
- shapes at sine
- modulation sends at zero

That is excellent advice. Build from there.

## Shape adds brightness fast
Since the operators can be saw/square-like, adding shape before adding much FM can already create dense spectra. If the patch gets brittle or noisy, reduce shape first.

## Gain CV is performance gold
Because gain affects both loudness and modulation intensity, patching envelopes here gives “acoustic-feeling” timbral articulation with very little patching.

## External AR FM deserves respect
It accepts audio-rate sources, and clipping is indicated with the red LED. This makes it ideal for performance feedback and hybrid patching, but also easy to overdrive into chaos.

---

# My favorite creative uses overall

If I had this module in a live system, I’d use it primarily in 5 ways:

1. **As a compact evolving FM voice**
   - locked ratios
   - envelopes on Gain CV
   - one output as main voice, one output as auxiliary layer

2. **As a 4-oscillator drone engine**
   - free mode
   - slight cross-modulation
   - stereo external mixing/effects

3. **As a resettable complex LFO bank**
   - LFO mode
   - synced reset
   - outputs used as animated CV

4. **As a feedback processor**
   - route one operator or external sound back into AR FM
   - control return path with VCA/filter

5. **As a hybrid timbre merger**
   - another oscillator, drum loop, or sample into AR FM
   - internal operators provide pitch skeleton
   - external source imprints texture

---

# Bottom line

The Quad Operator is best thought of as a **modular FM ecosystem**, not just a single oscillator. The most interesting pairings are modules that help you:

- **animate Gain CV**
- **control and attenuate modulation depth**
- **route audio back into AR FM**
- **mix the four outputs creatively**
- **shape the bright digital spectra afterward**

If you support it with:
- envelopes/functions
- VCAs/attenuverters
- filters/LPGs
- random/quantizers
- routing/feedback tools
- spacious effects

…it can cover everything from **precise tonal FM** to **chaotic self-modulating sound design**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)