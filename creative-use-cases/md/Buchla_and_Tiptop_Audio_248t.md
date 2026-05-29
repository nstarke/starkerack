# Buchla and Tiptop Audio — 248t

- [Manual PDF](../../manuals/Buchla_&_Tiptop_Audio_248t.pdf)

---

[Manual PDF](https://tiptopaudio.com/manuals/248t/Tiptop_Audio_248t_MARF_User_Manual.pdf)

# Tiptop Audio / Buchla 248t MARF — creative patch ideas and module pairing analysis

The **248t MARF** is much more than a sequencer. It’s really a **two-lane, stage-addressable, programmable CV choreography system** with:

- 16 stages
- per-stage voltage
- per-stage time
- per-stage pulse assignment
- per-stage behavior modifiers
- two independent function generators reading the same 16-stage memory
- internal or external addressing
- voltage and time outputs simultaneously
- ART + analog CV outputs
- external CV substitution for stage voltage or stage time

That means it can behave as:

- a pitch sequencer
- a timing sequencer
- a burst/gate pattern generator
- a dual related sequencer
- a programmable slew/portamento source
- a voltage-addressed preset scanner
- a CV processor for external signals
- a semi-generative compositional brain

Below are practical and musical ways to pair it with other Eurorack modules.

---

## Quick mental model: what the 248t is best at

The MARF shines when you use it for **phrasing**, not just note order.

Its real strengths are:

- **different duration per step**
- **different behavior per step**: stop, sustain, enable, first/last loop boundaries
- **different pulse maps per step**
- **independent stage traversal by two function generators**
- **external CV becoming “stage data”**
- **continuous stage addressing for scanning/morphing behavior**

So instead of asking “what melody should I sequence?”, a better question is:

> “What musical process do I want staged over time?”

---

# Best partner module categories

## 1. Complex oscillators / precision VCOs
The obvious pairing, but still one of the richest.

### Why it works
- Quantized MARF stages become melodic structure.
- Sloped stages create glides tied to stage duration.
- Half-range and limited range are especially useful for playable pitch spans.
- ART output is designed for 259t-style precision control.

### Great pairings
- **Tiptop/Buchla 259t**
- **Make Noise DPO**
- **Frap Tools Brenso**
- **Instruō Cs-L**
- **Intellijel Rubicon 2 + Dixie 2+**
- any stable 1V/oct VCO

### Creative uses
- **Lane 1 = pitch, Lane 2 = timbre animation**  
  Send FG1 voltage to oscillator pitch and FG2 voltage to wavefolder amount, FM index, or symmetry.
- **Time-derived timbre**  
  Patch a MARF **Time Output** to wavefolder depth or filter resonance, so longer notes also become brighter or more intense.
- **Glide only on chosen notes**  
  Use the **Sloped** modifier only on specific stages to create selective portamento instead of global glide.

---

## 2. Low pass gates and VCAs
This is one of the most Buchla-native uses of the MARF.

### Why it works
The manual specifically notes the **Reference Output** is a downward ramp over the stage interval and is useful for driving a **292t LPG** directly.

### Great pairings
- **Tiptop/Buchla 292t**
- **Make Noise Optomix**
- **Doepfer A-101-2**
- **Random*Source LxD style LPG/VCA combos**
- any clean VCA for amplitude articulation

### Creative uses
- **Patch the Reference Output directly to LPG CV**
  - Voltage output controls pitch
  - Reference output shapes amplitude
  - Pulse output triggers secondary events
  This creates very “self-contained phrase cells.”
- **Use Pulse 1 and Pulse 2 to articulate different VCAs**
  - Pulse 1 opens a melodic voice
  - Pulse 2 opens a noise/percussion layer
- **Unequal note lengths become unequal envelope lengths**
  Since the reference ramp follows stage duration, the amplitude contour naturally reflects rhythmic phrasing.

---

## 3. Envelope generators / function generators
MARF becomes a conductor for layered articulation.

### Great pairings
- **Make Noise Maths**
- **Frap Falistri**
- **Intellijel Quadrax**
- **Xaoc Zadar**
- **Befaco Rampage**
- **Doepfer A-140-2 / A-171-2**

### Creative uses
- **Use Pulse 1 for short envelopes, Pulse 2 for long envelopes**
  Send them to different envelope generators, then mix or route them to different destinations.
- **Gate pattern extraction**
  Program pulse outputs on certain stages and use them to trigger envelopes independently of the main pitch line.
- **Conditional envelope shape**
  Use MARF’s **Stop / Sustain / Enable** stages to create places where an external gate must “unlock” the phrase, while envelopes continue to behave differently downstream.

---

## 4. Sequential switches / matrix routers
This is one of the best non-obvious uses.

### Great pairings
- **Doepfer A-151 / A-152**
- **Boss Bow Two / similar router**
- **Verbos Sequence Selector**
- **Worng SoundStage-style routing context**
- **Any sequential switch / matrix mixer**

### Creative uses
- **Pulse outputs as routing logic**
  Use Pulse 1 / Pulse 2 / All Pulses to switch audio sources, FX sends, or modulation destinations.
- **Stage-addressed orchestration**
  Let MARF pitch a voice while also changing:
  - which oscillator is heard
  - which filter receives it
  - which effect send is active
- **Two FGs, one memory, different outputs**
  One FG can drive pitch while the other, with different addressing, triggers switches for arrangement-level changes.

---

## 5. Sample & hold / random / uncertainty modules
MARF pairs beautifully with controlled randomness.

### Great pairings
- **Make Noise Wogglebug**
- **Mutable Marbles**
- **Verbos Random Sampling**
- **SSF Ultra-Random**
- **Doepfer A-149-1 / A-149-2**
- **Turing Machine + expanders**

### Creative uses
- **External voltage source mode**
  Set some stages’ voltage source to **External**, and patch random CV into A/B/C/D.  
  Now the slider chooses which external stream is active per stage.
- **External time control**
  Feed random CV into A/B/C/D and use it as **time source** on selected stages, making note duration probabilistic.
- **Structured randomness**
  Alternate between internal programmed stages and externally sourced random stages.  
  Result: composed phrases with pockets of uncertainty.
- **Generative gate unlocking**
  Use random gates into the **Start** input on stages programmed with **Enable** or **Sustain** to create semi-autonomous phrasing.

---

## 6. Quantizers and harmonic processors
Even though the MARF already quantizes, external harmonic processors expand it.

### Great pairings
- **Intellijel Scales**
- **ADDAC quantizers**
- **Shakmat Bard Quartet**
- **O_C / Ornament & Crime**
- **precision adder / transposer modules**

### Creative uses
- **Use MARF unquantized, then quantize externally**
  This lets you preserve MARF slider nuance while changing scale systems on the fly externally.
- **Dual-layer pitch logic**
  - FG1 = melody
  - FG2 = transposition offset into precision adder or secondary quantizer
- **Patch Time Output into quantizer transpose**
  Longer notes can force harmonic shifts or modal changes.

---

## 7. Precision adders / offsets / utility mixers
This is where MARF becomes compositional rather than merely sequenced.

### Great pairings
- **Doepfer A-185-2**
- **Frap 321**
- **Happy Nerding 3xMIA**
- **Intellijel Triplatt**
- **Befaco A*B+C**
- any offset/attenuverter/mixer utility

### Creative uses
- **Two-FG harmonic relationship**
  Mix the outputs of both function generators:
  - one sets root movement
  - the other sets interval color
- **Use one FG as transposition of the other**
  Create phrases that recur with shifting interval frameworks.
- **Dynamic time scaling**
  Send slow CV through an attenuverter into the **Time Multiplier CV** for macro-form tempo breathing.

---

## 8. Filters and resonators
The per-stage timing and voltage control make for excellent spectral choreography.

### Great pairings
- **Rossum Morpheus**
- **Mutable Ripples / clones**
- **QPAS**
- **Belgrad**
- **Three Sisters**
- **Twin Peak or multimode filters**
- **resonator banks / modal filters**

### Creative uses
- **Pitch to oscillator, Time Output to filter cutoff**
  Longer notes open the filter further, or vice versa.
- **Second FG as formant sequencer**
  Keep one FG on pitch and use the other to sequence filter frequency or resonance.
- **Continuous stage address as scanned filter choreography**
  Set stage address to continuous and sweep across programmed voltages like a performance macro over a filter bank.

---

## 9. Effects: delay, reverb, granular, spectral processors
MARF can create highly staged FX composition.

### Great pairings
- **Mimeophon**
- **Chronoblob / delay**
- **Erbe-Verb**
- **FX Aid**
- **Arbhar / granular**
- **Data Bender**
- **Beads / Clouds-style texture processors**

### Creative uses
- **Pulse 2 as sparse FX send trigger**
  Only certain stages bloom into delay or reverb.
- **Voltage output to dry voice, Time output to effect parameter**
  For example:
  - Time output → delay time, feedback, grain density, or reverb size
- **External input processing**
  Feed an LFO, random source, or joystick voltage into A/B/C/D, then let MARF decide which external source controls an FX parameter at each stage.

---

## 10. Clock dividers, logic, and trigger processors
MARF is especially deep when paired with timing utilities.

### Great pairings
- **Pamela’s Pro Workout**
- **4ms QCD**
- **Shakmat Clock O’Pawn / Time Wizard**
- **Doepfer logic modules**
- **Mutable Branches / logic probability**
- **vpme Euclidean modules**

### Creative uses
- **All Pulses output as a variable clock**
  Since each new stage emits a pulse, and each stage can have different lengths, the resulting clock is *phrased* rather than metronomic.
- **Use All Pulses to drive another sequencer**
  A second sequencer or percussion engine will inherit MARF’s irregular rhythm.
- **Logic-conditioned starts**
  Feed logic-combined gate signals into a Function Generator’s Start input so certain stages only progress under specific rhythmic conditions.
- **Stop/Sustain/Enable as form logic**
  These are effectively compositional timing conditions; use clock utilities to create “if/when” advancement behavior.

---

## 11. Joysticks, touch controllers, pressure controllers
Excellent for performance because MARF has external addressing and external source selection.

### Great pairings
- **Intellijel Planar 2**
- **Make Noise Pressure Points + Brains**
- **Soundmachines Lightstrip**
- **Bela Gliss**
- **Tetrapad / Tête**
- **joystick or CV fader banks**

### Creative uses
- **External stage address performance**
  Put stage address in **External** and scan stages manually with a joystick or fader.
- **Continuous mode as a CV lookup table**
  Program 16 stage voltages, then sweep across them like a custom transfer function.
- **Gesture to structure**
  One joystick axis controls stage address, another goes into time multiplier CV.
- **Performance-selected external sources**
  Send different controller voltages into A/B/C/D and use stage programming to choose among them across the phrase.

---

## 12. Samplers and drum modules
MARF is superb for “composed rhythm.”

### Great pairings
- **Assimil8or**
- **Bitbox**
- **Squid Salmple**
- **Basimilus Iteritas Alter**
- **WMD drum voices**
- **Tiptop one-shots / drum modules**
- any trigger-based percussion voice

### Creative uses
- **Pulse 1 = kick/snare grid, Pulse 2 = fills**
- **All Pulses = master advancement trigger for drum variation**
- **Reference output to drum timbre**
  A ramp over stage duration can modulate decay, pitch, or sample start.
- **Stage-specific duration for fills**
  Short stages for ratchets/bursts, long stages for rests or sustained space.
- **Use second FG to sequence sample select or drum morphing**
  while first FG handles pitch or melodic percussion.

---

# Especially powerful MARF-specific patch concepts

## 1. One memory, two readers
This is maybe the single most important creative feature.

Both function generators read the same 16 stages, but they can behave differently.

### Patch idea
- **FG1**: normal run, internal clock, melodic line
- **FG2**: external stage address, manually scanned or CV-addressed timbre line

Result: one set of programmed stage values yields two related but non-identical performances.

### Modules to pair
- oscillator + filter
- switch + effect
- VCA matrix

---

## 2. Stage-specific external CV substitution
This is uniquely powerful.

A stage can use internal programmed voltage or choose an external source A/B/C/D instead.

### Patch idea
Use:
- A = slow random
- B = envelope follower
- C = joystick
- D = LFO

Program different stages to select different external sources.

Now the MARF is acting like a **composed CV router/processor**, not just a sequencer.

### Great downstream targets
- oscillator pitch
- filter cutoff
- effect depth
- panning
- wavefolder amount

---

## 3. Time as music, not just timing
The lower sliders aren’t just step lengths. The **Time Output** gives you a second expressive CV related to that programmed duration.

### Patch idea
- Pitch from Voltage Output
- Amplitude contour from Reference Output
- Brightness from Time Output

Now each stage has:
- a note
- a duration
- an amplitude decay shape
- a corresponding timbral brightness value

That’s almost like per-note articulation metadata.

---

## 4. Stop, Sustain, Enable as compositional grammar
These aren’t mere performance functions; they let you create **decision points** in a sequence.

### Patch idea
- Use **Enable** on stage 8
- Feed Start input from a probabilistic gate source
- Sequence only advances past stage 8 when the condition is met

This creates:
- looping hesitation
- phrase elongation
- evolving form
- call/response delays

### Great pairings
- Bernoulli gate
- random trigger module
- logic combiners
- manual gate button
- footswitch gate interface for performance

---

## 5. Continuous Address mode as a wavetable-like CV scanner
When stage address is in **Continuous**, you can sweep through the 16 programmed values.

### Patch idea
Program stage voltages as:
- a custom scale
- non-linear modulation curve
- stepped waveshape
- chord voicing offsets

Then scan with:
- LFO
- envelope
- random smooth voltage
- joystick

This turns MARF into:
- a transfer function
- a custom quantized contour
- a CV wavetable

### Great pairings
- vector joystick
- smooth random
- envelope follower
- pressure controller

---

# Patch recipes

## Patch 1: Buchla-style animated melody voice
**Modules:**
- 248t
- 259t or any complex oscillator
- 292t or LPG
- reverb

**Patch:**
- MARF Voltage Out → oscillator pitch
- MARF Reference Out → LPG CV
- MARF Pulse 1 → LPG trigger or envelope trigger
- oscillator → LPG → reverb

**Program:**
- Quantize selected stages
- Add Sloped to a few transitions
- Vary interval times heavily
- Use First/Last to define a shorter cyclic phrase within 16 stages

**Result:**
An organic line with natural note lengths, selective glide, and Buchla-like articulation.

---

## Patch 2: Melody + timbre counterpoint
**Modules:**
- 248t
- oscillator
- filter or wavefolder
- VCA
- envelope

**Patch:**
- FG1 Voltage Out → oscillator pitch
- FG2 Voltage Out → filter cutoff or wavefolder amount
- Pulse 1 → envelope trigger
- envelope → VCA CV

**Program:**
- FG1 cycles stages 1–8
- FG2 cycles stages 5–12 or is manually addressed
- Different time multipliers for each FG

**Result:**
Pitch and timbre evolve in related but offset phrasing, giving a strong “composed” feeling.

---

## Patch 3: Composed random
**Modules:**
- 248t
- random voltage source
- quantizer or VCO
- LPG/VCA
- clock source

**Patch:**
- random CV → external input A
- some stages set Voltage Source to External
- others remain Internal
- Pulse outputs trigger articulation

**Program:**
- Stages 1–4 internal melody
- Stage 5 random note
- Stage 6 internal
- Stage 7 random note with slope
- Stage 8 stop or enable

**Result:**
A melody that feels authored but keeps opening windows of surprise.

---

## Patch 4: Irregular master clock brain
**Modules:**
- 248t
- percussion sequencer or trigger sequencer
- drum voices
- clock divider / logic

**Patch:**
- All Pulses Out → external clock input of another sequencer
- Pulse 1 → kick trigger
- Pulse 2 → accent/fill trigger
- Time sliders define macro rhythm

**Result:**
Instead of fixed clock divisions, your whole system moves according to MARF’s stage durations.

---

## Patch 5: Custom CV lookup table for effects
**Modules:**
- 248t
- joystick or LFO
- delay/reverb/granular module

**Patch:**
- Stage Address set to Continuous + External
- joystick or LFO → address CV
- Voltage Out → effect parameter
- Time Out → second effect parameter

**Program:**
Create 16 deliberate “sweet spots” for:
- feedback
- size
- texture
- grain density

**Result:**
A performance-friendly morphing effect macro that avoids dead zones.

---

## Patch 6: Harmonic duet from one sequencer memory
**Modules:**
- 248t
- 2 oscillators
- 2 VCAs/LPGs
- mixer

**Patch:**
- FG1 Voltage Out → Osc 1 pitch
- FG2 Voltage Out → Osc 2 pitch
- Pulse 1 → voice 1 envelope
- Pulse 2 → voice 2 envelope

**Program:**
- Shared stage memory
- Different first/last points
- One voice quantized, one partially sloped/unquantized

**Result:**
Two interrelated melodic voices with deep internal cohesion.

---

# Specific module recommendations that would be especially fun

## Best “Buchla-adjacent” pairing set
- **259t** — natural partner for ART and complex pitch motion
- **292t** — Reference Output becomes immediately musical
- **281t** — pulse-derived contour generation
- **245t / 246t / 257t** — utility and compositional expansion

## Great modern utility partners
- **Pamela’s Pro Workout** — clocks, gates, conditional starts
- **Maths** — shaping, slewing, mixing, envelope extraction
- **Happy Nerding 3xMIA** — indispensable offsets/scaling
- **Doepfer A-151** — cheap but transformative for routing
- **O_C** — harmonic processing, quantization, CV logic
- **Planar 2** — outstanding for external addressing and live scanning

## Great “generative” partners
- **Mutable Marbles**
- **Verbos Random Sampling**
- **Turing Machine**
- **A-149-1**
- **Branches / Bernoulli gate style modules**

## Great timbre destinations
- **QPAS**
- **Morpheus**
- **Mimeophon**
- **Data Bender**
- **Brenso / DPO / Cs-L**

---

# Less obvious but excellent uses

## Use MARF as a CV processor, not a sequencer
Feed external CV into A/B/C/D and let stage programming decide:
- whether it’s quantized
- whether it’s sloped
- what range it occupies
- when it appears

This can turn a boring LFO into a staged musical structure.

## Use it to stage modulation density
Program Pulse 1 and Pulse 2 sparsely, then use them to trigger additional modulation events only on important stages.

## Build “phrases with checkpoints”
Use Stop and Enable stages so the sequence pauses at dramatic points until another module “permits” continuation.

## Make a pseudo-arpeggiator with continuous addressing
Program chord tones across stages, then externally scan stage address with an LFO/envelope for unusual directional arpeggiation.

## Create asymmetrical loop nesting
Set First/Last boundaries differently for the two function generators so they phase against each other while sharing stage content.

---

# Practical advice for getting the most out of it

## 1. Start with half range for pitch work
The manual recommends **half range** or limited ranges with 259t. In practice this also makes all pitch sequencing easier and more musical.

## 2. Treat Time Output as equally important as Voltage Output
That’s one of the biggest “secret weapons” of the module.

## 3. Use Pulse 1, Pulse 2, and All Pulses separately
These three gate streams can drive:
- envelopes
- switches
- clocks
- resets
- accents

## 4. Reserve a few stages for external source mode
Even in a mostly programmed sequence, external-source stages create a great balance of structure and variation.

## 5. Exploit the two FGs as separate performers
Think of them as two musicians reading the same score differently.

---

# Best pairings by musical goal

## For melodic composition
- stable VCO
- quantizer or precision adder
- LPG/VCA
- envelope

## For generative music
- random CV source
- Bernoulli gate / probability gate
- logic
- clock tools

## For live performance
- joystick
- macro controller
- sequential switch
- reverb/delay

## For sound design
- complex oscillator
- wavefolder
- resonant filter
- granular/effect processor

## For rhythmic systems
- drum voices
- trigger sequencer
- clock divider
- logic processor

---

# Final thought

The 248t is most rewarding when you stop using it like a normal 16-step sequencer and start using it like a **programmable timeline of decisions**.

If you want, I can also give you any of these in one of these formats:

1. **10 concrete patch sheets** with exact cable routing  
2. **Best companion modules by budget**  
3. **A starter workflow for learning the 248t in 30 minutes**  
4. **A “best modules to pair with 248t” shopping list by manufacturer**

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)