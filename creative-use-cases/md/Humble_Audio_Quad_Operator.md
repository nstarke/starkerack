# Humble Audio — Quad Operator

- [Manual PDF](../../manuals/Quad Operator Manual.pdf)

---

[Quad Operator Manual PDF](https://www.dropbox.com/paper/doc/print/JsIQoU7GbeAboEJku9ZgE?print=true)

# Humble Audio Quad Operator: creative patch ideas and module pairings

The **Humble Audio Quad Operator** is basically a **4-operator digital FM voice / oscillator bank / modulation matrix** with a very unusual Eurorack-friendly workflow:

- 4 operators with **independent outputs**
- each operator can be **locked** to harmonic integer ratios or set **free** as an independent oscillator
- variable waveshape per operator: **sine → triangle → square → saw**
- per-operator **gain CV** acts like a built-in VCA for both output level **and FM send intensity**
- full FM routing via **modulation matrix**, including **self-modulation**
- external **AR FM input** with its own gain and sends
- **reset input** for phase reset
- **LFO mode**
- optional **Algo expander** for storing/crossfading matrix states

That means this module is not just “an FM oscillator.” It can be:

- a classic 4-op FM voice
- a 4-oscillator drone lab
- a phase-locked complex LFO generator
- a modulation matrix processor for external audio
- a chaotic feedback network
- a quad voice source for stereo or quadraphonic patching

Below are the most interesting ways I’d use it with other Eurorack modules.

---

## 1. Use it as a classic FM voice, but animate the operator index with VCAs and envelopes

One of the coolest things in the manual is that **Gain CV affects both output level and how strongly an operator modulates other operators via its sends**. That means each operator already behaves somewhat like an FM operator with a built-in VCA.

### Patch concept
- Keep all operators in **lock**
- Start with **sine shapes**
- Set one operator as the audible carrier
- Use 1–3 other operators as modulators
- Patch **envelopes** into the **Gain CV** inputs of the modulators
- Take the carrier output to a **VCA/filter/effects chain**

### Why this is powerful
This gives you **DX-style evolving FM index** behavior without extra routing complexity. Instead of just static timbre, you can make attacks bright and metallic, then decay into purer tones.

### Great companion modules
- **Quad envelope generators**: Intellijel Quadrax, Xaoc Zadar, Frap Falistri
- **VCAs** if you want additional shaping after the operator outputs: Veils, A-132-3, Mutable Veils clones
- **Precision pitch sequencer**: Metropolix, Rene, Oxi One, Bloom, or any quantized CV source

### Musical result
- electric pianos
- marimbas
- bells
- basses with sharp transient bite
- glassy plucks

---

## 2. Build “algorithm morphing” patches with switches, mute matrices, or the Algo expander

The modulation matrix means you can create your own FM algorithms instead of being stuck with Yamaha-style presets. The **Algo expander** makes this much more performable by storing and crossfading matrix states.

### If you have the Algo expander
Use saved algorithms as:
- **A:** simple 2-op bass
- **B:** stacked 4-op metallic bell
- **C:** self-modulated noise/percussion

Then crossfade between them during a sequence.

### If you don’t have the expander
You can still emulate “algorithm changes” by pairing Quad Operator with:
- a **sequential switch**
- CV-addressable attenuators
- mute matrix modules
- CV preset modules

### Good companion modules
- **Sequential switches**: Doepfer A-151, Joranalogue Step 8, Erica Sequential Switch
- **CV preset/scene modules**: Verbos Voltage Multistage, Acid Rain Maestro, Make Noise Pressure Points + Brains style setup, Malekko Varigate + voltage memories
- **Mute/performance mixers**: Happy Nerding 3xMIA, WMD SSM if available used, Bastl Aikido for amplitude interaction

### Musical result
- one-note timbral progression
- algorithm morphing leads
- morphing percussion kits
- evolving drones that feel “composed”

---

## 3. Treat it as a 4-voice oscillator bank in free mode

The manual explicitly says in **free state** each operator becomes its own oscillator, with ratio knob as coarse tuning and ratio CV as **1V/oct**.

That’s huge.

### Patch concept
- Put all 4 operators in **free**
- Tune them to chord tones or intervals
- Send separate pitch CVs or related sequences
- Use each output independently

### Pair it with
- **4-channel quantizer**: Ornament & Crime, ADDAC quantizer, Instruo Harmonaig for harmonic relation
- **4 VCAs / LPGs**
- **4 envelopes**
- **4-channel panner or mixer**

### Interesting ways to use it
#### A. Chord machine
- Tune ops to root/third/fifth/seventh
- Use slight detune differences
- Modulate shape independently
- Mix to stereo

#### B. Four-part counterpoint
- Separate sequencers or clock divisions to each operator
- Minimal FM between them for interaction

#### C. Pseudo-paraphonic voice
- Same pitch source to all four, slightly offset tuning and different shapes
- Mix for a super oscillator / organ stack

### Good companion modules
- **Mixers/panners**: Happy Nerding PanMix, Worng SoundStage, Intellijel Mixup + stereo FX
- **Quad VCA**: Intellijel Quad VCA, Veils
- **Polyphonic sequencers**: Flame Chord Machine, Sinfonion ecosystem, Oxi Coral/sequencing ecosystem, Hermod+

### Musical result
- organ-like clusters
- harmonic drones
- stacked techno leads
- four-voice minimalist patches

---

## 4. Use LFO mode as a phase-locked complex modulation generator

The manual notes **LFO mode** and **reset** make it useful as a modulation source. This is one of the most underrated uses.

### Patch concept
- Switch to **LFO**
- Keep operators in **lock**
- Use integer ratios for rhythmic relationships
- Send operator outputs to:
  - filter cutoff
  - wavefolder symmetry
  - stereo panning
  - delay time
  - reverb size
  - VCA amplitude
- Use **reset** from a clock or trigger so all modulation restarts in sync

### Why this is special
You get **phase-coherent, related modulation signals**. Much more structured than using a bunch of unrelated LFOs.

### Pair with
- filters
- stereo processors
- resonators
- vector mixers
- matrix mixers
- clock/reset utilities

### Great companion modules
- **Clock/reset**: Pamela’s Pro Workout, Tempi, 4ms QCD
- **Targets for modulation**:
  - filter: QPAS, Three Sisters, Belgrad, Ikarie
  - effects: Mimeophon, FX Aid, Magneto, Beads, Data Bender
  - panning: XAOC Ostrawa, Happy Nerding PanMix, Worng LRMSMSLR

### Musical result
- locked polyrhythmic movement
- repeating evolving stereo gestures
- synchronized modulation for live sets
- “one module animates the whole patch”

---

## 5. Feed external oscillators or whole submixes into the AR FM input

A major feature here is the dedicated **AR FM input** with gain and modulation sends to all operators. This lets you use **anything in the rack** as an FM modulator.

### Great signal sources for AR FM
- a second oscillator
- noise
- a filtered drum loop/submix
- resonator output
- wavefolder output
- another operator output for feedback structures
- speech/sample playback
- another digital oscillator with harmonic content

### Patch concept
- Patch an external oscillator into **AR FM**
- Set gain so clipping LED barely flickers or intentionally clips
- Send AR FM to 1–4 operators at varying amounts
- Mix operator outputs

### Pair with these module types
#### Analog VCOs
FM from a stable analog sine/triangle can sound smoother.
- Dixie II+, STO, ZPO, AJH oscillators, A-110 variants

#### Complex/digital oscillators
Feeding rich harmonics into AR FM gets gnarlier fast.
- Plaits, Odessa, Ensemble Oscillator, Piston Honda, Loquelic Iteritas, Shapeshifter

#### Sample/drum modules
Audio-rate drum signals used as modulators = wild transient spectra.
- Assimil8or, Bitbox, Squid Salmple, sample player submixes

### Musical result
- hybrid analog/digital FM
- speech-modulated metallic textures
- percussion-imprinted drones
- aggressive industrial tones

---

## 6. Create controlled feedback patches

The manual specifically hints at **feedback patches with lock mode operators** and external AR FM. This is absolutely where the module gets special.

### Safe feedback recipe
- Keep operators in **lock**
- Start with low modulation send values
- Patch one operator output into an external processor:
  - VCA
  - filter
  - wavefolder
  - delay with short time
- Feed that processor output back into **AR FM**
- Use Gain AR FM to control feedback intensity

### Better yet
Insert something in the loop to make the feedback “playable”:
- **VCA** for voltage-controlled feedback amount
- **filter** to tune feedback emphasis
- **wavefolder** for nonlinear feedback coloration
- **frequency shifter/ring mod** for inharmonic mayhem
- **delay** for Karplus-adjacent metallic recursion

### Great companion modules
- **VCA**: Tallin, Quad VCA, Blinds
- **Filter**: Doepfer SEM, Bastl Ikarie, QPAS, SSF Stereo Dipole
- **Wavefolder**: Bifold, Fold 6, Serge-style folders
- **Frequency shifter/ring mod**: Frap Fumana? no, better: Doepfer A-126-2 frequency shifter, Xaoc Koszalin, ring mod modules
- **Limiter/saturator** in feedback path: tanh[3], L-1, Instruo tràigh in support role, or just a mixer with saturation

### Musical result
- metallic drones
- unstable machine tones
- pseudo-physical modeling
- screaming but controllable feedback leads

---

## 7. Use self-modulation per operator for “single-operator wavefolding-like” tones

Because each operator can modulate **itself**, you can create tones that blur the line between FM, PM-feel, and nonlinear distortion.

### Patch concept
- Choose one operator as audio output
- Turn up its own modulation send
- Keep others off at first
- Sweep shape from sine toward brighter waves
- Modulate gain CV with an envelope or LFO

### Pair with
- envelope followers
- random stepped CV
- performance macro controls

### Why it works
Self-mod FM often gives:
- sharpened transients
- buzzy edge
- tearing digital tones
- unstable pseudo-wavefolding behavior

### Good pairings
- **Random source**: Wogglebug, Marbles, Sapel, Chance
- **Envelope source**: Maths, Quadrax, Zadar
- **Macro attenuverters**: 3xMIA, MISO, Quadratt

### Musical result
- acid-adjacent basses
- glitch percussion
- ripping drones
- animated monosynth leads

---

## 8. Use operator outputs as both sound sources and modulation sources elsewhere

Because each operator has its own output, you don’t have to think of “carriers” and “modulators” only internally. Any operator can also leave the module and modulate something else.

### Patch concept
- Build an FM patch internally
- Take one or more operator outputs externally to modulate:
  - filter FM
  - wavefolder CV
  - VCA AM
  - delay clock/position
  - resonator excitation
- Still use another operator as the main audio voice

### Pair with
- analog filters with FM input
- wavefolders
- LPGs
- resonators
- granular effects

### Great module matches
- **Resonators**: Rings, Res-4, 4ms SMR, Any physical modeling voice
- **Wavefolders**: Bifold, Toppobrillo folder, Serge style
- **Low-pass gates**: Optomix, LxD, Natural Gate
- **Audio-rate capable filters**: Joranalogue Filter 8, Belgrad, Morgasmatron

### Musical result
- deeply interlocked patches
- one source creating multiple correlated layers
- acoustic-ish metallic behavior
- animated timbral ecosystems

---

## 9. Make percussion without needing a traditional drum module

FM is excellent for percussion, and Quad Operator’s matrix makes it easy to build multiple drum families from one patch.

### Patch concepts
#### Kick
- One operator as sine carrier
- Slight pitch envelope via **LF FM**
- very little mod for thump
- optional self-mod for click

#### Snare
- one or two operators inharmonic or self-modulated
- one sine/triangle for body
- one brighter operator for noise-ish snap

#### Tom/conga
- lock state, integer ratio modulator
- envelope on modulator gain CV
- medium decay

#### Hat/cymbal
- multiple operators with square/saw shapes
- free state or detuned lock ratios
- more inharmonic modulation

### Great companion modules
- **Fast envelopes**: Maths, Quadrax, Zadar, Function Junction
- **Trigger sequencers**: Pam’s, Steppy, Grids, Numeric Repetitor
- **Transient shapers / LPGs / VCAs**
- **Compressor/saturation** after the mix

### Musical result
- all-FM drum voice
- metallic percussion banks
- techno hats and zaps
- electro toms and laser hits

---

## 10. Build stereo and spatial FM patches

Since you have four outs, you can distribute operators in stereo or even surround/quad setups.

### Patch concept
- Use two operators as left-side voices, two as right-side voices
- Cross-modulate asymmetrically
- Pan outputs with CV
- Send different operators to different effects chains

### Companion modules
- **Stereo panners**: PanMix, Planar 2, Jumble Henge, SoundStage
- **Dual/stereo filters**
- **Stereo delays/reverbs**

### Fun variations
- Left channel = harmonic operators in lock
- Right channel = detuned/free operators
- Modulate shape differently per side
- Reset modulation periodically for rhythmic image collapse/rebuild

### Musical result
- animated stereo metallic fields
- “orbiting” FM swarms
- immersive drones
- performance-friendly wide leads

---

## 11. Pair it with precision utilities for harmonic FM that stays musical

The manual is clear: if you want harmonic results, use:
- **VCO mode**
- **lock state**
- **detune at noon**
- **sine waves**
- **mod sends low to start**

To really exploit this musically, pair it with precision tools.

### Best utility companions
- **Precision adder**
- **Buffered mult**
- **Quantizer**
- **Offset/attenuverter**
- **Oscilloscope/tuner**

### Recommendations
- Buffered mult: Links, Buff Mult, etc.
- Quantizer: O_c, Scales, Bard Quartet
- Utility: 3xMIA, Quadratt, MISO
- Visualizer: Mordax Data, O’Tool

### Why this matters
FM gets messy fast. Precision support modules let you:
- keep pitch stable
- dial exact intervals
- reproduce patches
- intentionally move between harmonic and inharmonic territories

---

## 12. Use free/lock switching as a compositional gesture

The switch per operator is not just setup—it’s performable.

### Patch concept
- Start with all operators in **lock**
- Build a stable harmonic patch
- Flip one operator to **free**
- Now it becomes an independently tunable oscillator, but still connected by modulation
- Sequence or retune it for controlled destabilization

### Pair with
- external quantizer to free operators
- manual controller
- sequential CV sources

### Musical result
- harmonic patch “breaking apart”
- evolving from chord to chaos
- tonal center with one rogue voice
- live improvisation transitions

---

## 13. Use it as a modulation source for wavetable, filterbank, or spectral modules

Because outputs can be audio or CV-rate in LFO mode, Quad Operator pairs beautifully with modules that reward **multiple related modulations**.

### Excellent destinations
- filter banks
- spectral processors
- scan mixers
- wavetable position inputs
- granular parameter CVs

### Specific pairings
- **Rossum Morpheus**: multi-axis evolving FM-derived modulation is incredible here
- **XAOC Odessa/Hel**: use Quad Operator as spectral animation CV source or external audio interplay
- **4ms SMR**: use operators to animate bands or excite resonances
- **Mutable Frames / scan mixers**: use related LFOs for coordinated movement
- **Morphagene / granular modules**: synchronized but different modulation on slide/gene/size/varispeed

### Musical result
- structured complexity
- very “composed” modulation
- repeating-but-not-repetitive motion
- digital ecosystem sounds

---

## 14. Cross-patch with another FM oscillator for a larger operator network

Quad Operator gets especially wild when combined with another FM-capable oscillator or voice.

### Ideal partners
- Make Noise **DPO**
- Intellijel **Rubicon 2**
- Instruo **Cs-L**
- Yamaha-ish digital sources like **Akemie’s Castle**
- any clean sine-capable oscillator

### Patch ideas
#### A. External master modulator
Use a second VCO into AR FM to drive all operators from one external source.

#### B. Carrier extraction
Use Quad Operator as a 4-op modulator bank and another oscillator as the audible carrier elsewhere.

#### C. Cross-feedback duet
Patch one Quad operator into the second oscillator’s FM input, then return that oscillator to AR FM.

### Musical result
- larger FM networks
- hybrid analog/digital complexity
- more organic beating and drift
- massive drones

---

## 15. Use the reset input for repeatable transients and “sequenced timbre”

Reset is easy to overlook, but very powerful.

### Patch concept
- Send a trigger or gate pattern into **Reset**
- Especially useful in **LFO mode** or for short percussive FM phrases
- Every note or bar begins with the same phase relationship

### Why that matters
FM can sound wildly different depending on phase start. Resetting:
- tightens attacks
- makes percussive patches more repeatable
- makes modulation patterns line up rhythmically

### Pair with
- trigger sequencer
- clock divider
- burst generator

### Great modules
- Pam’s
- Temps Utile
- Marbles gates
- logic modules for irregular resets

### Musical result
- repeatable digital plucks
- sequenced timbre loops
- more punchy percussion
- synchronized modulation choreography

---

## 16. Pair with matrix mixers and feedback utilities for “meta-FM”

If you like deep patching, put the Quad Operator into a larger patch-programmable network.

### Modules that shine here
- **Matrix mixer**: A-138m, Instruo Lion, AI Synthesis Matrix Mixer, Livestock Maze if available
- **Polarizer/attenuverter**
- **Feedback/route processors**
- **Comparators and logic**

### Patch concept
- Take 2–4 operator outputs into a matrix mixer
- Route combinations to:
  - AR FM
  - filter FM
  - wavefolder CV
  - VCA CV
- Send external audio back into the matrix
- Use attenuation to control chaos

### Musical result
- recursive patches
- cybernetic drones
- self-playing systems
- “instrument as ecosystem” behavior

---

## 17. Best module categories to pair with Quad Operator

If you want a shopping/prioritization list, these are the most synergistic companions.

### Highest-value pairings
1. **Quad envelopes**
2. **Quad VCA / CV processor**
3. **Precision quantizer**
4. **Stereo mixer/panner**
5. **Filter with good audio-rate FM response**
6. **Wavefolder or saturation**
7. **Delay/reverb for metallic FM tails**
8. **External oscillator for AR FM**
9. **Clock/reset source**
10. **Matrix mixer**

---

## 18. A few complete patch recipes

## Patch 1: Glass electric piano
- All operators in lock
- All shapes sine
- Op 1 = main output
- Op 2 modulates Op 1 moderately
- Op 3 modulates Op 2 lightly
- Envelope to Gain CV of Op 2 and Op 3 with fast decay
- Slight detune on Op 2 or Op 3
- Output to stereo chorus/reverb

**Add-on modules:** Quadrax, FX Aid, stereo mixer

---

## Patch 2: Metallic drone organism
- Ops 1–3 in lock, Op 4 free
- Op 4 slowly tuned against the others
- Self-mod on Op 2 and Op 4
- Op 1 output to main mixer
- Op 3 through filter into AR FM as feedback path
- Slow random CV to shapes and gains
- Heavy reverb after stereo mix

**Add-on modules:** random source, filter, VCA, reverb

---

## Patch 3: Quad phase-locked modulation brain
- LFO mode
- All operators locked at different integer ratios
- Reset from master clock every 1 or 2 bars
- Op 1 modulates filter cutoff
- Op 2 modulates stereo pan
- Op 3 modulates delay feedback
- Op 4 modulates wavefolder symmetry
- Main audio comes from another oscillator or voice

**Add-on modules:** Pam’s, stereo effect chain, filter, panner

---

## Patch 4: Industrial percussion lab
- VCO mode
- Op 1 = kick/tom body
- Op 2 and Op 3 = noisy/metallic modulators
- Op 4 free/self-mod for clank
- Triggered envelopes to gain CVs
- Reset per hit or per pattern
- Distortion and compressor after mix

**Add-on modules:** trigger sequencer, envelopes, distortion, compressor

---

## Patch 5: Harmonic chord swarm
- All ops free
- Tune to 1–3–5–7 chord tones
- Slightly different shapes
- Slow independent LFO to gain CVs
- Pan each output differently
- Send only one or two operators into internal FM matrix for subtle coupling

**Add-on modules:** quantizer, panner, modulation sources, reverb

---

## Final thoughts

The most important insight from the manual is this:

**Quad Operator is at its best when you think of it as a network, not a single oscillator.**

The magic comes from:
- animating **Gain CV**
- exploiting **lock vs free**
- using the **AR FM input** as a bridge to the rest of the rack
- treating the **4 outputs** as independent voices or modulation sources
- using **reset** and **LFO mode** for structured, phase-related modulation

If you want, I can also turn this into:
1. a **“best companion modules by budget” list**,  
2. a **set of techno/ambient/experimental patch recipes**, or  
3. a **signal-flow diagram cheat sheet** for Quad Operator patching.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)