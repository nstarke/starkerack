# Black Noise — Cosmos

- [Manual PDF](../../manuals/BLACK-NOISE_COSMOS_User-Manual_V1.pdf)

---

[Cosmos User Manual (PDF)](contact@blacknoisemodular.com)

# Black Noise Cosmos: using it to create melodic components

Cosmos is unusually good at **turning simple voltages and waveforms into pitch-related musical material**. It is not just a logic module: it can behave like a **comparator, rectifier, octave doubler, oscillator, wave shaper, PLL, envelope utility, random gate source, and clock processor**. That makes it very useful for building melodic systems out of a small Eurorack setup.

Below is a musician-focused guide to using Cosmos to create **melodies, tuned voices, pitch motion, rhythmic melody triggers, and harmonic variation**.

---

## What Cosmos does best for melody

At a high level, Cosmos helps melodic patching in 5 main ways:

1. **Generate or derive oscillators**
   - Self-patched oscillator
   - Triangle-to-+1 octave voice
   - PLL-based tracking oscillator
   - Looping envelope as oscillator

2. **Shape timbre while preserving pitch relationships**
   - Saw to triangle
   - Variable pulse width from triangle/saw
   - Harmonic wave shaping
   - Clamping ring modulation / AM-RM hybrids

3. **Extract gates and triggers from CV/audio**
   - Comparators and window comparators
   - Rising/falling edge trigger extraction
   - Clock doubling and trigger multiplying

4. **Combine modulation sources into pitch-useful control**
   - Min / Max analog logic for envelope combining
   - Offset-controlled thresholds for note articulation
   - Envelope following for pitch-adjacent response

5. **Create musically useful probabilistic phrasing**
   - Random gate routing
   - Swinged doubled clocks
   - Delayed trigger multiplication

---

## Core melodic building blocks from the manual

## 1. Use Cosmos as a pitch-related oscillator

The manual shows that Cosmos can become a **self-oscillating square source** by feeding the **XNOR gate back to an input**.

### Why this matters musically
This gives you a raw pitched tone source. If you place a **slew or filter in the feedback path**, you gain control over frequency, and with CV over the slew time, you get a kind of **VCO-like voice**.

### Patch concept
- Patch **XNOR gate output** back to one input
- Insert a **slew limiter or LPF** in the loop
- Modulate slew time from:
  - sequencer CV
  - keyboard CV
  - envelope
  - another LFO

### Musical use
- Add as a **second oscillator** for a lead or bass
- Use as a **substitution voice** when your system is small
- Sequence the slew for stepped melodic lines
- Mix with a more stable VCO for grit and edge

### Character
This is not a precision VCO first; it is an **analog-computer-style oscillator**. Best for:
- raw melodic lines
- dirty basses
- unstable harmonics
- pseudo-digital square sequences

---

## 2. Create a melody-supporting octave layer

One of the strongest melodic tricks in the manual is:

## Triangle wave to +1 octave VCO

Patch a **bipolar triangle** into Cosmos, then patch the **corresponding inverted output** back into the second input. The **MAX output** becomes a signal **one octave higher**. The **OR gate output** becomes a square-wave version.

### Why this matters musically
This is excellent for making a single oscillator feel like a composed melodic voice:
- root + octave
- mellow + bright layer
- triangle + pulse hybrid

### Musical applications
- Add the octave-up output quietly under a bassline
- Use the OR gate output as a pulse layer for articulation
- Process the octave-up separately through a VCA/filter
- Create a two-register lead from one VCO

### Nice performance trick
The manual notes that adding **offset** creates a **sync-like sweep**. That means you can animate the octave relation with:
- an envelope for attack brightness
- an LFO for animated lead lines
- sequencer CV for phrase-dependent harmonic changes

This is one of the best ways in the manual to get a **melodically useful harmonically rich voice from a single VCO**.

---

## 3. Convert triangle or saw to pulse for melodic articulation

## Triangle or saw to variable pulse width

Using Cosmos as a comparator:
- send triangle or saw through an **offset**
- patch into a Cosmos input
- use the **OR gate output** as the resulting pulse wave

