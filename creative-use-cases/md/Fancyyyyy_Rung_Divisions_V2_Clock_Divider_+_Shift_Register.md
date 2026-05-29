# Fancyyyyy — Rung Divisions V2 Clock Divider + Shift Register

- [Manual PDF](../../manuals/RungDivisionsManual.pdf)

---

[Manual PDF](attachment)

# Fancyyyyy Rung Divisions — creative patch ideas and module pairings

Rung Divisions is a pretty unusual hybrid:  
- **clock divider / pulse processor**
- **dual OR bus rhythm mixer**
- **universal shift register**
- **1-bit / 3-bit / 8-bit CV source**
- **noise source**
- **direction / length / chance voltage-addressable pattern logic**
- and it all works from **sub-audio up to audio rate**

That means it can sit at the center of a system as:
1. a **polyrhythmic trigger brain**,  
2. a **looping / chaotic stepped CV sequencer**,  
3. a **feedback instrument**, or  
4. an **audio-rate digital chaos oscillator / subharmonic source**.

Below are the most musically useful and weird combinations I’d try.

---

## Quick character summary

A few important things from the manual shape how to patch it:

- **Bus1 clocks the shift register.**
- The divider outputs `/2` to `/8` can be routed to **Bus1 or Bus2** with switches.
- **Bus outputs are OR combinations** of selected divisions.
- **Chance** determines whether the register tends to:
  - take in new data,
  - mix in noisy interference,
  - or fully **loop** existing data.
- **Direction** can be manually toggled or triggered with a gate.
- **Length** changes loop point and can be voltage controlled.
- **3-bit and 8-bit outputs are reverse encoded**, so they often create complementary/contrapuntal motion.
- At audio rate, the module becomes a **complex digital/noise oscillator**.

So the golden rule is:

> Use **Bus1** as your internal rhythmic engine, and use **Bus2 / 1-bit / 3-bit / 8-bit** as related but differently-behaving outputs to animate the rest of the patch.

---

# 1. Use it as a polyrhythmic drum brain

## Patch concept
Send a master clock into **Clock**.  
Route several divisions to **Bus1** and **Bus2** in different combinations.

Example:
- **Bus1**: `/3 + /5`
- **Bus2**: `/2 + /7`
- **1-bit**: use as a third rhythm line
- **Reset**: occasional manual trigger or bar reset from a master sequencer

## What happens
- Bus1 creates a composite rhythm that also clocks the shift register.
- Bus2 becomes a second correlated but offset gate stream.
- The shift register then generates stepped voltages tied to the rhythm complexity of Bus1.

## Pair with
- **Drum modules**: WMD Crucible, Noise Engineering Basimilus, Jomox ModBase, Tiptop drum voices
- **Envelope + VCA chains** for pinging LPGs
- **Sequential switch** to distribute Bus outputs across voices
- **Accent VCAs / logic modules** to create fills

## Nice trick
Use:
- **Bus1** for kick/low percussion clocking
- **Bus2** for hats/claps
- **/8 or /7** directly into reset or fill logic
- **3-bit output** to modulate drum pitch or decay

### Great companion module types
- Trigger sequencers
- Clock utilities
- Logic modules
- Drum voices
- Envelope generators

### Specific module ideas
- **Shakmat Time Wizard** or **4ms Rotating Clock Divider** for expanded clock interplay
- **Noise Engineering Integra Solum** or **Vice Virga** to route rhythms dynamically
- **Doepfer A-166 logic** to derive accents and odd resets
- **Steppy / Varigate / Pam’s** as master clock and reset source

---

# 2. Make an evolving melodic sequencer with controlled instability

Rung Divisions is basically begging to be patched as a semi-random melody source.

## Patch concept
- Feed a steady clock into **Clock**
- Put a few divisions into **Bus1**
- Set **Chance** around the middle
- Set **Length** somewhere between 3 and 7
- Take **8-bit output** into a **quantizer**
- Send quantizer output to oscillator pitch
- Use **Bus2** or **1-bit** to trigger envelopes

