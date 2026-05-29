# Noise Engineering — Integra Solum

- [Manual PDF](../../manuals/Integra Solum Manual - Noise Engineering Documentation.pdf)

---

[Manual PDF / Documentation](https://manuals.noiseengineering.us/is/)

# Noise Engineering Integra Solum — creative modular patch ideas

Integra Solum is much more than “just” a clock divider. It’s really a **dual rhythmic pattern generator**, with:
- **2 independent or normalized clock lanes**
- **16 trigger outputs total**
- **3 core output organizations**
  - **/2N** = powers-of-two divisions
  - **N** = sequence-of-eight style stepping
  - **/2N+1** = odd divisions
- **Shift/Offset rotation** per side
- **Independent reset per side**
- **Wack mode** for randomized trigger behavior

That makes it especially strong for:
- drum programming
- gate animation
- switching/routing
- clock-derived modulation
- controlled randomness
- polyrhythms and polymeters
- generating structured chaos from a single clock

---

## Quick functional read of what it wants to do in a patch

A useful way to think about Integra Solum:

- In **regular mode**, it creates **related timing families**
- In **Wack mode**, it creates **probabilistic variations** of those timing families
- **Shift** turns fixed relationships into moving rhythmic phrases
- **Dual sides** let you do either:
  - one “stable” section + one “wild” section
  - one for percussion + one for modulation
  - one master clock source split into two rhythmic layers
  - two fully independent temporal systems

Because the outputs are triggers/gates in the **0–5 V** range and trigger around **3.4 V**, it pairs well with most Eurorack trigger inputs, envelope generators, logic, switch modules, burst generators, sequential switches, percussion voices, and sample players.

---

# Best module pairings

## 1. Drum voices and percussion modules
This is the most immediate and rewarding use.

### Great pairings
- **Noise Engineering Basimilus Iteritas Alter**
- **WMD Crucible / Fracture / Chimera**
- **Tiptop drum voices**
- **ALM Squid Salmple**
- **1010 Bitbox / Rample**
- **Hexinverter Mutant series**
- **generic:** kick, snare, hat, clap, sampler, physical modeling percussion

### Why it works
Each output can drive a different percussion voice, or several outputs can address:
- different samples in a sampler
- different layers of one drum patch
- accent inputs
- choke/mute behavior through VCAs or switches

### Creative patch
**One side for backbone, one side for fills**
- Left side in **/2N** for kick/snare scaffolding
- Right side in **N** or **/2N+1** for hats, claps, and percussion
- Put right side into **Wack mode**
- Send a few right-side outputs to:
  - hi-hat trigger
  - sampler slice advance
  - burst generator trigger
- Result: stable groove with evolving top-end detail

---

## 2. Sequential switches and trigger routers
Integra Solum really shines when its triggers don’t just fire sounds, but **reconfigure the patch**.

### Great pairings
- **Doepfer A-151**
- **Noise Engineering Vice Virga**
- **Befaco Muxlicer**
- **Joranalogue Step 8**
- **ALM Boss Bow Two**
- **generic:** sequential switch, addressable switch, gate router

### Why it works
The module’s rotating/divided outputs create excellent switch-advance signals. Different outputs can:
- advance a sequence selector
- change effect send destinations
- alternate oscillators
- rotate modulation targets
- swap between envelopes

### Creative patch
**Rhythm-controlled timbre switching**
- Send one output from Integra Solum to advance a sequential switch
- Patch 4 different modulation sources into the switch:
  - slow LFO
  - stepped random
  - envelope
  - chaos source
- Switch output goes to filter cutoff or oscillator FM
- Use another Integra Solum output to trigger envelopes
- Result: every rhythmic event can have a different modulation character

---

## 3. Envelope generators and function generators
Triggers become much more musically rich when converted into envelope motion.

### Great pairings
- **Make Noise Maths**
- **Frap Tools Falistri**
- **Xaoc Zadar**
- **Intellijel Quadrax**
- **Befaco Rampage**
- **Mutable Stages**
- **generic:** AD envelope, function generator, multi-envelope

### Why it works
Instead of using Integra Solum only as a drum trigger source, use it to generate:
- amplitude envelopes
- filter plucks
- FM accents
- pitch envelopes
- ratcheted modulation

### Creative patch
**Distributed envelope orchestra**
- Patch 4–8 Integra Solum outputs into multiple envelope channels
- Send those envelopes to:
  - VCA level
  - wavefolder amount
  - filter resonance
  - oscillator sync amount
- Use **Shift** to rotate which envelope arrives when
- Result: a static drone or oscillator pair becomes a constantly re-articulated rhythmic texture

---

## 4. Logic modules
A divider becomes dramatically more powerful when combined with Boolean rhythm processing.

### Great pairings
- **Joranalogue Compare 2**
- **Doepfer A-166**
- **Bastl Kompas**-adjacent logic workflows
- **Mystic Circuits ANA / tree / logic tools**
- **Klavis Logica XT**
- **generic:** AND, OR, XOR, NAND, flip-flop, comparator, logic combiner

### Why it works
Integra Solum provides related but distinct clocks/triggers. Logic can derive:
- syncopation
- accents
- missing beats
- composite rhythms
- Euclidean-like structures from basic divisions

### Creative patch
**XOR swing generator**
- Take two outputs from one side, preferably neighboring divisions or sequence positions
- Feed into an **XOR**
- Send XOR result to a hi-hat or accent path
- Send original outputs to kick/snare
- Result: derived “between-the-lines” rhythmic material

### Another patch
**AND = rare events**
- Patch a slower output from left side and a rotated output from right side into an **AND**
- Use result to trigger:
  - crash
  - bass drop
  - sample reset
  - scene change on a switch
- Result: musically sparse structural markers

---

## 5. Burst generators and ratchets
Integra Solum can act as the “when,” while a burst generator supplies the “how intensely.”

### Great pairings
- **Noise Engineering Numeric Repetitor**
- **4ms PEG / QCD + expander**
- **SSF Ultra-Random trigger modes**
- **Bastl Kompas / Knit Rider ecosystems**
- **generic:** burst generator, ratchet generator, trigger repeater

### Why it works
You can make some outputs act as phrase markers that launch bursts, rather than directly firing sounds.

### Creative patch
**Occasional ratchet percussion**
- Main hi-hat gets regular triggers from one Integra Solum output
- Another less frequent output triggers a burst generator
- Burst generator output goes to open hat, clap, or LPG ping
- Use **Wack /2N** or **Wack N** for irregular burst placement
- Result: dense fills without manually programming them

---

## 6. Sample and slicer modules
This is an excellent trigger brain for sample-based rhythm systems.

### Great pairings
- **ALM Squid Salmple**
- **1010 Bitbox**
- **Rossum Assimil8or**
- **Tiptop One**
- **Make Noise Morphagene** for rhythmic splices
- **generic:** sample player, slicer, granular module with trigger inputs

### Why it works
Different trigger outputs can control:
- sample playback
- slice advance
- reverse toggles via logic/switches
- record arming
- occasional resets

### Creative patch
**Polymetric breakbeat engine**
- Left side clocked from master clock
- Right side clocked from a clock that is slightly offset or differently divided
- Use left side to trigger main drum samples
- Use right side to:
  - advance slices
  - trigger glitch percussion
  - reset phrase points
- Put right side in **Wack N**
- Result: breakbeat variation that stays rhythmically anchored

---

## 7. Clock modulators, master clocks, and transport tools
Integra Solum becomes much deeper if the incoming clock itself changes.

### Great pairings
- **Pamela’s Pro Workout / New Workout**
- **Tempi**
- **4ms QCD**
- **Shakmat Clock O’Pawn / Time Wizard**
- **ALM mmMidi / MIDI clock tools**
- **generic:** clock source, clock divider/multiplier, swing source, transport/reset module

### Why it works
A static divider on a static clock can still be good, but feeding it:
- swung clock
- changing clock rate
- clock skips
- external reset phrases
- multiplied/subdivided clocks per side

turns it into a **form generator**.

### Creative patch
**Phrase-aware dual lane**
- Clock both sides from same source
- Reset left side every 16 steps
- Reset right side every 12 or 20 steps
- Use different modes per side
- Result: long-form polymeter that only fully repeats after many bars

### Advanced variant
- Clock left side from quarter notes
- Clock right side from swung eighths or triplets
- Patch both to related drum or modulation destinations
- Result: groove with interlocking metric layers

---

## 8. VCAs, LPGs, and audio-rate “ping” systems
Triggers don’t have to hit only drum modules.

### Great pairings
- **Make Noise Optomix**
- **XAOC Tallin**
- **Intellijel Quad VCA**
- **Befaco LPG / Percall**
- **Takaab LPG**
- **generic:** VCA, low-pass gate, transient shaper

### Why it works
If you use Integra Solum to ping LPGs or fire envelopes controlling VCAs, you can rhythmically animate:
- drones
- noise sources
- FM tones
- resonant filters
- feedback loops

### Creative patch
**Rhythmic drone carving**
- Mult a drone source to several VCAs/LPGs
- Trigger each channel with different Integra Solum outputs
- Pan them across the stereo field
- Rotate one side’s **Shift** slowly by hand or CV if available in your setup via external control tricks
- Result: one drone becomes an intricate pulse cloud

---

## 9. Filters and resonators
Trigger outputs are excellent for pinging resonant systems.

### Great pairings
- **Mutable Rings**
- **QPAS**
- **Bastl Ikarie**
- **Three Sisters**
- **Doepfer resonant filters**
- **generic:** resonant filter, resonator, comb filter, LPG

### Why it works
A trigger into:
- a resonator excite input
- a short envelope to filter cutoff
- a VCA opening noise into a filter

creates tuned percussion and melodic rhythm.

### Creative patch
**Pseudo-melodic percussion network**
- Noise source into VCA
- VCA into resonant filter or Rings
- Integra Solum triggers a very short envelope opening the VCA
- Different outputs trigger different pitch changes or damping changes
- Use left side for note triggers, right side for parameter changes
- Result: tuned percussive line that evolves structurally

---

## 10. Random, chaos, and uncertainty modules
Because Integra Solum already has **Wack mode**, it pairs beautifully with external randomness for “bounded unpredictability.”

### Great pairings
- **Mutable Marbles**
- **Make Noise Wogglebug**
- **SSF Ultra-Random Analog**
- **Qu-Bit Chance**
- **Clank Chaos**
- **generic:** random CV, sample-and-hold, chaos, probability gate processor

### Why it works
Use Integra Solum for **temporal structure**, and random modules for **parameter variation**.

### Creative patch
**Structured chaos drum patch**
- Integra Solum side A = deterministic rhythm triggers
- Integra Solum side B in **Wack mode** = fill/accent triggers
- Random CV controls:
  - sample selection
  - decay time
  - pitch
  - effect send amount
- Result: a groove that never collapses into mush because timing remains organized

---

## 11. Sequencers and quantizers
Even though it’s not a pitch sequencer, Integra Solum can be the **rhythmic spine** for melodic systems.

### Great pairings
- **Make Noise René**
- **Intellijel Metropolix**
- **Xaoc Moskwa**
- **Verbos Voltage Multistage**
- **After Later/Mutable Turing machine variants**
- **generic:** CV sequencer, gate sequencer, quantizer

### Why it works
Use different outputs to:
- clock sequencer advance
- reset the sequencer
- change sequence stage via switches
- trigger S&H for melodic variation
- accent note articulation

### Creative patch
**Melody with self-generated phrase accents**
- One Integra Solum output advances sequencer
- Another resets it occasionally
- Another triggers an envelope for VCA articulation
- Another triggers a second envelope into filter FM or pitch envelope
- Right side in **/2N+1** or **Wack N** creates irregular accents
- Result: one melodic line feels composed rather than looped

---

## 12. Matrix mixers and modulation hubs
The 16 outputs become much more useful if combined downstream.

### Great pairings
- **Livestock Maze**
- **4ms VCA Matrix**
- **Befaco Hexmix VCA / CV tools**
- **AI Synthesis matrix mixers**
- **generic:** matrix mixer, trigger combiner, gate mixer, CV router

### Why it works
By combining multiple Integra Solum outputs, you can produce:
- trigger densities
- composite envelopes
- grouped accents
- pattern clusters

### Creative patch
**Section-based percussion bus**
- Route 4 outputs to one voice family, 4 outputs to another
- Mix or logic-combine selected gates before hitting voices
- Change **Shift** to rearrange which sub-cluster is active first
- Result: pattern changes without repatching the whole system

---

# Mode-by-mode musical uses

## /2N mode
Powers-of-two divisions are your most “classic clock divider” patterns.

### Best for
- kick/snare backbones
- phrase markers
- regular resets
- stable sync points
- modulation clocks

### Great tricks
- Use the slower divisions to reset sequencers or rotate switches
- Use faster divisions for hats or envelope retriggers
- Cross-patch with logic to create sparse derived accents

### In Wack mode
The manual says this becomes a **probabilistic divide-by-two behavior** with roughly 50% chance at each step, averaging similar density over time.

**Best use:** humanized percussive layers, unstable accents, generative hats.

---

## N mode
This behaves like a stepped sequence of eight outputs.

### Best for
- trigger sequencing
- rotating event order
- switching destinations
- “which voice fires next?” style patches

### Great tricks
- Send outputs 1–8 to eight different drum samples
- Or send 1–8 to a switch matrix controlling one voice’s timbre
- Rotate with Shift to change phrase start point instantly

### In Wack mode
The manual says **a single random trigger is generated at each step**.

**Best use:** random voice addressing, non-repeating melodic articulation, generative switch addressing.

This mode is especially strong with:
- samplers
- sequential switches
- multi-envelope rigs
- percussion banks

---

## /2N+1 mode
Odd divisions give more asymmetry and are perfect for lopsided or interlocking rhythms.

### Best for
- syncopation
- off-grid-feeling percussion
- polymetric structures
- weird but still repeatable relationships

### Great tricks
- Put one side in /2N and the other in /2N+1
- Route both to related voices
- You get immediate stable-vs-skewed interplay

### In Wack mode
Each output independently has a 50% chance of going high on each step.

**Best use:** trigger clouds, dense random modulation, unpredictable sample triggering, texture generation.

This can get busy fast, so it pairs well with:
- VCAs
- logic AND gates
- envelope followers
- selective muting
- comparators

---

# Especially strong dual-side strategies

## 1. Deterministic left / random right
- Left side: regular mode
- Right side: Wack mode
- Left drives core groove
- Right drives ornaments, fills, modulation

This is probably the most musically useful “default” patch concept.

---

## 2. Same clock, different resets
Because both sides can share the same clock but have independent reset behavior, you can make long-form evolving structures.

### Example
- Same incoming clock to both sides
- Left reset every 16 steps
- Right reset every 15 steps
- Different modes on each side

This creates long cycles with repeating internal logic.

---

## 3. Percussion side / modulation side
- One side triggers drum voices
- Other side triggers envelopes, switches, sample-and-holds, and effect changes

This keeps the whole patch rhythmically related.

---

## 4. Fast side / slow side
- Side A clocked at master rate
- Side B clocked by a divided or multiplied version
- Use A for micro-rhythm, B for macro structure

Excellent for:
- fills vs phrases
- voice triggers vs scene changes
- notes vs resets

---

# Patches you can try immediately

## Patch 1: Generative drum machine
**Modules:**
- Integra Solum
- 3–6 drum voices or a sampler
- 1 logic module
- 1 mixer
- optional effects

**Patch:**
- Clock both sides from Pam’s or other master clock
- Left side in **/2N**
- Right side in **Wack N**
- Left outputs to kick, snare, closed hat
- Right outputs to percussion voices and clap accents
- Combine one left output and one right output in an **AND** for occasional crash

**Result:** groove with stable center and variable ornamentation

---

## Patch 2: Rhythmic modulation laboratory
**Modules:**
- Integra Solum
- 2 oscillators
- filter
- 3 envelopes/functions
- 2 VCAs

**Patch:**
- Several Integra Solum outputs trigger different envelopes
- Envelope 1 → VCA amplitude
- Envelope 2 → filter cutoff
- Envelope 3 → FM depth
- Another output resets one function generator
- Shift one side during performance

**Result:** one note or drone becomes an articulated evolving phrase

---

## Patch 3: Stereo ping network
**Modules:**
- Integra Solum
- noise source or oscillator
- 2 LPGs or resonant filters
- stereo mixer
- delay/reverb

**Patch:**
- Same audio source to both LPGs
- Left-side outputs trigger left LPG
- Right-side outputs trigger right LPG
- Different mode on each side
- Add effects send from one side only

**Result:** animated stereo percussion from a single source

---

## Patch 4: Switch-driven melodic variation
**Modules:**
- Integra Solum
- sequencer
- quantizer
- sequential switch
- oscillator + voice chain

**Patch:**
- One output advances the pitch sequencer
- Another output advances a sequential switch selecting among 4 modulation sources
- Another output resets the sequencer every phrase
- Wack mode on side B for irregular articulation or accents

**Result:** melody evolves in phrasing and timbre without losing coherence

---

## Patch 5: Controlled chaos texture patch
**Modules:**
- Integra Solum
- sampler or noise source
- random CV source
- logic module
- reverb/delay

**Patch:**
- Right side in **Wack /2N+1**
- Send several outputs to:
  - sample trigger
  - grain trigger
  - envelope trigger
  - freeze input via logic-conditioned gate
- Left side provides regular structural timing
- Random CV changes sample start, pitch, or effect depth

**Result:** chaotic texture with a strong rhythmic skeleton

---

# Performance ideas

## Use Shift as arrangement
Since Shift rotates output order, treat it like a **pattern reindexer**:
- leave all patch cables fixed
- rotate the pattern origin live
- the whole groove changes without changing module assignments

This is especially effective when each output goes to a different drum or modulation destination.

---

## Use resets as “scene changes”
Manual reset isn’t only for correction; it can be a performance gesture.
- Hit reset to force both sides back into phrase alignment
- Or reset only one side to deliberately create a new relationship

---

## Use one side for audible rhythm, one side for invisible rhythm
Not every output has to make sound directly.
Patch some outputs to:
- effect send gates
- switch advance
- sequencer reset
- hold/sample commands
- envelope retrigger
- comparator windowing

These invisible events are often what make a patch feel alive.

---

# Modules I’d especially recommend with Integra Solum

## If you want a compact drum/generative system
- **Pamela’s Pro Workout** — master clock and modulation source
- **ALM Squid Salmple** — sample-based rhythm playground
- **Intellijel Quadrax** — trigger-to-envelope powerhouse
- **Doepfer A-151** — cheap and incredibly useful switching
- **Joranalogue Compare 2 or a logic module** — derived rhythms

---

## If you want experimental/generative results
- **Marbles** — random CV and timing interplay
- **Morphagene** — trigger-driven splice/granular actions
- **Maths / Falistri** — rhythmic modulation and event shaping
- **Vice Virga** — trigger-controlled rerouting
- **Rings or resonant filters** — pinged melodic/percussive textures

---

## If you want techno/club utility
- **Basimilus Iteritas Alter**
- **Crucible / hats**
- **sampler for one-shots**
- **VCA matrix or mixer with mutes**
- **clock source with reset control**

Integra Solum can easily become the centerpiece of a live performance rhythm section.

---

# Bottom line

Integra Solum is best understood as a **dual structured trigger ecosystem** rather than a simple divider. Its real strengths are:

- generating many related trigger streams from very little input
- making those streams feel different via **mode**
- recontextualizing them via **Shift**
- introducing controllable randomness with **Wack mode**
- allowing one side to be the groove and the other to be the mutation engine

If you patch it only to drum triggers, it will already be useful.  
If you patch it to **switches, envelopes, logic, samplers, and modulation destinations**, it becomes a powerful compositional tool.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)