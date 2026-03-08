# Intellijel — MultiGrain

- [Manual PDF](../../manuals/multigrain_manual_v1.2_2025.09.02.pdf)

---

[Manual PDF: Intellijel Multigrain v1.2](#)

# Using Intellijel Multigrain to Create Melodic Components in Eurorack

The attached manual is for the **Intellijel Multigrain**, a **live stereo morphing granular sampler**. Even though it is not a traditional oscillator/VCO voice, it is extremely capable of producing **pitched, melodic, and harmonic material** when patched thoughtfully.

Below is a musician-focused analysis of how this module can be used to create melodic components in music.

---

## What Multigrain is, musically

Multigrain is best understood as a **granular voice and sample-based sound source** with:

- **8 playable sounds**
- **2 scenes per sound**
- **morphing between scenes**
- **pitch control**
- **quantization**
- **CV-addressable sound selection**
- **syncable grain generation**
- **sample recording / live input processing**

So for melody work, it can act like:

- a **pitched sample voice**
- a **granular lead**
- a **chord/texture generator**
- a **quantized melodic percussion source**
- a **multi-sound pseudo-rompler**
- a **live resampling melodic processor**

---

# Core melodic features

## 1. Pitch control

The most obvious melodic function is the **PITCH** parameter.

From the manual:

- Pitch spans **±2 octaves** from the knob
- With modulation, pitch can extend to **±3 octaves**
- Pitch can be modulated by **X / Y / Z CV**
- Full-depth modulation from X/Y/Z can give **1V/oct-style control**
- Fine tune is available on the **Alt Page**

### Why this matters
This means Multigrain can be patched like a playable voice:

- send a sequencer CV to **X**, **Y**, or **Z**
- assign that mod input to **PITCH**
- set mod depth to full
- optionally enable the quantizer

That gives you melodic lines from any loaded sample or live sound.

---

## 2. Built-in quantizer

The module includes a **per-sound pitch quantizer**.

You can:

- enable any notes in a 12-TET scale
- set a root note
- choose whether quantization affects:
  - **pitch knob + modulation**
  - or **modulation only**

### Musical implication
This is one of the strongest melody-oriented features in the module.

You can use Multigrain as:

- a **scale-locked lead voice**
- a **harmonically constrained texture source**
- a **tonal sample player**
- a **melodic granular arp machine**

This is especially useful when granular playback would otherwise feel too unstable or atonal.

---

## 3. 8 sounds as playable note colors

The **8 sound slots** are not just storage—they are part of performance.

Each sound can hold:

- its own sample or live source
- its own scene states
- its own quantizer settings
- its own fine tuning
- its own pitch/rate/size relationships

### This allows:
- one sound per note family
- one sound per chord tone
- one sound per articulation
- one sound per section of a melody

For example:

- Sound 1 = soft vowel pad
- Sound 2 = plucked piano transient
- Sound 3 = bright string scrape
- Sound 4 = vocal chop
- Sound 5 = breathy flute attack
- Sound 6 = granular bell
- Sound 7 = noisy harmonic texture
- Sound 8 = low drone support

Then use **SELECT CV** or **NEXT** to sequence through them.

This gives melody a kind of **sample-orchestrated phrasing** instead of fixed timbre.

---

# Best melodic patch approaches

## A. Classic quantized granular lead

### Patch
- Load a pitched sample into one sound
  - good choices: sine-ish tone, flute, vocal, string harmonic, piano note, synth waveform
- Patch sequencer pitch CV into **X**
- Assign **X → PITCH** at full depth
- Enable **Quantizer**
- Set desired scale
- Use **GATE** input to trigger notes
- Keep:
  - **SCAN** near center
  - **WRAP** modest
  - **SIZE** medium
  - **RATE** low or linked carefully

### Result
A playable melodic voice where each trigger produces a pitched grain or stream of grains.

### Musical character
Compared with a normal oscillator, this gives:
- more texture
- more sample identity
- more transient variation
- more unstable or expressive tone

Excellent for:
- leads
- hooks
- fragile melodies
- cinematic top lines

---

## B. Multi-articulation melodic voice

Because each sound can be separately configured, you can create a **performance bank of articulations**.

### Example setup
Use all 8 sound slots as versions of one instrument:

- Sound 1 = short pluck
- Sound 2 = soft sustain
- Sound 3 = reverse swell
- Sound 4 = filtered muted tone
- Sound 5 = wide blurred version
- Sound 6 = bright harmonic version
- Sound 7 = noisy attack version
- Sound 8 = lower octave variation

Then:
- use one CV source for pitch
- use **SELECT** or **NEXT** to choose timbre per note/event

### Result
A single melodic line can feel much more alive, because timbre changes note-to-note.

This is especially strong for:
- generative melodies
- evolving ostinatos
- “acoustic-like” phrasing
- IDM / ambient / soundtrack writing

---

## C. Melodies from scanned sample regions

The **START / WRAP / SCAN** controls are very important musically.

These let you choose where the grains come from in the sample.

### Melodic use
Instead of using a whole sample as one static source, you can load:

- a multisampled instrument phrase
- a vocal phrase
- a recording of several pitches in sequence
- a chord arpeggio
- a plucked riff

Then use:

- **START** to select a region
- **WRAP** to constrain the usable area
- **SCAN** to move through the region

### Result
The melody is shaped not only by pitch CV, but also by **which fragment of the sample is being harvested**.

This can create:
- melodic variation
- pseudo-formant shifts
- changing note attacks
- phrase internal movement

This is one of the most “granular” ways to make melody feel alive.

---

## D. Chord and harmonic melody source

Multigrain is stereo and sample-based, so it works very well with **chord samples**.

### Technique
Load:
- sustained chords
- stacked intervals
- vocal harmonies
- orchestral clusters
- synth stabs

Then use:
- **PITCH** for transposition
- **QUANT** to keep movement tonal
- **SIZE–PITCH link** if you want content-preserving transposition behavior
- **SCENE morphing** to move between harmonic densities

### Result
You can generate:
- chord pads
- harmonic stabs
- parallel harmonies
- melodic phrases with built-in interval content

This is especially effective when your “melody” is really a **harmonized line**.

---

# Scene morphing as melodic expression

Each sound has **Scene A** and **Scene B**, and the **Morph fader/CV** blends between them.

This is huge for melody, because it means one note source can have two states:

- Scene A = stable, centered, tonal
- Scene B = unstable, bright, scattered, reversed, blurred

### Example uses

## 1. Phrase shaping
Use Scene A for verse-like clarity and Scene B for chorus-like expansion.

## 2. Dynamic articulation
Morph amount can act like an expressive control similar to:
- bow pressure
- breath intensity
- filter opening
- picking angle

## 3. Harmonic transformation
Because scene morphing also morphs modulation depths, you can go from:
- static pitch
- to heavily randomized pitch/scan behavior

without repatching.

## 4. Performance transitions
For melody, this is fantastic:
- intro = pure sustained grain
- buildup = more scan and blur
- drop = tighter, brighter, percussive
- outro = slow, reversed, diffused

---

# The two link modes are especially important for melodic use

## RATE–SIZE link

When linked:
- grain rate depends on grain size
- smaller grains = faster triggering
- larger grains = slower triggering

### Melodic effect
This helps maintain more coherent texture as pitch material changes.

Useful when you want:
- sustained notes with overlap
- a more “playable instrument” feel
- less manual balancing of size/rate

---

## SIZE–PITCH link

When linked:
- pitch changes also affect grain duration so the same audio content stays inside the grain

### Why this matters melodically
This is often the better setting for pitched material such as:
- vocals
- piano
- plucks
- acoustic notes
- phrases

It preserves identity across transposition more naturally than simple independent pitch/size control.

For melodic patches, this can make the voice feel much more intentional and musical.

---

# Using live sounds melodically

Version 1.2 adds **Live Sounds**, where any sound can derive grains from the live input via the Looping Recorder.

This is extremely useful for melody.

## Live melodic use cases

### 1. Turn another oscillator into a granular melody voice
Patch an oscillator, voice, or external synth into **IN L / IN R**.

Then:
- assign a sound as **Live Sound**
- send pitch CV to Multigrain’s pitch modulation
- trigger via GATE
- use quantizer if desired

Now your incoming audio becomes raw material for a new granular melodic layer.

### 2. Granular harmonizer
Feed in a monophonic melody from another module or external instrument.

Then use Multigrain to:
- transpose it
- quantize it
- freeze it
- generate new melodic material from it

### 3. Resample-and-play workflow
Capture a phrase, then:
- assign it to a sound
- transpose it melodically
- scan different parts for note variation

This is a strong way to derive melody from field recordings, vocals, or other modules.

---

# Using sound selection as a melodic sequencer dimension

Multigrain has three sound control inputs:

- **GATE**
- **NEXT**
- **SELECT**

These are not pitch CV, but they are still highly musical.

## SELECT input
Maps 0–5V across sounds 1–8.

### Melodic uses
If each sound contains:
- a different pitch center
- a different sample
- a different harmonic region
- a different articulation

then SELECT becomes a **meta-sequencer for melodic timbre**.

This can create:
- timbral melodies
- phrase alternation
- call-and-response
- note-family switching

## NEXT input
Advances to the next occupied sound.

### Melodic uses
This is excellent for:
- stepping through tuned samples
- rotating through chord tones
- cycling through attack/sustain/reverse variations
- creating pseudo-arpeggios

If you organize sounds carefully, NEXT becomes a **musical phrase rotator**.

---

# Sample choices that work best for melody

The manual’s sample guide is very useful here. For melodic work, the best sample types are usually:

## Strong choices
- single sustained notes
- plucked instrument notes
- vocal vowels
- choral tones
- bell tones
- mallet hits
- waveforms or simple synth tones
- strings and harmonics
- short musical phrases
- multisample chains

## Also strong
- stereo split samples with different content L/R
- chord samples
- arps and strums
- nature sounds with pitch identity
- breathy/noisy acoustic sources for expressive upper voices

## Less straightforward
- very dense full-mix material
- samples with too much silence
- poorly trimmed one-shots

These can still be musical, but are harder to control melodically.

---

# Best parameter strategies for melodic clarity

If your goal is melody, not pure texture, here’s how I’d approach the main controls.

## START
Use to choose the musically useful part of the sample:
- the onset for attack
- the steady-state region for sustain
- the tail for airy texture

## WRAP
Keep fairly narrow for more stable note identity.

## SCAN
- centered for stable tones
- slight movement for life
- large movement for phrase animation

## SHAPE
For melody:
- **Bell**, **Tukey**, or **Triangle** often feel most natural
- **Square** and **Ramp** can be more effect-like

## LEVEL
Straightforward note balancing.

## TONE
Useful for fitting a melodic line into a mix:
- lowpass for background lines
- highpass for airy leads

## RATE
- low rate for discrete notes
- higher rate for shimmer / sustained clouds

## SIZE
- medium-to-long for recognizable pitch/body
- short for pointillistic melodic fragments

## BLUR
Great for melodic ambience, but too much can smear note definition.

## REVERSE
Excellent for alternate articulations and phrase endings.

---

# Modulation strategies for melodic writing

Multigrain really shines when melody is not static.

## 1. Modulate pitch subtly
Use small modulation on pitch for:
- vibrato-like movement
- note instability
- humanized phrasing

If you want real melodic accuracy, keep the main pitch under sequencer control and use subtle mod only.

## 2. Modulate START
This is one of the best melodic gestures on the module.

A little START modulation changes:
- attack
- spectral emphasis
- vowel/formant character
- sample micro-position

This makes repeated notes feel alive.

## 3. Modulate MORPH
For expressive phrase shaping, patch an envelope, slow LFO, or performance CV into **MORPH**.

## 4. Use random on non-pitch parameters
For melody, random is best applied lightly to:
- START
- TONE
- LEVEL
- SHAPE
- SCAN

This creates variation without destroying tonal intent.

## 5. Be careful with random pitch
Unless you want aleatoric melody, random pitch should be restrained or quantized.

---

# Quantized pitch modulation patch recipe

A practical melodic patch:

## Patch
- Load a pitched sample into SOUND 1
- Sequencer CV → **X**
- Gate sequencer → **GATE**
- Assign **X to PITCH** at 100%
- Enable **Quantizer**
- Choose scale
- Fine tune sample root if needed
- Set:
  - SIZE medium
  - RATE low/moderate
  - SHAPE bell/tukey
  - WRAP narrow
  - SCAN near center

## Optional additions
- Envelope or pressure CV → **MORPH**
- Slow random → **START**
- Clock → **SYNC**
- THRU enabled with external source for hybrid layering

## Result
A stable granular lead voice that remains musically scaled.

---

# Using SYNC for melodic rhythm

The **SYNC** input does not quantize pitch, but it does quantize the grain engine rhythmically.

For melody this matters because rhythmic note structure often defines the phrase as much as pitch.

## With SYNC enabled:
- RATE can divide/multiply clock
- Live sound grain position can quantize to clock multiples

### Musical result
You can build:
- clocked melodic pulses
- sync’d granular arps
- tempo-locked repeated notes
- rhythmic harmonic clouds

This is very useful for:
- techno
- electronica
- rhythmic ambient
- generative melodic loops

---

# Multigrain as a melodic percussion instrument

Not all melody needs to be legato or tonal in a traditional way.

Using short samples and careful pitch sequencing, Multigrain can become:

- tuned percussion
- mallet voice
- kalimba-like line generator
- vocal chop melody source
- bell arp generator

### Best approach
- short, trimmed samples
- lower RATE
- smaller SIZE
- quantized PITCH modulation
- clear envelope shape
- restrained BLUR

This works especially well for:
- plucks
- pointillist melodies
- glitch-pop lines
- percussive ostinatos

---

# Multigrain as a harmonic counterpoint generator

A very strong advanced use is to derive **countermelodies** from existing material.

## Method
Feed in or sample:
- a vocal phrase
- a pad chord
- a lead line
- a sustained instrument note

Then:
- retune it with quantized pitch CV
- isolate different parts with START/WRAP
- use scene morphing for articulation changes
- select different sounds for contrasting phrase fragments

### Result
Instead of writing a second voice from scratch, you generate one from related material, which often sounds more cohesive.

This is one of the nicest compositional uses of Multigrain.

---

# Strong melodic workflows

## Workflow 1: Granular lead
- One pitched sample
- X = pitch CV
- GATE = note trigger
- Quantizer on
- Morph for expression

## Workflow 2: Sample-orchestrated melody
- Several sounds, each with different articulation/sample
- SELECT or NEXT changes timbre
- One shared pitch source

## Workflow 3: Harmonic clouds
- Chord or choir samples
- Pitch sequenced and quantized
- Long size, moderate blur
- Scene morphing for density

## Workflow 4: Vocal chop instrument
- Record or load vocal phrase
- Use START/WRAP/SCAN to isolate regions
- Pitch-sequence via X/Y/Z
- Quantize to scale

## Workflow 5: Live harmonizer texture
- Live input as source
- Freeze loop
- Play it melodically with quantized pitch CV

---

# Limitations to be aware of for melody

Multigrain is excellent for melodic material, but it is not a perfect substitute for a dedicated oscillator voice.

## Things to keep in mind
- Pitch depends heavily on source material
- Some samples won’t transpose musically across wide ranges
- Granular behavior can reduce note definition if RATE/SIZE are too extreme
- Too much SCAN/WRAP/randomization can make pitch identity vague
- Blur can smear fast lines

So if you want very clear melody:
- choose clean samples
- tune carefully
- use quantizer
- keep grain parameters conservative at first

Then expand into more experimental settings.

---

# Best companion module types for melodic use

If you're asking how this module can be used “together” with other Eurorack tools, Multigrain pairs especially well with:

## Sequencers
For pitch CV into X/Y/Z and gates into GATE.

## Quantized CV sources
Even though it has its own quantizer, external quantized modulation can also be useful.

## Envelope generators
For dynamic MORPH control.

## Clocks / trigger generators
To sync grain rhythm and stepping through sounds.

## Audio sources / oscillators / samplers
For Live Sound input and resampling.

## Mixers / VCAs / filters
To shape Multigrain like a full voice in a patch.

## Reverb / delay / spatial tools
Though Blur exists, external effects can widen melodic context further.

---

# Bottom line

The **Intellijel Multigrain** is a highly capable **melodic sound source**, especially if you think of it as a **granular instrument** rather than just a sampler.

Its strongest melodic assets are:

- **pitch control with CV**
- **built-in quantizer**
- **fine tuning**
- **sound selection by CV**
- **scene morphing**
- **live/sample hybrid sources**
- **expressive control over grain identity**

It excels at:

- granular leads
- harmonic textures
- melodic chops
- tuned percussive lines
- evolving sample-based phrases
- live-derived melodic resynthesis

If I were using it in a melodic patch, I would most often treat it as one of these three things:

1. **A quantized granular lead voice**
2. **A bank of timbrally shifting melodic articulations**
3. **A harmonic/countermelodic texture generator derived from recorded material**

If you want, I can also turn this into:
- a **set of concrete patch recipes**
- a **“best companion modules” guide**
- or a **melodic use cheat sheet** for Multigrain.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)