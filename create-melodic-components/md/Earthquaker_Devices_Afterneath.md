# Earthquaker Devices — Afterneath

- [Manual PDF](../../manuals/EQD-EU-Afterneath-Eurorack-R1.pdf)

---

[Manual PDF](attachment)

# EarthQuaker Devices Afterneath (Eurorack) — melodic use analysis

The attached manual is for a single Eurorack module:

- **EarthQuaker Devices Afterneath (Eurorack module)**

So there aren’t multiple modules in this PDF to combine with each other directly. But the **Afterneath itself can absolutely be used as a melodic sound-shaping and quasi-pitched voice** when patched with the rest of a modular system.

## What makes it melodic?

The key melodic features in the manual are:

- **Drag** changes the spacing of the internal delay lines
- **Mode** changes how Drag responds, including:
  - unquantized
  - 1V/oct-style response
  - quantized scales:
    - chromatic
    - major
    - minor
    - pentatonic
    - octaves + fifths
    - octaves
- **Self-oscillation** can turn the module into a kind of unstable pitched source
- **Drag CV input** can be driven by external CV for note-like movement
- **Reflect Send/Return** lets you reshape the feedback path, which can emphasize resonances and pitch behavior

In short: **Afterneath is primarily a reverb, but it can behave like a melodic processor and sometimes like a strange oscillator.**

---

## Core melodic roles for Afterneath

## 1. Quantized melodic processor for incoming notes

One of the strongest uses is to feed Afterneath with a sound source that already has pitch content:

- VCO
- plucked voice
- sampled percussion
- short envelopes
- noise bursts through a filter

Then use:

- **Mode 3–9**
- **Drag CV input**
- a sequencer, keyboard, random voltage, or quantized CV source

This lets Afterneath **re-pitch or melodically transform the material in its buffer**.

### Best modes for melody
From the manual:

- **Mode 3**: Unquantized Volt/Octave
- **Mode 4**: Chromatic
- **Mode 5**: Major
- **Mode 6**: Minor
- **Mode 7**: Pentatonic
- **Mode 8**: Octaves & Fifths
- **Mode 9**: Octaves

These are the modes most relevant for musical pitch structure.

### Musical result
You can play a note or phrase into Afterneath, then use CV into **Drag** to create:

- harmonized trails
- stepped melodic echoes
- scale-constrained shimmer-like movement
- pseudo-arpeggiation from a held sound

This is especially effective when the input is sparse and percussive.

---

## 2. Self-oscillating pseudo-oscillator

The manual explicitly says that with higher **Length** and **Reflect** settings, Afterneath will self-oscillate, and that with CV over **Drag**, this becomes an interesting **voltage-controlled oscillator**.

Important caveat from the manual:

- it is **not a precision oscillator**
- pitch depends partly on the sound fed into it
- harmonic/enharmonic transformations occur in feedback
- Drag responds only to **positive voltages between about 1.6V and 4.1V**
- the **Drag knob acts as an offset** for incoming CV

### Musical result
This gives you a voice that is great for:

- ghost melodies
- unstable lead lines
- drone melodies
- tuned feedback motifs
- haunted interval jumps

It is especially good for:

- ambient
- experimental
- soundtrack work
- generative tonal patches

Not ideal if you need perfect tuning over many octaves.

---

## 3. Scale-locked generative melody source

Modes **5–9** are especially good for this.

Patch:

- random stepped CV
- sample-and-hold
- a slow sequencer
- chaotic CV
- a modulation source into Drag CV

Then select:

- **Major**
- **Minor**
- **Pentatonic**
- **Octaves & Fifths**
- **Octaves**

According to the manual, random voltages into Drag CV in these modes produce **random melodies based on the selected scale**.

### Musical result
This makes Afterneath a very strong module for:

- generative melodic layers
- scale-safe ambient patterns
- semi-random pitched washes
- evolving background motifs

If you use **Mode 8 or 9**, the pitch behavior becomes more sparse and consonant.

---

## 4. Buffer-based melodic transposition effect

The manual repeatedly refers to audio in the **buffer**. That’s important.

Afterneath isn’t just adding reverb tail; it’s holding and transforming content in its delay structure. This means you can:

- feed in a single note
- let it ring
- modulate Drag slowly
- get warped pitch glides or stepped scale movement

### Good input material
For melodic use, feed it:

