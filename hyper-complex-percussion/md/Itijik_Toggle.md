# Itijik — Toggle

- [Manual PDF](../../manuals/toggle.pdf)

---

[Manual PDF](#)

# itijik Toggle for dense, hyper-complex percussion

The **itijik Toggle** is basically **4 independent gate flip-flops**, each with:

- **SET** = force ON
- **RST** = force OFF
- **CLK** = toggle state each pulse
- **OUT** = main gate output
- **VERT** = inverted output, *unless* something is patched into **IN**
- **IN** = external logic input for the inverter side; patching here breaks the normal inversion from OUT

That makes it deceptively powerful for **rhythm generation**, especially if you want:

- evolving gate patterns
- odd-length phrases
- interlocking percussion
- pseudo-clock division with memory
- mirrored/inverted rhythms
- polyrhythmic trigger structures
- manual or sequencer-controlled pattern mutation

---

## What the module is best at rhythmically

This is not a traditional trigger sequencer. It is more like a **logic-based pattern state machine**. Each channel remembers whether it is ON or OFF, and pulses can:

- turn it on,
- turn it off,
- or flip its state.

That means you can create percussion structures that are **stateful**, not just repetitive clock divisions.

For drums, that’s useful because you can build:

- kick patterns that only switch on at certain structural moments
- snares that alternate phrase-by-phrase
- hats that flip between dense and sparse modes
- accents that appear only after specific reset conditions
- polymetric loops where different channels re-align only after long cycle lengths

---

# Core patch ideas

## 1. Basic alternating percussion lane

**Goal:** turn one trigger stream into alternating hits.

### Patch
- Send a steady trigger clock into **CLK** on one Toggle section.
- Take **OUT** to one percussion voice, like a kick.
- Take **VERT** to another percussion voice, like a snare or closed hat.

### Result
Each incoming pulse flips the state:
- hit 1: OUT high, VERT low
- hit 2: OUT low, VERT high
- hit 3: OUT high, VERT low
- etc.

This gives you a simple **alternating 1-0-1-0 logic rhythm**.  
Very useful for creating **interlocking voices** from a single source.

### Make it better
Feed a **faster clock** to the percussion envelope/VCA, and use Toggle outputs as enable gates or accent gates. This gives structured alternation without losing speed.

---

## 2. Build odd-length rhythmic cycles

**Goal:** create patterns that imply unusual meters like 5, 7, 9, 11.

### Patch
- Use an external trigger sequencer, clock divider, or logic source that emits pulses in an odd count cycle.
- Send that pattern into **CLK**.
- Use **RST** to force the phrase back to a known state every larger bar cycle.

### Example
- A 5-step trigger pattern clocks Toggle A.
- Reset it every 16 master steps.

Because Toggle changes state only when clocked, the output becomes a **derived pattern with memory**, not just a copy of the 5-step pulse train.

This works beautifully for:
- **5 against 4**
- **7 against 8**
- **3 against 5 against 4**

The key is that the channel holds its state between pulses, so silences matter as much as hits.

---

## 3. Polyrhythmic drum routing

**Goal:** derive multiple related but non-identical drum streams from one clock ecosystem.

### Patch
Use the 4 channels like this:

- **Channel 1:** CLK from a /3 pulse stream
- **Channel 2:** CLK from a /5 pulse stream
- **Channel 3:** CLK from a /7 pulse stream
- **Channel 4:** CLK from a manually programmed irregular trigger stream

Then patch:
- **OUTs** to kick, snare, tom, rim
- **VERTs** to accent inputs, alternate voices, open hats, or burst generators

### Result
Each lane toggles according to a different periodicity.  
Because each lane is binary-state based rather than simple pulse copying, the combination produces **long composite cycles** and rhythmic density fast.

This is excellent for **polyrhythmic percussion forests**.

---

## 4. Use SET and RST as phrase controls

**Goal:** create sections, fills, and structural changes.

The magic of Toggle is not just the clock input. **SET** and **RST** let you impose larger-scale form.

### Patch idea
- Send fast or medium rhythm pulses into **CLK**.
- Send a slower structural pulse into **SET**.
- Send another phrase-ending pulse into **RST**.

### Example
For a snare lane:
- **CLK** gets irregular triggers from a Euclidean sequencer.
- **SET** gets a pulse at the start of every 8 bars.
- **RST** gets a pulse every 3 bars.

Now the lane is constantly being pushed into and out of active states by overlapping phrase structures.

This yields:
- sections where the lane becomes dense
- sections where it drops out
- non-obvious phrase lengths
- long-form rhythmic evolution

This is especially strong for **complicated time signatures** because you can reset against different bar lengths than the clocks generating activity.

---

## 5. Generate mirrored percussion with OUT and VERT

As long as **IN is unpatched**, **VERT** is the inverse of **OUT**.

That means every channel can create:
- a main rhythm
- and its logical opposite

### Drum use
- OUT → closed hat
- VERT → open hat
- or OUT → kick trigger
- VERT → clap enable

If one voice sounds on the high states and the other on the low states, you get tightly interlocked parts with no overlap unless you intentionally shape them that way.

This is incredibly useful for:
- call-and-response hats
- alternating hand percussion
- ghost note logic
- negative-space rhythms

A lot of “hyper-complex” rhythm comes not from more notes, but from **intelligent use of absence**. VERT is perfect for that.

---

## 6. Break the normalization for conditional logic

The **IN** jack is where things get more advanced.

Per the manual:
- if nothing is in **IN**, **VERT** is just the inversion of **OUT**
- if you patch **IN**, you break that normalization
- then **VERT** responds to the logic at **IN**

Specifically:
- signal present / high at IN → VERT low
- no signal or low at IN → VERT high

So VERT becomes a kind of **independent inverted logic output** for whatever you patch into IN.

### Why this matters
Now one channel can act like:
- a flip-flop on **OUT**
- and a separate inverted gate processor on **VERT**

### Use case
Patch:
- irregular trigger/gate pattern into **IN**
- use **OUT** as your flip-flop rhythm
- use **VERT** as the “not-that-pattern” stream

This lets one section support two related but distinct rhythmic functions.

### Drum examples
- OUT → kick pattern state
- VERT → hat suppression or clap window
- OUT → burst generator enable
- VERT → alternate burst source enable

---

# Advanced strategies for hyper-complex percussion

## 7. Clock toggling instead of direct triggering

Instead of sending Toggle outputs directly to drum voices, use them to **gate other clocks**.

### Patch
- Fast clock or ratchet source → VCA, logic AND, sequential switch, or gate combiner
- Toggle OUT → control whether that fast stream passes
- Toggle VERT → control another stream

### Result
Toggle becomes a **density controller**.

For example:
- a 1/16 clock is only allowed through when OUT is high
- a triplet clock is only allowed through when VERT is high

Now your percussion doesn’t just alternate hits; it alternates **whole rhythmic behaviors**.

This is one of the best ways to get into:
- hyper-detailed hats
- shifting ratchets
- polymetric fills
- unstable but repeatable groove structures

---

## 8. Create long least-common-multiple cycles

To get very long evolving percussion loops, make each Toggle channel operate on a different cycle length.

### Example setup
- Ch1 CLK from /3
- Ch2 CLK from /4
- Ch3 CLK from /5
- Ch4 CLK from /7

Then use different reset intervals:
- Ch1 RST every 16 steps
- Ch2 RST every 15 steps
- Ch3 RST every 14 steps
- Ch4 RST every 21 steps

The interactions can take a very long time to fully repeat.

Then use:
- OUTs for primary drum triggers
- VERTs for accents, mutes, or fill gates

This creates exactly the kind of **dense, mathematically rich percussion architecture** used in advanced modular rhythm systems.

---

## 9. Use resets to impose asymmetric meter

A great way to imply unusual time signatures is to let the underlying pulse run steadily, but reset different rhythmic states at asymmetrical times.

### Example
Master clock at 16ths.

- Toggle A clocks every 2 steps, reset every 7 steps
- Toggle B clocks every 3 steps, reset every 10 steps
- Toggle C clocks every 5 steps, reset every 16 steps
- Toggle D clocks from a hand-programmed fill stream, reset every 13 steps

Even though the base clock is regular, the state resets create **phrase asymmetry** that feels like:
- 7/8
- 5/4
- 11/8
- mixed meter

This is a very modular-friendly way to get complex signatures without needing a dedicated time-signature sequencer.

---

## 10. Patch fills with SET bursts

Because **SET** forces the state high, it’s perfect for injecting accents and fills.

### Patch
- Irregular burst or manual trigger → SET
- Regular clock division → CLK
- Periodic reset pulse → RST

### Effect
Whenever SET gets hit, that lane is forced active immediately, regardless of where it was.

You can use this for:
- fill entry points
- guaranteed downbeat accents
- sudden activation of dense subdivisions
- “drop in” percussion behavior

For example:
- OUT enables snare rolls
- VERT enables sparse rim clicks
- a burst into SET suddenly flips the section into high-energy mode

---

## 11. Self-referential cross-patching

If your system has enough utilities, Toggle gets very interesting when channels influence each other.

### Example
- Ch1 OUT clocks Ch2
- Ch2 VERT resets Ch3
- Ch3 OUT sets Ch4
- Ch4 VERT resets Ch1

This can create semi-chaotic but bounded rhythmic systems.

More practical version:
- Ch1 = kick state machine
- Ch2 = snare alternator
- Ch3 = hat density gate
- Ch4 = fill activator

Then use outputs from one to set/reset another at strategic phrase points.

This gives you **emergent percussion structures** rather than manually written sequences.

---

# Example performance patches

## Patch 1: 4-voice polymetric drum machine

### Sources needed
- master clock
- clock divider or trigger sequencer
- 4 drum voices

### Connections
- Ch1 CLK ← /4
- Ch2 CLK ← /5
- Ch3 CLK ← /7
- Ch4 CLK ← irregular trigger pattern

- Ch1 OUT → kick
- Ch1 VERT → kick accent or sub hit
- Ch2 OUT → snare
- Ch2 VERT → clap
- Ch3 OUT → closed hat
- Ch3 VERT → open hat
- Ch4 OUT → percussion voice
- Ch4 VERT → burst or metallic accent

Then patch:
- global bar reset to some RST inputs
- a different slower phrase pulse to some SET inputs

### Result
A highly interlocked percussion patch with long-cycle variation and clear voice relationships.

---

## Patch 2: Complex hats and accents

### Connections
- Fast 16th clock → Ch1 CLK
- Every 5th pulse → Ch1 SET
- Every 7th pulse → Ch1 RST

- Ch1 OUT → closed hat trigger enable
- Ch1 VERT → open hat trigger enable

Then:
- patch a fast trigger stream through VCAs or logic under control of OUT/VERT

### Result
The hats alternate between dense and sparse behaviors according to competing 5- and 7-step structures. This quickly becomes intricate and non-obvious.

---

## Patch 3: Mixed-meter percussion skeleton

### Connections
- Ch1 CLK ← pulse pattern representing 3
- Ch2 CLK ← pulse pattern representing 4
- Ch3 CLK ← pulse pattern representing 5
- Ch4 CLK ← pulse pattern representing 7

Use:
- SET pulses at phrase beginnings
- RST pulses at different bar lengths

Map outputs to:
- kick, snare, low tom, high percussion

### Result
You get a rhythm network that naturally suggests:
- 3 over 4
- 5 over 4
- 7 over 8
- changing composite meters

---

# Best practices

## Start from known states
Because this is a flip-flop module, initial state matters. Use **RST** or **SET** to establish predictable behavior at the beginning of a patch or performance.

## Use it as control logic, not only triggers
It often works best when controlling:
- mutes
- enables
- accent inputs
- burst activity
- switch addressing
- probability windows

rather than directly striking every drum.

## Pair with:
- clock dividers/multipliers
- Euclidean trigger generators
- logic modules
- burst generators
- sequential switches
- VCAs for gate control
- comparators and random gates

## Exploit VERT constantly
The normalled inversion is one of the most musically useful features on the module. A lot of complex percussion can come from one rhythm and its inverse.

## Use different reset lengths
This is one of the fastest ways to make patterns feel “composed” and asymmetrical.

---

# Practical rhythmic mindset

For **densely rhythmic, hyper-complex percussion**, think of Toggle as a module for:

- **state**
- **alternation**
- **inversion**
- **phrase forcing**
- **structural interference**

Rather than asking “what trigger pattern does it output?”, ask:

- when is this lane active?
- when is it silenced?
- when does it invert?
- what other lane is its opposite?
- what pulse stream can force it into a new phase?

That is where the module gets deep.

---

# A strong recipe for your goal

If your goal is **complex percussion with polyrhythms and odd meter**, try this workflow:

1. Create 3–4 independent pulse streams with different lengths: 3, 5, 7, 11.
2. Send them to different **CLK** inputs.
3. Use slower, mismatched pulses on **SET** and **RST**.
4. Use **OUT** for main hits.
5. Use **VERT** for complementary hits, accents, or mutes.
6. Use some outputs to gate dense clocks rather than directly trigger drums.
7. Reset selected channels only occasionally to preserve long-form evolution.

That will get you into very rich territory very quickly.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)