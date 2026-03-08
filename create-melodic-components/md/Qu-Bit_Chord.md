# Qu-Bit — Chord

- [Manual PDF](../../manuals/QB_Chord.pdf)

---

[Manual PDF](#)

# Qu-Bit Chord v2 — using it to create melodic components

This manual is for the **Qu-Bit Chord v2**, a 4-voice polyphonic oscillator for Eurorack. Since only this module is included here, I’ll focus on how to use **Chord v2 by itself and with common supporting Eurorack companions** to build melodic material: leads, chord progressions, arpeggio-like motion, drones, counterpoint, and harmonized lines.

## What this module is musically

Chord v2 is essentially:

- **four oscillators in one**
- internally related by **chord quality** and **voicing**
- with **independent outputs** for root / third / fifth / seventh
- plus a **mix output**
- and several modes that turn it from “chord oscillator” into a more flexible **polyphonic pitch structure generator**

That makes it especially strong for melodic duties because it can produce:

- a full chord from one pitch CV
- a chord plus a separate melody
- four quantized independent pitch lanes
- stacked unison voices for thick monophonic lines
- interval-based motion that stays musical

---

## Core musical functions that matter for melody

## 1. One CV can generate full harmonic melody

The **V/Oct input** controls the root note.  
In standard chord mode, the module builds the other notes around that root according to:

- **Quality**: maj7, min7, dom7, half-diminished, diminished, sus, augmented, etc.
- **Voicing**: inversion and octave spacing

So a simple sequencer into **V/Oct** gives you:

- moving root notes
- harmonized vertical structures
- melodic chord changes from a single line

This is the easiest way to get musical melodic content quickly.

### Good use:
- Send an 8-step sequence into **V/Oct**
- Take the **Mix** output to a filter/VCA
- Modulate **Quality** slowly
- You get a harmonic progression with evolving color

---

## 2. Melody mode creates “chord + lead”

This is probably the most immediately useful feature for songwriting.

In **Melody Mode**:
- the **Lead input** controls the **Seventh output** as an independent melodic voice
- the other voices still behave as a chord tied to the root
- inversions still affect that seventh voice

So you can patch:

- one sequencer to **V/Oct** for the chord progression
- a second sequencer to **Lead** for a melody line
- take **Mix** for the harmony bed
- take **Seventh out** separately for the lead

This gives you:
- backing harmony and lead from one module
- tightly related melodic material
- easy “solo over chords” patches

### Great patch idea:
- **V/Oct**: slow 4-step progression
- **Lead**: faster 8- or 16-step melody
- **Triad mode on** so the seventh is omitted from Mix
- Send **Mix** through one voice chain
- Send **Seventh** through a different VCA/filter/effect

Result:
- the chord accompaniment stays clean
- the melodic lead sits independently above it

This is one of the best uses of Chord v2 for melodic composition.

---

## 3. Auto-Harm makes melodic lines stay in key

The **Harm** button enables automatic harmonization and scale quantization.

In normal or melody mode:
- **off** = no quantization
- **blue** = major
- **green** = minor

When enabled:
- **V/Oct** and **Lead** are quantized to the chosen scale
- chord quality is automatically adjusted to fit the key

This means you can feed in:
- a loose sequencer
- random CV
- voltage from a sample & hold
- pressure/joystick/manual CV

…and Chord will pull it into usable melodic territory.

### Musical value:
This is huge for creating:
- melodic fragments that remain tonal
- harmonized lines without needing an external quantizer
- evolving generative melodies that still sound composed

### Example:
- random stepped CV into **V/Oct**
- another random stepped CV into **Lead**
- **Harm = Minor**
- **Melody Mode on**

Now you get:
- a shifting chord progression
- a separate melody
- both constrained to minor tonality

Very effective for ambient, soundtrack, and generative music.

---

## 4. Free Poly Mode turns it into four pitch voices

In **Free Poly Mode**:
- **Coarse knob / V/Oct CV** control root
- **Fine knob / Lead CV** control third
- **Voicing knob / Voicing CV** control fifth
- **Quality knob / Quality CV** control seventh

So instead of one chord relationship system, you now have **four independently pitched oscillators**.

This can be used melodically for:

- 4-note counterpoint
- four-note step-sequenced harmonies
- pseudo-paraphonic sequencing
- canon-like pitch structures
- clustered melodic motion

If you have multiple pitch sequencers or CV lanes, this mode is extremely powerful.

### Example:
Patch four related but different pitch CV sources:
- bassline CV → **V/Oct**
- upper melody → **Lead**
- slower supporting motion → **Voicing**
- tension note/random lane → **Quality**

Then take the separate outputs:
- **Root**
- **Third**
- **Fifth**
- **Seventh**

Process each differently.

This creates true multi-part melodic content, not just static chord stacks.

---

## 5. Unison Poly Mode creates thick mono lines or interval riffs

In **Unison Poly Mode**:
- all four oscillators are tuned together internally
- each voice has its own pitch input:
  - V/Oct → root output
  - Lead → third output
  - Voicing → fifth output
  - Quality → seventh output

This is excellent for:
- layered lead synth lines
- octave/unison riffs
- detuned-feeling stacks via interval offsets
- powerfully articulated melodic phrases

Even though the manual describes them as tuned together, each voice can be externally addressed by its dedicated pitch input. That means you can create:

- same melody on all 4 voices with small differences
- parallel interval melodies
- stacked chord stabs from four sequencer lanes

### Great lead patch:
- copy the same sequence to all four pitch inputs
- offset some CVs by octaves or intervals externally
- use different outputs separately or mix them
- add slight modulation to waveform or FM

This gives a huge supersaw / organ / ensemble style melodic line.

---

## 6. Separate outputs make melody orchestration easy

Chord gives you:

- **Root out**
- **Third out**
- **Fifth out**
- **Seventh out**
- **Mix out**

This matters because melodic writing is not just notes — it’s also **arrangement**.

You can use the outputs as:

- **Root** = bass melody
- **Third/Fifth** = inner harmony
- **Seventh** = top line / tension line
- **Mix** = complete harmonic blend

### Practical routing ideas:
- Root → lowpass filter for bass
- Third/Fifth → stereo effects
- Seventh → brighter voice for melody
- Mix → pad or drone layer

This lets one module generate multiple melodic roles at once.

---

# How to use Chord v2 for specific melodic components

## A. Chord progression generator

### Patch:
- sequencer → **V/Oct**
- envelope/LFO → **Wave**
- slow CV → **Quality**
- slow CV or manual changes → **Voicing**
- output: **Mix**

### Result:
A chord progression with timbral evolution.

### Why it works:
The root sequence defines the harmonic movement; Quality and Voicing add emotional and spatial variation.

---

## B. Chords plus lead melody

### Patch:
- progression sequencer → **V/Oct**
- melody sequencer → **Lead**
- **Mode = Melody**
- **Triad = on**
- **Mix** out = accompaniment
- **Seventh** out = lead

### Result:
One module performs both harmony and melody.

### Best for:
- techno hooks
- synth-pop progressions
- soundtrack textures
- live improvisation

---

## C. Generative tonal melody machine

### Patch:
- random stepped CV → **V/Oct**
- random stepped CV → **Lead**
- **Mode = Melody**
- **Harm = Major or Minor**
- moderate clocking differences between the random sources

### Result:
Self-generating harmonized melodic material that stays in key.

### Tip:
Use **minor mode** for darker melodic behavior; use **major** for brighter, more diatonic movement.

---

## D. Four-voice contrapuntal patch

### Patch:
- **Mode = Free Poly**
- 4 CV lanes or sequencers into:
  - V/Oct
  - Lead
  - Voicing
  - Quality
- use individual outs instead of Mix

### Result:
Independent melodic lines from one oscillator module.

### Best for:
- experimental polyphony
- minimal music
- phase patterns
- evolving harmonic webs

---

## E. Thick mono lead

### Patch:
- **Mode = Unison Poly**
- same or closely related sequence to all pitch inputs
- mix outputs externally
- use a bright wavetable bank
- add linear FM lightly

### Result:
Dense, harmonically rich lead melody.

### Best for:
- solos
- hooks
- arpeggiated riffs
- big synth lines

---

## F. Bass + upper extension melody

### Patch:
- sequencer → **V/Oct**
- **Mode = Melody**
- another sequencer → **Lead**
- Root out → bass voice chain
- Seventh out → lead voice chain
- Mix out or Third/Fifth outs → harmonic support

### Result:
A complete melodic arrangement with low foundation and top-line motion.

---

# The waveform side: why it matters melodically

Chord v2 has **8 factory waveform banks**:

1. Bandlimited traditional waveforms
2. Saw through low pass
3. FM
4. Distorted
5. Voice
6. Square with pulse-width control
7. Video game
8. Organ

For melody, these banks change the role of the line dramatically.

## Best banks for melodic use

### Traditional / filtered saw
- best for clear pitch perception
- ideal for leads, chord stabs, bass melodies

### FM
- adds brightness and motion
- great for expressive melodic hooks

### Voice
- excellent for pseudo-choir melodies and formant-like chord lines
- especially strong for sustained harmonic melodies

### Video game
- focused, characterful melodic tone
- good for arps and memorable lead lines

### Organ
- ideal for block chords, drones, and contrapuntal lines

---

# Voicing as a melodic tool, not just chord spacing

The **Voicing** control changes inversion and octave spacing.

This is important because changing voicing can create the feeling of melodic movement even when the root stays the same.

For example:
- one held root CV
- manually or via CV change the voicing
- the upper voices jump octaves and invert

That produces:
- internal line motion
- rising/falling upper-register phrases
- pseudo-arpeggiated movement without changing the root

### Good compositional trick:
Hold a single bass note, then sweep or sequence **Voicing**.  
The chord “breathes” and generates melodic contour in the upper notes.

Especially useful for:
- ambient
- drones
- slow harmonic music
- cinematic transitions

---

# Quality as emotional melodic motion

The **Quality** control changes the intervals:

- major 7
- minor 7
- dominant 7
- half diminished
- diminished
- sus 2 / sus 4 style variants
- augmented

This can be sequenced or modulated to create melodic color changes.

### Musical effect:
Even if the root sequence stays simple, changing quality causes upper notes to move:
- third shifts between major/minor/sus
- fifth may flatten or sharpen
- seventh changes tension

That creates **embedded melodies inside the harmony**.

### Example:
Hold one root note and sequence Quality:
- Major 7 → Minor 7 → Dominant 7 → Sus → Augmented

The upper voices create a moving harmonic melody over a pedal tone.

---

# Triad mode is important for clear melodic separation

The **Triad** function removes the seventh from the Mix output and boosts level to compensate.

This is especially useful when:
- the seventh is being used as a separate lead voice in Melody mode
- you want the chord to stay less dense
- you want less harmonic clutter in the accompaniment

### In practice:
- Turn on Triad
- Use **Mix** as the backing harmony
- Use **Seventh out** as the melody

This is one of the most practical “song arrangement” features in the module.

---

# User chords: excellent for custom melodic languages

Chord v2 can load **12 user chords** from SD card.

You can define custom interval structures, including microtonal or cluster-based chord shapes.

Examples from the manual:
- major: `4,7,11`
- minor: `3,7,10`
- dominant: `4,7,10`
- tone cluster: `0.2,0.4,0.6`

This means you can design your own melodic-harmonic system.

## Why that matters musically

You can create:
- quartal chords
- cluster harmony
- suspended interval sets
- gamelan-like stacks
- custom modal structures
- microtonal melodic ecosystems

Then sequence the root note and get a whole custom harmonic melody system from one CV line.

### Great advanced use:
Create 12 user chords that represent your own harmonic vocabulary, then sequence/changing the **Quality** selection across them.  
Now Chord v2 becomes a personal harmonic instrument rather than a fixed chord box.

---

# User wavetables for melodic identity

The SD card also allows custom wavetable loading.

That matters for melody because timbre strongly affects perceived phrasing and identity.

You can use custom waves to create:
- vocal-ish leads
- metallic melodic lines
- sampled spectral movement
- unique pads and chord colors

The manual even notes you can drop in a song or sample for unusual results. That’s not always “clean,” but it can yield very distinctive melodic textures.

---

# Best companion modules for making melody with Chord v2

Even though only Chord is shown in this manual, here’s how it naturally pairs with typical Eurorack tools.

## 1. Sequencer
Use one or more pitch sequencers for:
- root progression
- separate lead line
- free poly pitch lanes

Best roles:
- one sequencer for chord roots
- one sequencer for lead melody
- one CV lane for quality changes

---

## 2. Quantizer
Less necessary because Harm mode already quantizes, but still useful if:
- you want different scales
- you want external harmonic control
- you use Free Poly mode without auto-harm

---

## 3. Envelope + VCA
Chord is an oscillator, so for melodic phrasing you need articulation:
- note on/off shape
- plucks
- stabs
- sustained pads
- pulsed chord rhythms

Without VCA/envelope, you have pitch but not phrasing.

---

## 4. Filter
Vital for turning raw oscillator output into expressive melody:
- lowpass for warm chords
- bandpass for vocal-like lead
- resonance for movement
- envelope modulation for articulation

---

## 5. Clocked random / sample & hold
Excellent with Harm mode:
- random CV becomes tonal melody
- changing root and lead independently makes evolving musical structures

---

## 6. Mixer
Very useful because Chord already provides multiple audio lanes. A mixer lets you:
- balance root vs upper voices
- pan voices
- mute tones
- build arrangement structure

---

## 7. Effects
Especially effective:
- chorus for pads and chord beds
- delay on lead voice
- reverb on upper harmonies
- saturation on bass/root

---

# A few complete patch recipes

## Patch 1: Instant melodic synth-pop voice
- Sequencer A → **V/Oct**
- Sequencer B → **Lead**
- **Mode = Melody**
- **Harm = Major**
- **Triad = On**
- **Mix** → filter → VCA → reverb
- **Seventh** → separate VCA → delay

You get:
- chord progression
- top-line melody
- clean separation between accompaniment and lead

---

## Patch 2: Evolving ambient harmony
- slow random CV → **V/Oct**
- very slow random CV → **Quality**
- slow LFO → **Voicing**
- **Harm = Minor**
- choose **Voice** or **Organ** wavetable bank
- **Mix** through long reverb

You get:
- drifting harmonic melody
- scale-constrained changes
- rich ambient chord movement

---

## Patch 3: Polyphonic machine-music counterpoint
- **Mode = Free Poly**
- four sequencer lanes into all four pitch inputs
- all four outputs to separate VCAs/filters
- each voice gets a different rhythm gate

You get:
- quasi-polyphonic independent melodic lines
- interlocking voices
- very sophisticated musical texture from one module

---

## Patch 4: Thick lead hook
- **Mode = Unison Poly**
- copy one melody CV to all pitch inputs
- offset one or two copies by octave externally
- use FM or distorted bank
- mix outputs externally with slight panning/effects

You get:
- huge melodic line
- layered intervals
- strong front-of-mix synth hook

---

## Patch 5: Bassline plus chord stabs
- Sequence root notes into **V/Oct**
- Root out → bass filter/VCA
- Mix out → separate VCA for chord stabs
- trigger both from related but different envelopes
- modulate Quality every few bars

You get:
- coordinated bass and harmony
- strong melodic coherence
- compact patching

---

# Important operational details from the manual

## CV ranges
Several parameter CV inputs are **-5V to +5V**, added to knob position:
- Bank
- Waveform
- Voicing
- Quality

Pitch-related jacks are described as **0V to 5V inputs**:
- V/Oct
- Lead

So for melody building, be aware of your source ranges and attenuation.

---

## Calibration
Chord v2 can be calibrated for:
- standard 1V/oct
- or other systems like Buchla-style standards

If your melodic intervals feel off across octaves, calibration is worth checking.

---

## LFO mode
There is also a config option for **LFO_MODE**, which shifts the module 6 octaves lower.

That turns Chord into four related LFOs instead of audio oscillators.

While not directly melodic audio, this is very useful for:
- self-modulating melodic patches
- slow harmonic CV motion
- interval-related modulation sent elsewhere

For example:
- use Chord in LFO mode
- send outputs as related modulation to another oscillator’s pitch/filter/index
- create harmonically structured modulation patterns

---

# Bottom line

## The strongest melodic uses of Qu-Bit Chord v2 are:

1. **Chord progression from one pitch line**
2. **Chord + independent melody in Melody mode**
3. **Generative tonal sequencing with Harm quantization**
4. **Four-voice contrapuntal writing in Free Poly mode**
5. **Stacked lead sounds in Unison Poly mode**
6. **Separating bass, harmony, and lead via individual outputs**
7. **Designing your own melodic language with custom chords and wavetables**

If you approach it just as a “chord oscillator,” you’ll use only part of it.  
If you approach it as a **compact harmonic composition engine**, it becomes a very powerful melodic module.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)