# Erica Synths — Octasource

- [Manual PDF](../../manuals/black_octasource_manual.pdf)

---

# [Erica Synths Black Octasource Manual (PDF)](https://www.ericasynths.lv/media/Black_Octasource_manual.pdf)

## Erica Synths Black Octasource: using it for melodic duties in a Eurorack patch

The attached manual is for the **Erica Synths Black Octasource**, an advanced multi-output LFO/modulation source. By itself, it is **not a sound source or quantizer**, so it does not directly generate “notes” in the traditional V/Oct sense unless you patch it cleverly into pitch destinations. But in a melodic Eurorack system, it can be extremely powerful as the **motion engine** behind melody, harmony, phrasing, and variation.

## What the module does musically

The Black Octasource provides:

- **8 simultaneous outputs**
- Either:
  - **one waveform phase-shifted across 8 outputs** in **SINGLE** mode, or
  - **8 different waveforms simultaneously** in **MULTI** mode
- **Rate control**
- **Clock sync**
- **Wave morphing**
- **CV control of wave selection**
- **CV control of phase distribution**
- **FM/rate modulation**
- **Freeze function** at 12 o’clock on the Rate knob

This means it works beautifully as a **central modulation hub** for:

- melodic pitch animation
- transposition
- interval generation
- call-and-response lines
- canon/round-like phase melodies
- harmonic movement across several voices
- clock-synced phrase development

---

## Core idea: how an LFO becomes melodic

A module like this becomes melodic when you patch its outputs to things such as:

- **VCO 1V/Oct inputs** for stepped or limited pitch movement
- **quantizer inputs**
- **sequential switch inputs**
- **precision adders / transposers**
- **filter cutoff** for pitch-tracked timbral melody
- **wavefolder / FM index / LPG CV** to create contour that feels melodic
- **envelope decay / VCA level** to shape phrase accents

If you have a **quantizer**, the Octasource becomes much more directly useful for melody. Without one, it still creates melodic contours, drones that move harmonically, or pseudo-melodies if attenuated carefully.

---

## Important functions from the manual

## 1. SINGLE mode: one waveform, 8 phase-shifted outputs

In **SINGLE** mode:

- all 8 outputs carry the **same waveform**
- each output is shifted in phase by **45 degrees**
- the **PHASE CV** input can alter the phase relationship

### Musical result
This is ideal for:

- **8 related melodic CV lines**
- staggered note events
- multi-voice canons
- harmonic swells where each oscillator or voice moves similarly but at different times

### Example melodic use
Patch:

- Output 1 → Quantizer A → VCO A 1V/Oct
- Output 3 → Quantizer B → VCO B 1V/Oct
- Output 5 → Quantizer C → VCO C 1V/Oct
- Output 7 → Quantizer D → VCO D 1V/Oct

Now all voices derive from the same shape, but each enters at a different point in the cycle. This creates:

- rotating chord tones
- arpeggio offsets
- melodic imitation between voices

If all voices are clocked by the same gate source, you get **phase-related counterpoint**.

---

## 2. MULTI mode: 8 different waveforms at once

In **MULTI** mode:

- all 8 outputs provide **different waveforms simultaneously**
- the **WAVE** knob shifts waveforms from one output to another

### Musical result
This is great when you want one module to supply:

- one CV for pitch
- one for transposition
- one for envelope time
- one for filter movement
- one for wavefold amount
- one for trigger probability or comparator input
- one for stereo movement
- one for sequence variation

### Example melodic use
Patch:

- Output 1 (sine-like) → quantizer → lead pitch
- Output 2 (triangle-ish) → quantizer → bass pitch
- Output 3 (pulse/S&H-like) → transposition CV for the lead
- Output 4 → filter cutoff on bass voice
- Output 5 → VCA CV attenuation of a second modulation source
- Output 6 → decay time on envelope
- Output 7 → FM index on lead oscillator
- Output 8 → effect send or stereo pan

Now the entire melodic patch evolves from a single synchronized source.

---

## 3. Wave morphing as melodic contour design

The manual lists these principal waves:

- sine
- ramp
- inverted absolute sine
- triangle
- pulse
- absolute sine
- saw
- sample & hold

And there are **in-between morphed waveforms**.

### Why this matters melodically
Wave shape strongly affects melodic feel:

- **Sine**: smooth, gliding, cyclic pitch movement
- **Triangle**: regular up/down scalar motion
- **Ramp / saw**: repeating rises or falls that feel sequencer-like
- **Pulse**: octave/interval jumps when quantized
- **S&H**: random melodies
- **Absolute-value shapes**: repeated mirrored phrases, useful for symmetrical melodies

A quantizer will turn these shapes into scales and note patterns. Even without a quantizer, attenuated waveforms can create subtle pitch inflection.