## What happens
The shift register produces repeating-but-mutating pitch patterns.  
Changing:
- **Length** changes phrase length
- **Direction** changes melodic contour
- **Chance** changes how much it loops vs refreshes

The reverse encoding means:
- **8-bit** often gives broad, stepped contours
- **3-bit** gives a smaller, chunkier melodic motion

## Pair with
- **Quantizer**
- **Oscillator**
- **Envelope + VCA**
- **Precision adder / transposer**
- **Slew limiter** if you want it less stepped

### Specific module ideas
- **Intellijel Scales**, **ADDAC207**, **Toppobrillo Quantimator**, **uO_C in Quantermain**
- **Precision adder** like **Doepfer A-185-2**
- **Sequential switch** to switch scales or destinations
- **Slew / lag** like **Make Noise Function**, **Joranalogue Contour 1**, **Doepfer A-171-2**

## Nice variation
Quantize both:
- **3-bit output** to oscillator A
- **8-bit output** to oscillator B

Because of the complementary encoding, they often feel like two lines “answering” each other.

---

# 3. Build a self-playing duet or canon

One of the best uses of the reverse-encoded outputs is contrapuntal voice-leading.

## Patch concept
- **3-bit output** → quantizer channel 1 → VCO 1
- **8-bit output** → quantizer channel 2 → VCO 2
- **Bus1** triggers voice 1 envelopes
- **Bus2** triggers voice 2 envelopes
- **Direction input** receives sparse triggers from another divider or gate sequencer
- **Length CV** is modulated slowly

## Why it works
The 3-bit and 8-bit outputs move differently enough to create:
- call/response
- mirrored contour
- inside/outside harmonic drift

## Pair with
- dual quantizer
- dual oscillator
- dual LPGs or VCAs
- stereo mixer / panner

### Specific module ideas
- **XAOC Zadar** for two independently shaped envelopes
- **QPAS / Ikarie / Dual Dagger** for stereo movement
- **Mutable Veils / Intellijel Quad VCA** to animate dynamics
- **Happy Nerding PanMix** or any stereo panner

## Fun extension
Send one voice through a **wavefolder** and the other through a **low-pass filter**.  
Now the same hidden data structure produces two very different personalities.

---

# 4. Patch it as a “probability without a probability module” system

The Chance control is not just a randomizer; it crossfades pattern behavior between fresh data, noise interaction, and looping memory.

## Patch concept
- Clock from a stable source
- Data input from:
  - **noise**
  - or another gate sequence
  - or one of its own divisions
- Modulate **Chance CV** slowly with an LFO, envelope, or another sequencer row
- Use **Bus outputs** for percussion triggers
- Use **8-bit** for modulation or pitch

## What happens
You get changing density and pattern memory:
- low chance = more new data / instability
- middle = noisy interference
- high = looping / locked pattern

This is fantastic for making phrases that gradually “remember themselves,” then dissolve again.

## Pair with
- Slow random CV
- Function generators
- Attenuverters
- Manual offset modules

### Specific module ideas
- **Batumi**, **Ochd**, **Delta-V**, **Maths**, **Sapèl**, **Marbles**, **Sloths**
- **Happy Nerding 3xMIA**, **Frap 321**, **Quadratt** for dialing in Chance CV range

## Patch tip
A very small modulation depth on **Chance CV** can make a huge musical difference.  
Use attenuation.

---

# 5. Clock extractor / rhythm miner for messy signals

The manual notes that the clock input turns any signal crossing 1V into a pulse for driving the counters. That means Rung Divisions can derive usable timing from weird sources.

## Patch concept
Feed into **Clock**:
- a raw oscillator
- a complex LFO
- a burst generator
- a comparator output
- audio loops from an external source after gain/comparison

Then use divided outputs and buses as structured rhythmic extractions from that source.

## Great source modules
- **Comparator / window comparator**
- **Envelope follower**
- **External input preamp**
- **Chaos oscillator**
- **Burst generator**

### Specific module ideas
- **Joranalogue Compare 2**
- **Doepfer A-119**
- **Frap Falistri** as a cycling source
- **NLC / chaotic function generators**
- **SSF Ultra Random Analog**

