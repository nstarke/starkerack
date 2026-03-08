# Xaoc Devices — Batumi

- [Manual PDF](../../manuals/xaoc_batumi2_poti2_manual.pdf)

---

[Batumi II & Poti II Manual (Xaoc Devices)](https://xaocdevices.com/manuals/xaoc_batumi2_poti2_manual.pdf)

# Using Xaoc Batumi II + Poti II to create melodic material

Batumi II is “just” a quad LFO on paper, but in practice it can be a **4-channel modulation brain** that easily produces **pitch movement, stepped note patterns, clock-related sequences, pseudo-counterpoint, and audio-rate melodic voices**. Poti II turns it into a more performance-friendly melodic tool by adding **per-channel attenuation, per-channel assignable ASGN waveform choice, and waveform-shape CV control**.

## What matters musically

From the manual, the key features for melody-making are:

- **4 channels** of oscillation/modulation
- Each channel outputs simultaneously:
  - **Sine**
  - **ASGN** waveform
  - **Rect**
- **ASGN choices**:
  - triangle
  - downward saw
  - upward saw
  - trapezoid
  - stepped random
  - smooth random
- Modes:
  - **Free**
  - **Phase**
  - **Divide**
  - **Mult**
- **Wide range**:
  - LFO rates up to **audio rate**
  - **1V/oct tracking** on CV inputs
- **Reset/sync per channel**
- In external sync mode, channels can become **clock divisions**
- With **Poti II**:
  - attenuate pitch/rate CV
  - attenuate sine/asgn outputs
  - select **different ASGN waveform per channel**
  - shape CV can modulate:
    - sine = wavefolding
    - asgn = waveform switching
    - rect = pulse width

So the module can function as:

1. **4 independent pitch CV sources**
2. **A bank of related melodic modulators**
3. **A clock-derived sequencer substitute**
4. **A harmonic oscillator bank**
5. **A canon/fugue engine** via phase offsets and synced random
6. **A melody source plus rhythmic gates** from the rect outs

---

# The core idea: Batumi as a melodic source

Batumi II does not quantize by itself, so for conventional tonal melody you’ll usually patch it through a:

- **quantizer**
- precision adder
- sample & hold / track & hold
- sequential switch
- clock divider / trigger source
- envelope + VCA + oscillator voice

Typical melodic patch flow:

**Batumi output → quantizer → oscillator 1V/oct**

And often simultaneously:

**Batumi rect out → envelope trigger / LPG / clock input**

This is where Batumi becomes very musical: one channel can create the pitch contour, while its rect output or another channel controls when notes happen.

---

# Best waveform choices for melody

## 1. Stepped random ASGN
This is the most direct route to notes.

- Patch **ASGN out** with waveform set to **step-random**
- Send to a **quantizer**
- Clock note events using:
  - that same channel’s **rect out**
  - or an external trigger stream
- Result: evolving random melodies

Musically:
- In **free mode**, each random channel is independent, so you get **multiple unrelated melodic lines**
- In **phase/divide/mult**, the random outputs are related, so you get **themed variations** rather than chaos

## 2. Smooth random ASGN
Great for “wandering” melodies.

- Smooth random into a quantizer gives gliding voltages forced into scale notes
- Excellent for ambient or generative lead lines
- Add sample & hold after it if you want more discrete note steps

## 3. Triangle / saw / trapezoid
These are excellent for **repeating scalar patterns**.

When quantized:
- **Triangle** = up/down melodic motion
- **Upward saw** = rising ramps with sudden reset
- **Downward saw** = descending ramps
- **Trapezoid** = repeated held notes with quick transitions

These produce very usable sequence-like shapes once quantized.

## 4. Sine
Sine into a quantizer can be surprisingly musical:
- smoother revisiting of nearby notes
- cyclical basslines
- nice for slow transposition patterns

---

# The four modes and how they help with melody

## 1. Free mode: four independent melodic sources

In **free mode**, all four channels are independent. This is ideal for:

- four separate quantized melodies
- pitch CV + gate pattern + transposition + ornament
- one module driving an entire small generative patch

### Melodic uses
- **Channel A**: stepped random → quantizer → lead pitch
- **Channel B**: slow triangle → precision adder transpose input
- **Channel C**: rect out → clock a sample & hold or envelope
- **Channel D**: smooth random → filter cutoff or second voice pitch

Because Batumi tracks **1V/oct**, you can also treat a channel as an oscillator at audio rate. That opens another trick:

- Use **A** as audio oscillator
- Use **B/C/D** as slow melodic modulators affecting pitch, fold, filter, or FM depth

### Strong patch idea: 4-voice generative ensemble
- Set all four channels to **step-random**
- Quantize each to the same scale
- Use each rect output as its own gate/trigger source
- Send to 4 voices or to a voice allocator / switch
- Adjust each channel speed independently

This makes Batumi feel like a compact algorithmic sequencer.

---

## 2. Phase mode: canon, fugue, and melodic imitation

In **phase mode**, channels B/C/D follow channel A’s frequency but are **phase shifted** relative to it.

This is one of the most musically special features.

### Why it matters for melody
In this mode, the manual says the random waves are **copies of channel A’s random sequence, delayed by phase amount**. That means you can create:

- melodic imitation
- canons
- staggered repetitions
- “same tune, different entrance point”
- tightly related counterpoint

This is gold for melodic composition.

### Patch: Fugue machine
- Set ASGN to **step-random**
- Put Batumi in **phase mode**
- Quantize outputs of A/B/C/D separately
- Set phase offsets on B/C/D to different values
- Use similar or divided gate streams for note articulation

Result:
- the same underlying note stream appears at different time offsets
- sounds like canon/counterpoint rather than random unrelated notes

### Patch: rotating arpeggio
- Use **triangle** or **saw** as the source waveform
- Quantize all channels
- Set phase offsets to 90°, 180°, 270°
- Each channel becomes a shifted version of the same contour

Use with:
- one voice and a sequential switch
- or multiple oscillators for interlocking harmony

### Advanced note
The manual mentions **deep phase modulation** can radically deform the waveform and even act like FM at audio rates. In melodic use, that means:
- a simple source contour can morph into more complex note shapes before quantization
- subtle CV on phase can create **variation without losing structure**

---

## 3. Divide mode: rhythmic melodic hierarchy

In **divide mode**, B/C/D become integer subdivisions of A:
- 1, 2, 3, 4, 5, 8, 16, 32

This is amazing for **tempo-locked melody layers**.

### Melodic consequence
All channels are related to A, but slower. So you can patch:

- **A** = fast melody
- **B** = slower bassline
- **C** = even slower transposition source
- **D** = ultra-slow phrase-level movement

### Patch: melody + bass + phrase transpose
- Channel A ASGN step-random → quantizer → lead
- Channel B ASGN step-random → quantizer → bass
- Channel C triangle → quantizer or precision adder transpose
- Channel D rect → reset a sequencer every long cycle

Because divide mode keeps things related, the whole patch feels coherent.

### Why the random mode is useful here
The manual says divided random channels are **downsampled copies** of channel A’s random sequence. So if A is a fast random note stream, B/C/D become slower extractions of that same source. Musically this creates:

- motif at different time scales
- phrase-level unity
- less “everything independent” chaos

This is ideal for generative music where you want a family resemblance across voices.

---

## 4. Mult mode: embellishment, ornament, upper voices

In **mult mode**, B/C/D become integer multiples of A.

That means:
- one base motion in A
- faster related motions in the other channels

### Great melodic uses
- ornament around a main line
- ratcheting note motion
- high-register companion lines
- harmonic overtone-like pitch movement if run at audio rate

### Patch: lead with ornament voices
- A = slow quantized contour for main lead
- B = x2 related line
- C = x3 related line
- D = x4 or x5 related line
- Quantize them all to the same scale

Result:
- upper voices move more rapidly but remain tied to the same underlying cycle

### Random in mult mode
The manual says random sequences are **upsampled** relative to A, sharing values periodically. That means:
- the faster channels reuse material from A
- good for decorations and variations around a motif

This makes mult mode very useful for:
- grace-note-like melodic behavior
- dense top-line texture over a slower foundation

---

# Poti II: why it matters for melodic control

Poti II makes Batumi much more useful as a melody tool.

## 1. Output attenuation
This is extremely important because quantizers respond strongly to voltage range.

With Poti II, you can reduce output amplitude for each channel:
- narrow melodic range
- keep notes within one octave
- create voice-dependent contours

Example:
- Channel A wide range = lead
- Channel B attenuated = bassline with small movement
- Channel C tiny range = subtle transposition CV

Without attenuation, some Batumi outputs may jump too widely for practical tonal melodies.

## 2. Per-channel ASGN waveform selection
This is huge.

You can choose different ASGN waveforms per channel:
- A = stepped random
- B = triangle
- C = upward saw
- D = smooth random

Now Batumi becomes a **mixed melodic ecosystem** instead of four copies of the same waveform type.

## 3. Shape CV inputs
The shape inputs are extremely playable for melody generation.

Per channel, shape CV can affect one selected destination:

### Sine: wavefolding
If you quantize folded sine motion, you get:
- more complex repeated note patterns
- symmetry breaking
- pseudo-arpeggiated shapes from a simple cycle

### ASGN: waveform switching
This is especially strong for melodic work.

If shape CV is assigned to ASGN:
- external CV can switch among waveforms
- the melodic contour can jump between triangle, saw, trapezoid, random, etc.

That means one melodic line can morph between:
- ordered
- ramping
- held
- random

Great for arrangement and variation.

### Rect: pulse-width modulation
This does not directly create pitch, but it changes gate timing/duty behavior, which affects note length and rhythmic phrasing if rect is used as a gate source.

---

# Practical melodic patch recipes

## Patch 1: Simple generative melody
**Goal:** one evolving tonal line

- Batumi in **free mode**
- Channel A ASGN set to **step-random**
- A ASGN → quantizer → oscillator pitch
- A RECT → envelope trigger
- Envelope → VCA → oscillator

Optional:
- Poti II attenuate A ASGN to keep melody within a narrower range
- Slow modulation into A FRQ CV for phrase speed changes

Why it works:
- stepped random provides note selection
- rect provides timing
- quantizer keeps it musical

---

## Patch 2: Canon melody
**Goal:** related voices with delayed entrances

- Batumi in **phase mode**
- ASGN = **step-random**
- A/B/C/D ASGN → separate quantizer channels or multiple quantizer inputs
- Set B/C/D to different phase offsets
- Use rects or external triggers to articulate voices

Result:
- the same sequence appears staggered in time
- ideal for minimalist or contrapuntal music

This is one of the best “melodic identity” uses of Batumi II.

---

## Patch 3: Bassline + lead from one source family
**Goal:** coherent two-part composition

- Batumi in **divide mode**
- A = medium-fast stepped random to lead quantizer
- B = divide by 2 or 4 to bass quantizer
- C = triangle, attenuated, to transpose the bass or lead by a few scale steps
- D RECT = phrase reset trigger somewhere else in the patch

Result:
- lead and bass feel related because they derive from shared timing/material

---

## Patch 4: Arpeggiator from continuous waves
**Goal:** sequencer-like melodic loops without a sequencer

- Batumi in **phase mode** or **free mode**
- Use **triangle** or **saw** outputs
- Quantize outputs
- Clock a sample & hold from rect or external trigger if you want discrete note changes

Options:
- Triangle gives pendulum-style arps
- Saw gives rising or falling arps
- Trapezoid gives repeated held notes

---

## Patch 5: Ornament engine
**Goal:** primary melody plus embellishment

- Batumi in **mult mode**
- A ASGN → quantizer → main pitch
- B/C ASGN → quantizer → secondary voices at x2 / x3
- D sine or rect modulates filter, LPG, or wavefolder

This can sound like:
- one melody with ornamentation
- clustered lines
- baroque-style decorations
- shimmer on top of a slower line

---

## Patch 6: Batumi as four VCOs for harmonic melody
Because Batumi II goes to **audio rate** and supports **1V/oct**, it can be used as a bank of oscillators.

### Patch
- Put channels in **phase**, **divide**, or **mult**
- Feed pitch CV to the frq input(s)
- Take sine or asgn outputs as audio
- Mix channels

### Melodic applications
- **Phase mode**: detuned/phase-shifted unison or chord-like movement
- **Divide mode**: subharmonic relationships for bass and drones
- **Mult mode**: harmonic interval / overtone-like melodic stacks

If you send a keyboard or sequencer CV to channel A:
- in divide/mult, other channels become related pitch structures
- not equal-tempered harmony automatically, but very rich for experimental melody

---

# Sync-based melodic strategies

Batumi’s **reset/sync** behavior is very useful when you want melody tied to song tempo.

## Reset mode
- incoming trigger resets phase
- useful for restarting melodic contours at bar lines
- good for keeping looping note curves aligned with the groove

Example:
- A saw → quantizer → pitch
- send a bar-reset trigger to A reset
- melody restarts every measure

## Sync mode
- Batumi adapts to external clock period
- sliders then select **division factors**
- in non-free modes, only channel A can sync to external tempo

This effectively lets Batumi become a **clock-relative melodic generator**.

### Patch: clocked note divisions
- External clock into A sync
- A/B/C/D outputs to quantizers or modulation destinations
- Use the resulting divided cycle lengths as phrase lengths

This is excellent for:
- tempo-locked ambient melodies
- self-playing Berlin-school style structures
- polymetric note streams

---

# How to get more “musical” melodies from Batumi

## Use a quantizer
This is the big one. Batumi makes voltages; the quantizer makes notes.

Good scale choices:
- pentatonic for instant consonance
- dorian/aeolian for melodic ambient lines
- chromatic for experimental lines

## Limit voltage range with Poti II
Attenuation is your friend. Smaller voltage ranges mean:
- fewer leaps
- more motif coherence
- basslines that stay in register

## Combine with sample & hold
Continuous shapes become stepped note sequences when sampled.

Examples:
- triangle + S&H = repeating scalar melody
- smooth random + S&H = wandering but articulated line
- phase-shifted channels sampled by same clock = related parallel melodies

## Use rect outputs as note triggers
Every channel provides its own rect output. This can drive:
- envelopes
- logic
- clocking
- sample & hold

So one Batumi channel can generate both:
- note voltage
- note timing

## Use channel relationships intentionally
- **Free** = independence
- **Phase** = imitation/canon
- **Divide** = structural hierarchy
- **Mult** = embellishment/density

That gives you compositional roles, not just modulation modes.

---

# Best pairings with other Eurorack modules

These modules really shine with:

- **Quantizer**
  - Intellijel Scales, Ornament & Crime, ADDAC quantizers, etc.
- **Sample & hold / T&H**
- **Precision adder**
- **Sequential switch**
- **Logic / clock divider**
- **Envelope + VCA or LPG**
- **Oscillator / voice module**
- **Mixer**
- **Comparator** for deriving extra gates from smooth shapes

Especially powerful combinations:

## Batumi + quantizer + switch
Four channels become four phrase sources; the switch chooses which phrase is active.

## Batumi + quantizer + precision adder
One channel makes note motion, another makes transposition, another makes phrase-length movement.

## Batumi + chord oscillator / multi-voice synth
Use multiple Batumi outputs to animate root, inversion, spread, or parallel pitch lines.

---

# Performance-oriented melodic ideas

## Morph from ordered to chaotic
Using Poti II per-channel ASGN selection and shape CV:
- start with triangle/saw for regular melody
- morph into stepped random
- then into smooth random
- return to structured shapes

This feels like moving from composition to improvisation.

## Bring voices in by channel role
- A = main melody
- B = delayed imitation
- C = bass
- D = ornament

Because all are on one module, this is easy to perform as a “mini ensemble.”

## Use resets for phrase boundaries
Manual resets into channels create controlled re-alignments:
- all voices land together
- then drift through their own relationships
- then rejoin

Very musical for live generative sets.

---

# A few especially strong melodic concepts from the manual

## 1. Phase-mode random as delayed copies
This is probably the standout melodic feature.
It enables:
- canon
- fugue-like structures
- offset repetition
- related motif streams

## 2. Divide/mult random as derived versions of one sequence
This gives:
- coherent family resemblance
- phrase hierarchy
- ornament vs foundation behavior

## 3. Audio-rate operation with 1V/oct
Batumi can cross from modulation into sound generation, so a patch can use the same module for:
- pitch CV generation
- audio oscillation
- internal self-modulation
- rhythmic gating

That makes it unusually rich for melodic composition.

---

# Bottom line

**Batumi II + Poti II can absolutely be used as a melodic composition tool, not only as an LFO.**  
Its strongest melodic use cases are:

- **random quantized melodies**
- **phase-shifted canons**
- **clock-related bass/lead hierarchies**
- **ornamented multi-speed related lines**
- **audio-rate harmonic or quasi-harmonic voices**
- **self-playing patches where one module supplies pitch, timing, and phrase structure**

If I were using it specifically for melodic work, I’d think of the modes like this:

- **Free** = 4 independent composers
- **Phase** = 1 melody, 3 imitators
- **Divide** = 1 fast idea, 3 slower structural layers
- **Mult** = 1 core idea, 3 embellishers

And Poti II makes the difference between “interesting modulation” and **usable melodic control**, mainly because of attenuation and per-channel waveform assignment.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)