# Instruo — Tona

- [Manual PDF](../../manuals/Tona-Manual-A5.pdf)

---

[Manual PDF](attachment)

# Instruō tòna — using it for melodic patching

The **Instruō tòna** is an **analog VCO** designed to be the main pitched sound source in a Eurorack melodic voice. From the manual, it provides:

- **1V/Oct tracking** for keyboard/sequencer pitch control
- Four standard waveform outputs:
  - Square
  - Saw
  - Triangle
  - Sine
- A **wavefolded output**
- **Linear FM**
- **Hard sync**

This means tòna is best understood as the **core tone generator** in a melodic system: it makes the pitch, and its outputs can be shaped downstream by filters, VCAs, envelopes, and modulation.

---

## What role it plays in a melodic patch

For melodic music, a patch usually needs:

1. **Pitch source** — sequencer, keyboard, quantizer, or CV recorder
2. **Sound source** — oscillator
3. **Amplitude shaping** — VCA + envelope
4. **Tone shaping** — filter and/or timbre modulation
5. **Optional animation** — FM, sync, wavefold CV, vibrato, etc.

In this ecosystem, **tòna is the sound source**.

The manual’s patch examples explicitly show it used as:

- an **East Coast synth voice oscillator**
- an **FM carrier oscillator**
- a **self-modulated wavefold voice**

---

## Core melodic uses

## 1. Classic mono synth lead or bass voice

This is the most straightforward use.

### Patch concept
- Send **1V/Oct CV** from a sequencer or keyboard into **tòna’s 1V/Oct input**
- Use one of the waveform outputs:
  - **Saw** for bright lead/bass tones
  - **Square** for hollow/reedy melodies
  - **Triangle** for softer, rounder lines
  - **Sine** for pure bass, sub-melodies, or FM-friendly tones
- Route oscillator output to:
  - **filter**
  - then **VCA**
- Trigger an envelope from the same sequencer gate to shape the VCA, and optionally the filter

### Musical result
This gives you:
- basslines
- arpeggios
- leads
- sequenced motifs
- simple drones with pitch movement

### Good waveform choices
- **Saw + filter envelope**: classic subtractive melody
- **Square + resonance**: stronger, nasal sequences
- **Triangle**: great for understated melodic layers
- **Sine**: pure tonal melodies, often ideal for doubling another voice

---

## 2. Layered waveform melodic voice

Because tòna provides multiple simultaneous waveform outputs, you can use it as a **multi-timbre melodic source**.

### Patch concept
- Patch **saw, square, and triangle** into separate mixer inputs
- Blend them before the filter/VCA
- Control pitch from the same 1V/Oct line

### Why this matters musically
This lets you build a more complex melodic timbre without needing multiple oscillators.

### Example uses
- **Bassline**: mostly square with a little saw for bite
- **Lead**: saw-heavy with a little triangle to soften edges
- **Sequence**: mix square and triangle for a more animated but not harsh tone

### Performance benefit
You can alter the harmonic content of the melody by moving mixer levels rather than repatching.

---

## 3. West Coast flavored melodic timbres via wavefolding

A major strength of tòna is the **wavefold output**. The manual notes that the wavefolder processes the oscillator’s **sine waveform** and can move from nearly sine-like to rich harmonic content.

### Patch concept
- Use the **Wavefold Output** as your main audio output
- Sequence pitch with **1V/Oct**
- Route to VCA and optionally filter
- Adjust the **Wavefold fader** to set timbral complexity

### Musical result
This is excellent for:
- expressive melodic lines
- plucked or bell-like tones
- bright, animated sequences
- evolving motifs that cut through a mix

### Why it’s melodic-friendly
Unlike a filter sweep that generally removes harmonics, wavefolding can **add harmonics dynamically**, making the same melody feel more alive and articulate.

### Best use cases
- minimal techno sequences
- generative melodies
- modern “Buchla-ish” lead lines
- tuned percussion-style patches

---

## 4. Animated melodic phrases with wavefold CV

The manual shows a patch where one of tòna’s own waveforms is sent to the **Wavefold CV input**. This creates synchronized audio-rate timbral modulation.

