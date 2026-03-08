# ADDAC Systems — ADDAC-112 Granular Looper

- [Manual PDF](../../manuals/ADDAC112_Granular_E_0.pdf)

---

[ADDAC112 VC Looper & Granular Processor Manual (PDF)](https://media.addacsystem.com/manuals/ADDAC112_manual.pdf)

# Using the ADDAC112 to Create Melodic Components in a Eurorack System

The **ADDAC112 VC Looper & Granular Processor** is not just a texture machine. It can be used very effectively as a **melodic instrument**, especially when you treat its **looper**, **pitch controls**, **quantizer**, **preset system**, and **granular engine** as compositional tools rather than just effects.

## What the module gives you musically

From the manual, the ADDAC112 combines:

- a **stereo looper**
- a **granular processor** that works on the selected loop
- **CV over nearly every front-panel control**
- **quantized pitch control**
- **preset recall**
- **loop selection by CV**
- the ability to **record, overdub, repitch, and resample**
- up to **99 loops** and **99 presets** per bank

That means it can act as:

- a **melodic sampler**
- a **phrase looper**
- a **quantized granular voice**
- a **pitched resampling oscillator**
- a **bank of playable notes/chords/phrases**
- a **generative melody source**

---

## The main melodic building blocks

## 1. Loops as playable notes or phrases

The most direct melodic use is to record or load short loops that contain:

- a single note
- a sustained harmonic tone
- a chord stab
- a pluck
- a vocal syllable
- a melodic phrase

Then use:

- **LOOP SELECT** to choose which sample is active
- **LOOP PITCH** to transpose it
- **QUANTIZE** to constrain pitch musically
- **PRESET SELECT** to switch complete granular settings

### Good loop material for melody
For melodic composition, load or record:

- one-shot notes from an oscillator
- tuned percussion
- vocal vowels
- filtered saw/square tones
- chords from external gear
- short arpeggio fragments

A useful strategy is to build a bank where each loop is:

- the same approximate loudness
- similar duration
- tuned to a root note

Then the module becomes a playable melodic memory.

---

## 2. Quantized pitch for tonal control

The manual shows that both **loop pitch** and **grain pitch** can be quantized, depending on menu settings.

### Quantizer options
You can set the quantizer to affect:

- **both** loops and grains
- **loops only**
- **grains only**

There are also selectable scales, including default or custom scale sets. This is very important for melodic use.

### Musical implication
If you send CV to:

- **Loop Pitch CV**
- **Grain Pitch CV**

and quantization is enabled, the pitch changes can snap to scale tones. This turns the module into something much more like a playable voice.

### Best melodic use
- Use **Loops Only** if you want stable sampled phrases that transpose in key.
- Use **Grains Only** if the loop stays fixed but the granular layer creates the melody.
- Use **Both** if you want a harmonically locked but highly animated result.

---

## 3. Grains as a melodic voice

The granular engine reads from the currently selected loop, and each grain has control over:

- **position**
- **length**
- **delay/intermittency**
- **direction**
- **repeat**
- **volume**
- **panning**
- **pitch**
- **envelope**
- **deviation/randomness**

This is where the module becomes especially interesting for melody.

Instead of thinking "granular = texture," think:

- each grain can be a **note event**
- grain pitch can define the melodic interval
- grain position can choose which part of the source is heard
- grain repeat/intermittency can form rhythms
- envelope shapes can turn grains into plucks, pads, or bowed tones

---

# Practical melodic patch ideas

## Patch 1: Quantized sample voice

### Goal
Use the ADDAC112 like a pitchable sampler voice.

### Setup
1. Record a stable tone into a loop, such as:
   - sine
   - triangle
   - filtered saw
   - vocal hum

2. Bring up:
   - **Loop Volume**
   - optionally **Dry Volume** down
   - **Grains Volume** down for now

3. Enable quantization for **Loops Only** or **Both**.

4. Send a sequencer CV into **Loop Pitch CV**.

### Result
The loop plays back as a transposable sampled tone. Because the pitch range can be set in the menu, you can choose finer or wider behavior.

### Best for
- basslines
- lead lines
- drones with chord changes
- transposed vocal tones

### Enhancement
Use **Play/Reset** and **On Loop Change** options to control whether playback retriggers or continues smoothly.

---

## Patch 2: Granular melody from a static loop

### Goal
Create a melodic line using grain pitch while the loop itself stays fixed.

### Setup
1. Record or load a harmonically rich loop.
   - a chord
   - sustained oscillator
   - field recording with identifiable pitch content
   - vocal tone

2. Keep **Loop Volume** low or off.
3. Bring up **Grains Volume**.
4. Set:
   - moderate **Grains Active**
   - short-to-medium **Play Length**
   - low **Length Deviation**
   - low **Position Deviation**
   - moderate **Attack/Decay**

5. Send melodic CV into **Grain Pitch CV**.
6. Set quantizer to **Grains Only** or **Both**.

### Result
The granular engine becomes the actual melodic voice. The loop is just source material.

### Why it works
A stable source with moving grain pitch gives you:
- a coherent timbre
- melodic control
- evolving articulation

### Best for
- shimmering leads
- choral melodies
- bell-like lines
- ambient motifs

---

## Patch 3: Scan different loop positions as different notes

### Goal
Turn one recorded phrase into many melodic events.

### Setup
1. Record a loop containing several different notes or timbral regions.
   Example:
   - a short melody
   - a scale
   - a spoken word
   - multiple plucks

2. Use the granular engine.
3. Modulate **Position** with:
   - stepped random
   - sequencer CV
   - sample & hold
   - keyboard CV offset/attenuated

4. Set low **Position Deviation** for more precise scanning.
5. Set short **Play Length**.

### Result
Each grain picks a different slice of the loop, so the loop acts like a wavetable or phrase memory. If the recorded material contains separate notes, scanning position becomes a melodic selection method.

### Best for
- cut-up melodies
- phrase rearrangement
- pseudo-wavetable lead sounds
- vocal formant melodies

---

## Patch 4: Use loop banks as a note/chord palette

### Goal
Use different loops as separate notes, intervals, or chords.

### Setup
Create a bank where loop numbers correspond to musical material, for example:

- Loop 1 = C
- Loop 2 = E
- Loop 3 = G
- Loop 4 = Bb
- Loop 5 = Dm chord
- Loop 6 = G chord
- Loop 7 = vocal note
- Loop 8 = noise transient

Then sequence **Loop Select CV**.

### Result
The ADDAC112 behaves like a sample-addressed melodic instrument. This is especially strong if each loop is normalized and similar in length.

### Best for
- chord progression playback
- note selection by CV
- switching among melodic motifs
- live performance scenes

### Extra musical trick
Set **On Loop Change** to:
- **Immediate** for abrupt jump-cuts
- **On Loop End** for phrase-aligned changes

This gives you either chopped rhythmic melody or phrase-safe musical transitions.

---

## Patch 5: Granular arpeggiator

### Goal
Make repeating grains function like arpeggiated notes.

### Setup
1. Use a harmonically rich loop.
2. Set:
   - short **Play Length**
   - clear **Attack/Decay**
   - moderate **Grain Loop Delay**
   - low/moderate **Delay Deviation**
   - **Repeat Mode** to Repeat X or Probability

3. Patch stepped CV to:
   - **Grain Pitch**
   - or **Position**
   - or both

4. Use quantization.

### Result
Grains become repeating note attacks. With envelope shaping, they behave like plucked notes.

### Best for
- arps
- pointillist melodies
- clocked melodic textures
- sequenced microsound lines

---

## Patch 6: Resampling melody generator

### Goal
Use the looper and overdub path to recursively build melodic material.

The manual explains that recording input is a mix of:
1. input signal
2. current loop playback
3. grains feedback

### Setup
1. Start with a simple recorded note or phrase.
2. Granularly process it.
3. Increase **Grains Feedback** so grains feed the recorder.
4. Use **Overdub Decay** to keep some of the old buffer while replacing part of it.
5. Repitch loops and grains while re-recording.

### Result
The buffer gradually evolves into a new pitched source. Over time, your melody becomes self-derived and transforms while staying related.

### Best for
- evolving melodic drones
- self-mutating ostinatos
- recursive harmonic layering
- experimental tonal composition

---

## Patch 7: Phrase harmonizer

### Goal
Create harmony from a monophonic phrase.

### Setup
1. Record a melodic phrase into the looper.
2. Keep loop playback present.
3. Add grains with:
   - different **Grain Pitch**
   - moderate **Grains Active**
   - medium **Attack/Decay**
   - panning spread

4. Quantize grains to a useful scale.

### Result
The loop plays the original line while the grains add harmonized intervals around it.

### Best for
- vocal harmonies
- synthetic counterlines
- thickened leads
- melodic ambient layering

---

# How the two sections work together melodically

## Looper = phrase memory and tonal source
The looper is best thought of as:
- the sample pool
- the root pitch body
- the rhythmic/melodic phrase source

## Granular engine = articulation and variation
The granular side provides:
- note extraction
- alternate pitch layers
- repeated fragments
- harmonic extension
- microtiming variation

Together, they can behave like:
- a sampler + harmonizer
- a phrase looper + granular sequencer
- a wavetable-ish voice made from recorded sound

---

# Most important controls for melody

## LOOP PITCH
This is central if you want the looper itself to act melodically.

Use it for:
- transposition
- basslines
- chord changes
- tuned phrase playback

## GRAIN PITCH
Use this when the grains are the “notes.”

Use it for:
- harmonies
- lead melodies
- arps
- interval clouds

## POSITION
Very useful if your loop contains several notes or timbral regions.

Use it for:
- selecting note zones
- changing vowel/formant region
- slicing recorded phrases

## PLAY LENGTH
This determines whether grains sound like:
- clicks
- plucks
- syllables
- sustained tones

For melody, short-to-medium lengths often work best.

## ATTACK / DECAY
These shape articulation.

For melodic roles:
- short attack/decay = plucked
- longer attack/decay = pad or bowed
- asymmetry = speech-like phrasing

## GRAIN LOOP DELAY
This sets spacing between grain events.

Use it as a rhythmic density control for:
- arps
- repeated melodic pulses
- sparse pointillism

## REPEAT MODE
This matters a lot musically.

- **Probability** gives generative variation
- **Repeat X** gives motif persistence

---

# Strong musical workflows

## Workflow 1: Build a playable note bank
- record one note per loop
- normalize levels
- use Loop Select CV for note choice
- use Loop Pitch for transposition
- use presets for articulation variants

This gives you a sample-based melodic instrument.

## Workflow 2: Build a phrase bank
- record riffs, chord stabs, short lines
- switch loops under CV
- set loop changes to immediate or phrase-end
- add grains for ornamental harmony

This is excellent for live melodic performance.

## Workflow 3: One loop, many melodies
- record a single rich source
- use grains only
- sequence grain pitch and/or position
- let deviation add small variation

This is probably the most “granular” melodic use.

---

# Presets as melodic scenes

The manual notes that presets store:
- loop lists
- granular settings

This is very useful compositionally.

You can make presets like:

- **Preset 0** = dry loop playback
- **Preset 1** = short plucked grains
- **Preset 2** = octave-up shimmer
- **Preset 3** = reverse grain melody
- **Preset 4** = long pad harmonization

Then sequence or manually switch presets as arrangement sections.

This turns the module into a **scene-based melodic processor**.

---

# Good companion module roles in a rack

Even though this manual only covers the ADDAC112, it clearly benefits from being paired with standard Eurorack utility categories.

## 1. Pitch sequencer
Use for:
- loop pitch melodies
- grain pitch melodies
- quantized transposition

## 2. Random stepped CV
Use for:
- grain position
- loop select
- repeat density
- panning and variation

## 3. Clock / trigger source
Use for:
- loop control
- synced recording
- clocked mode behavior
- rhythmic loop changes

## 4. Envelope/LFO/Function generator
Use for:
- modulating position slowly
- sweeping grain length
- changing density and articulation

## 5. External oscillator or voice
Use as source material to record tuned notes/chords into the looper.

---

# Particularly powerful melodic features from the manual

## Quantizer with custom scales
This is one of the biggest musical advantages. You can constrain pitch material to a compositionally useful set.

Because the scale file can be customized, you can create:
- standard tonal scales
- modal scales
- just intonation-ish ratio sets
- harmonic series mappings
- non-octave scales

That makes the module unusually strong for melodic experimentation.

## Independent playback, recording, and grains
The updated firmware allows:
- loop playback
- grains processing
- recording

to happen in parallel.

This means you can:
- play one melodic loop
- granularly decorate it
- simultaneously record a new loop from the mixture

That is ideal for iterative melodic development.

## CV over almost everything
This means melody on the ADDAC112 does not have to be static. You can voltage-control:
- pitch
- density
- position
- volume
- selection
- feedback behavior

So the melodic output can evolve constantly.

---

# Performance-oriented melodic strategies

## 1. Live resampled soloing
- record a short phrase live
- immediately granularize it
- transpose grains with CV
- overdub new notes into the same buffer

This gives a live-looping solo instrument feel.

## 2. Preset-based verse/chorus changes
Use presets to shift between:
- sparse plucks
- dense harmony
- reverse shimmer
- wide stereo melody

## 3. Loop-select chord progression
Assign different chord tones or chord stabs to loop slots, then use CV or manual selection for harmonic movement.

## 4. Reverse melody accents
Use grain direction probability or reverse loop playback for occasional backward note phrasing.

---

# A few concrete melodic patch recipes

## Recipe A: Granular lead
- Record a steady saw wave note
- Loop volume low
- Grains volume high
- Grains active: low to medium
- Position fixed
- Length short-medium
- Attack low
- Decay medium
- Grain pitch sequenced and quantized

Result: expressive digital lead.

## Recipe B: Vocal chord instrument
- Load sung vowels at different pitches into separate loops
- Sequence loop select
- Add grains pitched a third or fifth above
- Moderate panning
- Longer envelope

Result: choir-like harmonic pad or melodic line.

## Recipe C: Broken tape melody
- Record a melodic phrase
- Use loop pitch under quantized CV
- Add moderate delay deviation and grain repeat
- Anti-aliasing off for rougher pitching

Result: degraded but tonal phrase mutation.

## Recipe D: Arp cloud
- Harmonic loop source
- Short grains
- Grain repeat active
- Grain pitch quantized
- Position slightly modulated
- Delay controls set for pulsed spacing

Result: sparkling arpeggiated cloud.

---

# Limitations to keep in mind for melodic use

## 1. Knob pickup behavior with presets
When changing presets, panel knobs do not immediately reflect stored values. You have to cross the stored value before the knob becomes active. In performance, this matters.

## 2. Loop memory is finite
The bank has about 30 MB total shared loop memory, so if you want many melodic loops, keep them short and efficient.

## 3. Save your bank
Recorded loops live in volatile memory until saved. For melody-building sessions, save often.

## 4. Grain pitch can stall in one pitch range mode
The manual warns that in the **-INF to +24** mode, grain pitch at -INF can stop the grain engine. Avoid that setting unless you intend it.

---

# Best overall musical concept

The ADDAC112 works best melodically when you think in three layers:

## Layer 1: Source
Record or load something with pitch identity:
- note
- chord
- phrase
- voice
- harmonic texture

## Layer 2: Selection
Choose what musical material is active via:
- loop select
- grain position
- preset changes

## Layer 3: Tuning and articulation
Shape it into melody with:
- loop pitch
- grain pitch
- quantization
- envelope
- density
- repetition

That is the core of how this module becomes a melodic instrument rather than only a sound processor.

---

# Bottom line

The **ADDAC112** can be used for melody in at least four strong ways:

1. **As a quantized looper-sampler voice**  
   Record notes/phrases and transpose them musically.

2. **As a granular melodic voice**  
   Keep the loop static and sequence grain pitch, position, and rhythm.

3. **As a phrase/chord switching instrument**  
   Use loop select and presets as musical scene changes.

4. **As a self-resampling melody generator**  
   Feed loops and grains back into recording for evolving tonal material.

If your goal is melodic composition, the most powerful combination is:

- tuned source loop
- quantized pitch CV
- controlled grain envelopes
- moderate position scanning
- preset-based scene changes

That gives you everything from **pitched leads and basslines** to **harmonized phrases**, **granular arpeggios**, and **evolving melodic textures**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)