- short sine/triangle notes
- plucked LPG sounds
- filtered saw stabs
- FM plinks
- vocal-like resonant hits
- tuned percussion

Less dense input usually gives clearer melodic behavior.

---

# Patch ideas for melodic components

## Patch 1: Scale-quantized echo melody

**Goal:** turn a simple note source into a melodic echo line

### Patch
- VCO or voice -> **Audio Input**
- Sequence that voice normally
- Set **Mode** to:
  - **5 Major**, **6 Minor**, or **7 Pentatonic**
- Patch a stepped CV sequencer or random CV -> **Drag CV In**
- Turn **Drag CV attenuator** clockwise
- Set **Mix** moderately high
- Set **Length** medium
- Set **Reflect** low to medium
- Use **Diffuse** to choose sharper repeats or washier trails

### Result
Each incoming note generates a tail whose internal pitch movement follows the chosen scale. This can act like:

- a counter-melody
- harmonized echo
- melodic extension of a lead line

---

## Patch 2: Tuned self-oscillating lead/drone

**Goal:** use Afterneath as a strange playable voice

### Patch
- No sustained input required after excitation, but start by feeding a note or pulse burst into **Audio Input**
- Raise **Length** and **Reflect** above noon until self-oscillation starts
- Select **Mode 3–9**
- Patch keyboard or sequencer CV -> **Drag CV Input**
- Set Drag attenuator full clockwise initially
- Use the manual’s scaling method:
  1. Drag CV attenuator full clockwise
  2. Drag knob at noon
  3. choose Mode 3–9
  4. bring in self-oscillation
  5. find upper usable Drag range with highest note
  6. back off Length/Reflect if needed

### Result
A playable unstable oscillator-like texture that works well for:

- drones
- eerie leads
- melodic feedback lines
- textured bass motifs

### Tip
Use **Mode 7 Pentatonic** or **Mode 8 Octaves & Fifths** first; these tend to produce musically forgiving results.

---

## Patch 3: Generative melody cloud

**Goal:** create autonomous melodic ambience

### Patch
- Send occasional plucks, clicks, or filtered noise bursts -> **Audio Input**
- Set **Dry Kill** on if you only want the effected layer
- Set **Mode** to **5, 6, 7, 8, or 9**
- Random stepped CV -> **Drag CV Input**
- Slow triangle or random smooth CV -> **Diffuse CV** if available in your system
- Another slow CV -> **Length CV**
- Set **Reflect** near the edge of regeneration
- Tune **Dampen** to manage brightness

### Result
The module becomes a melodic atmosphere engine:
- notes smear into harmony
- random voltages become tonal motion
- tails turn into motifs

This is excellent for background melodic content that doesn’t feel like a conventional sequencer line.

---

## Patch 4: Pseudo-arpeggiator from one held note

**Goal:** derive a melody from a single sustained sound

### Patch
- Hold a steady oscillator note or a long envelope into **Audio Input**
- Set **Mode** to **4 Chromatic** or **5/6/7** for scale-based motion
- Send clocked stepped CV or sequencer CV to **Drag**
- Keep **Length** and **Reflect** moderate
- Adjust **Diffuse** lower for more articulated delay taps
- Use **Mix** to blend with original note

### Result
The reverb tail behaves like a broken, magical arpeggiator. Great for:

- melodic ornamentation
- accompaniment lines
- rhythmic pitch motion behind drones

---

## Patch 5: Feedback-loop melodic coloration

**Goal:** use Reflect send/return to make pitch behavior more pronounced

### Patch
- **Reflect Send** -> external processor -> **Reflect Return**
- Good processors:
  - filter
  - VCA
  - wavefolder
  - distortion
  - LPG
- Use **Reflect** as feedback amount / return attenuation
- Then modulate **Drag** with sequenced or random CV
- Choose a quantized Mode

### Result
The feedback loop becomes a tone-shaping resonant network. This can create:

- more pronounced pitch centers
- sharper resonant notes
- unstable melodic overtones
- animated harmonic motion

### Warning
The manual notes this can self-oscillate very easily, especially with distortion or resonant filters in the loop.

---

# Best external modules to pair with Afterneath for melody

Since this PDF is just Afterneath, here’s what works best around it in a real rack.

## 1. Sequencer or keyboard CV source
Needed for intentional melodic control of **Drag**.