### Why this matters musically
Pulse width is one of the most classic melodic timbre tools. With this patch you can:
- derive a pulse voice from a non-pulse oscillator
- animate the harmonic content without losing pitch tracking
- create PWM-like leads and basses

### Good melodic uses
- Slow LFO to offset input = evolving pulse width
- Envelope to offset input = brighter attack
- Sequencer CV to offset input = different timbre per note
- Mix original triangle with pulse for richer melody tone

### Best in a patch with
- VCF after mixing
- VCA under envelope
- sequenced V/oct source into the original VCO

This turns Cosmos into a **melody timbre animator**.

---

## 4. Turn saw into triangle or “shark tooth” for melodic tone design

## Saw wave to triangle wave

Using full-wave rectification:
- patch bipolar saw into X
- patch inverted version to Y
- use **MAX output** as triangle-like output

With offset, the manual says you can get in-between shapes like **“shark tooth”**, similar to classic Minimoog-style timbral territory.

### Musical use
This is useful when you want:
- smoother lead tones from a brighter oscillator
- a more rounded melodic waveform
- filter-like movement from CV-controlled offset

### Why it’s melodic
Because the pitch source stays the same, the harmonic shape changes while **the note identity remains stable**. That’s ideal for:
- expressive monophonic leads
- basses that need controlled brightness
- melodic phrases with timbral contour

---

## 5. Use harmonic wave shaping for animated lead lines

## Harmonic wave shaper

This patch combines:
- oscillator into X
- TZ clipper gate through slew
- negative offset
- result patched to Y
- output from TZ clipper

### Why this matters
This is effectively a **harmonic enrichment engine**. The manual describes results close to:
- wavefolding
- sync-like tones
- asymmetric shaping

### Musical role
Perfect for:
- lead lines that need motion
- acid-adjacent melodic voices
- harmonically evolving arps
- aggressive counter-melodies

### Controls that matter musically
- **Rise**: smoothness of added harmonics
- **Fall**: number of harmonics
- **Negative offset**: intensity of shaping

### Melodic strategy
Use this after you already have a stable pitch source. Then:
- modulate Fall slowly for phrase movement
- use envelope on offset for attack harmonics
- use sequencer row or random CV to change harmonic density per note

This is one of the most useful “make melody more alive” patches in the manual.

---

## 6. Build tracked doubled voices with the PLL patches

The manual includes three especially melodic PLL applications.

## Phase locked loop: VCO tracking

Patch:
- main sequenced VCO into Cosmos
- second VCO into Cosmos
- Inv. TZ clip out through slew/filter
- back into FM or V/oct of second VCO

### Musical result
A second oscillator **locks and tracks** the main one over a few octaves. The result is described as close to **PWM-like** tonal behavior.

### Why this is excellent for melody
This gives you a melodic voice with:
- stable note relationship
- moving phase interaction
- sync-like complexity
- richer harmonics than simple detune

### Best use cases
- dual-osc lead
- thicker melody line
- animated bass doubling
- pseudo-sync solo timbre

---

## Phase locked loop: looping envelope

This is one of the coolest melodic tricks in the manual.

A **looping envelope** becomes an audio-rate oscillator and is made to **track a VCO** through the same PLL idea.

### Musical use
This lets you create a second voice with a very different shape than a normal VCO:
- buzzy
- snappy
- envelope-shaped
- sync-sweep capable

This is especially good for:
- expressive melodic leads
- unusual paired voices
- bright top layer above a root oscillator

---

## Phase locked loop: external tracking

An external audio source can drive the tracking behavior:
- guitar
- synth
- voice

### Melodic implications
If you feed a simple pitched source, Cosmos can help create **resynthesized melodic doubling**. This is useful if you want:
- voice-controlled synth melody
- guitar-doubled melodic line
- pitched external sound converted into modular melody material

---

## 7. Use comparators to derive melodic structure from pitch CV

Cosmos is great at creating gates from voltages.

## Comparator

The **OR gate** acts as an **over-zero comparator**. Offset the source first, and you can define a threshold.

### Melodic uses
Feed in:
- sequencer CV
- quantized pitch CV
- LFO
- envelope

Then generate a gate when the signal exceeds a chosen level.

