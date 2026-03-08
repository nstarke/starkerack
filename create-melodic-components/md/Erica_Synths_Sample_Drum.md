# Erica Synths — Sample Drum

- [Manual PDF](../../manuals/FINAL_sample_drum_instrukcija_A4.pdf)

---

[Erica Synths Sample Drum Manual (PDF)](https://www.ericasynths.lv/media/SampleDrum_manual_v1.1.pdf)

# Erica Synths Sample Drum: creating melodic components in a Eurorack patch

The attached manual is for the **Erica Synths Sample Drum**, a dual sample player/recorder with slicing, CV control, envelopes, effects, and **1V/Oct tracking**. Even though it’s often used for drums, it can be very effective for **melodic work**.

## What matters most for melody

From the manual, these features are the key melodic tools:

- **Two simultaneous sample players**
- **1V/Oct tracking** over **C0–C8**
- **Per-channel sample selection**
- **Start / Loop / End control**
- **Automatic and manual slicing**
- **AD envelope + level control**
- **Assignable CV inputs per channel**
- **Realtime FX**
- **Recording and saving your own samples**
- **Project recall for live performance**

This means Sample Drum can function as:

- a **pitched sample voice**
- a **wavetable-like oscillator substitute**
- a **loop-based melodic phrase player**
- a **granular-ish texture voice** using slices and CV
- a **dual melodic sampler** for counterpoint, chords-by-layering, or call/response

---

## Important operating constraints

Before patching melodically, note these limitations and strengths from the manual:

### Sample format / memory
- Samples are loaded into RAM for instant playback
- Supported format: **WAV, mono, 48kHz, 16-bit**
- Lower sample rates also work and are interpolated
- Shared RAM: **32MB total**, about **5 minutes**
- Both channels share the same RAM pool

### Channel architecture
- There are **2 identical sample channels**
- Each channel has:
  - trigger input
  - 3 CV inputs
  - one audio output
- Channel 2’s **CV3** is also used as the **recording input**

### Tuning behavior
- The module supports **1V/Oct**
- Tune is set relative to the original sample pitch
- **Tuning is global per channel**
- Other settings are generally stored per sample/project context

That “global to channel” tuning point is important: if you switch between samples on one channel, your tuning setup affects that whole channel.

---

# Best ways to use Sample Drum for melodic parts

## 1. Use it as a pitched one-shot instrument

This is the most direct melodic use.

### Patch idea
- Send a sequencer’s **pitch CV** to one CV input
- In the **CV Assign menu**, assign that CV to **SMP: TUNE**
- Set that CV input range to **1V/Oct**
- Send gates/triggers from your sequencer to **TRIG 1** or **TRIG 2**
- Load a sample with a clear pitch:
  - sine hit
  - pluck
  - vocal tone
  - mallet
  - sampled analog wave
  - single-cycle-ish waveform with body

### Why it works
Each trigger restarts the sample, and the pitch CV transposes it chromatically. This turns the Sample Drum into a kind of **digital sample oscillator**.

### Good source samples
Best melodic results usually come from:
- short, harmonically simple samples
- loopable sustained tones
- plucks with strong fundamental
- single notes from acoustic instruments
- resampled synth notes

### Tips
- Use **forward** mode for standard playback
- Set **Start/End** tightly to remove silence
- In the **Amplitude** menu, shape attack/decay to make it behave like a synth voice
- Assign CV to **AMP: LEVEL** if you want velocity-like dynamics

---

## 2. Make a sustained melodic voice with looping

Because the module has **Start / Loop / End** controls and loop modes, you can turn a sample into a sustained instrument.

### Setup
- Load a pitched sample with a stable middle section
- In the Sample menu, choose **forward loop**
- Set:
  - **Start** at the transient or just after it
  - **Loop** around a stable waveform region
  - **End** at the tail
- Tune via **1V/Oct**

### Result
You get something closer to a **sampled oscillator with sustain** than a one-shot.

### Best use cases
- pads
- drones
- bass tones
- vocal sustain
- string-like tones

### Envelope strategy
Use the **Amplitude** menu:
- **short attack** for plucks
- **longer attack/decay** for pads
- in loop mode, **Decay defines fadeout**
- for effectively infinite sustain, the manual notes decay defaults to **100**

This is one of the strongest melodic tricks in the module: finding a loopable center in a sample and sequencing pitch like an oscillator.

---

## 3. Build a two-voice melodic instrument

Because Sample Drum has **two simultaneous channels**, you can create a compact melodic pair.

### Common pairings
- **bass + lead**
- **lead + harmony**
- **melody + drone**
- **pluck + texture**
- **root note + fifth/octave layer**

### Patch structure
- Channel 1:
  - 1V/Oct melody line
  - short envelope
- Channel 2:
  - same sequence transposed elsewhere, or a different sequence
  - slower envelope or different sample
- Mix outputs externally

### Musical uses
- parallel intervals
- octave doubling
- antiphonal phrases
- pseudo-polyphony by alternating notes between channels
- layered timbres for a single melodic line

If your sequencer can output two pitch/gate tracks, this becomes a very playable **dual digital voice**.

---

## 4. Sequence slices chromatically or rhythmically as melodic material

The slicing functions are not only for breakbeats. They’re excellent for melody if your source sample contains **pitched segments**.

## Automatic slicing
The module can slice a sample:
- **1 to 32 slices**
- by **linear** spacing
- or near **zero crossings**

## Manual slicing
You can:
- zoom in
- add slice markers
- move them precisely
- remove them

### Melodic applications
#### A. Slice a phrase of individual notes
Record or load:
- a scale
- arpeggio
- vocal phrase
- multisampled notes

Then manually slice each note.

Assign CV to:
- **SLICE: INDEX**
- set CV range to **1V/Oct** if desired

Now different voltages can select different note slices, while triggers fire them.

This gives you a kind of **addressable note bank**.

#### B. Use a single melodic phrase as a sequenced ornament source
Load a phrase and slice it into pieces. Then:
- trigger slices in **FWD**
- **BKW**
- **RND**
- or **CV** playback mode

This can create:
- glitch melodies
- micro-arpeggios
- phrase scrambling
- generative melodic fragments

#### C. Clock-synced loop repitching
The manual specifically suggests slicing a 1-bar loop into 16 slices and triggering each slice per clock tick. If that loop is tonal, it becomes:
- a synced melodic ostinato
- a stuttered harmonic phrase
- a controllable motif source

---

## 5. Use CV-controlled sample selection for melodic timbre switching

A less obvious melodic technique is assigning a CV input to **SMP: SAMPLE**.

### Why this is interesting
Instead of changing pitch only, you can change which sample plays at each note.

For example, load:
- different single notes
- different articulations
- different oscillator waveforms
- different vowel samples
- different chord stabs

Then sequence sample selection with CV.

### Results
- timbral melody
- pseudo-round-robin articulation
- note-dependent multisampling
- wavetable-like scan through sample slots

The manual notes:
- in **1V/Oct** mode with **SMP: SAMPLE**, **64 samples** are selected with 64 notes starting from C-0

That means a pitch sequencer can effectively become an **index selector** for a bank of samples.

### Advanced approach
Use one CV for:
- **sample select**
and another for:
- **tune**

Then you can choose a source sample while separately transposing it.

This is especially powerful for building **sampled scales** or **wavetable-style melodic morphs**.

---

## 6. Create melodic percussion and tuned drums

Since the Sample Drum is designed for fast triggering, it excels at:
- tom melodies
- tuned kicks
- tuned blips
- FM-ish percussion samples
- pitched noise hits

### Patch idea
- Load short drum/transient samples with tonal body
- Sequence them with **1V/Oct**
- Use short decay envelopes
- Add FX like delay or reverb for space

### Great musical roles
- techno bass riffs from pitched kicks
- electro tom lines
- tuned percussion arps
- metallic melodic accents
- IDM-style micro-melodies

This is one of the most natural melodic uses for the module in a Eurorack context.

---

## 7. Record your own oscillator or synth into it, then play melodically

The **recording** function makes it easy to turn the rest of your system into source material.

### Recording notes from another module
You can sample:
- an analog oscillator
- a full synth patch
- external synths
- field recordings
- vocals

Record into **CV3/REC** on channel 2’s lower CV3 input.

### Why this matters musically
You can capture:
- one note from an oscillator
- a filtered chord stab
- a complex FM tone
- a resonant sweep
- a pluck from elsewhere in your rack

Then replay it as a **pitched melodic voice** using 1V/Oct.

This is great for:
- freezing a patch into a playable instrument
- saving RAM by using one source note and transposing
- creating custom digital voices from your analog system

### Practical strategy
1. Patch an oscillator or complete synth voice into the recorder
2. Record a stable note
3. Trim tightly
4. Set loop points if sustain is desired
5. Assign 1V/Oct to tune
6. Sequence triggers and melody

That effectively turns Sample Drum into a **custom sampler-oscillator** made from your own rack.

---

## 8. Use envelopes to make the sample behave like a synth voice

The **Amplitude** menu is critical if you want convincing melodic behavior.

Available controls include:
- Attack
- Hold
- Decay
- Attack shape
- Decay shape
- Range: **Short / Mid / Long / Relative**

### For melodic synth-like use
#### Plucks
- short attack
- moderate hold
- short/medium decay
- exponential decay shape

#### Pads
- slower attack
- longer hold
- long decay
- log or linear shapes

#### Sequence-friendly bass
- very fast attack
- low hold
- medium decay
- keep sample start tight

#### Slice-based melodic phrases
Use **Relative** mode. The manual says this mode automatically adapts envelope timing to the sample or slice length, which is especially useful when changing the number of slices.

This is useful because melodic slices can otherwise become too choked or too long.

---

## 9. Use effects to turn static melodic samples into expressive voices

The built-in FX are:

- Delay
- Reverb
- Lowpass filter
- Highpass filter
- Bitcrush
- Fold
- Drive
- None

Each effect has three parameters and can be CV controlled.

### Melodic use cases
#### Delay
- dubby lead lines
- widening sparse melodies
- pseudo-polyphonic repeats

#### Reverb
- ambient one-shots
- pad extension
- vocal wash

#### Lowpass / Highpass
- animated filter sweeps
- dynamic articulation
- note brightness modulation

#### Bitcrush / Fold / Drive
- gritty digital leads
- aggressive bass
- lo-fi arpeggios
- evolving harmonic color

### Strong performance patch
Assign one CV or one performance encoder to:
- **FX: PARAM1**
- **FX: MIX**
- **FX: TYPE**

Then your melodic voice can shift from clean pluck to distorted lead to filtered texture live.

---

## 10. Use Performance mode as a playable melodic macro interface

Performance mode is especially useful if you want the Sample Drum to function as a real instrument in a live patch.

### What it does
You can assign the six encoders:
- A/B/C to channel 1
- D/E/F to channel 2

Each can be mapped to a parameter for live control.

### Great melodic assignments
For a lead voice:
- Encoder A: **TUNE**
- Encoder B: **SAMPLE**
- Encoder C: **DECAY**

For a second voice:
- Encoder D: **TUNE**
- Encoder E: **LEVEL**
- Encoder F: **FX PARAM1**

That lets you perform:
- transposition
- timbre switching
- envelope articulation
- dynamic FX sweeps

For live melodic music, this is one of the best features in the module.

---

# Concrete melodic patch ideas

## Patch 1: Sampled lead synth
**Goal:** use Sample Drum like a monophonic lead voice.

### Setup
- Load a bright synth note sample
- Set playback to **forward**
- Trim Start/End tightly
- Assign CV1 → **SMP: TUNE**
- Set CV1 range to **1V/Oct**
- Trigger from gate sequencer into TRIG1
- Shape envelope with short attack, medium decay
- Add a little reverb or delay

### Result
A clean melodic lead voice with instant trigger response.

---

## Patch 2: Looping bass oscillator
**Goal:** sustained bassline from a sampled waveform.

### Setup
- Record or load a bass tone
- Set mode to **forward loop**
- Find a stable loop region
- Assign pitch CV to **SMP: TUNE**
- Use short attack, medium hold, longer decay
- Optional: assign CV2 to **FX: PARAM1** if using lowpass filter
- Trigger from bass sequence

### Result
A playable bass voice that behaves much like a digital oscillator.

---

## Patch 3: Addressable scale from note slices
**Goal:** create a melodic note bank from one sample file.

### Setup
- Make a WAV containing separate notes of a scale
- Load it
- Enter manual slicing and slice each note
- Assign CV input to **SLICE: INDEX**
- Set CV range to **1V/Oct**
- Feed pitch sequence into slice index
- Feed rhythm/gates into trigger input

### Result
Each incoming note selects a different slice, so one long file becomes a playable note set.

This is excellent for:
- vocal chops
- mallet scales
- multisampled instruments
- spoken-word melodies

---

## Patch 4: Generative melodic texture
**Goal:** semi-random melodic motion.

### Setup
- Load a tonal loop or phrase
- Slice it into 8–16 pieces
- Set slice playback mode to **RND**
- Trigger with clock or probabilistic triggers
- Assign CV to:
  - **START** or **LOOP**
  - or **FX MIX**
- Use reverb/delay

### Result
A generative melodic texture source, ideal for ambient, experimental, and IDM patches.

---

## Patch 5: Two-channel harmony instrument
**Goal:** use both channels as a duet.

### Setup
- Channel 1: plucked sample, 1V/Oct melody
- Channel 2: sustained or softer sample, harmony line
- Different envelopes on each
- Slightly different FX on each
- Use external mixer/pan for width

### Result
A compact two-voice melodic system with contrast and movement.

---

## Patch 6: Sample-scan wavetable-style melody
**Goal:** emulate wavetable movement through sample slots.

### Setup
- Load many related waveform samples or resampled synth tones
- Assign a CV input to **SMP: SAMPLE**
- Sequence or modulate sample selection
- Optionally also assign another CV to **TUNE**
- Trigger per note

### Result
Each note can call a different timbre, making melodies morph as they play.

---

# Best companion modules for melodic use

Since you asked how modules can be used together: with the Sample Drum, the most useful companion module types are:

## Pitch sequencers
Anything that outputs precise **1V/Oct CV + gate**
- step sequencers
- keyboard controllers
- quantizers with CV sources

These are essential if you want stable melodies.

## Envelope and modulation sources
Although Sample Drum has internal envelopes, extra modulation helps for:
- sample select
- loop point
- effect mix
- slice index

## Clock / trigger sources
For slice playback and phrase sequencing:
- clocks
- trigger sequencers
- ratchets
- probability triggers

## Mixers / VCAs / filters
The Sample Drum can act as a complete voice, but external processing adds a lot:
- VCA for final articulation
- analog filter for warmth
- stereo FX for space
- mixer for balancing the two outputs

## Quantized CV sources
Very useful if you want:
- slice index melodies
- sample selection by note
- harmonic transposition

---

# Especially powerful melodic strategies

## Strategy 1: multisample your own synth
Sample several notes or articulations from another oscillator/filter chain, load them as separate files, then use:
- **SMP: SAMPLE**
- **SMP: TUNE**
to build a custom melodic instrument.

## Strategy 2: vocal melody machine
Record sung vowels or spoken syllables, slice them, and control:
- slice index
- tune
- FX
for highly expressive vocal melodies.

## Strategy 3: loop-to-lead conversion
Take a longer musical sample, isolate a tiny stable portion with loop points, and convert it into a playable sustained lead or pad.

## Strategy 4: dual-register arrangement
Use channel 1 for low register bass ostinato, and channel 2 for upper melody or harmonic punctuation.

---

# Things to watch out for

## 1. Tuning quality depends on the source sample
Pitch tracking works, but some samples transpose better than others. Clean, harmonically stable material usually gives the most musical results.

## 2. Tuning is channel-global
If you rely on radically different source samples on one channel, be aware that tuning behavior is shared at the channel level.

## 3. Shared RAM
Because both channels share the same 32MB, long multisample sets can fill memory quickly.

## 4. Triggered architecture
This is a trigger-oriented sample player, not a traditional sustained keyboard sampler. For long-note melodic playing, looping and envelope setup matter a lot.

## 5. CV assignment planning matters
Each of the three CV inputs per channel is valuable. For melody, a smart default is often:
- CV1 = Tune
- CV2 = Sample or Slice Index
- CV3 = Level / FX / Start / Loop

---

# My recommended melodic setups

## Minimal melodic voice
- Trigger in
- 1V/Oct to Tune
- Short sampled waveform
- Envelope shaped internally
- Reverb on board

## Expressive lead voice
- CV1 = Tune
- CV2 = Level
- CV3 = FX Param or Start
- Manual performance encoder control for sample select/decay

## Phrase-based melodic instrument
- One long file containing notes or syllables
- Manual slices
- CV controls slice index
- Trigger sequencer clocks playback

## Full two-voice arrangement
- Ch1: bass or arp
- Ch2: lead or chord stab
- Different FX and envelopes
- Project saved for instant recall live

---

# Summary

The **Erica Synths Sample Drum** can absolutely be used as a melodic Eurorack instrument, not just a drum module. Its strongest melodic roles are:

- **pitched sample oscillator via 1V/Oct**
- **looped sustained voice**
- **dual melodic sampler**
- **slice-addressed note bank**
- **timbrally shifting sample-scan voice**
- **resampled custom instrument from your own rack**

If you pair it with a good pitch/gate sequencer, clocks, and a mixer or filter, it becomes a very flexible melodic source for:
- basslines
- leads
- harmonies
- vocal chops
- generative melodic textures
- live performance sample instruments

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)