Best for:
- Mode 3 volt/oct style
- chromatic melodic lines
- scale-based note movement

## 2. Quantized random source
Best for:
- generative melody
- ambient tonal movement
- pseudo-composition without manual note entry

## 3. Short-envelope voice source
Because Afterneath responds beautifully to struck or plucked material.

Best sources:
- LPG plucks
- percussive VCO hits
- resonant filter pings

## 4. Filter in Reflect loop
A filter in the feedback path is especially powerful for melodic shaping.

Use it to:
- emphasize a pitch range
- tame harsh regeneration
- create vowel-like resonances
- make self-oscillation more singable

## 5. VCA in Reflect loop
Lets you dynamically control feedback intensity.

This is useful for:
- notes that bloom into melody
- ducked feedback
- rhythmic gating of the tail
- controlled self-oscillation onset

---

# Control details that matter for melodic patching

## Drag CV range is limited
The manual says Drag responds only to **positive voltages from about 1.6V to 4.1V**.

That means:

- some sequencers may not hit the useful range directly
- 0–1.6V may need offset from the **Drag knob**
- bipolar LFOs/random may need external offset before they behave musically

This is extremely important. If pitch behavior seems weak or wrong, it’s often a voltage-range issue.

## The parameter knob acts as an offset
For CV-controlled parameters, the associated knob acts as an offset.

So for Drag:
- external CV provides movement
- the **Drag knob** shifts the operating window

This makes calibration crucial for melodic use.

## Diffuse changes note clarity
- Lower Diffuse = more attack, more discrete delay texture
- Higher Diffuse = smoother, washier, less articulated pitch events

For clearer melodic lines, keep **Diffuse** lower to moderate.

## Dampen affects melodic intelligibility
- Too dark: melodic movement may disappear into murk
- Too bright: feedback can become harsh

For melodic patches, a moderate setting often works best.

---

# Most useful modes for different melodic goals

## Mode 3 — Unquantized Volt/Octave
Best for:
- gliding pitch effects
- continuous melodic bends
- experimental tuning
- oscillator-like self-oscillation control

## Mode 4 — Chromatic
Best for:
- semitone-based sequences
- compatibility with traditional tonal lines
- weird but structured melodies

## Mode 5 — Major
Best for:
- consonant ambient lines
- uplifting harmonic trails
- easier generative patching

## Mode 6 — Minor
Best for:
- darker melodic atmospheres
- moody generative passages
- cinematic reverb voices

## Mode 7 — Pentatonic
Best for:
- highly usable random melodies
- fewer clashes
- modal drones and plucks

## Mode 8 — Octaves & Fifths
Best for:
- sparse consonant movement
- drone accompaniment
- power-interval shimmer

## Mode 9 — Octaves
Best for:
- very stable-feeling interval structure
- organ-like octave reinforcement
- minimalist melodic architecture

---

# Practical musical applications

## Countermelody generator
Feed your main melody line into Afterneath and drive Drag with a slower or related CV sequence. The tail becomes a second melodic actor.

## Harmonic ghost voice
Use Dry Kill and only monitor wet signal. The result is a detached melodic shadow of your source.

## Tuned ambient lead
Push into self-oscillation, tune the Drag CV range, and play it like a fragile voice.

## Tonal generative bed
Use random stepped voltage with a scale mode to make ever-changing melodic ambience.

## Melodic transition effect
Send single notes, chord stabs, or percussion fills into Afterneath and automate Drag for transition sweeps that still remain tonal.

---

# Bottom line

The **Afterneath module is not just a reverb**. According to the manual, it is especially powerful for melody because it can function as:

- a **scale-aware pitch-transforming reverb**
- a **CV-controlled melodic buffer effect**
- a **generative melody source**
- a **self-oscillating pseudo-oscillator**
- a **harmonic feedback instrument**

If you want melodic results, the most effective workflow is:

1. Use **Modes 3–9**
2. Patch a sequencer, keyboard, or random CV into **Drag CV**
3. Carefully set **Drag knob + attenuator** as offset/range calibration
4. Feed it simple pitched sounds
5. Use **Length** and **Reflect** to decide whether it behaves like:
   - an echo voice
   - a harmonic tail
   - a sustaining tonal buffer
   - a weird oscillator

For many systems, **Mode 7 (Pentatonic)** is the easiest starting point for immediately musical results.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)