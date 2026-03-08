# Worng Electronics — Vector Space

- [Manual PDF](../../manuals/Vector Space Manual v1.00.pdf)

---

[Vector Space Manual PDF](attachment)

# WORNG Electronics Vector Space: using it for melodic patching

Vector Space is not a pitch source by itself. It’s a **CV relationship generator**: you feed it **three modulation or pitch-related voltages**, and it gives you **17 related outputs**. That makes it extremely useful for building **melodies, harmonies, counterpoint, voice-leading, and evolving pitch structures**.

## What the module does musically

Vector Space takes three inputs: **i, j, k**.

It then derives 17 outputs in three families:

- **8 Cube outputs**
- **6 Plane outputs**
- **3 Sphere outputs**:
  - Sphere
  - NegSphere
  - UnSphere

It can process CV or audio, but for melody-making the key idea is:

> Send in three changing voltages, then use the different outputs as related melodic control voltages.

Because all 17 outputs are derived from the same three sources, they tend to sound **coherent together**, even when they are different enough to create separate melodic lines.

---

## Important setup idea: unipolar vs bipolar

Each input has a **++ / +- switch**:

- **+-** = bipolar, about **±5V**
- **++** = unipolar, about **0–10V**

This matters a lot for melodic work.

### For pitch use:
- **Stepped random**, sequencers, or addressed voltages usually work well in **unipolar**
- **LFOs** and many modulation sources often make more sense in **bipolar**
- Flipping the switch acts like an **offset/performance move**, which can instantly reshape the melodic relationships

If you’re patching into a quantizer, these switches are a great way to push a line into a different register or change its contour.

---

# How each output family helps create melody

## 1. Cube outputs: the clearest melodic material

The **Cube outputs** are the most straightforward combinations of the three inputs, with in-phase and out-of-phase mixtures.

### Musically, use them for:
- Related melodies across several voices
- Voice-leading variants of one harmonic motion
- Pitch CVs for multiple oscillators via quantizers
- Root / inversion-like movement when the inputs are sequenced differently

### Why they work
These outputs are easier to understand and tend to preserve the identity of the incoming CVs. If your three inputs are:
- a sequence
- a slow transposition source
- a rhythmic stepped random

then each Cube output becomes a different weighted/sign-flipped combination of those three behaviors.

### Best use case
Run **several Cube outputs into separate quantizers** or into a **multi-channel quantizer**, then send them to multiple VCOs. This gives you:
- one melody
- a countermelody
- a bassline
- a harmony voice

all evolving from the same underlying motion.

---

## 2. Plane outputs: excellent for harmonic clustering and counterpoint

The manual specifically points out a special property of the **Plane outputs**:

> at any one moment, three of the outputs will have similar voltages, but which three changes as the input phases change

That is extremely musically useful.

### Musically, use them for:
- three-part counterpoint
- clustered harmony that opens and closes
- canon-like related voices
- melodic lines that converge and diverge
- pseudo-chord voicings from moving CVs

Because these outputs use **rectified versions** of two inputs plus a phased version of the third, they are more skewed positive and can create very interesting pitch behavior after quantization.

### Why they’re powerful for melody
When quantized, the “three outputs tracking together” behavior can produce:
- temporary unisons
- close intervals
- shifting triad-like movement
- melodic braiding between voices

This is especially effective when each Plane output goes to its own oscillator voice.

### Extra bonus
Rectification can effectively **double modulation frequency**, so if one of your inputs is an LFO or oscillating stepped source, Plane outputs can generate more active note changes than the original source.

---

## 3. Sphere / NegSphere / UnSphere: contour, center gravity, and tension

These three are less like “normal mixed pitch CVs” and more like **meta-melodic controls**.

### Sphere
A sum of all rectified inputs, representing how far the point is from the center.

**Use it for:**
- a master transposition lane
- melody intensity
- opening into higher register as motion increases
- quantized “energy melody”

Because it’s based on rectified inputs, it tends to stay positive and can create a strong upward-biased melodic contour.

### NegSphere
Negative version of Sphere.

**Use it for:**
- contrary-motion bassline
- opposite-register melodic reflection
- downward counterline to a Sphere melody

This is especially useful if Sphere controls a high voice and NegSphere controls a bass voice.

