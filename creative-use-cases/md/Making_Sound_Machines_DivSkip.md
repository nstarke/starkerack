# Making Sound Machines — DivSkip

- [Manual PDF](../../manuals/SKORPION_Manual.pdf)

---

[Manual PDF](https://wmdevices.com/cdn/shop/files/Skorpion_Manual_Rev1.00.pdf)

# WMD Skorpion — Creative Patch Ideas and Pairings

Skorpion is much more than a wavefolder. Reading the manual closely, it behaves like a **threshold-analyzed waveform reanimation system** with:

- 8 comparator thresholds
- a vector core that slews toward a target
- selectable target behavior
- per-segment target sequencing
- feedback-based slope shaping
- stereo widening/delay
- a surprisingly deep internal modulation system
- lots of derived outputs for self-patching and ecosystem integration

That means it sits somewhere between:

- wavefolder
- comparator bank
- segmented function generator
- waveshaper
- stereo processor
- control voltage extractor
- weird oscillator core companion

So the most interesting use of Skorpion is often **not** “audio in, more harmonics out,” but rather:
- **using the thresholds as a control structure**
- **using the TRGTs as a sequence engine**
- **using the auxiliary outputs as modulation infrastructure**
- **using external modules to animate target, halt, fold, and shape in coordinated ways**

---

## Best companion module types

These are the module categories that pair especially well with Skorpion:

1. **Clean analog VCOs**
   - Sine/triangle sources let you hear the threshold behavior clearly.
   - Examples: Intellijel Dixie II+, Joranalogue Generate 3, Doepfer A-110-1, AJH VCOs

2. **Complex or unstable sound sources**
   - Wavetables, drum voices, feedback oscillators, or physical modeling voices create rich threshold crossing behavior.
   - Examples: Noise Engineering voices, Make Noise DPO, Instruō Cs-L, Mutable Plaits, SSF Zephyr

3. **Function generators / envelopes**
   - Great for animating FOLD, SHIFT, TARGET, HALT, or OUTPUT.
   - Examples: Make Noise Maths, Joranalogue Contour 1, Frap Tools Falistri, Befaco Rampage

4. **Matrix mixers / CV mixers / attenuverters**
   - Essential because Skorpion is a self-modulation playground.
   - Examples: Doepfer A-138m, Happy Nerding 3xMIA, Frap Tools 321, Mutable Shades

5. **Sequential switches / comparators / logic**
   - Excellent for exploiting G(IN>0), ±G(DIR), COUNT, and DAC outputs.
   - Examples: Doepfer A-151, Joranalogue Compare 2, Noise Engineering Vice Virga, Klavis Two Bits

6. **VCAs**
   - Needed to dynamically control feedback and self-patching intensity.
   - Examples: Intellijel Quad VCA, Mutable Veils, Xaoc Tallin, ALM Tangle Quartet

7. **Filters / resonators**
   - Because Skorpion can get aggressive quickly; filtering after or before it is powerful.
   - Examples: Xaoc Belgrad, Bastl Ikarie, Rossum Linnaeus, QPAS, Doepfer SEM filter

8. **Delays / reverbs / granular modules**
   - Since Skorpion already creates complex transient-rich material, time-based modules make it explode into atmosphere.
   - Examples: Mimeophon, Magneto, Nautilus, Desmodus Versio, Arbhar, Beads

9. **Oscilloscope / tuner / analyzer**
   - Seriously useful here. This module’s behavior is easier to understand visually.
   - Examples: Mordax Data, O’Tool+

---

# How to think about Skorpion musically

A useful way to approach it:

- **FOLD** = how hard the signal engages the threshold structure
- **SHIFT** = asymmetry / bias / pseudo-frequency-shift-like motion
- **SLOPE** = the “speed” and harmonic density of the output core
- **TARGET** = what the vector core is trying to become
- **SHAPE** = nonlinear behavior / feedback law
- **THLD sliders** = where folding events occur
- **TRGT sliders** = per-segment destination/slope sequence
- **HALT** = freeze motion for rhythmic or stepped artifacts
- **OUTPUT** = dry/wet/wide stereo animator

This makes Skorpion ideal for:
- animated timbral sequencing
- stereo sound design
- pseudo-resynthesis
- patch-programmable distortion
- CV generation from audio

---

# Creative patch ideas

## 1. Precision animated wavefolder voice
**Pair with:** clean VCO, envelope, VCA, filter

### Patch
- VCO sine or triangle → **IN**
- 1V/OCT sequence → VCO and **Skorpion 1V/OCT**
- Envelope → VCA for amplitude
- Slow LFO → **SHIFT**
- Another envelope or velocity CV → **FOLD**
- OUT L/R → stereo mixer

### Why it works
The manual notes that **1V/OCT controls slope and is necessary for equal timbre across notes**, so Skorpion can track musically more consistently than many wavefolders. This makes it unusually good as part of a melodic voice rather than just an effect.

### Extra move
- Set **EQUALIZE THLDs ON** for more classic wavefolder behavior.
- Then switch it off and manually spread thresholds for more formant-like uneven spectra.

---

## 2. Use it as a “comparator sequenced timbre engine”
**Pair with:** any oscillator, clocked modulation, quantizer optionally

### Patch
- Put **TARGET** to **SLIDERs**
- Hold spring toggle left and set the **TRGTs** to a pattern of voltages
- Feed a harmonically changing oscillator or chord mixture into **IN**
- Use **TARGET ORDER**:
  - **SEQ** for count-based target stepping
  - **TIED** for “most recently crossed threshold” behavior

### Why it works
Every threshold crossing can select or influence a different target. So the incoming waveform isn’t just being folded — it is effectively **navigating a table of destination voltages**. That’s way beyond standard wavefolding.

### Pairing suggestion
- Put a **quantizer** after the **TRGTs output** and use it elsewhere in your patch.
- Or use **TRGTs output** to modulate another oscillator’s FM index or filter cutoff.

---

## 3. Audio-rate CV extractor / control bus generator
**Pair with:** logic, sequential switch, percussion modules, LPGs

Skorpion’s lower jack row is gold:
- **ABS(IN)**
- **G(IN>0)**
- **TRGTs**
- **DIFF**
- **±G(DIR)**
- **COUNT**
- **DAC**
- **DELAY**

### Patch concept
Use one audio source into Skorpion, but use the aux outputs to drive the rest of your rack.

### Example
- Drum loop or percussion oscillator → **IN**
- **G(IN>0)** → trigger percussion accents or logic
- **COUNT** → filter cutoff staircase
- **DAC** → oscillator FM amount
- **DIFF** → wavefolder amount on a second voice
- **±G(DIR)** → panner or bipolar CV destination
- **ABS(IN)** → VCA CV or LPG strike level

### Why it works
Skorpion effectively turns one sound into a **family of musically related control signals**. This is amazing for coherent patches where everything “breathes” with one source.

---

## 4. Stereo psychoacoustic lead processor
**Pair with:** mono synth voice, stereo mixer, reverb

### Patch
- Mono lead voice → **IN**
- Set OUTPUT around noon and above
- Toggle **OUTPUT SWITCH** between:
  - **DC** for raw width
  - **FILTERS** for centered low end and widened highs
- OUT L/R → stereo reverb

### Why it works
The manual explains the **WIDE** section introduces a very short delay plus optional mid/side filtering. That makes Skorpion an excellent **stereoizer** even before getting extreme with fold/shaping.

### Nice companion modules
- Stereo reverb: Desmodus Versio, Erbe-Verb, FX Aid Pro
- Stereo mixer: Worng, Toppobrillo, Cosmotronic mixer systems

---

## 5. Metallic percussion from halted segments
**Pair with:** trigger source, envelope generator, noise or sine source

### Patch
- Sine or short-decay sound → **IN**
- Set **TARGET** to **SLIDERs**
- Set some TRGT sliders fully down to 0
- Turn **HALT IF TARG=0** on
- Use a sequencer or random CV to animate thresholds or target mod
- Optionally use **SYNC HARD**

### Why it works
The manual states that when a target is 0 and this mode is enabled, the vector core can **halt for just that segment**, creating square/flat regions. This can generate jagged, percussive, digitally fractured tones.

### Extra spice
- Patch **±G(DIR)** or **COUNT** into **HALT** through a VCA for intermittent freezing.
- Great with LPGs after Skorpion.

---

## 6. Drum loop destroyer / re-animator
**Pair with:** sample player, breakbeat source, envelope follower, filterbank

### Patch
- Drum loop or hi-hat pattern → **IN**
- **SYNC HARD** on for aggressive resets, or **SOFT** for smoother contour following
- Modulate **FOLD** and **SHIFT** slowly
- Use **DRY IF NO THLDs** on if modulating heavily, so signal remains present
- WIDE output to stereo mixer

### Why it works
The manual specifically mentions fast switching from cymbals and handling complex signals well. Skorpion seems excellent on transient-rich audio.

### Pairing recommendations
- Any sample player: Squid Salmple, Bitbox, Assimil8or
- Envelope follower before or after to create closed-loop modulation
- Filterbank for spectral emphasis after Skorpion

---

## 7. “Pseudo frequency shifting” motion using SHIFT
**Pair with:** slow LFO, random source, stereo delays

### Patch
- Sustained saw or sine drone → **IN**
- Keep **SHIFT** near noon, modulate slowly with triangle/random
- Moderate **FOLD**
- Experiment with **SHAPE = DIR**, **OUT**, or **DIFF**
- OUTPUT into WIDE region

### Why it works
The manual explicitly notes: **slow modulation of SHIFT produces a frequency shift effect**. It’s not true frequency shifting, but it gives spectral drift and asymmetry movement that feels similar.

### Great companion modules
- Slow random CV: Triple Sloths, Sapèl, Wogglebug, Marbles
- Stereo delay/reverb after Skorpion for moving cloud textures

---

## 8. Self-modulated chaos patch
**Pair with:** mixer/attenuverter, VCA, optional limiter

Skorpion invites self-patching.

### Patch ideas
- **DIFF** → **SHAPE CV**
- **COUNT** → **FOLD CV**
- **DAC** → **SHIFT CV**
- **DELAY** → **SHAPE source = DELAY**
- **TRGTs out** → **TARGET CV**
- **±G(DIR)** → external VCA that controls amount of one of the above

### Why it works
The module already exposes internal logic and trajectory-related signals. Feeding them back through attenuation gives evolving, nonlinear behavior that can go from organic to feral.

### Important
Use attenuverters or VCAs. Raw self-patching may jump to extremes quickly.

### Best helper modules
- Happy Nerding 3xMIA
- Frap Tools 321
- Intellijel Quad VCA
- Doepfer matrix mixer

---

## 9. Segment-by-segment waveshaping with TRGTs as a wavetable
**Pair with:** VCO, clock divider, sequencer, sample-and-hold

### Patch
- Oscillator → **IN**
- **TARGET** toward **SLIDERs**
- Hold left and set a custom 8-step TRGT pattern
- Set **TARGET ORDER** to **SEQ**
- Modulate threshold positions so the active count changes dynamically

### Why it works
The TRGT sliders effectively form a **voltage table** that can be addressed by threshold crossings. You can think of this as a kind of analog “wavetable by threshold state.”

### Extended version
- Send **TRGTs output** to a precision adder or quantizer
- Use the same sequence to drive pitch-related changes elsewhere, tying timbre and harmony together

---

## 10. Use Skorpion as an oscillator companion, not the main effect
**Pair with:** thru-zero FM oscillator, sub-oscillator, LPG

### Patch
- Main oscillator goes dry to mixer
- Duplicate same oscillator to **Skorpion IN**
- Process only Skorpion path
- Use **OUTPUT** to blend dry/wet/wide
- Tune the processed channel lower in mix and stereo spread it

### Why it works
Since Skorpion doesn’t simply amplify the original into folds, it can act like a **parallel synthetic overtone layer**. Blending processed and dry paths creates unusually rich and mix-friendly tones.

### Great sources
- TZFM oscillator like Generate 3 or Rubicon 2
- A pure sine carrier is especially strong here

---

## 11. Cross-synthesis using external CLIP input
**Pair with:** second oscillator, drum voice, speech/sample source

### Patch
- Oscillator A → **IN**
- Oscillator B or drum/sample voice → **CLIP**
- Turn **TARGET** toward **CLP**
- Optionally patch modulation into **TRGT MOD**

### Why it works
The manual says the input normally goes to CLIP, but you can override it. This lets one signal determine how another signal’s target behavior is clipped/overlaid. That’s a pretty unusual cross-modulation route.

### Good pairing sources
- Spoken word sample into CLIP
- Kick drum into CLIP while a bass tone goes into IN
- Another VCO at a harmonic or inharmonic interval

This can create vocalized, sync-like, or punctuated timbres.

---

## 12. Rhythmic gating and animation from direction outputs
**Pair with:** logic, VCAs, switches, panners

### Patch
- **±G(DIR)** → bipolar CV for panner
- **G(IN>0)** → trigger envelope
- **COUNT** → switch address or logic threshold
- **DAC** → slew limiter input or offset generator

### Why it works
Skorpion reveals the **movement state** of the vector core. That means you can synchronize other events to whether its internal waveform is rising/falling, above/below zero, or how many thresholds are currently active.

### Result
A whole patch can be rhythmically “played” by Skorpion’s internal motion rather than by clocks alone.

---

## 13. Audio-to-CV articulation extractor
**Pair with:** envelope follower, LPG, filter, resonator

### Patch
- Voice, field recording, or acoustic instrument through preamp → **IN**
- Use:
  - **ABS(IN)** as a rough excitation contour
  - **G(IN>0)** as polarity-derived gate
  - **COUNT** for brightness control
  - **DIFF** for resonator excitation
- Send those to other modules while also using OUT L/R as audio

### Why it works
Skorpion can derive **structure** from incoming audio, not just transform tone. This makes it useful in hybrid/acoustic modular setups.

### Strong companions
- Preamp/external input module
- Resonator: Rings, Sealegs resonant modes, QPAS pinging, 4ms ensembles

---

## 14. Threshold-LFO macro performance patch
**Pair with:** keyboard controller, gate source, sequencer

The internal macro section is easy to overlook but very powerful.

### Patch
- Use the **MACRO ENV** gate from external keyboard or sequencer
- Program:
  - threshold LFO amount
  - threshold LFO rate
  - FOLD/SLOPE/SHIFT/SHAPE macro modulation
- Build a performance patch where each note opens a whole moving timbral ecosystem

### Why it works
All LFOs are amplitude-controlled by the macro envelope and **reset on each gate**, so repeated notes can have **consistent animated timbre articulation**. That is very performable.

### Musical use
This is ideal for:
- animated leads
- evolving bass
- repeatable IDM percussion
- “same note, new motion” phrasing

---

## 15. Patch it with a filter before and after
**Pair with:** multimode filter(s)

### Before Skorpion
Filtering before changes which parts of the source cross thresholds.

### After Skorpion
Filtering after sculpts the newly generated harmonics.

### Example chain
- VCO → bandpass filter → Skorpion → lowpass filter → stereo FX

### Why it works
Because Skorpion responds strongly to waveform geometry, **pre-filtering** is as meaningful as post-filtering.

### Especially good
- Bandpass or notch before Skorpion
- LPG or resonant lowpass after it

---

## 16. Use DELAY output as a modulation source
**Pair with:** VCA, filter FM, panning, phase modulation destination

The manual notes the **DELAY** output is tied to the WIDE portion of the output control and changes delay time/modulation depending on the knob position.

### Patch
- Bring OUTPUT above noon so DELAY becomes active
- **DELAY output** → SHAPE CV, filter cutoff, or panner
- Audio out still goes to stereo path

### Why it works
This gives you a delayed/modulated copy of Skorpion’s motion as a CV/audio source. Very useful for internal “echo modulation.”

---

## 17. Make it a weird CV processor for non-audio signals
**Pair with:** sequencers, stepped CV, envelopes, joystick

You do not have to feed only audio into Skorpion.

### Patch ideas
- Envelope or LFO → **IN**
- Use threshold crossings to create staircase, folded, or halted control trajectories
- Output to:
  - filter FM
  - wavetable position
  - panning
  - granular position

### Why it works
Skorpion’s vector core and threshold system can turn simple CV into:
- segmented envelopes
- staircase hybrids
- asymmetrical modulation
- direction-aware control signals

This is one of the most underused ways to exploit it.

---

# Specific pairing ideas by module

## With Make Noise Maths
- Use channels 2/3 as attenuation for self-patching Skorpion outputs back into CV inputs
- Use Maths envelopes to modulate HALT, SHIFT, and FOLD
- Feed **DIFF** or **COUNT** into Maths for slewed derived CV

## With Joranalogue Generate 3
- Very clean source for hearing threshold topology
- Use Generate 3’s phase/routing options to feed Skorpion harmonically precise material
- Patch Skorpion **TRGTs** or **DAC** back into Generate 3’s FM index or phase modulation

## With Mimeophon
- Use Skorpion for primary stereo widening, then Mimeophon for larger spatial extension
- DELAY output can modulate Mimeophon color or zone

## With Xaoc Belgrad
- Belgrad before Skorpion for focused band emphasis
- Belgrad after Skorpion to tune the harmonic chaos into vocal resonances

## With Mutable Rings / resonator-type modules
- Use **DIFF**, **COUNT**, or **ABS(IN)** to excite/modulate resonator parameters
- Use Skorpion output as exciter audio for metallic, animated resonances

## With random modules like Marbles / Sapèl / Wogglebug
- Randomly modulate threshold equalization on/off via jack
- Animate SHIFT and TARGET subtly
- Use stepped randomness on TRGT MOD for spectral jumps

## With matrix mixer
Probably one of the best utilities for Skorpion.
- Route **COUNT**, **DAC**, **DIFF**, **TRGTs**, and **DELAY** into a matrix mixer
- Send blended versions back to **FOLD**, **SHIFT**, **SHAPE**, and **TARGET**
- This creates deeply connected feedback ecosystems

---

# Particularly strong self-patching ideas

## Self-patch 1: DIFF into SHAPE
- Set SHAPE source to **DIFF**
- Also patch **DIFF out** externally through attenuation back into **SHAPE CV**
- Result: edgy, spiky, unstable harmonic emphasis

## Self-patch 2: COUNT into FOLD
- COUNT is a staircase based on active thresholds
- Feed it gently into FOLD CV
- Result: more threshold activity begets more fold intensity

## Self-patch 3: DAC into SHIFT
- Weighted threshold count gives more nuanced asymmetry changes
- Result: continuously morphing asymmetry tied to comparator state

## Self-patch 4: DELAY into TRGT MOD
- Great for ghosted, smeared target behavior
- Especially effective in stereo/wide settings

## Self-patch 5: G(IN>0) or ±G(DIR) into external switch
- Switch between two modulation sources feeding FOLD or TARGET
- Result: waveform-dependent timbral branching

---

# Modes and switches worth exploiting

## EQUALIZE THLDs
This is not just convenience. It is a tonal mode switch.

- **ON**: more classic, orderly, predictable fold intervals
- **OFF**: irregular threshold spacing = speech-like, formant-like, broken spectra
- **CV controlled**: ideal for switching between orderly and unruly states mid-performance

Use a gate sequencer, logic output, or random gate here.

---

## DRY IF NO THLDs
Useful when:
- heavily modulating FOLD
- processing dynamic material
- wanting continuity rather than dropout

This can make Skorpion act more like a morphing timbre processor than a hard-effect box.

---

## SYNC soft vs hard
- **SOFT**: smoother, more “rubbery” and less clicky
- **HARD**: sharper resets, more aggressive and percussive
- **X**: freer motion, often more organic

Good idea: modulate related parameters while manually changing SYNC mode during performance.

---

## TARGET ORDER: SEQ vs TIED
This is one of the most musically consequential switches.

- **SEQ** = active-threshold count selects target  
  Feels more like addressable sequence behavior
- **TIED** = most recently crossed threshold selects target  
  Feels more event-driven and contour-sensitive

Use:
- **SEQ** for repeatable timbral sequences
- **TIED** for expressive, waveform-reactive articulation

---

# Patch recipes by musical goal

## For bass
- Sine/triangle in
- 1V/OCT patched
- EQUALIZE THLDs on
- TARGET around 5V or slight CLIP
- mild SHAPE from OUT
- FILTERS mode on output
- low wet/wide blend

## For harsh industrial leads
- Saw or wavetable in
- TARGET to SLIDERs
- SHAPE source = DIFF
- SYNC HARD
- modulate SHIFT and TRGT MOD
- output into saturation or reverb

## For evolving drones
- Slow LFO/random into SHIFT, SHAPE, TARGET
- SHAPE source = DELAY or OUT
- wide stereo output
- post-process with reverb/granular

## For percussion
- short sine burst or click into IN
- TARGET sliders with some zero stages
- HALT IF TARG=0 on
- SYNC HARD
- use COUNT or DIFF elsewhere in patch for coherent percussion CV

## For generative patches
- use macro envelope + threshold LFOs
- self-patch aux outputs through matrix mixer
- route TRGTs output to other modules
- randomize equalize/sync/target behavior externally

---

# A few “hidden gem” uses from the manual

## 1. TRGTs output as its own sequencer
This is easy to miss. The TRGTs are not just internal. Use them externally as:
- 8-step wavetable-ish source
- sequencer for filter cutoff
- modulation lane tied to threshold events

## 2. ABS(IN) output
Full-wave rectified input is super useful for:
- unipolar envelope-like behavior
- modulation from bipolar oscillators
- driving VCAs or LPGs

## 3. COUNT vs DAC
These are related but distinct:
- **COUNT** = equal 0.5V steps
- **DAC** = weighted threshold contributions

COUNT is rhythmic and obvious. DAC is subtler and more “encoded.”

## 4. CLIP external override
This turns Skorpion into a cross-processor, not just a folder.

## 5. Non-audio-rate modulation on thresholds
Threshold modulation can radically alter where folds occur. This is one of the most powerful and least conventional aspects of the module.

---

# Recommended support rack around Skorpion

If you wanted to build a mini ecosystem around it, I’d suggest:

- **1 precise analog oscillator**
- **1 weird digital/noisy oscillator or sample source**
- **1 dual function generator**
- **1 matrix mixer**
- **1 quad VCA**
- **1 multimode filter**
- **1 stereo reverb/delay**
- **1 random/stepped CV source**
- **1 logic/switch module**

That setup would let Skorpion operate as:
- voice processor
- modulation extractor
- stereo timbre designer
- self-patched chaos engine
- cross-modulation hub

---

# Final thoughts

Skorpion rewards treating it less like a conventional wavefolder and more like a **threshold-addressed analog computation module for sound and CV**. The deepest patches come from:

- modulating the threshold structure
- using TRGTs as an addressable voltage table
- self-patching the auxiliary outputs
- leveraging external VCAs/mixers to control feedback paths
- processing non-sine, nontraditional sources
- using stereo width as part of the composition, not just a finishing effect

If you want, I can also provide:
1. **10 beginner-friendly Skorpion patches**
2. **10 advanced self-patching feedback patches**
3. **a “best companion modules by brand” list**
4. **a compact performance cheat sheet for this module**

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)