# Acid Rain — Chainsaw

- [Manual PDF](../../manuals/Chainsaw_Manual_1.1.pdf)

---

[Manual PDF](#)

# Acid Rain Technology Chainsaw — melodic use in a Eurorack system

Chainsaw is a **stereo super-oscillator** designed to generate rich, harmonically dense pitched material. From the manual, it is a **digital oscillator** with:

- **3 independent voices**
- **7 waves per voice**
- up to **21 total waves**
- **1V/oct pitch inputs** for each voice
- global **detune**, **wave morph**, and **linear FM**
- stereo outputs with the internal waves spread across **left/right**

This makes it especially strong for melodic duties like:

- supersaw leads
- stacked chords
- unison basses
- animated arpeggios
- wide stereo pads
- pseudo-paraphonic lines

---

## What the module does musically

### 1. Three pitchable voices
Chainsaw has three separate **V/Oct inputs**:

- **V/O 1**
- **V/O 2**
- **V/O 3**

Each input activates one voice when patched. Since each voice is independently pitch-controlled, you can use the module for:

- **single-oscillator unison melodies**
- **interval stacking**
- **triads and chord voicings**
- **parallel melodic lines**

A very practical melodic interpretation:

- patch one sequencer to **V/O 1** for the melody root
- patch transposed copies or separate sequencer rows to **V/O 2** and **V/O 3**
- create chords such as:
  - root + major third + fifth
  - root + minor third + fifth
  - octaves + fifth for powerful riffs
  - suspended voicings for ambient lines

Because each voice contains **7 detuned oscillators**, even simple pitch material becomes huge and animated.

---

## Core sound-shaping controls for melody

### 2. Root frequency encoder
The encoder sets the root pitch in semitones when the **note** LED is lit.

- each encoder step = **1 semitone**
- press once to enter **fine tune** mode
- fine tune mode = **1 cent per step**
- hold for 2 seconds to reset to **C1 (32.7 Hz)**

Musically, this is useful for:

- quickly tuning the module to your patch
- setting a performance key center
- creating fixed drone roots against sequenced voices
- precise tuning for intervals and harmonic layering

---

### 3. Detune
The **detune** knob spreads the 7 oscillators in each voice around the root:

- 3 above
- 3 below
- 1 at root

At minimum, they are in perfect unison. As you increase detune, the spread follows a curve that creates the classic supersaw widening effect.

There is also a **detune CV input** accepting **-5V to +5V**.

For melodic work, detune is one of the most important controls:

- **low detune**: focused melodic lines, basses, tighter harmony
- **medium detune**: lush leads and chords
- **high detune**: trance-style supersaws, smeared harmonic clouds, wide pads

Patch ideas:

- slow LFO to detune CV for evolving pad movement
- envelope to detune CV for notes that “bloom” wider after attack
- stepped random CV for phrase-by-phrase variation

---

### 4. Saw-to-square morph
The second large knob morphs all waveforms from **sawtooth to square**.

There is also a **morph CV input** accepting **-5V to +5V**.

Musically:

- **saw side**: brighter, buzzy, harmonically dense, ideal for leads and supersaw stacks
- **square side**: hollower, weightier, excellent for bass and retro chord textures
- **in-between**: animated hybrid timbres that keep melodies lively

Great melodic uses:

- use an envelope on morph CV for per-note timbral articulation
- use a slow modulation source to gradually shift a progression from bright to hollow
- automate morph with sequencer CV to make each step of a melody feel orchestrated differently

---

### 5. Linear FM
Chainsaw has a global **linear FM input** for all voices, accepting **-5V to +5V** and responding predictably up to **2 kHz**.

This is useful melodically for:

- vibrato with a sine/triangle LFO
- audio-rate FM for brighter, more aggressive harmonic content
- subtle motion to keep held notes alive

Recommended musical use:

- for tonal melodic patches, keep FM **subtle**
- use very small modulation depth for expressive vibrato
- for more modern/aggressive lead tones, apply light audio-rate FM from another oscillator

Since FM affects all voices together, it works well when Chainsaw is used as a chord or supersaw stack.

---

## Stereo behavior and why it matters melodically

The 7 oscillators of all 3 voices are spread across:

- **Out L**
- **Out R**

This creates a naturally wide stereo image.

For melodic composition, that means:

- a single note already occupies space like a layered production
- intervals and chords sound large without external panning
- arpeggios can feel cinematic even before adding effects

You can also use only one output for mono operation, which is useful if:

- you want to process the sound through a mono filter or VCA chain
- you are building a more focused bass or lead patch
- your system has limited mixer inputs

---

# How to use Chainsaw for melodic roles

## 1. Monophonic supersaw lead
Patch:

- sequencer pitch CV → **V/O 1**
- gate → envelope → VCA controlling Chainsaw output
- Chainsaw **Out L/R** → stereo mixer or stereo filter/VCA

Settings:

- low-to-medium detune
- saw-heavy morph
- subtle FM vibrato from LFO

Result:

- huge lead sound with width and energy
- ideal for trance, melodic techno, synthwave, or cinematic hooks

Tip: keep detune lower for faster melodies so pitch remains articulate.

---

## 2. Massive bassline
Patch:

- pitch sequence → **V/O 1**
- use one output or both summed carefully to mono/stereo chain
- envelope-controlled filter after Chainsaw

Settings:

- low detune
- morph toward **square**
- very subtle or no FM

Result:

- thick, hollow basses
- stable pitch with lots of harmonic weight for filtering

Tip: too much detune can weaken low-end focus, so keep spread restrained for bass parts.

---

## 3. Three-note chord generator
Patch:

- root sequence → **V/O 1**
- transposed CV (+3 or +4 semitones) → **V/O 2**
- transposed CV (+7 semitones) → **V/O 3**

This gives:

- minor triad: root / +3 / +7
- major triad: root / +4 / +7

Alternative:
Use three independent sequencer rows to create changing voicings and inversions.

Settings:

- medium detune
- saw-to-square based on desired tone
- slow modulation to detune or morph

Result:

- instant supersaw chords
- excellent for stabs, pads, and chord progressions

---

## 4. Moving chord stabs
Patch:

- same triad setup as above
- gate sequence → snappy envelope → VCA
- second envelope or modulation lane → morph CV
- optional LFO → detune CV

Settings:

- moderate detune
- bright saw start, slightly more square during decay or vice versa

Result:

- dynamic chord hits
- very effective for house, techno, and synth-pop harmonic parts

---

## 5. Arpeggiated stereo texture
Patch:

- clocked pitch sources or sequential switching to **V/O 1/2/3**
- Chainsaw stereo outputs → delay/reverb

Approach:

- assign different intervals to each voice
- create broken chords over time
- use slow detune modulation for motion

Result:

- wide, immersive arpeggios
- complex harmonic movement from relatively simple pitch material

---

## 6. Pseudo-paraphonic patch
Since there are three pitch inputs, you can treat Chainsaw as a kind of compact chord/paraphonic voice source.

Patch:

- three separate pitch streams to **V/O 1, 2, 3**
- one shared envelope/VCA/filter path after the outputs

Result:

- three-note harmonic content with shared articulation
- excellent for:
  - chord memory style riffs
  - held intervals
  - ensemble lines

Important limitation:
This is not a fully separate 3-voice synth voice, because the module provides shared audio outputs rather than independent outputs per voice. So each voice is independently pitched, but they are mixed internally into stereo.

---

# Best supporting modules to pair with Chainsaw for melody

Chainsaw is an oscillator, so to build complete melodic parts it works best with:

## Sequencers
Needed for:

- note patterns
- transposition
- chord interval generation
- arpeggios

Especially useful:
- quantized CV sequencers
- precision adders
- chord interval generators

## Envelopes and VCAs
Needed for:

- note articulation
- plucks
- stabs
- swells

Without a VCA/envelope, Chainsaw will behave more like a continuously sounding drone source.

## Filters
Very effective after Chainsaw because the waveform is harmonically dense.

Use filters for:

- opening/closing lead brightness
- carving basses
- creating animated chord stabs
- taming high-frequency density

## Stereo effects
Because Chainsaw already has a stereo image, it pairs extremely well with:

- stereo delay
- stereo reverb
- chorus
- phaser

This can turn simple melodies into polished, finished-sounding musical layers.

## Modulation sources
Use LFOs, envelopes, random, or sequencer CV to animate:

- detune
- wave morph
- FM amount

This is the key to making repeated melodic phrases feel alive.

---

# Strong melodic patch recipes

## A. Trance lead
- sequencer → V/O 1
- medium detune
- morph near saw
- subtle LFO → FM for vibrato
- stereo delay + reverb after output

Why it works:
The supersaw architecture naturally creates the classic uplifting lead sound.

---

## B. Minor chord pad
- root CV → V/O 1
- root + 3 semitones → V/O 2
- root + 7 semitones → V/O 3
- slow envelope or LFO → morph CV
- slow random/LFO → detune CV
- long reverb

Why it works:
The internal 21-wave total architecture makes even static triads feel orchestral and wide.

---

## C. Octave/fifth bass stack
- bass sequence → V/O 1
- same sequence +12 semitones → V/O 2
- same sequence +7 semitones → V/O 3
- low detune
- morph toward square
- mono or centered stereo mix

Why it works:
This creates a harmonically reinforced bass that stays musical and powerful.

---

## D. Evolving melodic drone
- fixed or slowly sequenced CV to V/O 1, 2, 3
- very slow modulation to detune and morph
- slight FM from slow LFO
- stereo reverb/delay

Why it works:
Chainsaw excels at sustained harmonic material because of its layered oscillators and stereo spread.

---

# Things to keep in mind

## It needs external articulation
Chainsaw is a sound source, not a complete voice. To make traditional notes, you will usually want:

- VCA
- envelope
- often a filter

## Detune affects clarity
For melodic precision:

- use less detune for bass and fast lines
- use more detune for pads, leads, and sustained chords

## One shared timbral engine
All three voices share the same overall waveform morph and FM behavior. That means it is best thought of as:

- a unified chord/supersaw engine
rather than
- three completely independent synth voices

That shared architecture is actually an advantage for cohesive melodic textures.

---

# Summary

Chainsaw is excellent for melodic work because it combines:

- **accurate 1V/oct tracking**
- **three independently pitched voices**
- **supersaw-to-supersquare timbral range**
- **CV control over detune and morph**
- **stereo width built into the oscillator**

In a system, it works especially well as:

- a **lead oscillator**
- a **bass voice**
- a **stereo chord generator**
- a **pad/arpeggio source**
- a **compact paraphonic harmonic engine**

If you pair it with a sequencer, envelopes, VCA, and ideally a filter/effects chain, Chainsaw can serve as the core melodic voice for a very wide range of electronic styles.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)