---

## 4. Clock sync for rhythmic melody

The **SYNC** input lets you synchronize the LFO to an external clock.

The manual notes:
- when synchronized, the **RATE** knob has no effect
- except at the **freeze** position

### Musical use
This is crucial for melodic composition because it ties modulation to tempo.

Patch a master clock into SYNC, then use Octasource outputs to drive:

- quantized pitch CV
- rhythmic transpositions
- filter accents
- phrase-length macro modulation

This gives you melodies that are:

- repeatable
- bar-aligned
- easy to layer with drums and sequencers

### Example
If your clock is 16th notes or a divided bar clock, Octasource can become a **phrase LFO**:

- one cycle per bar = melodic contour over one measure
- one cycle every 4 bars = slow harmonic drift
- one cycle per beat = rhythmic repeated pitch figure

---

## 5. Rate knob and freeze function

The large **RATE** knob behaves unusually:

- **12 o’clock** = **freeze**
- clockwise increases frequency and phase progresses **CW**
- counterclockwise increases frequency and phase progresses **CCW**

### Musical importance
The freeze function is excellent for melody performance.

If you are using Octasource to generate pitch-related CV, freezing the LFO effectively captures the current melodic/harmonic state. This lets you:

- hold a chord
- lock a transposition
- stop a melodic contour at a useful note cluster
- perform “pause” moments live

### Performance trick
Use Octasource outputs to control several quantized voices, then:
- let the modulation evolve
- set the Rate knob to 12 o’clock
- freeze the current voltages

You’ve now “sampled” a harmonic frame or chord voicing from a moving modulation field.

---

## 6. Phase CV for interval and voicing movement

The **PHASE CV** input changes the phase shift of each output.

Manual note:
- at **0V**, outputs are evenly shifted by **45 degrees**
- CV changes phase shift within a **45-degree window** for each output

### Musical use
This is one of the most interesting melodic features.

If several outputs are patched to:
- multiple quantizers
- multiple oscillators
- or pitch plus transposition destinations

then PHASE CV can dynamically alter the relationship between voices.

This can produce:

- changing voicings
- melody-to-harmony transformations
- widening/narrowing interval structures
- canon lines that tighten or spread apart

### Example patch
- Outputs 1–4 → four quantizers → four oscillators
- Common gate source to all envelopes
- Slow envelope or another LFO into **PHASE CV**

Result:
- The harmonic spacing between voices shifts over time
- The chord pattern breathes and reorganizes
- Voices feel related but not static

This is very effective for generative ambient melody.

---

## 7. Wave CV for melodic mutation

The **WAVE CV** input lets you control waveform selection with external CV.

### Musical use
If waveform determines melodic contour, then WAVE CV becomes a **meta-sequencer** for phrase shape.

For example:
- a slow envelope changes the waveform every phrase
- a random source nudges between triangle, pulse, and S&H areas
- one Octasource output self-patched into WAVE CV causes recursive motion

### Results
This can create:
- evolving motifs
- melody variation without changing the clock
- smooth-to-stepped phrase transitions
- controlled randomization

---

## 8. FM input and FM level: tempo and phrase modulation

The module has:
- **FM IN**
- **FM LEVEL** attenuator

This modulates the LFO rate.

### Musical use
When Octasource is driving pitch, modulating its speed changes how quickly melodic motion unfolds.

This is useful for:
- accelerando/ritardando-like pitch cycles
- phrase compression/expansion
- ratcheting feel if used with comparators or gates downstream
- making one melody line “push” another

### Example
- Envelope from your voice → FM IN
- Each note slightly modulates the Octasource speed
- The melodic modulation breathes with the performance

Or:
- clocked random → FM IN
- phrase length changes unpredictably but musically

---

## 9. Bipolar vs unipolar outputs

The manual says the Octasource defaults to **bipolar outputs**:
- **-5V to +5V**

It also supports **unipolar outputs**:
- **0V to +5V**

To switch:
- set **Rate** to **12 o’clock**
- flip **Multi/Single** switch **6 times**

LED behavior confirms the mode.

### Why this matters for melody
This is very important when patching to pitch.

- **Bipolar** output is useful for modulation around a center pitch
- **Unipolar** output is often easier for:
  - quantizers
  - transposition inputs
  - melodic sequencing
  - VCO pitch control with less unwanted downward swing

### Recommendation
For melodic CV:
- try **unipolar mode** first if going directly into quantizers or precision adders
- use **bipolar mode** for vibrato, centered pitch drift, or transposition around a root note

---

# Practical melodic patch ideas

## 1. Quantized rotating canon
Best with: 2–4 oscillators, quantizers, envelopes, VCA