### Patch concept
- Main melodic pitch enters via **1V/Oct**
- Listen to the **Wavefold Output**
- Patch one of tòna’s own outputs — often **saw** — into **Wavefold CV Input**
- Set the **Wavefold CV attenuator** to taste

### Musical result
This produces:
- harmonically animated notes
- buzzing, vocal-like timbres
- timbral motion locked to oscillator pitch
- more aggressive melodic textures

Because the modulation source tracks the same pitch as the oscillator, the timbre remains tightly related to the melody.

### Practical musical use
This is great for:
- acid-adjacent melodic lines
- metallic sequences
- animated arps
- one-oscillator complex timbre voices

---

## 5. FM melodic voice

The manual specifically describes tòna as the **carrier** in an FM patch, with another oscillator patched into **Linear FM**.

### Patch concept
- Pitch sequence goes into **1V/Oct**
- Another oscillator’s output goes to **Linear FM Input**
- Use **Linear FM Attenuator** to control modulation depth
- Use tòna’s **sine** or **triangle** as the main output for cleaner FM behavior, or saw/square/wavefold for more complex results

### Musical result
This can create:
- metallic melodies
- glassy bells
- inharmonic plucks
- aggressive lead tones
- rich bass timbres

### Melodic strategy
For tonal melodic work:
- keep FM depth lower for stable pitch identity
- use a modulator tuned to musically related intervals if possible
- start with sine-to-sine FM, then increase complexity

### Especially useful for
- melodic percussion
- evolving lead lines
- digital-sounding motifs from analog modules
- contrast against more traditional subtractive voices

---

## 6. Hard sync leads and sequenced riffs

tòna has a **Sync Input** for hard synchronization. On each rising edge, the oscillator resets its cycle.

### Patch concept
- Use a second oscillator as the **master sync source**
- Send a hard-edged waveform like **saw or square** into **Sync Input**
- Sequence pitch on tòna using **1V/Oct**
- Listen to saw, square, triangle, or wavefold output

### Musical result
Hard sync creates:
- cutting lead sounds
- tearing harmonics
- bright, expressive solo tones
- harmonically rich riffs

### Why it works for melody
Sync preserves a strong pitch center while adding dramatic overtone motion. That makes it ideal for:
- solos
- hook lines
- sync bass
- tension-building sequences

### Extra tip
Sweep tòna’s frequency while sync is active for classic ripping sync timbres.

---

## How tòna combines with common companion modules

The manual’s examples reference a broader voice architecture. Here’s how tòna works with each type of module to create melody.

## 1. With a sequencer or keyboard
This is the most important pairing.

### Connections
- Sequencer/keyboard **pitch CV** → **1V/Oct**
- Sequencer/keyboard **gate** → envelope trigger/gate

### Result
You get:
- playable notes
- repeating patterns
- transposable basslines
- melodic phrases tied to a clock or performance input

Without a pitch CV source, tòna is mainly a drone oscillator. With one, it becomes a melodic instrument.

---

## 2. With an envelope generator
An envelope shapes each note over time.

### Connections
- Gate from sequencer → envelope
- Envelope output → VCA CV
- Optional second envelope copy → filter cutoff CV or wavefold CV

### Result
Your pitches become actual **notes** instead of continuous tones.

### Musical possibilities
- short percussive plucks
- long legato leads
- swelling pads
- dynamic filter articulation per note

---

## 3. With a VCA
The VCA makes the melodic line rhythmic and performable.

### Connections
- tòna audio out → VCA audio in
- Envelope → VCA CV in

### Result
Each note starts and stops cleanly.

This is essential for:
- basslines
- melodies
- staccato sequences
- accents

---

## 4. With a filter
The filter shapes brightness and emphasis.

### Connections
- tòna output or waveform mix → filter input
- Filter output → VCA
- Envelope or LFO → filter cutoff CV

### Result
Classic subtractive melodic phrasing.

### Musical uses
- mellow bass from saw or square
- expressive resonance on leads
- plucky sequences with envelope modulation
- spectral movement over repeated pitch patterns

