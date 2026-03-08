# Itijik — Toggle

- [Manual PDF](../../manuals/toggle.pdf)

---

[Manual PDF](#)

# itijik Toggle — patch ideas for aggressive rhythm, bass movement, and eerie textures

The **itijik Toggle** is not a sound source by itself — it’s a **quad flip-flop / logic utility** with **inverted outputs**. That means its real power is in creating **rhythmic state changes, sub-octave divisions, alternating gates, logic inversions, and stepped modulation**. In practice, that makes it excellent for:

- **turning simple clocks into complex rhythmic structures**
- **alternating between two modulation states**
- **creating stepped CV/gate patterns**
- **generating divided pulse streams for sub-bass and percussion**
- **making evolving on/off modulation for filters, VCAs, wavefolders, distortion, and effects**

## Quick summary of what the module does

Each of the 4 sections has:

- **SET**: forces `OUT` high
- **RST**: forces `OUT` low
- **CLK**: toggles `OUT` on every pulse
- **IN**: feeds the inverter section directly and **breaks normalization** from `OUT`
- **OUT**: main flip-flop output
- **VERT**: inverted output

### Important behavior
If **nothing is patched to IN**, then:

- `VERT = inverse of OUT`

If **you patch something into IN**, then:

- `VERT = inverse of whatever is at IN`
- the normal inversion from `OUT` is broken

So each section can act as either:

1. a **toggle flip-flop with complementary outputs**, or  
2. a **standalone logic inverter**

That combination is what makes it useful for brutal percussive patching and animated basslines.

---

# Best ways to think about Toggle musically

## 1. As a rhythm divider / alternator
Sending regular triggers to **CLK** makes `OUT` flip high/low every trigger. So one section can turn a fast clock into an **alternating gate pattern**. That gives you:

- every-other-hit kick accents
- alternating snare/noise layers
- bass note switching between two filter states
- left/right or dry/wet switching behavior

## 2. As a complementary modulation source
Because `OUT` and `VERT` are opposites, one pulse stream can create **two opposite control behaviors**:

- one VCA opens while another closes
- one distortion goes harder while another backs off
- one filter opens while another closes
- one oscillator FM index increases while another decreases

This is very useful for making patches feel animated and “arguing with themselves.”

## 3. As a binary state memory
Using **SET** and **RST** instead of just CLK lets you force sections into specific states. That’s huge for patches where you want:

- fills every 8 bars
- bass “phrase changes”
- only occasional distortion bursts
- long-form ambient state changes

## 4. As a logic inverter for gates and pulses
Patching something into **IN** gives you an immediate opposite version at **VERT**. Use that for:

- ducking one layer against another
- anti-phase trigger structures
- opening reverb only in the gaps
- making negative-space rhythms

---

# Patch ideas for distorted percussive sounds

These patches assume you have common Eurorack companions like:
- noise source
- oscillator
- filter
- VCA
- envelope generator
- distortion / wavefolder / feedback / LPG
- clock / trigger sequencer

## 1. Alternating kick destruction patch
Goal: make a kick alternate between tight and absolutely wrecked.

### Patch
- Clock or kick trigger stream → **CLK** on Toggle section 1
- `OUT` → envelope trigger for your normal kick voice
- `VERT` → trigger a second envelope or modulation path that opens:
  - distortion amount
  - wavefolder CV
  - filter FM depth
  - feedback VCA
  - parallel noise burst

### Result
Every other hit gets a different treatment:
- clean / smashed
- short / long
- dry / distorted
- normal / noisy

### Make it nastier
Use:
- `OUT` to trigger the kick
- `VERT` to trigger a **very short noise burst into distortion**
This creates a kind of **alternating click-crunch transient**, great for industrial kicks.

---

## 2. Snare ghost-note inverter patch
Goal: create syncopated ghost hits and negative-space snares.

### Patch
- Main snare trigger pattern → **IN** on Toggle section 2
- `VERT` → trigger a second VCA holding filtered noise or metallic FM percussion

### Result
Whenever the main snare is absent, the inverted rhythm can fire ghost textures or atmospheric tail hits.

### Great destinations for `VERT`
- noise burst VCA
- resonant bandpass ping
- clap layer
- short reverb send envelope
- burst generator

This is especially good for **broken beat DnB percussion**.

---

## 3. Clocked percussion state switcher
Goal: use one percussion voice but change its character every few hits.

### Patch
- Master 16th note clock → **CLK** on section 1
- `OUT` → filter cutoff CV switch amount or VCA accent CV
- `VERT` → second modulation destination:
  - decay time modulation
  - bitcrusher mix
  - FM index
  - LPG strike level

### Result
A static percussion voice becomes a **two-state machine**, ideal for:
- metallic hats
- acid percussion
- rimshots
- glitchy tops

### Better version
Use another Toggle section clocked slower, and send its `OUT` to **SET** or **RST** of section 1.  
Now the alternation itself changes over time.

---

## 4. Distorted burst-fill generator
Goal: occasional brutal fills.

### Patch
- Fast trigger stream / ratchet / burst source → VCA controlling a percussion voice
- Use Toggle section 3 as a memory state:
  - occasional manual gate, sequencer gate, or long phrase trigger → **SET**
  - another later phrase trigger → **RST**
- `OUT` while high enables the burst stream to reach:
  - hi-hat voice
  - FM percussion
  - noise through distortion
  - feedback patch

### Result
The module acts like an **armed/disarmed fill switch**.  
When high, the patch spits out chaotic fill material. When low, it stays controlled.

This is excellent for **live performance transitions**.

---

## 5. Complementary percussion buss abuse
Goal: make percussion pump and tear itself apart.

### Patch
- Section 1 `OUT` → opens VCA for clean drum bus
- Section 1 `VERT` → opens VCA for crushed/driven parallel bus
- Clock section 1 with a divided trigger or use SET/RST from sequencer

### Result
Instead of a static parallel distortion, the patch **switches emphasis between clean and dirty signal paths** rhythmically.

If you modulate the dirty path with resonant filtering, feedback, or wavefolding, you get very animated drum aggression.

---

# Patch ideas for dubstep / drum & bass basslines

Toggle is very strong for bassline work because flip-flops naturally create **subdivisions and binary switching**, which translate beautifully into:
- octave switching
- alternating envelopes
- wobble states
- modulation lane switching
- gate pattern generation

## 1. Sub-octave gate logic bass
Goal: make a bassline feel wider and more mechanical.

### Patch
- Send a fast rhythmic trigger pattern to **CLK** on section 1
- `OUT` and `VERT` control two VCAs or two filter/envelope paths on a bass voice:
  - `OUT` opens sub layer
  - `VERT` opens midrange distorted layer

### Result
Each trigger alternates which layer is dominant:
- sub / growl / sub / growl
- clean low end / aggressive top / clean / aggressive

This creates instant **call-and-response inside one bass patch**.

### Nice source voice
- saw or square VCO
- lowpass filter
- parallel wavefolder or distortion
- separate VCAs for low and high bands

---

## 2. Two-state wobble patch
Goal: create classic but less predictable wobble movement.

### Patch
- LFO square, clock divider, or trigger sequencer → **CLK** on section 2
- `OUT` → one CV level to filter cutoff / distortion / wavetable position
- `VERT` → opposite CV via another attenuator / offset path

### Result
The bass jumps between two contrasting timbral states.

Examples:
- low cutoff / high resonance
- open filter / heavy FM
- dry / wet
- wavefolder off / wavefolder slammed

Because Toggle gives strict logic states, the movement is **hard-edged and rhythmic**, ideal for heavier bass styles.

### Advanced version
Use section 3 as a slower phrase-level switch:
- section 3 `OUT` triggers or enables the clock to section 2
- section 3 `VERT` disables it or reroutes it

Now the wobble itself appears and disappears in phrases.

---

## 3. Resequenced accent growl
Goal: create bass hits that alternate accents without reprogramming the sequencer.

### Patch
- Bass note gate from sequencer → **CLK** section 1
- `OUT` → envelope A trigger (short, punchy)
- `VERT` → envelope B trigger (longer, distorted, more FM)

Route both envelopes to different destinations:
- VCA amplitude
- filter cutoff
- distortion amount
- pitch envelope depth

### Result
Every successive note can become:
- stab / growl / stab / growl
- muted / screaming / muted / screaming

This works extremely well with:
- Reese basses
- FM basses
- wavetable growls
- filtered noise + oscillator hybrids

---

## 4. Controlled chaos bass reset patch
Goal: make a bassline mutate but remain performable.

### Patch
- Fast rhythmic trigger → **CLK** section 1
- Phrase trigger from sequencer every bar or 2 bars → **RST**
- Occasional fill trigger → **SET**

### Result
The bass alternates internally, but you can periodically **force it back into a known phase**.  
That means the movement feels wild but still lands correctly in the groove.

This is very useful live when free-running modulation starts feeling too detached.

---

## 5. Cross-rhythmic DnB reese modulation
Goal: generate rolling, off-balance bass motion.

### Patch
- Main 16th trigger stream → **CLK** section 1
- Slower triplet or off-grid trigger → **SET** section 1
- Bar reset pulse → **RST** section 1

Use:
- `OUT` for stereo spread increase / chorus depth / filter opening
- `VERT` for distortion reduction / lowpass closing

### Result
You get a bassline that seems to “lean” and evolve across the bar rather than just wobble evenly.

This is excellent for:
- neuro-ish bass movement
- DnB reese animation
- tense rolling subs

---

## 6. Bassline lane switcher with external IN
Goal: turn Toggle into a true inversion utility for control patterns.

### Patch
- Patch a gate or square LFO into **IN**
- Use `VERT` as the opposite pattern
- Route original and inverse to:
  - two VCAs controlling two modulation signals
  - two effect sends
  - two filter FM depths
  - two oscillator sync paths

### Result
The bass can alternate between **two totally opposed modulation lanes**.

For example:
- original gate opens lowpass cutoff
- inverted gate opens distortion send

So when one sound feature rises, the other falls. This creates very polished “produced” movement.

---

# Patch ideas for haunting atmospheric pads

Even though Toggle is a logic module, it can be extremely useful in ambient and pad patches because it creates **slow binary structure**, which is great for:
- opening and closing effects
- changing drone layers
- alternating modulation routings
- injecting absence and contrast
- shaping long-form evolution

## 1. Drone layer alternator
Goal: make two pad layers breathe against each other.

### Patch
- Very slow square LFO or sparse trigger stream → **CLK** section 1
- `OUT` → VCA for bright layer
- `VERT` → VCA for dark layer

Bright layer:
- shimmer, upper harmonics, wavefolder, bandpass, chorus

Dark layer:
- lowpass, noise bed, sub drone, reverb-heavy oscillator

### Result
The pad slowly shifts between emotional colors:
- icy / shadowy
- hollow / rich
- distant / intimate

This can be beautiful if the timing is very slow.

---

## 2. Reverb-space inversion patch
Goal: create haunted negative space.

### Patch
- Main pad gate or envelope gate → **IN** on section 2
- `VERT` → open a VCA sending:
  - noise bed
  - reverb return
  - granular wash
  - filtered feedback

### Result
When the main pad is active, the haunted background recedes.  
When the pad stops, the inverted layer blooms.

This is a fantastic way to create **ghostly after-images** around chords.

---

## 3. Alternating modulation target patch
Goal: one LFO, two different emotional results.

### Patch
- Clock Toggle section 3 slowly
- Use `OUT` and `VERT` to switch which VCA receives a modulation signal from an LFO or random source

For example:
- `OUT` enables LFO to modulate filter cutoff
- `VERT` enables same LFO to modulate FM amount or wavefolder depth

### Result
The same modulation source “changes meaning” over time.  
The pad feels like it’s evolving compositionally, not just moving.

---

## 4. Binary chord shimmer control
Goal: make pad harmonics flicker between stable and uncanny.

### Patch
- Sparse trigger pattern or slow clock → **CLK** section 4
- `OUT` → open VCA to octave-up shimmer / resonator / frequency shifter send
- `VERT` → keep dry or lowpass version dominant

### Result
The harmonic field alternates between:
- normal
- spectral
- fragile
- eerily luminous

Very strong with:
- long reverb
- resonators
- granular delay
- frequency shifters
- ensemble effects

---

## 5. Long-form ambient phrase memory
Goal: manually or sequencer-controlled scene changes.

### Patch
Use **SET** and **RST** instead of free clocking:
- Manual gate button / sequencer phrase output → **SET**
- Another phrase event → **RST**

Then use `OUT` to enable:
- extra reverb send
- noise floor
- filter opening
- secondary oscillator drone
- modulation depth

Use `VERT` for the opposite state.

### Result
You get a **two-scene ambient patch**:
- scene A: intimate, dry, low, stable
- scene B: wide, spectral, noisy, unstable

Very useful for live ambient transitions.

---

# Advanced patching concepts

## Cascading sections
Since there are 4 identical sections, patch one into another:

- section 1 clocks section 2
- section 2 resets section 3
- section 3 enables section 4

This creates **hierarchical rhythmic logic** from very simple clocks.

### Example
- Fast clock → section 1 CLK
- section 1 OUT → section 2 CLK
- section 2 OUT → open distortion
- section 2 VERT → open clean path

Now the distortion changes at half the rate of section 1, producing more structured phrasing.

---

## Use with clock divisions and odd resets
Toggle behaves especially well when the clock and reset are from different rhythmic grids.

Examples:
- 16ths to CLK, every 5th step to RST
- 8ths to CLK, triplets to SET
- burst generator to CLK, bar line to RST

This produces patterns that feel **designed but unstable**, ideal for DnB and dark techno.

---

## Create stepped pseudo-sequences
Toggle outputs are just gates, but gates become CV if you:
- attenuate them
- mix several sections together
- send them to quantized pitch inputs
- use them to switch between voltages

### Example
Use multiple sections to create binary-weighted CV:
- section 1 OUT = 1 unit
- section 2 OUT = 2 units
- section 3 OUT = 4 units
- section 4 OUT = 8 units

Mix them and send to pitch, filter cutoff, or wavefolder depth.  
Now you have a crude **binary sequencer** from a logic module.

For basslines, this is gold.

---

## Make fake sidechain / anti-sidechain structures
Because `VERT` is the opposite of `OUT` or `IN`, it’s useful for ducking and anti-ducking.

### Example
- kick trigger or kick gate into **IN**
- `VERT` opens pad VCA or reverb send

Result:
- kick present = pad ducks
- kick absent = pad swells

This can make ambient layers pulse around drums very musically.

---

# Specific sound-design recipes

## Distorted industrial percussion recipe
Use Toggle to alternate:
- short sine kick
- noise click through distortion
- metallic FM ping
- filtered feedback burst

Patch idea:
- 16th trigger stream to CLK
- OUT triggers kick
- VERT triggers noise burst
- slower section modulates distortion enable every 2 or 4 beats

This creates a brutal machine-like groove.

---

## Dubstep bass recipe
- Oscillator into lowpass filter into VCA
- parallel distortion/wavefolder path
- note gates into Toggle CLK
- OUT opens clean/sub emphasis
- VERT opens growl/distorted emphasis
- slower Toggle section controls filter envelope depth or FM amount

Result:
a bass that alternates between chesty low-end and snarling upper mids.

---

## Neuro / DnB rolling bass recipe
- Reese source
- band-split into low and high
- high band through phaser/distortion/filter
- Toggle section 1 alternates modulation between notch sweep and distortion amount
- Toggle section 2 resets section 1 every bar or every 2 bars
- optional IN inversion from snare gate to create spaces around backbeats

Result:
rolling bass with intentional phrasing and a lot of motion.

---

## Haunted pad recipe
- two detuned oscillators or a wavetable voice
- long envelope
- huge reverb
- noise or granular wash in parallel
- slow CLK into Toggle
- OUT opens shimmer/highpass layer
- VERT opens dark/noisy reverb return
- another section inverts the main gate to bloom background texture in the gaps

Result:
a pad that breathes between presence and absence, with ghostly tails.

---

# Practical tips

## 1. Gates are modulation, not just triggers
Don’t only think “trigger drums.”  
Use Toggle outputs for:
- VCA opens
- effect send opens
- switching CV paths
- selecting modulation destinations
- changing distortion/fold amount
- turning feedback loops on and off

That’s where the really unique sound design happens.

## 2. Run outputs through attenuators
Toggle outputs are logic high/low. If your destination accepts CV, attenuate them first.  
This makes the switching more subtle and usable for:
- filter movement
- FM amount
- resonance changes
- morph position
- effect depth

## 3. Pair with slew for softer shapes
If you run `OUT` or `VERT` through a slew limiter, the hard gate transitions become:
- rising/falling envelopes
- soft crossfades
- curved filter movement

Great for pads and more fluid bass wobble.

## 4. Use reset for musical control
Pure toggling can drift into patterns that are cool but hard to repeat.  
Adding periodic **RST** from your sequencer gives repeatable structure.

## 5. Exploit the normalization
If `IN` is empty, you get instant inverted logic from `OUT`.  
If you patch `IN`, that section becomes an inverter.  
This lets one module do both **pattern generation** and **negative-space logic** at once.

---

# Bottom line

The itijik Toggle is best treated as a **rhythmic state machine** rather than a simple utility. It excels at:

- **alternating drum layers**
- **creating clean/dirty or sub/growl bass switching**
- **adding phrase-level control to heavy bass patches**
- **opening atmospheric layers in the gaps**
- **making complementary modulation relationships**

For your targets specifically:

- **distorted percussion**: use `OUT`/`VERT` to alternate clean and crushed layers, noise transients, and feedback paths  
- **dubstep / DnB basslines**: use it to switch between sub and growl states, alternate envelopes, and structure wobble phrases  
- **haunting pads**: use inversion and slow toggling to make layers fade against each other and let spectral effects bloom in the spaces

If you want, I can also give you:
1. a **10-patch performance cheat sheet**,  
2. a **rack-specific patch plan** based on your modules, or  
3. a **signal-flow diagram** for bass, percussion, and pad patches using Toggle.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)