## Musical use
Take a complex source and derive:
- regular-ish percussion clocks
- unstable resets
- changing melodic clocks
- subharmonic structures at audio rate

This is especially strong if you want a patch to feel “played by physics” instead of step-sequenced.

---

# 6. Audio-rate subharmonic / organ / digital drone voice

The manual explicitly mentions audio-rate use and PWM-derived subharmonics. This is one of the coolest underused aspects.

## Patch concept
- Feed an audio-rate square or pulse wave into **Clock**
- Route several divisions to **Bus1** and **Bus2**
- Listen directly to:
  - `/2` to `/8`
  - **Bus1**
  - **Bus2**
  - **1-bit**
  - **3-bit**
  - **8-bit**
- Mix them and filter

## What happens
You get:
- subharmonic pulse trains
- organ-like mixtures
- digital edge textures
- prime-division interference effects

The manual specifically points out how prime divisions like `/5` and `/7` create interference-like movement against `/2`.

## Pair with
- Mixer
- Filter
- Wavefolder
- LPG
- Resonator
- Stereo effects

### Specific module ideas
- **CP3-style mixer** or overdriving mixer
- **Three Sisters**, **QPAS**, **Belgrad**, **Ikarie**
- **Wavefolder** like **Fold 6**, **Bifold**, **Serge-style**
- **Mimeophon / FX Aid / Magneto** for spatialized drones

## Patch recipe
- Clock input: pulse VCO
- Bus1: `/2 + /5 + /7`
- Bus2: `/3 + /4 + /8`
- Mix Bus1 + Bus2 + 1-bit
- Filter with resonance tracking the original oscillator pitch

This gives a very rich subharmonic stack.

---

# 7. Make a chaos feedback instrument

The manual directly suggests this: patch **3-bit or 8-bit** back into a CV input of the clock source.

## Patch concept
- Use a VCO or function generator as the **Clock** source
- Patch **8-bit** or **3-bit** into that clock source’s:
  - FM input
  - 1V/oct-ish input for quantized weirdness
  - symmetry/PWM
  - wavefold amount
- Optionally patch **Bus1**, **1-bit**, or **noise** elsewhere in the voice

## What happens
This is where Rung Divisions gets very alive:
- the clock determines the register evolution
- the register output modulates the clock rate
- the system finds temporary attractors, bursts, stalls, and lurches

The manual says:
- **3-bit** is more burst-like
- **8-bit** is more random but still attractor-prone

## Best pairings
- Through-zero FM oscillators
- Oscillators with strong linear/exponential FM response
- Function generators that can cycle into audio
- PLLs or tracking filters

### Specific module ideas
- **Generate 3**, **Rubicon 2**, **Dixie 2+**, **ZPO**
- **Joranalogue Filter 8** self-oscillating and FM’d
- **Falistri / Maths / Rampage** cycling as clock sources
- **Doepfer PLL A-196** for even more unstable lock behavior

## Patch tip
Use an attenuator or VCA in the feedback path.  
Then you can “play” the onset of chaos.

---

# 8. Use it with a sample & hold / track & hold for meta-sequencing

The manual mentions using the 1-bit output to clock a sample and hold that updates the length parameter at the start of each loop. That’s a brilliant patch.

## Patch concept
- Set up a looping pattern in the shift register
- Take **1-bit** output to clock a **sample & hold**
- Feed random or stepped CV into that S&H
- Send S&H output to **Length CV**

## Result
Each time the loop reaches a certain point, the pattern length changes.  
This creates phrases that reorganize themselves structurally rather than only melodically.

## Pair with
- Sample & hold
- Noise/random source
- Quantized random
- Attenuverter

### Specific module ideas
- **Mutable Kinks S&H**, **Doepfer A-148**, **SSF Ultra Random**, **Sapèl**
- **Turing Machine / Voltages / Marbles**
- **O_C** for stepped random or quantized CV

## Nice extension
Do the same with:
- **Direction CV**
- **Chance CV**
- or switch among different modulation sources via a sequential switch

