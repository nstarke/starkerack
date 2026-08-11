# Doepfer — A-151 Quad Sequential Switch

- [Manual PDF](../../manuals/A151_man.pdf)

---

[Doepfer A-151 Quad Sequential Switch Manual (PDF)](https://doepfer.de/a100_man/a151_man.pdf)

# Doepfer A-151 for dense, hyper-complex percussion

The **A-151 Quad Sequential Switch** is not a sound source by itself — it’s a **bi-directional 4-step sequential router**. That makes it extremely powerful for **rhythm design**, because in modular percussion, routing is composition.

Every trigger at **Trig In** advances the switch to the next stage. **Reset In** forces it back to step 1. On **version 2**, the **2/3/4-step switch** is especially useful for polyrhythms and odd cycles.

## What it does best for percussion

Think of the A-151 as a way to:

- rotate one clock across several destinations
- rotate several sources into one destination
- create uneven repeating cycles
- generate polymetric accents
- switch modulation per hit
- create “phrase logic” from simple triggers
- reorder drum voices or drum parameters over time

Because it is **bi-directional**, it works equally well as:

- **1 input -> 4 outputs**
- **4 inputs -> 1 output**

That means it can distribute gates, or select between CV/audio/modulation sources.

---

# Core percussion strategies

## 1. Rotate one trigger stream across multiple drum voices

Patch:

- master rhythm or trigger source -> **O/I**
- **I/O 1–4** -> triggers for kick, snare, hat, clap

Each incoming trigger advances to the next output, so one stream becomes a cycling voice allocator.

### Why this is useful
This creates instant interlocking rhythms from a single pulse train. If your incoming clock is steady 16ths, the voices will fire in rotation, producing a distributed pattern instead of a unison stack.

### Make it more complex
- Clock the A-151 with a divider or irregular trigger source instead of the same trigger being routed
- Use the **reset** input every 3, 5, or 7 pulses to break the expected 4-step cycle
- Put the **step switch** on 3 while the rest of your patch is in 4-based timing for 3-against-4 interplay

This is one of the easiest ways to get **pseudo-African cross-rhythm**, **rotating accents**, or **IDM-style drum displacement**.

---

## 2. Use it as a phrase-level accent distributor

Patch:

- accent gate stream -> **O/I**
- **I/O 1–4** -> accent CV/gate inputs on different percussion voices or VCAs

Now each accent pulse lands on a different destination in sequence.

### Result
Your percussion line becomes animated without needing a separate sequencer for every accent lane.

### Advanced variation
Send the outputs to:
- kick decay CV
- snare pitch envelope trigger
- hi-hat accent VCA
- clap filter ping

Now the same accent stream changes *which parameter* gets emphasized each hit.

This is excellent for **dense but controlled variation**.

---

## 3. Route multiple trigger patterns into one drum voice

Patch:

- several different rhythm sources -> **I/O 1–4**
- **O/I** -> one drum voice trigger input
- another clock/pattern -> **Trig In**

The A-151 will step through four trigger sources, deciding which pattern controls the drum voice at any given moment.

### Great for:
- one snare voice with shifting rhythmic identities
- one hat voice alternating between straight, triplet, burst, and sparse rhythms
- one kick that changes pattern every bar or half-bar

### For hyper-complex results
Use rhythm sources of different lengths:
- pattern 1 = 5 steps
- pattern 2 = 7 steps
- pattern 3 = 8 steps
- pattern 4 = 9 steps

Then clock the A-151 advancement independently from those patterns. The composite result takes a long time to repeat.

This is a powerful **meta-sequencing** trick.

---

## 4. Polyrhythm engine via step-length limitation

If you have **version 2**, the **2/3/4 switch** is gold.

### Patch idea
Use one A-151 in **3-step mode** while the rest of the system loops in 4, 8, or 16.

For example:
- 16th-note clock into **Trig In**
- O/I gets a trigger stream
- outputs go to 3 drum destinations
- A-151 set to **3 steps**

Now the trigger rotates every 3 hits while your measure structure remains 4-based. This yields a repeating phase relationship over 12 pulses.

### Musical effect
- 3 against 4
- asymmetrical accent cycles
- tumbling percussion
- evolving ostinatos

If you reset it only every few bars, the feel becomes even less square.

---

## 5. Use reset for non-4-step structures

The **Reset In** is the key to complex time signatures.

By forcing the switch back to stage 1 before completing 4 steps, you can create:

- 3-step loops
- 5-pulse phrases over 4-step routing
- irregular phrase restarts
- barline-dependent fills

### Example: 7/8 behavior
- send a steady 8th-note trigger to **Trig In**
- use the A-151 to distribute accents or hits
- send a reset every 7 pulses

Now the switching phrase cycles in a 7-pulse structure even though the module itself is 4-stage.

### Example: additive meter
Reset at changing intervals:
- 3 pulses
- then 2
- then 3
This gives a **3+2+3** phrasing feel.

If you have logic, clock dividers, or trigger sequencers, this becomes extremely expressive.

---

## 6. Switch between different modulation shapes per hit

Patch:

- four modulation sources into **I/O 1–4**
  - envelope
  - stepped random
  - fast decay envelope
  - LFO or chaotic CV
- **O/I** -> drum parameter CV input
  - pitch
  - decay
  - filter cutoff
  - wavefold amount
  - FM amount
- trigger stream into **Trig In**

Now each hit gets a different modulation source.

### Excellent percussion targets
- kick pitch: alternating punch profiles
- snare noise filter: changing brightness
- hi-hat decay: rotating closed/open/semi-open feel
- clap tone or reverb send level
- percussion oscillator FM depth

This is where the A-151 becomes a **variation machine**.

---

## 7. Switch audio sources into a single percussion processing chain

Because the module can switch audio, use it to select among several raw sound sources before one shared VCA/filter/distortion chain.

Patch:

- different audio sources into **I/O 1–4**
  - sine kick oscillator
  - noise burst
  - metallic source
  - click/transient source
- **O/I** -> filter/VCA/distortion chain
- trigger the A-151 with your rhythm structure

### Result
One percussion “voice” changes identity every hit or every phrase.

This is great for:
- glitch percussion
- machine-like drum mutation
- making a small system sound much larger

### Important manual note
Older versions handle a smaller signal range than v2. Version 2 supports the full A-100 range. If your module is older, keep audio/CV levels within the safe range described in the manual.

---

## 8. Build rotating layers of micro-percussion

Send one fast trigger stream into the A-151 and route outputs to:
- short noise ticks
- filtered clicks
- muted tom pings
- ring-mod metallic taps

Then mix all four voices.

Because each sound only gets every fourth hit, the pattern becomes sparse per voice but dense as a whole. This is a classic way to get **busy top-end percussion** that still feels organized.

### To intensify
Use a second irregular trigger stream to reset the A-151, causing the voice order to restart unexpectedly.

---

## 9. Create fills by changing destination mid-pattern

Use the A-151 to route a burst generator or ratchet source to different drum voices.

Patch:
- burst output -> **O/I**
- outputs to different percussion triggers
- another sequence/clock controls **Trig In**

Each burst lands on a different drum destination over time.

### Why this works
A single ratchet source becomes distributed fills:
- kick stutters
- snare rolls
- hat flams
- metallic glitches

This is especially effective in techno, jungle, breakcore, and experimental rhythm.

---

## 10. Use high-speed switching for timbral percussion

The manual explicitly mentions that **very fast triggering** can create **audio-frequency modulation**. This means the A-151 can act as a crude timbral combiner when switched fast enough.

### Patch
- feed several audio waveforms or percussion partials into **I/O 1–4**
- take **O/I** to a VCA/filter/output
- drive **Trig In** with a fast LFO or even a VCO square wave

### Result
The switching becomes so fast it creates a new composite timbre. For percussion, this can produce:
- aggressive digital-like transients
- tearing metallic hits
- unusual pseudo-bitcrushed attacks
- animated hybrid drum tones

### Best use
Don’t use this as your whole drum tone all the time. Use it for:
- attack layers
- transient enhancement
- occasional fills
- industrial percussion accents

---

# Polyrhythm and odd-meter patch recipes

## Patch 1: 3-against-4 hi-hat rotation
- steady 16th clock -> trigger source into **O/I**
- **I/O 1–3** -> three different hat or click voices
- set A-151 to **3 steps**
- use a normal 4/4 kick/snare under it

This gives a top layer that cycles every 3 hits against the bar.

---

## Patch 2: 5-step accent phrase using reset
- 16th trigger stream into **O/I**
- outputs -> accent inputs for four drum parameters
- send regular clock to **Trig In**
- send reset every **5 triggers**

The reset interrupts the natural 4-step order, creating a 5-pulse phrase contour.

---

## Patch 3: Multi-pattern snare brain
- four different gate patterns into **I/O 1–4**
- **O/I** -> snare trigger
- slow clock divider to **Trig In**
- reset every bar or every 3 bars

Your snare pattern changes identity over the course of a phrase instead of just repeating.

---

## Patch 4: 7/8 percussion distributor
- 8th-note pulse stream -> **O/I**
- outputs -> kick, rim, hat, clap
- regular pulse to **Trig In**
- reset every 7 pulses

Now the voice distribution lives in a 7/8 phrase.

---

## Patch 5: Evolving drum modulation matrix
- envelope A, random CV, slow triangle, decay envelope -> **I/O 1–4**
- **O/I** -> FM or decay CV of one percussion voice
- trigger advance from the same pulse that triggers the voice

Every hit changes the behavior of the sound source.

---

# Best percussion applications by target

## Kick
Use the A-151 to rotate:
- different pitch envelopes
- different decay CV amounts
- different click layers
- different trigger patterns

This gives kicks that alternate between:
- short punch
- long boom
- hard transient
- muted ghost hit

## Snare
Rotate:
- noise sources
- filter settings
- envelope shapes
- trigger densities

This can make one snare voice behave like a full evolving snare section.

## Hi-hats
This is where the A-151 really shines.
Rotate:
- closed/open hat triggers
- different decay CVs
- different noise/filter combinations
- accents
- burst density

You get extremely articulate upper percussion with minimal modules.

## Metallic percussion / FM percussion
Switch:
- modulation index sources
- oscillator relationships
- trigger streams
- waveforms

This creates animated clangorous rhythms perfect for industrial, electro, or broken beat.

---

# Performance tips

## Use reset musically
Don’t think of reset as only “start over.”
Use it as:
- barline correction
- phrase punctuation
- fill generator
- odd-meter enforcer
- live improvisation control

A manual gate button into reset can be very powerful in performance.

## Clock the switch separately from the triggers it routes
This is one of the most important tricks.

If the trigger stream being switched is not the same as the clock advancing the switch, you get much richer behavior:
- missed hits
- shifted accents
- phase patterns
- long non-repeating structures

## Pair it with dividers, multipliers, logic, and burst sources
The A-151 becomes far more powerful when fed by:
- clock dividers
- Euclidean rhythms
- logic outputs
- Bernoulli gates
- burst generators
- trigger delays

These modules create the complexity; the A-151 distributes and reorganizes it.

## Use multiple time scales
Try:
- fast triggers for local variation
- slower trigger advancement for phrase movement
- even slower resets for macro-structure

This gives nested rhythm:
- hit level
- beat level
- bar level
- phrase level

That is how you get genuinely complex percussion instead of mere randomness.

---

# A few “hyper-complex” patch concepts

## Rotating ratchet allocator
One ratchet source into O/I, outputs to 4 percussion voices, irregular clock on Trig In, reset every 11 or 13 pulses.

## Asymmetric modulation drummer
Four CV sources into I/O, O/I to drum pitch/decay/filter, step length set to 3, voice trigger in 4/4.

## Meta-polyrhythm selector
Four independent sequenced trigger patterns into I/O, O/I to one voice, switch advanced by a separate 5-step clock.

## Glitch voice compositor
Four audio transients into I/O, fast oscillator clocks Trig In, O/I to distortion/VCA for brutal digital percussion.

---

# Bottom line

The **Doepfer A-151** is excellent for **complex percussion**, not because it generates rhythms by itself, but because it lets you **reassign rhythmic function over time**.

For dense, advanced rhythmic music, use it to:

- rotate triggers across voices
- rotate modulation across drum parameters
- select between multiple trigger patterns
- create 3-, 5-, 7-, and mixed-length phrases with reset
- generate polymeter with the 2/3/4 step limit
- switch audio sources for composite drum timbres
- create fast-switched glitch percussion textures

In a percussion-focused rack, this module is basically a **rhythmic router/composer**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)