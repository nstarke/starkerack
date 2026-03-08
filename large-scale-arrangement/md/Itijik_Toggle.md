# Itijik — Toggle

- [Manual PDF](../../manuals/toggle.pdf)

---

[Manual PDF](#)

# Itijik Toggle — using a quad flip-flop to turn loops into full songs

The **Itijik Toggle** is deceptively simple: four independent **flip-flops**, each with:

- **SET** input
- **RST** input
- **CLK** input
- **IN** input
- **OUT** output
- **VERT** output

Its core job is to **remember state**. That makes it extremely useful for solving one of the hardest eurorack problems:

> how to move from “interesting loop” to “structured arrangement”

A lot of modules generate events, rhythms, melodies, and modulation. Fewer modules let you define **sections**, **mute states**, **entry/exit conditions**, **phrase changes**, and **performance logic**. Toggle does exactly that.

---

## What the module does musically

Each channel is basically a **latching logic state**:

- **SET** forces the channel ON
- **RST** forces it OFF
- **CLK** toggles between ON and OFF
- **OUT** gives the state
- **VERT** gives the inverted state, as long as nothing is patched to **IN**

If **IN** is patched, **VERT** becomes an inverter for the signal at **IN** instead of just inverting **OUT**.

In song-building terms, that means each section can become:

- a **mute/unmute memory**
- an **A/B section switch**
- a **phrase enable**
- a **fill trigger gate**
- a **transposition state**
- a **clock divider by 2**-style structural pulse source when clocked regularly
- a **scene bit** in a larger arrangement logic patch

This is not a sound source module. It’s a **song form module**.

---

# Why Toggle is powerful for full-length songs

In a typical modular patch, everything is “always happening.” Toggle gives you persistent conditions, which are essential for arrangement:

- Verse on / chorus off
- Drums active / fills inactive
- Bass muted for intro
- Melody only every 8 bars
- Open hi-hats enabled after breakdown
- Sequencer B selected only during chorus
- Reverb swell only in transition
- Ratchets only during fills
- Clock path switched between sparse and dense divisions

That turns looping material into **sections over time**.

---

# Important behaviors from the manual

## 1. Flip-flop behavior
Each of the four sections can store one binary state.

- Send a pulse to **SET** → `OUT = HIGH`
- Send a pulse to **RST** → `OUT = LOW`
- Send a pulse to **CLK** → toggles `OUT`

This is excellent for:
- turning tracks on/off
- alternating sections
- creating phrase-level switches

## 2. OUT normalized to IN
If nothing is plugged into **IN**, the **VERT** output is the inversion of **OUT**.

So by default:
- `OUT` and `VERT` are complementary
- one can represent **Section A**
- the other can represent **Section B**

That’s immediately useful for song structures.

## 3. IN breaks normalization
If you patch something into **IN**, **VERT** becomes the inverse of that incoming signal instead.

That means each channel can also be used as a standalone **logic inverter**, in addition to the flip-flop role.

---

# The big idea: use Toggle as an arrangement brain

The module shines when paired with:

- **clock dividers**
- **trigger sequencers**
- **sequential switches**
- **VCAs**
- **mute modules**
- **logic modules**
- **sequential voltage sources**
- **precision adders**
- **envelope generators**
- **switches**
- **burst generators**
- **samplers**
- **drum voices**

Think of each flip-flop as a **song-level decision layer** sitting above your rhythm and melody generators.

---

# Patch strategies for building full songs

## 1. Section mutes: intro, verse, chorus, breakdown

This is the most immediate use.

### Patch
- Use one Toggle channel per musical layer:
  - Channel 1 = kick/bass enable
  - Channel 2 = hats/percussion enable
  - Channel 3 = melody/arp enable
  - Channel 4 = FX/drone enable
- Send each **OUT** to:
  - a VCA CV input
  - a mute module
  - a logic AND with trigger streams
  - a switch that allows/disallows clocks or triggers

### Example arrangement
- **Intro**: only drone and sparse percussion ON
- **Verse**: kick, bass, hats ON
- **Chorus**: melody and extra percussion ON
- **Breakdown**: bass OFF, FX ON, kick sparse
- **Final chorus**: everything ON

### How to control it
- Manual button/gate controller to **SET/RST**
- Trigger sequencer programmed for bar-level pulses
- Clock divider sending pulses every 16 or 32 bars into different states

### Why it works
Instead of re-patching a loop, you’re creating **arranged entrances and exits**.

---

## 2. Use OUT and VERT as A/B section selectors

Because **VERT** is the inverse of **OUT** when **IN** is unused, each Toggle channel naturally creates a complementary pair.

### Patch
- **OUT** opens VCA or switch for **Verse sequencer**
- **VERT** opens VCA or switch for **Chorus sequencer**

Or:

- **OUT** selects bassline A
- **VERT** selects bassline B

Or:

- **OUT** routes clock to sparse rhythm
- **VERT** routes clock to dense rhythm

### Result
One pulse at **CLK** can flip the whole patch between two arrangement states.

### Song use
- alternate between:
  - A/B drum patterns
  - root-note bass / transposed bass
  - dry voice / effected voice
  - closed hats / open hats
  - straight groove / fill groove

This is one of the best ways to create recognizable song sections from minimal material.

---

## 3. Bar-counted section changes with clock dividers

A great way to build song form is to let sections change only after long time divisions.

### Patch
- Master clock → clock divider
- Divider outputs:
  - /16 = every 4 bars
  - /32 = every 8 bars
  - /64 = every 16 bars
- Send selected division pulses to Toggle **CLK**, **SET**, or **RST**

### Example
- `/64` into Channel 1 **CLK**: switches between Verse and Chorus every 16 bars
- `/128` into Channel 2 **SET**: enables melody every 32 bars
- `/96` or manually programmed pulse into Channel 3 **RST**: disables percussion before breakdown

### Combined with switches
Use the Toggle output to switch between:
- two melodic sequences
- two trigger patterns
- two modulation sources

### Result
Your patch self-arranges over longer musical timescales.

---

## 4. Structured drum fills

One common issue: a loop has groove, but no transitions.

Toggle is excellent for **fill windows**.

### Patch
- Main drum triggers go through one path
- Fill triggers go through another path
- Use one Toggle channel to enable fill logic only at transition points

For example:
- **OUT** opens VCA/logic path for normal snare pattern
- **VERT** opens VCA/logic path for fill generator

Or:
- main rhythm is always present
- Toggle **OUT** enables burst generator, ratchet, or alternate trigger stream for the last bar of every 8-bar phrase

### Control source ideas
- a bar counter module
- a clock divider into logic comparator
- manual gate button for live performance
- trigger sequencer with a pulse every 8th bar

### Result
Instant “end-of-phrase” energy that makes a patch feel composed instead of looped.

---

## 5. Bassline entry/exit and breakdown control

Bass is often the strongest way to define sections.

### Patch
- Bass trigger/gate stream → logic AND
- Toggle **OUT** → second input of the AND
- AND output → bass envelope or sequencer advance gate

When the Toggle state is high, bass plays.
When low, the bassline stops.

### More advanced variation
Use:
- **OUT** to enable bass trigger stream
- **VERT** to enable a bass drone or sub-oscillator sustain

So you can alternate between:
- active bassline
- held sub texture

### Song structure example
- intro: sub drone only
- verse: bassline enters
- breakdown: bassline drops out
- final section: bassline plus octave double

---

## 6. Melody/lead reveal across a song

Leads often sound best when introduced gradually.

### Patch
- Main melody sequencer always running
- Its gate output is passed through a VCA, logic gate, or switched path controlled by Toggle
- Another Toggle channel controls extra ornamentation:
  - ratchets
  - octave jumps
  - delay send
  - quantizer transposition

### Section strategy
- Verse: melody muted
- Pre-chorus: melody appears lightly
- Chorus: melody plus octave harmonization
- Outro: melody removed again

Toggle gives you persistent states so the melody doesn’t merely flicker on single triggers—it stays arranged over phrases.

---

## 7. Switching between sequencers for true song sections

This is one of the most powerful uses.

### Patch
Use Toggle with:
- a sequential switch
- an A/B switch
- a precision adder
- a switched clock path

### Method 1: Switch pitch sequences
- Sequencer A = verse notes
- Sequencer B = chorus notes
- Toggle **OUT/VERT** selects which sequence reaches the oscillator

### Method 2: Switch trigger streams
- Trigger pattern A = restrained groove
- Trigger pattern B = busier chorus groove

### Method 3: Switch sequencer clocking
- Same sequencer, but:
  - **OUT** = slower clock
  - **VERT** = faster clock or ratcheted clock

### Why it helps
You preserve thematic coherence while creating distinct song parts.

---

## 8. Automatic call-and-response arrangements

Because OUT and VERT are opposites, one section can play when the other rests.

### Patch ideas
- Bassline active on **OUT**
- Lead active on **VERT**

Or:
- Percussion bus A on **OUT**
- Percussion bus B on **VERT**

Or:
- Chord stab envelope on **OUT**
- Vocal/sample trigger on **VERT**

### Result
A patch breathes naturally because not everything is talking at once.

This is a huge ingredient in full-song feel.

---

## 9. Create phrase memory with SET and RST

The separate **SET** and **RST** inputs are important. They let you impose deterministic arrangement control.

This is better than only toggling, because you can ensure the system lands in a known song state.

### Patch
Use a trigger sequencer, gate sequencer, or manual controller to send:
- **SET** at bar 1 of chorus
- **RST** at bar 17 for breakdown
- **SET** again at bar 25 for final section

### Why it matters
With simple toggle logic, if you lose track of state, your arrangement can flip unpredictably.
With **SET/RST**, you can explicitly command:
- “drums ON now”
- “melody OFF now”
- “chorus pattern active now”

That makes it much more useful for repeatable songs and live sets.

---

## 10. Use it as a divide-by-2 phrase source

If you clock a flip-flop with a steady pulse, its output toggles every pulse.

That means each channel can effectively act like a **half-speed state alternator**.

### Patch
- Clock divider /16 into Toggle **CLK**
- **OUT** changes state every 16-beat event
- Use that to alternate:
  - two hi-hat patterns
  - two bass articulations
  - two effect sends
  - two chord voicings

### Result
Alternation over bars creates evolving phrases.

This is one of the easiest ways to escape a static loop.

---

## 11. Build a scene system with all four channels

With four flip-flops, you can think in terms of **four arrangement bits**.

Each channel controls one domain:
- Ch1 = drums density
- Ch2 = bass on/off
- Ch3 = melody on/off
- Ch4 = FX/wash on/off

Then create scenes such as:

| Scene | Drums | Bass | Melody | FX |
|---|---:|---:|---:|---:|
| Intro | 0 | 0 | 0 | 1 |
| Verse | 1 | 1 | 0 | 0 |
| Chorus | 1 | 1 | 1 | 1 |
| Breakdown | 0 | 0 | 1 | 1 |
| Finale | 1 | 1 | 1 | 1 |

### How to execute
Use:
- manual gate buttons
- preset manager outputs
- trigger sequencer rows
- clock-divided pulses plus logic

This effectively turns Toggle into a **mini arrangement matrix**.

---

# Best module pairings for songwriting

## With trigger sequencers
Examples: Varigate-style modules, Grids-style modules, Euclidean trigger modules

Use Toggle outputs to:
- mute rows
- switch patterns
- enable fills
- route alternate trigger streams

This makes drums evolve over minutes, not just bars.

---

## With clock dividers and multipliers
Examples: Pamela’s-style clocks, 4ms dividers, logic clocks

Use long divisions to:
- trigger section changes
- open transitions
- alternate A/B patterns
- set structure every 8, 16, or 32 bars

This is probably the most direct route to autonomous arrangement.

---

## With logic modules
Examples: AND/OR/XOR/compare modules

Toggle becomes even stronger when combined with logic.

### Example
- Trigger stream AND Toggle OUT = rhythm only when section enabled
- Trigger stream AND VERT = alternate rhythm in opposite section
- OUT OR manual button = performer can force a part on
- OUT XOR another pulse stream = create changing rhythmic variants

Logic plus Toggle is arrangement gold.

---

## With VCAs
A very musical use:
- Toggle **OUT** controls CV opening a VCA for audio or modulation

This works for:
- muting voices cleanly
- enabling modulation only in certain sections
- opening reverb sends for transitions
- bringing in parallel distortion only in chorus

Song structure often comes down to selective energy and texture. VCAs make that smooth.

---

## With switches
Sequential switches or A/B switches are one of the best companions.

Use Toggle to choose:
- sequence A vs B
- clean vs processed signal
- clock source 1 vs 2
- envelope A vs B
- modulation source A vs B

This creates true section contrast while keeping the patch compact.

---

## With precision adders and quantizers
Use Toggle outputs to apply transposition only in certain sections.

### Example
- Toggle OUT opens a VCA or switch feeding +7 semitones into a precision adder
- Chorus suddenly lifts harmonically
- RST returns to root for verse

This is a great songwriting move:
same sequence, new section identity.

---

## With samplers or loopers
If you use sample players, granular modules, or loopers:
- Toggle can enable a vocal chop only in chorus
- activate alternate sample banks during fills
- switch between dry loop and resampled texture

This gives modular tracks a more linear, record-like progression.

---

# Concrete full-song patch examples

## Patch 1: Techno arrangement engine

### Modules involved
- master clock
- clock divider
- drum trigger sequencer
- bass sequencer
- lead sequencer
- VCAs / logic AND
- Itijik Toggle

### Toggle assignment
- **Ch1**: kick/bass section enable
- **Ch2**: hats/percussion enable
- **Ch3**: lead enable
- **Ch4**: fill mode

### Structure
- Bars 1–16: Ch2 ON only, sparse hats/percussion
- Bars 17–32: Ch1 ON, bass and kick enter
- Bars 33–48: Ch3 ON, lead enters
- Bars 49–56: Ch1 OFF, breakdown
- Bars 57–64: Ch1/2/3 ON, Ch4 ON for fills

### How
Use divider outputs and/or a trigger sequencer to send:
- SET and RST pulses at section boundaries
- CLK for alternating fill states

This yields a complete track arc from one patch.

---

## Patch 2: Generative ambient song form

### Modules involved
- slow clock
- random melody source
- quantizer
- drone voice
- plucked voice
- effect send VCAs
- Toggle

### Toggle assignment
- **Ch1**: drone swell enable
- **Ch2**: pluck voice enable
- **Ch3**: delay/reverb send
- **Ch4**: transposition state

### Use
- OUT of Ch4 applies transposition to quantized melody
- VERT of Ch4 keeps root version active otherwise
- Ch2 only comes in every few long phrases
- Ch3 engages large spatial effects in transitions

### Result
Even a generative patch can have:
- intro atmosphere
- melodic emergence
- harmonic lift
- spacious breakdown
- return to core theme

---

## Patch 3: Live-performance song builder

### Modules involved
- pressure pad or gate button controller
- drums
- bass voice
- melodic voice
- FX chain
- Toggle

### Assignment
- Ch1 = drums
- Ch2 = bass
- Ch3 = melody
- Ch4 = FX wash

### Performance method
- Tap **SET** to bring parts in
- Tap **RST** to strip them away
- Use **CLK** for quick alternating A/B sections
- Use **VERT** to automatically open complementary elements

### Why it works live
You can improvise arrangement while keeping states stable.
A part stays on until you explicitly change it.

That’s far better than trying to maintain song form with only momentary triggers.

---

# Advanced ideas

## 1. Chorus lift via inversion
Patch **OUT** to one path and **VERT** to another:
- OUT = dry bass
- VERT = octave-up bass through distortion

Or:
- OUT = closed hats
- VERT = open hats

Now a single section change flips multiple arrangement dimensions at once.

---

## 2. Transition-only modulation
Use Toggle to enable an LFO, random source, or envelope only during selected sections.

Examples:
- filter wobble only in breakdown
- delay feedback rise only in fills
- FM depth increase only in finale

Modulation arrangement is just as important as note arrangement.

---

## 3. Rhythmic density control
Patch one rhythm source to normal triggers, another to denser triggers.
Use Toggle to switch or gate between them.

This can create:
- verse = sparse
- chorus = dense
- breakdown = almost empty
- final chorus = densest

That’s classic song energy shaping.

---

## 4. Manual plus automatic hybrid control
Use:
- bar clock divider for automatic section suggestions
- manual buttons to override with SET/RST

This is a great performance approach:
the patch has structure, but you remain the arranger.

---

# Practical songwriting tips with this module

## Think in phrases, not events
Don’t use Toggle just to flip every beat.
Use it on:
- 4-bar
- 8-bar
- 16-bar
- 32-bar

timescales.

That’s where songs live.

## Dedicate channels to musical roles
A very effective setup is:
- one channel for rhythm density
- one for bass presence
- one for melodic presence
- one for effects/transitions

## Use SET/RST for reliability
If you want repeatable structure, prefer explicit section commands over pure toggle behavior.

## Pair with mute-able VCAs or logic ANDs
This makes the module feel like a true arrangement console.

## Use VERT constantly
The complementary output is one of the best features here.
It gives you immediate A/B structure without needing another inverter.

---

# Limitations to keep in mind

Toggle does not by itself:
- count bars
- save presets
- sequence arrangements
- mix audio
- create sound

It becomes a songwriting tool when paired with:
- timing modules
- logic
- switches
- VCAs
- sequencers

So think of it as a **structural control hub**, not a standalone arranger.

---

# Bottom line

The **Itijik Toggle** is an excellent module for making **full-length songs** because it adds something many modular rigs lack: **persistent binary state**.

That means you can create:

- intros
- verses
- choruses
- breakdowns
- fills
- returns
- finales

by controlling when parts are active, which sequences are selected, how dense rhythms become, and when effects or transpositions appear.

Its strongest songwriting uses are:

1. **muting/unmuting parts over phrases**
2. **switching A/B patterns with OUT and VERT**
3. **creating deterministic section changes with SET/RST**
4. **building fills and transitions**
5. **acting as a central arrangement brain above your sequencers**

If your modular patches already make great loops, Toggle is the kind of module that helps turn those loops into **tracks**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)