This gives “form changes” in a patch.

---

# 9. Drive a matrix mixer or VC switch network

Because Rung Divisions makes several related gates and CVs at once, it’s excellent for routing systems.

## Patch concept
Use:
- **Bus1**
- **Bus2**
- **1-bit**
- `/7` or `/8`

to control:
- VC switches
- sequential switches
- mute logic
- matrix mixers
- preset manager address inputs

## Why this is strong
Instead of only triggering notes, Rung Divisions can trigger **signal path changes**.

So the patch can:
- switch oscillators
- reroute modulation
- change effects sends
- alternate filters
- move voices in stereo

### Specific module ideas
- **Doepfer A-151 / A-152**
- **Vice Virga**
- **Joranalogue Switch 4**
- **WMD Sequential Switch Matrix**
- **Livestock Maze**
- **matrix mixer** like **AI Synthesis**, **Doepfer**, **Bear Modules**

## Example
- Bus1 advances a sequential switch for oscillator selection
- Bus2 switches filter routing
- 8-bit controls pitch
- 3-bit controls timbre
- direction gates reverse phrase behavior

That’s basically a whole composition engine.

---

# 10. Turn it into a bassline machine with reset discipline

Because the divider section can be reset and all outputs syncopate interestingly, you can force large structures on top of smaller chaotic loops.

## Patch concept
- Clock from master transport
- Send a slower reset pulse every 1, 2, or 4 bars into **Reset**
- Build a looping sequence with **Chance** mostly high
- Use **8-bit → quantizer → bass oscillator**
- Use **Bus2** for note gates
- Use **/8** or another slow division to flip **Direction**

## Musical effect
You get:
- stable phrase centers from reset
- evolving note order from direction changes
- controlled mutation from chance and length changes

This is much more performance-friendly than fully free chaos.

## Pair with
- Master clock
- Reset-capable sequencer environment
- Quantizer
- Bass voice
- Filter envelope

### Specific module ideas
- **Pamela’s Pro Workout**
- **Metropolix** as a reset/transport manager
- **Tempi**
- **Scales** with stored scales
- Any solid analog bass VCO/filter combo

---

# 11. Use the noise and XOR behavior as a “data corruption” path

The manual says incoming front-panel data passes through an **XOR gate**, and that this makes the shift register inherently unstable when data is present.

That instability is musically useful.

## Patch concept
Patch into **Data**:
- noise
- a slow square LFO
- an envelope comparator
- a gate pattern
- audio-rate square

Then adjust **Chance** so the data input is partially competing with the loop point.

## What happens
The loop gets “corrupted” in intelligible ways:
- repeated pattern with bit flips
- syncopated glitches
- pseudo-random melody mutation
- unstable but recurring motifs

## Great pairings
- Noise source / random gate source
- Comparator
- Bernoulli gate
- Rectifier / waveshaper / pulse shaper

### Specific module ideas
- **Mutable Kinks**
- **Joranalogue Compare 2**
- **Branches / Integra Solum / other probability gate modules**
- **Schmitt trigger / pulse conditioner**

## Advanced move
Patch one of Rung Divisions’ own outputs back to **Data**:
- `/5` to Data
- or Bus2 to Data
- or 1-bit to Data

This creates internally related corruption instead of external randomness.

---

# 12. Pair it with LPGs for “West Coast rungler percussion”

Because it can generate stepped CV and strange pulse structures, it’s ideal for plucked low-pass gate patches.

## Patch concept
- **Bus1 / Bus2 / 1-bit** → LPG trigger inputs
- **3-bit / 8-bit** → oscillator pitch and/or LPG CV
- use a bright oscillator or noise source into the LPG audio input
- modulate **Length** and **Direction**

## Result
You get:
- pseudo-wooden melodic percussion
- unstable pluck lines
- repeating but shifting marimba/bongo behaviors

### Specific module ideas
- **Optomix**
- **LxD**
- **Meng Qi DPLPG**
- **Natural Gate**
- **Buchla-ish voices or simple sine/triangle oscillators**

