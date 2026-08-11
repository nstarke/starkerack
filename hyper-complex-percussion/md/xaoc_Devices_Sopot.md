# xaoc Devices — Sopot

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Fractaos Manual PDF](https://kaona.fr/wp-content/uploads/2025/04/FRACTAOS_manual_1.5.pdf)

# Using Kaona Fractaos for dense, hyper-complex percussion

Fractaos is primarily a **4-voice polyphonic fractal oscillator / synth voice**, not just an effect. That makes it very good for **building an entire percussion ecosystem inside one module**, especially because it has:

- **4 voices**
- **4 trig inputs**
- **4 separate 1V/oct inputs**
- **5 dedicated Drum fractals**
- per-voice envelopes and filters
- MIDI or CV polyphony
- multitimbral mode with different presets per voice

For dense rhythmic music, the key idea is to treat Fractaos as a **multi-lane percussion synthesizer**, where each voice becomes a different drum machine lane or hybrid percussion voice.

---

## Why Fractaos is strong for complex percussion

From the manual, these features matter most:

- **Drum fractals**: Kick, Tom, Snare, HiHat, Cymbal
- **Rule30, Collatz, Lorenz, Hénon, Hilbert** geometric fractals can also become percussive or pseudo-rhythmic
- **Triggered primitive/LFO behavior** using the **Loop/Trig/Morph/Spread/Chaos** switches
- **Per-voice trig inputs** for direct rhythmic control
- **Multitimbral mode** lets each voice load a different preset
- **ADSR with very short attack**
- **Texture** and **Chaos** can make hits gritty, unstable, metallic, noisy, or explosive
- **Morph** can blend drum attacks with pitched/fractal tails

This means Fractaos can do:
- normal drum synthesis
- hybrid acoustic/digital percussion
- metallic strikes
- glitch hats
- tuned tom lattices
- chaotic fills
- polyrhythmic layered percussion clouds

---

# Best overall strategy

## 1. Use it as a 4-part percussion synth
Assign each voice a role like:

- **Voice 1**: Kick
- **Voice 2**: Snare or noisy mid percussion
- **Voice 3**: HiHat / metallic ticks
- **Voice 4**: Cymbal / tom / weird accent voice

Use the **4 trig inputs** from different trigger lanes of your sequencer. This is the most direct route to **independent polyrhythms and odd-meter percussion**.

## 2. Use MULTI mode
MULTI is one of the best features for your goal.

Load different presets per voice, for example:
- Voice 1: Kick preset
- Voice 2: Snare preset
- Voice 3: HiHat preset
- Voice 4: Rule30 glitch percussion preset

This gives you a **single module behaving like four different drum voices**.

Because MULTI supports separate MIDI channels too, you can also sequence each voice independently from a DAW or MIDI sequencer if desired.

---

# Patch ideas for polyrhythms and complex time signatures

## A. 4-lane polyrhythm patch
Feed the 4 trig inputs from four clock divisions/multiplications:

- Voice 1 trig: every 5 steps
- Voice 2 trig: every 7 steps
- Voice 3 trig: every 11 steps
- Voice 4 trig: every 13 steps

This creates long-form evolving percussion cycles. Since Fractaos has distinct timbral identities per voice, the result feels composed rather than random.

### Suggested voice setup
- V1: **Kick**
- V2: **Snare**
- V3: **HiHat**
- V4: **Rule30** or **Cymbal**

Use very short envelopes on hats and medium release on tom/cymbal voices.

---

## B. Complex meter drum kit
Program different track lengths in your trigger sequencer:
- Kick: 16 steps
- Snare: 15 steps
- Hats: 9 steps
- Accent voice: 14 steps

Fractaos will handle this well because each voice is independently triggered. The percussion models plus chaotic fractals let the repeated phase-shifting patterns stay interesting.

---

## C. Euclidean burst percussion
Use Euclidean triggers into the 4 trig inputs:
- Kick: 5 hits over 16
- Snare: 3 hits over 8
- Hat: 11 hits over 16
- Metallic percussion: 7 hits over 12

Then change **Chaos** and **Texture** live for controlled mutation.

This is where Fractaos shines: you can keep the rhythm source stable while the timbre mutates organically.

---

# The most useful fractals for percussion

## Dedicated Drum fractals
These are your obvious starting point.

### Kick
Use for:
- pulse anchors
- broken techno kicks
- tuned low percussion

Manual notes:
- **Depth** = tail length
- **Chaos** = hardness/dirt/explosiveness
- MIDI/CV pitch still matters tonally

#### Good use
Keep **Attack near minimum**, moderate **Decay**, low or zero **Sustain**, short-medium **Release**.
Use **Morph** to blend in a geometric primitive for click or tonal tail.

---

### Tom
Great for:
- polyrhythmic tuned tom lines
- odd-meter tribal patterns
- melodic percussion

Because pitch tracks meaningfully, send different pitch CVs to different voices or sequence tom intervals.

---

### Snare
Use for:
- main backbeats
- granular rimshot-like strikes
- harsh industrial noise-snare hybrids

At higher Chaos, it becomes more aggressive and unstable.

---

### HiHat
Excellent for:
- dense subdivisions
- ratchets
- metric modulation layers

Depth controls opening/closing behavior. Great for:
- one lane = tight hats
- another lane = open hats

---

### Cymbal
Use for:
- accents
- long-cycle punctuation
- metallic wash in asymmetric patterns

---

## Geometric fractals that work well as percussion

### Rule30
One of the best non-drum percussion sources here.
Manual calls it dense, granular, useful for percussion and basses.

Use it for:
- glitch hats
- clicks
- digital rimshots
- random-ish burst textures

### Collatz
Stepped, jerky, rhythmic profile.
Very useful for:
- woody percussive plucks
- odd little click sequences
- machine clatter

### Hilbert
Stable plateaus with abrupt changes.
Good for:
- blocky digital percussion
- chattering pulse-strikes
- angular transient-heavy sounds

### Lorenz / Hénon
Use as accent voices only.
These can make:
- unstable, swerving, chaotic percussion
- fill sounds
- broken snare tails
- noisy impacts

Best in slower rhythmic roles or special hits rather than the main groove.

### Koch / Mandelbrot / Sierpinski
Good for:
- tonal click percussion
- bright synthetic claves
- tuned mallet-like attacks when envelope is short

---

# How to make Fractaos more punchy and percussive

## 1. Use very short ADSR settings
For percussion:
- **Attack**: minimum or near minimum
- **Decay**: short to medium
- **Sustain**: usually 0
- **Release**: short, unless you want tails

This is essential. Fractaos has a synth-style voice architecture, so envelope discipline is what turns it from evolving oscillator to drum voice.

### Useful starting ADSR
- Attack: 1–10 ms
- Decay: 40–250 ms
- Sustain: 0
- Release: 20–150 ms

For cymbals or drones-as-percussion, use longer release.

---

## 2. Use Depth as drum duration
On Drum fractals, **Depth mainly controls duration/tail behavior**.

So for percussive pattern design:
- low Depth = tight, punchy, dry
- high Depth = boomy, open, smeared, ringing

This is powerful if you automate or CV-sequence it across repeated hits.

---

## 3. Use Chaos for velocity-like variation
Chaos is one of the best "humanize/violence" controls here.

For percussion:
- low Chaos = more repeatable, machine-like
- medium Chaos = lively and animated
- high Chaos = explosive, dirty, unstable

Use this for:
- accent patterns
- fill sections
- phrase-end variation

If you have CV sequencing available, send stepped CV into **F-Chaos** to create evolving accent structures over fixed triggers.

---

## 4. Use Texture as impact complexity
Texture is not just filter amount; it affects:
- resonance
- formant extraction
- micro-detuning
- filter intensity

For percussion this becomes:
- body resonance
- metallic ring
- noisy edge
- unstable overtone splash

### Practical use
- low Texture = drier, tighter hits
- medium Texture = resonant, more physical
- high Texture = metallic, organic, splintered

For punchy drums, use **moderate Texture**, not always maximum.

---

## 5. Morph drums with geometric primitives
This is a major trick.

The manual says Drum curves can be blended with the second geometric fractal using **Morph**. This is huge for sound design.

Examples:
- **Kick + Sine-ish Rössler/Julia-like primitive** = tuned body + synthetic tail
- **Snare + Rule30** = noise crack + glitch layer
- **HiHat + Hilbert** = metallic hat + digital edge
- **Tom + Fibonacci/Koch** = tuned membrane + harmonic ring

This makes Fractaos much more unique than a standard drum synth.

---

# Use the primitive modulation system rhythmically

The primitive can behave like an internal modulation source, and the switches define what it modulates.

## Important switch behavior
- **Loop ON** = free-running or looping modulation
- **Trig ON** = note-triggered modulation restart
- **Morph ON** = primitive modulates Morph
- **Spread ON** = primitive modulates detune
- **Chaos ON** = primitive modulates fractal chaos

For percussion, **Trig ON** is especially useful because each hit can restart the modulation shape.

---

## Best switch combinations for percussion

### 1. Trig ON, Loop OFF
This gives you a **one-shot modulation envelope per hit**.

Excellent for:
- transient shaping
- hit-to-hit timbral articulation
- fake pitch envelopes
- pseudo-acoustic attack movement

Use this for kicks, snares, toms.

---

### 2. Trig ON, Morph ON
Every hit morphs during its lifespan.

Result:
- drum starts as attack, decays into another spectral shape
- ideal for snares, toms, hybrid metallic percussion

---

### 3. Trig ON, Chaos ON
Each hit has internal instability contour.

Result:
- attack starts cleaner and blooms into noise
- or starts chaotic and settles
- great for snares, cymbals, industrial percussion

---

### 4. Trig ON, Spread ON
Per-hit detune sweeps.

Result:
- pseudo-flams
- metallic widening
- animated hats
- unstable tom shells

---

## Speed and Amount for percussion
- **Speed** controls primitive/LFO rate
- **Amount** controls modulation intensity

In triggered one-shot behavior, these act like a complex transient/decay shaper.

### Try:
- fast Speed + moderate Amount = clicky, articulated attacks
- medium Speed + higher Amount = audible motion inside each hit
- slow Speed + low Amount = subtle drift over sustained percussion tails

---

# Simplified FM mode for metallic percussion

The manual describes a simplified FM mode:

- Loop OFF
- Trig OFF
- Morph ON
- Spread OFF
- Chaos OFF

Then **Amount** becomes bipolar:
- lower half = internal feedback
- center = neutral
- upper half = primitive modulates main fractal frequency

This is very useful for:
- metallic hats
- bells
- zaps
- synthetic cymbals
- industrial clanks

## Important notes
- FM does **not** work on Drum curves
- FM works on geometric main fractals
- high-register FM is limited for sound quality

### Best percussion FM candidates
Use these as main fractals:
- Rule30
- Hilbert
- Koch
- Mandelbrot
- Rössler
- Sierpinski

Then apply short ADSR to turn them into struck tones.

This gives you:
- metallic ping percussion
- glitch claves
- synthetic cowbells
- tuned digital strikes

---

# Advanced percussion voice recipes

## 1. Industrial kick
- Main fractal: **Kick**
- Primitive: **Rule30** or **Hilbert**
- Morph: low to medium
- Chaos: medium-high
- Depth: medium
- Texture: medium-high
- Trig ON
- Morph ON or Chaos ON

Result: punchy kick with shattered digital shell.

---

## 2. Hyper-detailed snare
- Main fractal: **Snare**
- Primitive: **Rule30**
- Morph: 30–60%
- Chaos: medium
- Texture: medium-high
- Speed: medium-fast
- Amount: medium
- Trig ON
- Chaos ON

Result: crack + noisy animated tail, ideal for IDM or broken beat.

---

## 3. Tick swarm hats
- Main fractal: **HiHat**
- Primitive: **Hilbert** or **Collatz**
- Depth: low
- Chaos: low-medium
- Texture: medium
- Speed: high
- Amount: low-medium
- Trig ON
- Spread ON or Morph ON

Result: articulate, machine-gun hats with internal micro-motion.

---

## 4. Metallic polyrhythm voice
- Main fractal: **Koch** or **Sierpinski**
- Primitive: **Rössler** or **Hilbert**
- FM mode enabled
- Very short envelope
- High pitch
- Texture: medium-high

Result: tuned metallic accents, ideal against drum voices.

---

## 5. Chaotic fill voice
- Main fractal: **Lorenz** or **Hénon**
- Primitive: **Rule30**
- Chaos: high
- Morph: medium-high
- Texture: medium
- Trig ON
- Chaos ON
- Spread ON

Use sparsely on a separate trigger lane for phrase endings.

---

# Best sequencing approaches

## 1. Separate trigger lanes per voice
This is the most important method for your goal.

Use a trigger sequencer that supports:
- separate lengths
- probability
- ratchets
- clock division/multiplication
- per-lane swing

Send each lane to one Fractaos trig input.

This lets Fractaos become the **sound engine**, while the sequencer handles structural complexity.

---

## 2. Sequence pitch CV into percussion voices
Do not ignore pitch on drums. The manual says pitch still matters on Drum fractals.

Use pitch CV for:
- tuned kick lines
- tom melodies
- snare color changes
- hi-hat brightness shifts
- cymbal spectral movement

Especially effective in odd meters where the pitch pattern length differs from trigger length.

Example:
- trig pattern = 7 steps
- pitch pattern = 5 steps

This creates evolving percussion phrases.

---

## 3. Modulate CV inputs with independent clocks
Fractaos has CV control over:
- Texture
- Pitch
- Spread
- Morph
- Speed
- Amount
- F-Chaos
- P-Chaos

For hyper-complex percussion, send stepped or slewed CV from different clock domains to these parameters.

### Most useful targets
- **F-Chaos**: hit violence / unpredictability
- **Morph**: hybridization across pattern
- **Texture**: resonance/body/noise emphasis
- **Amount**: modulation contour depth
- **Spread**: width/detune instability

Use one slow modulation cycle over many bars and one fast stepped source over a few beats.

---

# Great rhythmic patch concepts

## Patch 1: Fractaos as a full IDM drum machine
- Voice 1: Kick
- Voice 2: Snare
- Voice 3: HiHat
- Voice 4: Rule30 percussion

Trigger lengths:
- V1: 16
- V2: 15
- V3: 9
- V4: 13

CV:
- F-Chaos from random stepped sequencer
- Morph from slow triangle LFO
- Texture from accent sequencer

Result: long, evolving composite groove.

---

## Patch 2: Tribal odd-meter tom engine
- Voice 1: Tom low
- Voice 2: Tom high
- Voice 3: Snare
- Voice 4: Cymbal

Meters:
- 5/8 tom cycle
- 7/8 tom response
- snare in 4-beat overlay
- cymbal every 11 pulses

Pitch-sequence the toms with independent CV lanes.

Result: melodic percussion lattice.

---

## Patch 3: Glitch percussion matrix
- Voice 1: Kick
- Voice 2: Rule30
- Voice 3: Collatz
- Voice 4: HiHat

Enable triggered modulation on voices 2 and 3:
- Trig ON
- Morph ON
- Chaos ON

Short envelopes, high clock density, probability skips.

Result: very dense microsound percussion.

---

## Patch 4: Hybrid acoustic/synthetic drum kit
Use Drum curves as main fractals, geometric primitives as synthetic overtone layers.

- Kick + Koch
- Snare + Rule30
- Tom + Fibonacci
- HiHat + Hilbert

Set Morph differently on each voice. This gives a coherent kit with a shared synthetic identity.

---

# Performance tricks

## 1. Use Chaos like a macro fill control
During performance, raise Chaos on the active voice or globally via CV to push the groove into breakdown/fill territory.

## 2. Use Morph for transitions
Morph from more acoustic-feeling drum body to more synthetic geometric tone over 8 or 16 bars.

## 3. Use Texture to move from tight to explosive
Lower Texture in verses, raise it in climaxes.

## 4. Use LOAD mode for auditioning percussion presets
Since presets are applied immediately in LOAD, you can browse drum identities quickly.

## 5. Use MULTI + LIVE together
The manual says LIVE voices in MULTI still respond to panel controls normally.

That means:
- keep some voices locked as stable preset drums
- leave one voice LIVE for active improvisation

Very useful for live polyrhythmic performance.

---

# Sound design advice for punch and clarity

When making dense rhythms, the danger is mud. To keep things punchy:

- Keep **kicks** low Texture / moderate Chaos
- Keep **snares** shorter than you think
- Use **hats** with low Depth
- Reserve high Texture and long tails for one or two voices only
- Use tuned percussion voices in different pitch zones
- Put unstable fractals on sparse accents, not every subdivision

Fractaos can get very rich very fast, so rhythmic density works best when **not every voice is equally chaotic**.

---

# Best Fractaos roles in a complex-rhythm system

Fractaos is especially good as:

- **main percussion synth**
- **hybrid drum machine voice bank**
- **glitch percussion generator**
- **polyrhythmic metallic percussion source**
- **accent and fill synthesizer**
- **multitimbral drum expander**

It is less ideal as a fully self-generating rhythm sequencer by itself; it really benefits from being fed by:
- trigger sequencers
- Euclidean sequencers
- logic modules
- clock dividers
- probability/rachet generators

But as the **sound source**, it is extremely capable for your goal.

---

# Short practical setup recommendation

If I were building a hyper-complex percussion patch around Fractaos, I would do this:

1. Enter **MULTI**
2. Load:
   - V1 Kick
   - V2 Snare
   - V3 HiHat
   - V4 Rule30 or Tom
3. Set ADSR globally short and percussive
4. Send 4 independent trigger lanes
5. Send pitch CV to at least kick/tom/accent voices
6. Modulate:
   - F-Chaos with stepped random
   - Morph with slow CV
   - Texture with accent lane
7. Use Trig-based primitive modulation on snare and hats
8. Keep one voice LIVE for improvisation

That will get you into **dense, asymmetrical, high-information percussion** very quickly.

---

# Best takeaway

The most powerful concept from this manual for your use case is:

**Use Fractaos not as one poly synth, but as a 4-voice multitimbral fractal drum laboratory.**

The combination of:
- drum fractals
- geometric percussive fractals
- per-hit primitive retriggering
- Morph blending
- Chaos shaping
- MULTI mode

makes it especially suited to **complex percussion that feels alive, unstable, and mathematically intricate**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)