### UnSphere
Represents distance to the closest edge of the sphere; highest at the center, lower toward the edges.

**Use it for:**
- central “home note” behavior
- tonic-like stabilizing melody
- drone pitch selection
- a middle voice that is most active when the modulation space is balanced

This output is especially good for creating a sense of **melodic center** while the Cube and Plane outputs create more unstable motion around it.

---

# Best melodic patch strategies

## 1. Generative counterpoint patch
This is the most obvious melodic use from the manual.

### Patch:
- Send **three stepped voltages** into **i, j, k**
  - sequencers
  - Turing/random stepped CV
  - sample and hold
  - clocked voltage source
- Take **3 or more Plane outputs**
- Send each through a **quantizer**
- Patch each quantized output to separate VCOs

### Result:
You get several related melodic voices that:
- often move together
- then split apart
- then regroup in new combinations

### Improve it:
- Use different clock divisions for the 3 input sources
- Use one source as a slow transpose lane
- Flip input polarity/range switches live
- Use different quantizer scales for different voices:
  - one diatonic
  - one pentatonic
  - one chord-constrained

This can create rich ambient, generative, or minimalist melodic systems.

---

## 2. One module becomes “melody orchestra”
Use Vector Space as the center of a multi-voice patch.

### Inputs:
- **i** = primary sequencer
- **j** = slow random stepped CV
- **k** = envelope or slow triangle LFO

### Outputs:
- Cube output 1 → quantizer → lead voice
- Cube output 2 → quantizer → second voice
- Plane output 1 → quantizer → pluck voice
- NegSphere → quantizer → bass
- UnSphere → quantizer → drone or pad pitch

### Result:
A full melodic ecosystem from one sequencer plus two modulation sources.

The sequencer provides recognizable musical structure, while the other two sources constantly reshape interval relationships.

---

## 3. Harmonic voice-leading patch
This works well if you want music that sounds composed rather than random.

### Inputs:
- **i** = root movement sequencer
- **j** = slow transposition CV
- **k** = stepped interval source or octave offset source

### Outputs:
Use several **Cube outputs** into quantizers and then VCOs.

### Result:
The different outputs will behave like alternate harmonizations of the same motion. Since the outputs are mathematically related, your voices tend to move with internal logic rather than feeling disconnected.

This is great for:
- Berlin-school lines
- modal harmony
- evolving ostinati
- contrapuntal polysynth-style patches

---

## 4. Joystick-played melody space
The manual discusses joystick use for spatialization, but it also works beautifully for melody.

### Patch:
- Joystick X → i
- Joystick Y → j
- Slow CV or sequence → k

Take several Cube/Plane outputs through quantizers to oscillators.

### Result:
Your hand movement “navigates” a field of related notes and harmonies. This gives a very performable way to:
- sweep through chord voicings
- discover melodies by hand
- improvise harmonic changes
- control several voices at once

UnSphere is especially useful here as a center-focused voice.

---

## 5. Use Sphere outputs as melodic macro-controls
Instead of using all outputs directly as pitch, use some of them to control the melody system around a main sequence.

### Example:
- Main sequencer directly to lead oscillator
- Sphere → transpose input of quantizer
- NegSphere → bass quantizer CV
- UnSphere → secondary voice pitch or sequence address

### Result:
The melody stays anchored by a clear sequence, but the harmony and accompaniment breathe around it.

This is often more musical than using all 17 outputs as raw pitch.

---

# Input source combinations that work especially well

## Three stepped CV sources
Best for:
- generative melodies
- multi-voice pitch generation
- counterpoint

Examples:
- sequencer + random + sample & hold
- three differently clocked sequencers
- one sequence copied into two attenuated/offset variants plus a third random source

## Sequence + slow modulation + stepped random
Best for:
- melodic patches that feel structured but alive

This is probably the sweet spot for many musical uses.

## Three LFOs into quantizers
Best for:
- looping melodic systems
- phase-based canon patterns
- pseudo-polyrhythmic melodies

Since Plane outputs can frequency-double through rectification, this can make surprisingly complex note movement from simple LFOs.

## Audio-rate oscillators
Best for:
- timbral/audio use more than conventional melody

