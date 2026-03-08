# Frequency Central — Wonderland

- [Manual PDF](../../manuals/Wonderland-Build-Document.pdf)

---

[Manual PDF](http://www.frequencycentral.co.uk/)

# Frequency Central Wonderland — melodic use analysis

Wonderland is an **8×8 patchbay / matrix mixer / switcher** with:

- **8 inputs**
- **8 normal outputs**
- **8 inverted outputs**
- **64 push-on / push-off routing switches**
- **Per-input micro-attenuators**
- Ability to send:
  - one input to many outputs
  - many inputs to one output
  - many inputs to many outputs

From a musical Eurorack perspective, this makes Wonderland less of a “sound source” and more of a **melody routing brain**. It is especially useful for distributing, combining, and inverting pitch and modulation signals to generate structured melodic movement.

## What it does well for melody

Because multiple inputs can be mixed to a single output, Wonderland can act like a:

- **precision-ish CV combiner** for pitch-related control voltages
- **transpose distribution matrix**
- **variation router** for sequences
- **inversion source** using the dedicated inverted outputs
- **multi-destination melody sender** for layered voices

Its built-in input trimmers are important here: when summing melodic CV, you can reduce levels to avoid unwanted clipping or excessive pitch swings.

---

## Best melodic roles in a patch

## 1. Route one sequence to many voices

Patch a sequencer’s pitch CV into one Wonderland input.

Then use the switch matrix to send that same sequence to:

- Output A → VCO 1 pitch
- Output B → VCO 2 pitch
- Output C → quantizer input
- Output D → a filter tracking input
- Output E → FM index CV input

This lets one melodic line become the backbone of a whole patch.  
Because each routing is switch-based, you can quickly decide which destinations are part of the current melodic gesture.

### Musical result
- unison melodies
- octave-doubled lines
- one sequence controlling several timbral destinations
- easy live rearrangement

---

## 2. Mix multiple pitch sources into a single melodic line

One of Wonderland’s strongest uses is combining separate CV sources before they hit an oscillator or quantizer.

Example inputs:
- Input 1: main sequencer pitch
- Input 2: slow offset or transpose voltage
- Input 3: random stepped CV
- Input 4: keyboard or pressure CV
- Input 5: LFO at low attenuation

Route several of these to the same output.

### Musical result
You get a composite melodic control voltage made from:
- a base melody
- transposition
- ornamentation
- subtle drift or vibrato-like movement
- performance control

For melodic patching, this is especially powerful **before a quantizer**, because messy summed voltages can be forced back into a scale.

---

## 3. Use it before a quantizer for evolving melodies

A very practical patch:

- Several CV sources into Wonderland inputs
- Wonderland output into a **quantizer**
- Quantizer output into VCO pitch

Possible inputs:
- step sequencer row
- random stepped voltage
- envelope as a temporary pitch rise
- fixed offset
- another sequence running at a different clock division

The switch matrix becomes a **composition interface**. Turning routes on and off changes which ingredients feed the quantizer, producing melodic variations without changing the source modules.

### Why this works musically
Quantizers make Wonderland especially useful for melody because Wonderland can create rich but unstable CV mixtures, and the quantizer turns them into notes.

---

## 4. Create call-and-response lines with normal and inverted outputs

Every patched signal appears at both:

- **normal output**
- **inverted output**

This is excellent for melodic counterpoint.

Example:
- Output A (normal) → quantizer/VCO 1
- Output A inverted → another quantizer/VCO 2

If both are quantized to the same scale, the second voice can become a mirrored version of the first. Depending on offsets and quantizer behavior, this can produce:
- contrary motion
- descending responses to ascending phrases
- pseudo-fugal or mirror melody behavior

### Tip
Inverted pitch often needs an offset or requantizing stage to sit in a useful register.  
A quantizer after the inversion is often the key to making this musical.

---

## 5. Build transposition buses

Wonderland can serve as a central **transpose matrix**.

Patch:
- Input 1: base sequence
- Input 2: +1V offset
- Input 3: +0.583V or another interval source
- Input 4: keyboard CV
- Input 5: slow modulation

Then route different combinations to different outputs:

- Output A = base melody
- Output B = base + octave
- Output C = base + fifth-ish offset
- Output D = base + performance transpose

Send each output to a different voice or to different quantizers.

### Musical result
You get harmonized melodic layers from one central source.  
This is great for:
- bass + lead relationships
- canon-like voices at fixed intervals
- chord-tone derived lines

---

## 6. Distribute one modulation source to shape multiple melodic parameters

Melody isn’t only pitch. Wonderland can route one CV to many destinations affecting melodic articulation:

- sequence CV to oscillator pitch
- same CV to wavefolder amount
- same CV inverted to filter cutoff
- same CV attenuated to decay time CV

Because the module offers both normal and inverted outputs, one melodic contour can open one parameter while closing another.

### Musical result
A melody becomes more expressive because pitch movement is tied to timbre and dynamics.

---

## 7. Switch melodic layers live

The 64 pushbuttons make Wonderland particularly performance-friendly.

You can treat the matrix like a playable composition grid:
- add a transpose source to a voice
- remove random CV from a melody
- send a melodic line to a second oscillator
- suddenly introduce inversion to a counter-melody

This is useful in live techno, ambient, or generative patches where you want to reshape melodic relationships without repatching cables.

---

## Patch ideas for melodic creation

## Patch 1: Two-voice mirrored melody

**Goal:** main melody plus inverse companion line

Patch:
- Sequencer pitch CV → Input 1
- Input 1 routed to Output A
- Output A normal → Quantizer 1 → VCO 1
- Output A inverted → Quantizer 2 → VCO 2
- Same gate source triggers both envelopes

Result:
- Voice 1 plays the main line
- Voice 2 plays an inverted/mirrored line

Best for:
- contrapuntal melodies
- haunting ambient duets
- electro-style mirrored riffs

---

## Patch 2: Generative melody mixer

**Goal:** evolving quantized melody

Patch:
- Sequencer row 1 → Input 1
- Turing/random stepped CV → Input 2
- Slow triangle LFO → Input 3
- Manual offset voltage → Input 4

Route various combinations to Output B.

Then:
- Output B → Quantizer → VCO pitch

Use the matrix buttons to add/remove contributing sources.

Result:
- melody changes with each routing state
- easy movement between stable and unstable pitch material
- performance-friendly generative composition

---

## Patch 3: Harmony splitter from one sequence

**Goal:** derive several related melodic lines from one sequence

Patch:
- Main sequence → Input 1
- Octave offset → Input 2
- Fifth-like offset → Input 3

Create:
- Output A = Input 1 only
- Output B = Input 1 + Input 2
- Output C = Input 1 + Input 3

Send outputs to:
- bass voice
- lead voice
- pluck voice

Result:
- harmonically linked melodic parts
- simple arrangement from few sources
- strong for melodic techno and Berlin-school style patterns

---

## Patch 4: Sequence plus expressive performance control

**Goal:** playable melody variation

Patch:
- Main sequencer CV → Input 1
- Keyboard/controller pressure or joystick → Input 2
- Slow random voltage → Input 3

Route to one output feeding a quantizer and oscillator.

Result:
- the sequencer provides note structure
- your controller adds expressive transposition or bends
- random voltage adds slight melodic surprise

This works nicely for live improvisation.

---

## Patch 5: Use inversion for bass/lead opposition

**Goal:** bass and lead move against each other

Patch:
- Base melodic CV → Input 1
- Output C normal → lead quantizer/VCO
- Output C inverted → bass quantizer/VCO

Optionally add:
- fixed offset to the bass side after quantization or before a second quantizer

Result:
- when lead climbs, bass tends to fall
- strong tension and motion
- cinematic and very musical when restrained to a scale

---

## Things to watch out for

## 1. It is a mixer, so pitch accuracy may depend on context
When using Wonderland for melodic CV, remember it is fundamentally summing and routing voltages. If you are doing strict 1V/oct harmonic work, summed voltages should be tested by ear and tuner. It will still be highly useful, but exact interval behavior depends on the rest of your system and how carefully levels are set.

## 2. Input attenuators are very important
The micro-attenuators help prevent overblown pitch jumps when multiple CVs are combined. For melody, they let you decide whether an added source acts as:
- a full transpose
- a subtle inflection
- a tiny ornament

## 3. Inverted pitch usually benefits from quantization
Raw inverted pitch CV can be musically wild. Putting a quantizer after the inverted output often makes the result much more usable.

## 4. Multiple sources to one output can clip
The manual notes that many inputs summed to one output can cause clipping. For audio this may be desirable; for melodic CV it may produce unexpected note ranges or flattened behavior. Use the trimmers to tame this.

---

## Best companion modules for melody

Wonderland becomes especially strong when paired with:

- **sequencers** — for base note patterns
- **quantizers** — to force mixed CV into scales
- **precision adders / offsets** — for cleaner transposition
- **random stepped voltage generators** — for melodic variation
- **joysticks / keyboards / touch controllers** — for performance input
- **multiple oscillators** — to exploit the many outputs
- **logic and clocks** — for synchronized melodic changes

---

## Overall musical takeaway

Wonderland is not a melody generator by itself, but it is a very powerful **melodic infrastructure module**.

Used creatively, it can:
- distribute one melody across several voices
- combine several CV sources into evolving note lines
- create mirrored or contrary-motion melodies via inversion
- generate harmonized layers from a single sequence
- act as a live-performance matrix for rearranging melodic relationships on the fly

If your system already includes sequencers, quantizers, offsets, and oscillators, Wonderland can become the central place where those ingredients are recombined into **riffs, harmonies, counter-melodies, and generative pitch structures**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)