### Why this is musically useful
You can create:
- note accents only on higher notes
- transposition-dependent triggers
- phrase changes when pitch passes a threshold
- melody-conditioned gate routing

Example:
- Sequencer pitch CV to comparator
- Threshold set so only upper half of melody opens a second VCA
- Result: higher notes gain a second oscillator or more brightness

That is a very musical patch.

---

## Window comparator

The window comparator gives a gate when a signal lies **within a range**.

### Melodic uses
Apply it to pitch CV or sequencer output:
- only notes near a selected register trigger an event
- create a gate when melody hits a chosen pitch zone
- use very narrow width as an approximate “equal note” detector

### Great musical applications
- Add vibrato only for notes in a chosen range
- Trigger a secondary envelope only on certain notes
- Send a harmony layer only when melody lands near target voltage
- Create a repeating motif emphasis from continuous CV

This is one of the most composition-friendly features in the manual.

---

## 8. Build melodic rhythms with random gates

## Random Gates

This patch uses:
- a clock into X
- buffered clock to trigger random sample & hold
- S&H voltage into Y through offset
- XOR and AND outputs become randomly alternating rhythms

### Why this helps melody
Melody is not just pitch; it is also **when notes happen**. This patch gives you:
- probabilistic note triggers
- A/B trigger routing
- dynamic phrase generation

### How to use melodically
Route the different outputs to:
- different envelopes on the same voice
- two different VCAs
- separate quantizers or sequential switches
- different transposition events

Example:
- XOR triggers bass notes
- AND triggers higher accent notes
- OR trigger clocks a transposition or ornament

Now Cosmos is creating **melodic phrasing logic**, not just rhythm.

---

## 9. Double clocks and triggers for ornamented melodies

## Clock multiplier with swing
Mix **OR and NOR triggers** from a pulse source to get doubled timing with adjustable swing.

## Trigger multiplier with delay
Send a trigger through slew, then mix edge-derived triggers for a doubled trigger stream with controllable delay.

### Melodic uses
These are very good for:
- ratchets
- grace notes
- repeated note ornaments
- off-beat melodic echoes
- arpeggio enrichment

### Example patch
- Main sequencer clock to Cosmos
- Doubled/swinged triggers clock an envelope or strike a LPG
- Pitch stays steady while trigger density increases

Or:
- Use original clock for pitch advance
- Use doubled trigger stream to retrigger envelope between steps
- Result: repeated notes from one pitch step

That is a classic way to make melodies feel more alive.

---

## 10. Use envelope utilities to shape melodic phrasing

## Envelope to LFO

An envelope can self-loop by retriggering from the **NOR gate**.

### Melodic use
Create a tempo-related modulation source for:
- vibrato
- PWM
- wave-shaping animation
- pitch wobble
- filter movement tied to phrase behavior

---

## Envelope combiner

Patch two envelopes into Cosmos and use **MIN** and **MAX** outputs as combined envelopes.

### Why this matters for melody
Better melodic articulation often comes from more interesting amplitude/filter contours than from pitch alone.

### Musical uses
- Short attack envelope + longer slewed gate = ADSR-like contour
- Two different attacks = double-hit or “clap-like” articulation
- Decay envelope + fast LFO = burst-like ornament envelope

Use these envelopes to control:
- VCA
- filter cutoff
- wave-shaping depth
- PWM amount
- FM depth

This is a strong way to make a melody feel “played” rather than just sequenced.

---

## 11. Use envelope follower for audio-driven melody behavior

## Envelope follower

Audio into X, inverted version into Y, MAX to slew = a CV following audio dynamics.

### Melodic applications
If another performer or sound source exists, you can derive expressive control to influence melody:
- vocalist amplitude opens VCA on a melodic synth
- guitar dynamics increase harmonic shaping
- drum loop envelope transposes or accents melody

This is indirect melody generation, but very musical.

---

# Best ways to use Cosmos with other modules for melodic music

The manual repeatedly points to two especially important companion module types:

## 1. Slew limiter
Essential with Cosmos for:
- oscillator frequency control
- feedback loop timing
- trigger delay
- smoothing extracted CV
- PLL tuning
- envelope following

For melody, a slew becomes:
- glide
- oscillator core control
- rhythm ornament timing
- phrase smoothing