Patch:
- Octasource in **SINGLE**
- Sync to master clock
- Outputs 1, 3, 5, 7 → quantizers → 1V/Oct on 4 oscillators
- Same gate pattern to all voices
- Mix voices in different octaves

Result:
- one shared contour
- different phase positions
- interlocking melodic lines

This sounds like:
- canon
- minimalist phase music
- rotating arpeggios

---

## 2. One-module harmonic ecosystem
Best with: one lead voice, one bass voice, one chord voice

Patch in **MULTI**:
- Out 1 → quantizer → lead pitch
- Out 2 → quantizer → bass pitch
- Out 3 → chord voice transposition
- Out 4 → lead filter cutoff
- Out 5 → bass envelope decay
- Out 6 → VCA level modulation on chord voice
- Out 7 → effect depth
- Out 8 → panning CV

Result:
- the whole musical system moves together
- melody and timbre stay related
- very coherent generative composition

---

## 3. Sample-and-hold melody source
Patch:
- Set waveform near **S&H**
- Output → quantizer → oscillator pitch
- Clock the voice separately with triggers/gates
- Sync Octasource to your master clock

Result:
- random but tempo-locked melodies
- with WAVE CV you can morph between random and smooth phrases

This is excellent for:
- Berlin-school lines
- ambient generative leads
- evolving acid-like motifs

---

## 4. Chord generator via multiple quantizers
Patch:
- SINGLE mode
- Outputs 1–4 → separate quantizers all set to same scale
- Quantizers → 4 oscillators
- Mix as a chord stack
- Slow CV into PHASE CV

Result:
- not fixed chords in the traditional sense, but moving scale-related harmonies
- can sound like suspended chord clouds or modal parallel motion

---

## 5. Transposition matrix
If you already have a sequencer:
- sequencer pitch CV → main oscillator
- Octasource output → precision adder or quantizer transpose input
- another Octasource output → filter cutoff
- another → envelope decay

Result:
- your existing melody gets periodic or evolving transposition
- phrase-level structure emerges from the LFO network

This is one of the best uses in a performance-oriented rack.

---

## 6. Freeze-to-compose
Patch a generative setup where Octasource controls:
- 2 or 3 pitch paths
- a filter
- a VCA or LPG

Let it run, and when it hits a beautiful harmonic moment:
- move Rate to **12 o’clock**

Now the system holds that exact harmonic “snapshot.”

This is great live for:
- turning motion into a drone chord
- creating breakdowns
- capturing motifs to build a track section around

---

# Best companions for the Black Octasource in melodic systems

To get the most melodic value from this module, pair it with:

- **Quantizer**  
  Converts complex CV shapes into musical notes/scales

- **Precision adder / transposer**  
  Lets Octasource add interval motion to a written sequence

- **Multiple VCOs / voices**  
  Makes use of the 8 simultaneous outputs

- **Sequential switch**  
  Cycles among outputs for pseudo-sequencing

- **Sample & hold / track & hold**  
  Captures moving CV into discrete note events

- **Clock divider / multiplier**  
  Gives musical timing divisions to SYNC and downstream triggers

- **Comparators / window comparators**  
  Turn LFO shapes into melodic gate logic

- **VCAs / attenuverters**  
  Essential for scaling pitch modulation into useful note ranges

---

# Things to watch out for

## Output amplitude
The outputs are **10 Vpp**, so in bipolar mode that is substantial for pitch. You’ll often want:

- attenuation
- offset
- quantization

before sending the signal to oscillator pitch.

## LFO range
The rate is:
- **0.03 Hz to 30 Hz**

That means it is primarily an LFO/modulation source, not an audio-rate oscillator. So think:
- phrase generator
- modulation sequencer
- harmonic animator

rather than direct oscillator FM audio source.

## Sync behavior
When synced, the Rate knob won’t affect speed except at freeze, so timing will come from your clock source.

---

# Best musical roles for this module

The Black Octasource is especially strong at:

- **generative melody**
- **phase-based polyphony**
- **related modulations across many voices**
- **slow harmonic evolution**
- **clock-synced melodic animation**
- **live performance freezing of harmonic states**

It is less about writing exact note-by-note sequences, and more about creating a **living melodic field** that can be shaped into notes with quantizers and voice architecture.

---

# Summary

The **Erica Synths Black Octasource** is best understood as a **master melodic modulation engine** rather than a traditional sequencer. It excels at creating:

- interrelated pitch curves
- phase-shifted melodic lines
- synchronized harmonic motion
- evolving transpositions
- random-to-structured phrase morphing

If you combine it with:
- a quantizer,
- a few oscillators,
- envelopes/VCAs,
- and maybe a precision adder,

it can become the core of a very rich melodic Eurorack patch—especially for generative, minimal, ambient, Berlin-school, and experimental tonal music.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)