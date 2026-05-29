# Pittsburgh Modular — "Generator"

- [Manual PDF](../../manuals/Generator - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF / Source](https://pittsburghmodular.com/generator)

# Pittsburgh Modular Generator — creative patch ideas and combo recommendations

The **Pittsburgh Modular Generator** is a compact **dual analog oscillator / FM source / modulation hub** built for unstable, aggressive, and highly animated sounds rather than precise melodic tracking. From the manual:

- **2 triangle-core oscillators**
- **Internal FM path:** Generator 1’s **Index Out** internally FM’s Generator 2
- **External FM routing:** one external modulation path can be directed to either osc 1 or osc 2
- **Shared shape control:** morphs the two oscillators in opposite directions  
  - Gen 1: square → triangle  
  - Gen 2: triangle → square
- **Index section:** a VCA on Generator 1’s output, with CV, whose output both:
  - appears at **OUT**
  - acts as the **internal FM source** for Generator 2
- Not 1V/oct, not temp compensated: best approached as a **chaotic voice, percussion engine, drone core, modulation source, and texture oscillator**

In practice, Generator excels when treated as:
1. a **cross-influenced dual osc voice**  
2. an **FM/noise/percussion source**
3. a **compound modulation module**
4. a **feedback instrument**

---

## What is special about this module musically

A few things matter a lot:

### 1. The Index VCA is the heart of the module
Generator 1 passes through a VCA-like stage controlled by the **Index knob** and **Index CV**, and that post-VCA signal is used to FM Generator 2 internally. This means:

- envelopes into **Index CV** create **dynamic FM bursts**
- slow CV into **Index CV** creates **breathing timbre shifts**
- audio-rate CV into **Index CV** creates unstable amplitude/FM interactions

This is why the module is so strong for:
- metallic percussion
- tearing basses
- unstable drones
- game-console-ish zips and sputters

### 2. The shape knob is a macro timbre control
One knob simultaneously pushes the two oscillators in **opposite waveform directions**. So with one movement you’re changing:

- harmonic content of the modulator
- harmonic content of the carrier
- FM response character

That makes it especially good with:
- CV-addressed modulation
- manual performance gestures
- stepped random
- joystick control

### 3. It loves being patched “wrong”
Because it isn’t trying to be a precision VCO, it rewards:
- self-patching
- extreme CV
- feedback loops
- offset/attenuation tricks
- clocking at subaudio or audio edge zones

---

# Best module pairings

## 1. Envelope generators / function generators
**Highly recommended types:**
- Make Noise Maths
- Befaco Rampage
- Intellijel Quadrax
- ALM Pip Slope
- Frap Tools Falistri

### Why
The Generator’s **Index CV** input is begging for envelopes. This is one of the fastest ways to animate internal FM.

### Results
- percussive FM plucks
- toms, metallic hits, lasers
- dynamic drones with shifting overtones
- pseudo-acoustic transient behavior

### Tip
Use:
- a **snappy envelope** to Index CV
- a **slower envelope** to the external FM attenuverter path
- then send the external FM to whichever oscillator is not already doing the most interesting thing

This gives layered movement: one contour for internal FM intensity, another for pitch/timbre bend.

---

## 2. VCAs and modulation utilities
**Recommended types:**
- Happy Nerding 3xVCA
- Intellijel Quad VCA
- Veils
- Mutable Instruments Blinds / Joranalogue Select 2 / bipolar VCAs
- attenuverters, offsets, mixers

### Why
Generator becomes much more powerful when CV is carefully scaled. It can get wild very fast, so utilities turn “chaos” into “playable chaos.”

### Best uses
- tame the output before filters/waveshapers
- scale random voltages going to Shape or Index CV
- create **voltage-controlled external FM depth**
- mix Generator outputs with other oscillators before ring mod or filtering

### Especially useful
A **bipolar VCA / attenuverter** before the **External Input** lets you automate the amount and polarity of FM going into Gen 1 or Gen 2.

---

## 3. Random / chaos / sample & hold modules
**Recommended types:**
- Make Noise Wogglebug
- Mutable Marbles
- SSF Ultra-Random Analog
- Joranalogue Orbit 3
- Doepfer A-118 + S&H
- noise + slew combos

### Why
Generator responds beautifully to irregular but bounded control voltages.

### Great patch targets
- **Shape**
- **Index CV**
- **External FM input attenuverter** via manual or VC processing
- oscillator EXP inputs for unstable pitch fields

### Results
- clattering, insect-like percussion
- animated drones
- semi-repeating machine chatter
- “broken console” melodies and digital-sounding analog artifacts

### Trick
Use **stepped random** to one oscillator’s EXP input and **slewed random** to Index CV.  
That gives:
- stepped pitch regions
- continuously changing FM intensity  
Very effective for evolving electroacoustic textures.

---

## 4. Filters, especially aggressive or character filters
**Recommended types:**
- MS-20 style filters
- Steiner-Parker filters
- multimode state-variable filters
- low-pass gates
- resonant band-pass filters

Specific examples:
- Bastl Ikarie
- Xaoc Belgrad
- Doepfer A-124 Wasp
- Intellijel Polaris
- Make Noise QPAS
- LPGs like Optomix, LxD

### Why
Generator can make very dense spectra. A good filter turns the chaos into a playable voice.

### Best filter strategies
- **Band-pass** for metallic percussion
- **Low-pass gate** for woody, struck sounds
- **High resonance low-pass** for mutant bass
- **Stereo dual peak filter** for drones and moving textures

### Patch idea
Take:
- **2** (Generator 2 output) into a resonant filter
- **Index OUT** into a different filter or LPG
- pan them left/right

Now you have related but not identical timbral streams from one 10hp source.

---

## 5. Wavefolders, distortions, and nonlinear processors
**Recommended types:**
- wavefolder
- saturator
- fuzz/distortion
- comparator
- rectifier

Specific examples:
- Intellijel Bifold
- Frap Tools Fold 6
- Joranalogue Fold 6
- Schlappi Interstellar Radio
- Bastl Timber
- various analog distortion modules

### Why
Generator already produces rich, unstable tones. Folding or distortion can push it into:
- industrial leads
- exploding drums
- harsh drones
- sputtering machine textures

### Best combo
Patch **Generator 2** into a wavefolder while using **Index OUT** separately as modulation or submix content.  
Because Generator 2 is being internally FM’d, folded results can become extremely vocal or metallic.

### Bonus idea
Use a **comparator** on one of the outputs to derive a dirty gate/clock from the oscillator. That can drive envelopes that come back into Index CV for self-related rhythmic behavior.

---

## 6. Ring modulators and balanced modulators
**Recommended types:**
- Doepfer A-114
- Intellijel uMod II
- ring mod / four-quadrant multiplier
- bipolar VCA

### Why
You already have two related oscillators. Ring modulation with a third oscillator or one of Generator’s own outputs produces very complex sidebands.

### Patches
- Generator 1 out into ring mod input A
- Generator 2 out into ring mod input B
- then filter the result

Or:
- Generator 2 into ring mod
- clean sine/triangle from another VCO into the other input
- envelope the final output

### Results
- bells
- sci-fi alarms
- inharmonic percussion
- robotic voice-like tones

---

## 7. Precision oscillators as stabilizing partners
**Recommended types:**
- a stable analog VCO
- a digital sine oscillator
- through-zero capable FM source if available

Specific examples:
- Dixie II+
- Rubicon
- STO
- Ts-L
- Odessa / digital clean source

### Why
Generator is unstable in a good way. Pairing it with a more stable oscillator creates contrast.

### Uses
- stable VCO provides tuned bass/fundamental
- Generator provides upper grit and movement
- stable VCO can externally FM Generator
- Generator can modulate stable oscillator’s PWM/filter/folder instead of pitch

### Best musical role
Use Generator as the **chaos layer**, not necessarily the tuning anchor.

---

## 8. Sequencers and gate sequencers
**Recommended types:**
- CV sequencer
- trigger sequencer
- Euclidean trigger source
- random sequencer

Specific examples:
- Make Noise Rene
- Intellijel Metropolix
- Winter Modular Eloquencer
- Korg SQ-1
- Pamela’s New Workout / Pro Workout
- Euclidean Circles

### Why
The Generator often shines more from **rhythmic modulation events** than traditional pitch sequencing.

### Better than sequencing pitch:
- sequence **Index CV bursts**
- sequence external FM routing changes manually between takes
- sequence filter cutoff while Generator free-runs
- use stepped CV to jump coarse regions

### Great performance setup
- trigger sequencer → envelopes → Index CV
- random/sequencer CV → one EXP input
- clocked modulation → Shape

This turns Generator into a percussion/texture voice that still feels composed.

---

## 9. Low-pass gates
**Recommended types:**
- Make Noise Optomix
- LxD
- Natural Gate
- any vactrol-ish LPG

### Why
Generator can be brash and harmonically dense. LPGs soften edges in a very satisfying way.

### Results
- woody FM bongos
- struck metallic plucks
- Buchla-ish but dirtier transients
- animated drones with natural decay

### Patch
- Generator **Index OUT** → LPG → mixer
- short envelope → LPG CV
- another envelope → Index CV

This gives a timbral transient and an amplitude transient that feel linked but distinct.

---

## 10. Delay, reverb, and granular processors
**Recommended types:**
- tape/dub delay
- clocked delay
- shimmer/plate reverb
- granular texture module

Specific examples:
- Mimeophon
- Chronoblob
- Magneto
- FX Aid
- Desmodus Versio
- Beads / Arbhar style granular

### Why
Generator makes fantastic source material for spatial processing.

### Best roles
- short delay for metallic resonances
- long feedback delay for sci-fi dub drones
- granular capture of unstable FM bursts
- freeze/reverb for huge noise beds

### Patch idea
Create a percussive patch with Index CV, then feed the result into:
- a **very short modulated delay** for resonator-like clangs
- or into **granular freeze** for shimmering alien ambience

---

## 11. Clock dividers, logic, and comparators
**Recommended types:**
- logic module
- comparator
- clock divider
- PLL if you have one

### Why
At low frequencies, Generator can become a strange modulation and event source.

### Uses
- run one oscillator in low range as a CV/LFO
- compare it to derive gates
- combine with another clock source using logic
- use resulting rhythmic gates to trigger envelopes back into Index CV

### Results
- self-generating percussion systems
- irregular clocks
- machine chatter
- evolving trigger ecosystems

---

# Creative patch ideas

## 1. FM drum voice
**Goal:** metallic tom / kick / zappy percussion

### Patch
- Set **Gen 1** to **low**
- Set **Gen 2** to **mid**
- Patch envelope to **Index CV**
- Listen to **Index OUT**
- Optionally patch **Gen 2 out** into **External Input**
- Set destination switch to modulate **Gen 1**

This is close to the manual’s suggestion and is one of the module’s sweet spots.

### Add-ons
- LPG after output for organic decay
- transient shaper / VCA for punch
- band-pass filter for tuned drum bodies

---

## 2. Two-layer stereo beast
**Goal:** one module, wide stereo image

### Patch
- Send **1** to left channel processing chain
- Send **2** to right channel processing chain
- Put a filter on one side, a wavefolder or LPG on the other
- Modulate **Shape** slowly
- Modulate **Index CV** with a different LFO/envelope

### Why it works
The outputs are related but not identical. They split into beautiful stereo complexity very quickly.

---

## 3. Self-patched chaotic voice
**Goal:** unstable vocal/tearing lead

### Patch
- **2** → **External Input**
- Set destination to **Gen 1**
- Use internal FM as normal on Gen 2
- Slowly move **Shape**
- Add slow CV to **Index CV**

### Result
This creates a nested FM structure:
- Gen 1 influences Gen 2 internally through Index
- Gen 2 externally influences Gen 1

Very lively, very unstable, often vocal or shrieking.

### Add a filter
A resonant low-pass or band-pass after this patch can make it much more controllable.

---

## 4. Pseudo-duophonic drone machine
**Goal:** complex layered drone

### Patch
- Tune Gen 1 and Gen 2 to related but not exact intervals by ear
- Output **1** and **2** to separate VCAs/filters
- Slow random to **Shape**
- Slower triangle LFO to **Index CV**
- Optional external oscillator to **External Input** routed to Gen 2

### Add effects
- stereo delay
- long plate reverb
- subtle saturation

This gives a living drone voice with internal motion and timbral beating.

---

## 5. Audio-rate modulation hub
**Goal:** use Generator as a modulation source, not the main sound

### Patch
- Use **Gen 1** or **2** output to modulate:
  - filter cutoff FM
  - wavefolder symmetry
  - VCA amplitude at audio rates
  - delay time
- Meanwhile use another oscillator as the audible voice

### Why
Generator excels at “dirty modulation.” Its complex, shifting spectra can make ordinary modules sound far more animated.

### Especially effective targets
- analog filter cutoff FM
- resonance CV
- wavefolder fold amount
- phase modulation inputs on digital oscillators

---

## 6. Nintendo / zipper / sputter patch
**Goal:** glitchy, game-like, rude noises

### Patch
- Put one oscillator near the boundary between low and audio range
- Put the other oscillator in mid or high
- Use stepped random into one EXP input
- Send envelope bursts to Index CV
- Self-patch **2** into external FM for **Gen 1**
- Fast manual tweaks of Shape

### Optional extras
- bitcrusher
- sample rate reducer
- comparator for harsh gate extraction
- short digital delay

---

## 7. CV laboratory patch
**Goal:** Generator as dual LFO / audio-to-CV weirdness source

### Patch
- Run one oscillator in low range
- Use output **1** as modulation for another module
- Use output **2** as audio
- Use external FM to make the LFO irregular
- Send the low oscillator through a comparator for gates

### Great for
- weird clocking
- wobbling filter motion
- unstable panning
- chaotic envelope triggering

---

## 8. Resonator excitation patch
**Goal:** physical-model-ish textures

### Patch
- Create short FM bursts with envelope to Index CV
- Send output into:
  - resonator
  - Karplus/physical modeling voice
  - comb filter
  - short resonant delay

### Result
The Generator makes excellent “excitation material” because it can be noisy, sharp, and spectrally rich.

---

## 9. Dirty bass stack
**Goal:** tuned low-end plus mangled harmonic layer

### Patch
- Use a stable VCO for the fundamental bass
- Tune Generator above it
- Mix Generator output quietly underneath
- Envelope to Index CV for movement
- Filter both together or in parallel

### Why
Generator often works best in bass music as the **character layer**, not the only oscillator.

---

## 10. Envelope-following feedback patch
**Goal:** dynamic self-interaction

### Patch
- Generator output → distortion/filter → envelope follower
- envelope follower CV → Index CV or external FM depth control
- optional attenuverter in between

### Result
The louder/brighter the sound gets, the more it changes itself. This can create:
- snarling sustain
- unstable decays
- responsive noise gestures

---

# Modules that pair especially well

## If you want percussion
- Function generator / envelope
- LPG
- band-pass filter
- trigger sequencer

**Example chain:**  
Pam’s → envelope → Index CV → Generator → LPG → band-pass filter → delay

---

## If you want drones
- slow random
- stereo filter
- reverb/delay
- VCA mixer for separate outs

**Example chain:**  
Marbles / random LFOs → Shape + Index CV → outputs split to dual filters → stereo FX

---

## If you want harsh industrial sounds
- distortion
- wavefolder
- ring mod
- aggressive filter
- feedback mixer

**Example chain:**  
Generator 2 → folder → distortion → filter  
Generator 1/Index Out → ring mod sidechain or feedback modulation

---

## If you want melodic use despite weak tracking
- quantizer
- precision adder
- stable companion oscillator
- tuner utility
- sequencer with lots of attenuation control

### Important note
Because it does **not** track 1V/oct properly, use it for:
- approximate intervals by ear
- drones
- riffs in a limited register
- layered textures over a tuned voice

Don’t expect it to behave like a precision FM voice.

---

# Performance tips

## 1. Treat Shape as the macro knob
If you only touch one parameter live, make it **Shape**. It changes both oscillators and often gives the biggest “scene change.”

## 2. Use the Index knob carefully
Per the manual:
- **full left = 100% gain**
- **full right = 0% gain**

That’s easy to misread in performance. It behaves “backwards” compared to some expectations.

## 3. Separate “sound” and “animation”
A nice workflow:
- set base tone with ranges + fine tuning
- set Shape to taste
- use Index CV for animation
- use external FM only as spice

## 4. Exploit the two outputs independently
Even if you think of it as one voice, it is often more rewarding as:
- one raw output
- one processed output
- one center image, one side image
- one audio source, one modulation source

---

# Summary

The Generator is best understood not as a polite dual VCO, but as a **compact analog FM ecosystem**. It rewards:

- envelopes into **Index CV**
- self-patching through **External Input**
- random and slow CV into **Shape**
- splitting its multiple outputs into separate signal paths
- pairing with **filters, LPGs, VCAs, wavefolders, and time-based effects**

If you want the most immediate wins, pair it with:

1. **Function generator/envelope**
2. **LPG or character filter**
3. **Random source**
4. **VCA/attenuverter utility**
5. **Delay/reverb**

That combination turns Generator into a monster for:
- metallic percussion
- unstable drones
- noisy basses
- glitch effects
- chaotic modulation

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)