This pairing is especially nice because Rung Divisions can be both the **striker** and the **pitch brain**.

---

# 13. Use it as a control source for wavetable / macro oscillators

The stepped outputs are ideal for animating digital oscillators without needing a conventional sequencer.

## Patch concept
- **8-bit** → pitch or coarse tune via quantizer
- **3-bit** → wavetable position / morph / timbre
- **Bus2** → trigger envelope
- **1-bit** → sync or accent

### Great oscillator pairings
- **Plaits**
- **Shapeshifter**
- **Piston Honda**
- **E352**
- **Ensemble Oscillator**
- **Any macro digital VCO**

## Why it works
Rung Divisions naturally produces:
- correlated pitch and timbre motion
- looped or pseudo-random phrasing
- directionally altered contours

That creates coherent, “composed” movement instead of disconnected random modulation.

---

# 14. Pair with a quantizer that supports scale changes

One especially deep patch is using Rung Divisions not just for notes, but for harmonic structure.

## Patch concept
- **8-bit** → quantizer pitch in
- **3-bit** → quantizer scale select / root / transpose CV
- **Bus1** → note trigger
- **Bus2** → transposition or sample-hold trigger
- **/7 or /8** → reset or scale-change pulse

## Result
The melody and the harmonic frame both evolve from the same register but at different abstraction levels.

### Good pairings
- Quantizers with CV-addressable scales or roots
- Precision adders
- Sequential switches for chord sets

### Specific module ideas
- **O_C** custom quantizer apps
- **Sinfonion** if you want to go huge
- **Scales** with external transpose support
- **Bard Quartet**

This is one of the best ways to make the module feel “musical” in tonal systems.

---

# 15. Create pseudo-granular trigger clouds with burst modules

Rung Divisions excels when the input clock itself is unusual.

## Patch concept
- Feed a **burst generator** or irregular trigger source into **Clock**
- Use divisions and buses to derive smeared rhythm families
- Feed **Bus1** to clock the register
- Use **8-bit** to modulate sample playback position, decay, or filter

## Pair with
- Burst generator
- Granular/sample modules
- Envelopes
- VCAs
- percussion voices

### Specific module ideas
- **SSF Ultra-Kick / percussive voices**
- **Pam’s burst functions**
- **NE Numeric Repetitor** style trigger patterns
- **Sample players** like **Bitbox**, **Squid Salmple**, **Assimil8or**

This makes excellent broken IDM / electro-acoustic rhythm structures.

---

# 16. Exploit direction changes as phrase inversion

Direction is more than a gimmick here because the register is universal and the loop logic flips with direction.

## Patch concept
- Set a stable looping pattern with high chance
- Use sparse gates to the **Direction input**
- Derive those gates from:
  - a manual button
  - a slow divider
  - a random gate source
  - a performative pressure controller

## Musical use
Direction flips can act like:
- retrograde phrase inversion
- rhythmic mirror
- melodic reversal
- “tape turning around” effect

## Great pairings
- Manual gate controller
- Pressure controller
- Footswitch gate
- Slow random gate

### Specific module ideas
- **Pressure Points / 0-CTRL gate rows**
- **Planar 2 gates**
- **Tetrapad / controller modules**
- **Any button/gate interface**

This makes Rung Divisions highly playable in performance.

---

# 17. Cross-patch with other shift-register / Turing-style modules

Rung Divisions gets especially fun when paired with another memory/random sequencer.

## Patch concept
Use another shift-register style module as:
- clock source
- data source
- quantizer source
- reset source

Or send Rung Divisions outputs into the other module’s:
- write/lock/probability
- address
- clock
- length

### Specific module pairings
- **Music Thing Turing Machine**
- **Benjolin / Benjolin V2**
- **Marbles**
- **Shift-register DIY modules**
- **NLC cellular/chaotic logic modules**

## Why this works
You get two different memory systems influencing each other:
- one may handle note continuity
- the other rhythm continuity
- or one controls phrase shape while the other controls density

This is where emergent behavior gets really good.

---