---

## 5. With a mixer
Since tòna offers multiple simultaneous outputs, a mixer is especially useful.

### Connections
- Multiple waveform outputs → mixer channels
- Mixer output → filter or VCA

### Result
You can build a custom melodic timbre from one oscillator.

### Example blend ideas
- **Square + triangle** = woody bass
- **Saw + sine** = firm but smooth lead
- **Triangle + wavefold** = articulate but not overly harsh line

---

## 6. With another oscillator
A second oscillator expands tòna dramatically.

### Uses
- FM modulator
- Sync master/slave partner
- Detuned unison voice
- Interval doubling source

### Melodic benefits
- richer harmonies
- more animated timbres
- stereo layering
- more complex tracked sequences

---

## Best melodic patch recipes

## A. Simple melodic voice
**Good for:** leads, bass, arps

- Sequencer pitch → 1V/Oct
- Sequencer gate → envelope
- tòna saw out → filter → VCA
- Envelope → VCA CV
- Optional envelope → filter CV

This is the bread-and-butter patch.

---

## B. Smooth bass melody
**Good for:** sublines, low-end motifs

- Sequencer pitch → 1V/Oct
- Triangle or sine out → VCA
- Envelope → VCA CV
- Optional light filter shaping

This keeps the line focused and stable.

---

## C. Expressive folded lead
**Good for:** modern leads, solos, signature tones

- Sequencer pitch → 1V/Oct
- Wavefold output → VCA/filter
- Gate → envelope
- Envelope → VCA
- LFO or envelope → Wavefold CV input

This gives each note internal timbral movement.

---

## D. FM melody
**Good for:** bells, metallic hooks, sharp basses

- Sequencer pitch → 1V/Oct
- Second oscillator sine → Linear FM input
- tòna sine out → VCA/filter
- Envelope → VCA
- Raise FM attenuator carefully

Low FM depth = more tonal.  
High FM depth = more experimental.

---

## E. Sync lead
**Good for:** cutting solos and hooks

- Sequencer pitch → 1V/Oct
- Second oscillator saw/square → Sync input
- tòna saw or square out → filter → VCA
- Envelope → VCA and/or filter

Great for prominent melodic phrases.

---

## F. Self-patched animated sequence
**Good for:** complex one-oscillator riffs

- Sequencer pitch → 1V/Oct
- Wavefold output → filter/VCA
- Saw output → Wavefold CV input
- Set Wavefold and CV attenuation to taste
- Envelope → VCA

This creates movement without requiring extra modulation modules.

---

## Strengths of tòna for melody

Based on the manual, tòna is especially strong as a melodic oscillator because it combines:

- **Stable pitch tracking** via 1V/Oct
- **Immediate access to classic waveforms**
- **Built-in wavefolding** for more advanced timbres
- **Linear FM** for harmonic and inharmonic animation
- **Hard sync** for sharper lead sounds
- **Simultaneous outputs** for layering and mixing

So it can cover both:
- **traditional subtractive melodic roles**
- **more experimental timbral melody roles**

---

## Practical musical workflow

A good way to approach tòna in a rack is:

1. Start with **triangle or saw**
2. Patch a basic **sequencer → filter → VCA** voice
3. Get the melody working first
4. Then choose one enhancement:
   - add **wavefold**
   - add **FM**
   - add **sync**
   - blend multiple waveforms
   - self-patch wavefold CV

This keeps the melodic intention clear before adding complexity.

---

## Bottom line

The **Instruō tòna** is a strong **primary melodic oscillator**. It can function as:

- a classic mono synth VCO
- a layered subtractive voice source
- a wavefold-based melodic timbre generator
- an FM carrier
- a sync voice
- a self-patched complex oscillator for animated sequences

If paired with even a basic set of support modules — **sequencer, envelope, VCA, and optionally filter/mixer** — it can create a wide range of melodic components:
- basslines
- leads
- arpeggios
- plucks
- drones with pitch motion
- metallic FM motifs
- harmonically rich folded sequences

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)