## 2. Offset / attenuator / attenuverter
Essential for:
- setting comparator thresholds
- pulse width position
- harmonic shaper depth
- window comparator range
- manual melodic bias
- CV scaling

For melody, offset is what makes Cosmos behave compositionally instead of just reactively.

---

# Practical melodic patch recipes

## Patch 1: One-VCO melodic lead with octave shimmer
Use:
- VCO triangle out
- Cosmos triangle-to-+1 octave patch
- Mix original + octave-up
- Envelope to VCA
- Optional offset modulation for sync-like brightness

Result:
- a compact lead voice with natural top-end lift

---

## Patch 2: PWM bass voice from a triangle oscillator
Use:
- sequenced VCO triangle into offset into Cosmos
- OR gate output as pulse voice
- slow LFO or envelope to offset CV
- lowpass filter + VCA

Result:
- animated bass with stable pitch and moving harmonics

---

## Patch 3: Melody-conditioned accent layer
Use:
- quantized pitch CV into comparator
- threshold set so only high notes produce gate
- gate opens second VCA or extra oscillator layer

Result:
- automatic accents only on high notes of the melody

---

## Patch 4: Note-zone triggered harmony
Use:
- sequencer CV into window comparator
- when melody enters chosen voltage range, trigger:
  - transposition
  - second envelope
  - second oscillator VCA
  - wave-shaper depth

Result:
- specific notes or ranges in the melody get harmonic decoration

---

## Patch 5: PLL dual-oscillator solo voice
Use:
- master VCO from sequencer
- second VCO through PLL tracking patch
- slight slew tuning
- mix the two voices

Result:
- thick, animated lead with sync/PWM-like behavior

---

## Patch 6: Random melodic phrasing engine
Use:
- master clock into random gates patch
- XOR triggers main envelope
- AND triggers accent envelope
- OR trigger clocks a transposition event or ornament

Result:
- repeating but non-static melody phrasing

---

## Patch 7: Ornament generator
Use:
- trigger multiplier with delay
- original sequencer trigger advances pitch
- multiplied trigger retriggers same pitch before next step

Result:
- grace notes, ratchets, repeated-note ornaments

---

## Patch 8: Audio-reactive melodic voice
Use:
- external audio to envelope follower
- follower controls:
  - harmonic shaper amount
  - VCA level
  - filter cutoff
  - comparator threshold

Result:
- melody line dynamically follows another performer or sound source

---

# Strongest melodic features in Cosmos

If your goal is specifically melodic music, the most valuable features from the manual are:

1. **Triangle to +1 octave VCO**
2. **Triangle/saw to variable pulse width**
3. **PLL VCO tracking**
4. **Harmonic wave shaper**
5. **Comparator / window comparator**
6. **Random gates**
7. **Clock multiplier with swing**
8. **Trigger multiplier with delay**
9. **Envelope combiner**

Together, these cover:
- pitch generation
- harmonic layering
- note-dependent events
- melodic ornamentation
- phrase variation

---

# Suggested small-system melodic setup around Cosmos

If building a compact melodic rig with Cosmos, pair it with:

- **1 stable VCO**
- **1 slew limiter**
- **1 offset/attenuverter**
- **1 envelope**
- **1 VCA**
- **1 filter**
- **1 mixer**
- **1 random source / S&H**
- **1 sequencer or quantized CV source**

With just that, Cosmos can supply:
- extra oscillator behavior
- octave doubling
- PWM derivation
- comparators
- rhythmic phrase logic
- harmonic animation
- melodic trigger processing

---

# Summary

Cosmos is best thought of as a **melodic analog processor and patch-programmable music logic core**.

It helps create melodic components by letting you:

- derive **new pitched voices** from existing ones
- add **octaves, pulse versions, and sync-like harmonics**
- make **dual-oscillator tracked textures**
- create **note-conditioned gates** with comparators
- generate **probabilistic note rhythms**
- add **swing, retriggers, ratchets, and delayed ornaments**
- shape phrasing with **combined envelopes and audio-following control**

In a melodic Eurorack patch, Cosmos is not usually the “main sequencer,” but it can absolutely become the **main intelligence that turns simple pitch and timing into expressive musical structure**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)