But if heavily attenuated and quantized, audio-rate interactions can create unstable stepped melodic artifacts. More experimental than tonal.

---

# Practical melodic workflow

## Recommended signal chain
For pitch work, a very useful chain is:

**CV sources → Vector Space → attenuation/offset if needed → quantizer → VCO 1V/oct**

Why:
- Vector Space can output large voltages
- Some outputs may benefit from scaling before quantization
- Quantizers turn its complex CV relationships into musically usable note sets

## Use a shared quantizer scale
If multiple outputs are quantized to the same scale, the voices stay musically related even when the raw CVs diverge.

Good scales:
- minor pentatonic for forgiving generative patches
- dorian/aeolian for melodic ambient work
- chord quantization for strong harmonic identity

## Use different octave placements
Even if two outputs are close in voltage, placing oscillators in different octaves makes the result feel intentional and layered.

## Add slewing selectively
If some outputs are too jagged:
- keep one voice fully stepped
- slew another slightly
- leave a third un-slewed but quantized

This creates more expressive melodic contrast.

---

# Particularly strong “together” uses inside one patch

Since the module has several output families, a very musical approach is to assign them roles:

## Cube = principal melodic voices
Use for:
- lead
- alto
- tenor lines

## Plane = harmony/counterpoint voices
Use for:
- clustered voices
- inner parts
- accompaniment arps

## Sphere family = macro structure
Use for:
- bassline
- transposition
- tonic center
- phrase intensity

This division gives the patch a natural musical hierarchy.

---

# Concrete example patch: evolving 4-voice melody

## Inputs
- **i** = 8-step sequencer
- **j** = slow clocked random CV
- **k** = triangle LFO synced to phrase length

Set:
- sequencer likely **unipolar**
- random source depends on source, often **unipolar**
- LFO usually **bipolar**

## Outputs
- Cube out A → quantizer → VCO 1 (lead)
- Cube out B → quantizer → VCO 2 (countermelody)
- Plane out A → quantizer → VCO 3 (inner voice)
- NegSphere → quantizer → VCO 4 (bass)

## Supporting modulation
- UnSphere → filter cutoff on the lead
- Sphere → VCA level for one harmony voice

## Musical result
- Lead follows recognizable sequenced motion
- Countermelody tracks but deviates
- Inner voice periodically converges with others
- Bass moves in contrary contour
- timbre and dynamics reflect the same vector movement

This is a very efficient way to get a complete melodic composition from a small number of CV sources.

---

# Concrete example patch: playable harmonic improvisation

## Inputs
- Joystick X → i
- Joystick Y → j
- Slow random stepped CV → k

## Outputs
- 3 Plane outs → 3 quantizers → 3 oscillators
- UnSphere → fourth quantizer → central drone/melody
- Sphere → transpose amount for one or more quantizers

## Result
You can “steer” through harmonically related note regions by hand. This is excellent for:
- live improvisation
- soundtrack work
- ambient chordal movement
- controlled generative melody

---

# What it pairs well with for melodic systems

Vector Space works especially well with:

- **Quantizers**
- **Precision adders / transposers**
- **Sequential switches**
- **Stepped random modules**
- **Clock dividers**
- **Joysticks**
- **Multi-channel VCO setups**
- **VCAs** for voice balancing
- **Attenuverters/offset generators**

If your goal is melody, the most important companion is a **good quantizer**.

---

# Best musical roles for Vector Space

In a melodic patch, Vector Space is best thought of as one of these:

1. **Multi-voice melody generator**
2. **Harmony and counterpoint engine**
3. **CV orchestrator for several quantized voices**
4. **Performance interface for navigating pitch relationships**
5. **Meta-modulation source for transposition and phrase structure**

It is less about writing one exact melody and more about creating a **field of related melodic possibilities**.

---

# Bottom line

WORNG Vector Space is excellent for creating melodic components when used with quantizers and multiple voices. Its strength is not “a single tune,” but **families of interrelated pitch lines**:

- **Cube outputs** for clear melodic variants
- **Plane outputs** for converging/diverging counterpoint
- **Sphere outputs** for center, tension, and contrary motion

If you feed it:
- one structured source,
- one semi-random source,
- and one slow modulator,

you can get a whole melodic arrangement out of a single patch.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)