# 18. Use it as an animated modulation source, not just a sequencer

A lot of people will patch the 8-bit output to pitch and stop there. But the outputs are equally strong for modulation.

## Great destinations for 3-bit / 8-bit
- filter cutoff
- resonance amount
- wavefolder depth
- LPG decay
- delay time
- reverb size
- panning
- sample start
- grains density
- comparator threshold
- another sequencer’s transpose input

## Patch concept
- 8-bit → filter cutoff
- 3-bit → reverb/delay send
- Bus2 → envelope trigger
- 1-bit → sidechain ducking trigger
- Chance CV slowly modulated

This creates structural modulation that feels phrase-linked.

---

# 19. Best module types to combine with Rung Divisions

If you want to build around it, these module types give the most value:

## Essential pairings
- **Quantizer**
- **Attenuverter / offset**
- **VCA for modulation depth**
- **Master clock / reset source**
- **Logic module**
- **Sample & hold**
- **Sequential switch**

## Very strong pairings
- **Oscillator with good FM**
- **LPG**
- **Comparator**
- **Random voltage source**
- **Burst generator**
- **Stereo mixer / panner**
- **Filter that tracks pitch**

## Especially synergistic “flavor” modules
- Shift-register / Turing-like sequencers
- Benjolin-style chaotic modules
- PLLs
- Resonators
- Fixed filter banks
- Addressed switches
- Matrix mixers

---

# 20. Three full example systems

## A. Self-generating techno brain
- Master clock → Rung Divisions Clock
- Bus1 → kick + bass envelope trigger
- Bus2 → hats/clap trigger
- 8-bit → quantizer → bass VCO pitch
- 3-bit → filter cutoff
- /7 → Direction
- slow random → Chance CV
- S&H → Length CV
- reset every 16 bars

Result: evolving but danceable system with phrase memory.

---

## B. Audio-rate subharmonic drone
- Pulse VCO → Clock
- Bus1 `/2 + /5 + /7`
- Bus2 `/3 + /4 + /8`
- Mix Bus1 + Bus2 + 1-bit
- 8-bit → FM amount on source VCO
- 3-bit → filter cutoff
- noise through LPG using Bus2 triggers
- stereo delay/reverb at the end

Result: organ-meets-digital-chaos drone texture.

---

## C. Two-voice contrapuntal patch
- Clock from Pam’s or another sequencer
- Bus1 → voice A envelopes
- Bus2 → voice B envelopes
- 3-bit → quantizer A → VCO A
- 8-bit → quantizer B → VCO B
- slow square LFO → Direction
- random stepped CV → Length CV
- attenuated random → Chance CV
- reset every 8 or 16 bars

Result: mirrored, evolving duet with recurring motifs.

---

# Final performance tips

## 1. Treat Chance like a memory control
- CW = memory/looping
- CCW = mutation / incoming data
- Mid = unstable life

## 2. Length is structural
Tiny movements in Length can completely reorganize the phrase.

## 3. Direction is performative
Patch a manual gate source to it. It’s one of the most musical controls on the module.

## 4. Bus1 is the heart
What you send to Bus1 doesn’t just make rhythm—it defines the timing structure of the whole internal register behavior.

## 5. Use attenuation everywhere
This module gets wild quickly, especially with feedback and CV over chance/length.

---

# Best specific pairing shortlist

If I were assembling a small “Rung Divisions companion rack,” I’d pick:

- **Pamela’s Pro Workout** or other master clock/reset utility
- **Intellijel Scales** or **uO_C** for quantization
- **Joranalogue Compare 2** for extracting and reshaping data/clock signals
- **Doepfer A-151 or A-152** for routing/sequential switching
- **Maths / Falistri / Contour 1** for modulation and clock source duties
- **Quad VCA / 3xMIA / Quadratt** for modulation control
- **Optomix or another LPG**
- **A strong FM-capable oscillator**
- **A stereo filter or effect**
- **A sample & hold/random source**

That combination would let Rung Divisions function as:
- sequencer
- rhythmic brain
- modulation source
- chaos voice
- performance instrument

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)