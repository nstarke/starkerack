# Doepfer — A-140

- [Manual PDF](../../manuals/A140_man.pdf)

---

[Doepfer A-140 ADSR Manual PDF](https://doepfer.de/a100_man/A140_man.pdf)

# Doepfer A-140 ADSR — using it to create melodic components

From the attached manual, the module here is the **Doepfer A-140 ADSR**, an envelope generator for the A-100 system. By itself, it does **not generate pitch or audio**, but it is extremely useful for shaping the melodic behavior of other modules in a patch.

## What the A-140 does
The A-140 outputs a time-varying control voltage with the classic four stages:

- **Attack**
- **Decay**
- **Sustain**
- **Release**

It has:

- **Gate input**
- **Retrig input**
- **2 normal envelope outputs**
- **1 inverted envelope output**
- **LED envelope indicator**
- **3-position time range switch**
  - **H** = very slow, up to minutes
  - **M** = medium
  - **L** = very fast, down to very short times

The manual notes that it can modulate:

- **VCA**
- **VCF**
- **VCO pulse width**
- **VCO frequency**
- **phase processors**
- **voltage-controlled LFOs**

That means its role in melody is mostly about **articulation, timbre movement, accenting, and pitch contour**.

---

# How it helps create melodic parts

A melodic patch usually needs a few layers working together:

1. **Pitch source** — sequencer, keyboard CV, quantizer, random source
2. **Sound source** — VCO
3. **Tone shaping** — VCF
4. **Amplitude shaping** — VCA
5. **Timing/control** — gate/trigger source
6. **Envelope modulation** — the A-140

The **A-140 turns static notes into playable phrases**. Even a simple pitch sequence becomes musical once the ADSR shapes loudness, brightness, and motion.

---

# Best musical uses of the A-140 in melodic patches

## 1. Classic note articulation: ADSR -> VCA
This is the most important melodic use.

### Patch
- **Pitch CV** -> VCO 1V/Oct
- **VCO audio out** -> VCF or directly to VCA
- **A-140 Output** -> VCA CV input
- **Gate/keyboard/sequencer gate** -> A-140 Gate

### Result
Each note gets a contour:

- **Short attack, short decay, low sustain, medium release** = plucky sequence
- **Fast attack, medium decay, medium sustain, short release** = synth lead
- **Slow attack, high sustain, long release** = pads or swelling melodic lines

### Why this matters melodically
The envelope defines whether the melody feels:

- percussive
- legato
- soft
- aggressive
- sustained
- expressive

Even the same pitch sequence can sound like bass, lead, pluck, or pad just by changing the ADSR.

---

## 2. Brightness contour: ADSR -> VCF cutoff
This is the second major melodic use.

### Patch
- **VCO** -> **VCF audio in**
- **VCF out** -> **VCA**
- **A-140 Output** -> **VCF CV input**
- Same gate source -> **A-140 Gate**

### Result
Each note opens the filter differently over time.

### Good settings
- **Fast attack**
- **Short/medium decay**
- **Lower sustain**
- **Short release**

This gives a note a bright front edge, then a darker body — very useful for melodic phrasing.

### Musical effect
This adds:

- note definition
- expressiveness
- dynamic emphasis
- “speaking” synth timbre

For melodic lines, this helps notes feel shaped instead of flat.

---

## 3. Simultaneous melodic shaping: one ADSR to both VCA and VCF
The A-140 provides **two identical normal outputs**, so you can split the same envelope without a mult.

### Patch
- **Output 1** -> VCA CV
- **Output 2** -> VCF CV
- **Gate source** -> A-140 Gate

### Result
One note event controls both:
- loudness
- brightness

This is one of the most useful “together” functions described by the panel layout.

### Why it’s good
With one envelope, your melody gets cohesive articulation. The attack of the volume and the attack of the filter rise together, which feels natural and musical.

---

## 4. Pitch envelope for melodic attack: ADSR -> VCO FM / pitch CV
The manual specifically mentions **ADSR -> VCO (FM)**.

### Patch
- **A-140 Output** -> attenuator or FM input on VCO
- Gate source -> A-140 Gate

### Result
The note pitch moves during the envelope.

### Musical uses
- Tiny amount: subtle “analog” attack bend
- Medium amount: synth brass or punchy bass transient
- Large amount: dramatic swoops or unstable melodic effects

### Best settings
- **Very fast attack**
- **Short decay**
- **Zero or low sustain**
- **Short release**

This creates a pitch blip at note onset.

### Important note
Use a **small modulation amount** if you want stable melody. Too much envelope-to-pitch makes notes sound out of tune.

---

## 5. PWM movement tied to each note: ADSR -> VCO pulse width
The manual also suggests **ADSR -> VCO (PWM)**.

### Patch
- Use a square/pulse wave VCO output
- **A-140 Output** -> PWM CV input
- Gate source -> A-140 Gate

### Result
The harmonic content shifts with each note.

### Musical effect
This is great for:
- animated lead sounds
- expressive bass
- more vocal-sounding melodic timbres

### Why it helps melody
Instead of every note having the same spectral shape, each note has internal motion. That makes repetitive sequences sound more alive.

---

## 6. Inverse contour for counter-motion: Inverse Output
One special feature of the A-140 is its **inverted envelope output**.

### Patch idea
- **Normal Output** -> VCA CV or VCF CV
- **Inverse Output** -> second modulation destination

### Examples
- Normal out -> open filter
- Inverse out -> reduce another parameter at the same time

Or:

- Normal out -> one oscillator’s FM depth rises
- Inverse out -> another oscillator’s PWM falls

### Musical value
This creates **complementary motion**, which is excellent for more complex melodic voices. As one parameter rises, another falls.

That can make a melody feel more animated and intentional.

---

## 7. Re-triggered envelopes for rhythmic melodic animation
The **Retrig input** is especially useful.

The manual states that while the gate remains open, pulses arriving at **Retrig** restart the envelope.

### Patch
- Long gate or held keyboard note -> **A-140 Gate**
- LFO square, clock, trigger sequencer, or rhythmic pulse -> **Retrig**
- Envelope output -> VCF, VCA, PWM, or pitch amount

### Result
A sustained note can contain repeated internal articulations.

### Melodic applications
- Held drone with pulsing brightness
- Sustained lead note with repeating attack accents
- Trills or tremolo-like shape when routed to VCA
- Repeated filter pecks on a long note

### Why this is musically powerful
You can make **one pitch behave like a phrase** instead of a static sustained note.

This is excellent for:
- Berlin-school sequences
- pulsing leads
- ratcheting-style melodic textures
- expressive sustained solos

---

# Practical melodic patch recipes

## Patch 1: Simple monosynth melody
### Connections
- Sequencer pitch CV -> VCO 1V/Oct
- Sequencer gate -> A-140 Gate
- VCO saw -> VCF in
- VCF out -> VCA in
- A-140 Output 1 -> VCA CV
- A-140 Output 2 -> VCF CV

### Suggested ADSR
- Attack: low
- Decay: medium
- Sustain: medium-low
- Release: short-medium
- Time Range: M

### Sound
A classic articulate melodic line with punch and contour.

---

## Patch 2: Plucky sequence
### Connections
Same as above

### Suggested ADSR
- Attack: 0
- Decay: short
- Sustain: 0 or very low
- Release: short
- Time Range: M or L

### Sound
Short plucked notes, ideal for arpeggios and sequenced melodies.

---

## Patch 3: Expressive lead
### Connections
- Keyboard/sequencer gate -> A-140 Gate
- A-140 Output 1 -> VCA CV
- A-140 Output 2 -> VCF CV
- Optional: small amount of envelope -> VCO FM

### Suggested ADSR
- Attack: very short
- Decay: medium
- Sustain: medium-high
- Release: medium
- Time Range: M

### Sound
Lead voice with a touch of filter movement and optional pitch attack for expression.

---

## Patch 4: Long evolving melody
### Connections
- Pitch sequence -> VCO
- Gate -> A-140 Gate
- A-140 -> VCF and/or VCA
- Time Range -> H

### Suggested ADSR
- Attack: long
- Decay: long
- Sustain: medium
- Release: long

### Sound
Slow melodic swells and evolving phrase lines, useful for ambient or cinematic music.

---

## Patch 5: Pulsing sustained note with retrigger
### Connections
- Held gate -> A-140 Gate
- Clock or LFO pulse -> Retrig
- Envelope output -> VCF CV

### Suggested ADSR
- Attack: fast
- Decay: medium
- Sustain: low
- Release: short

### Sound
A sustained pitch with repeated note-like accents in tone.

This is very effective when a melody note needs internal rhythm.

---

## Patch 6: Accent programming with envelope-to-pitch
### Connections
- Sequence CV -> VCO 1V/Oct
- Gate -> A-140 Gate
- A-140 Output -> attenuated VCO FM input

### Suggested ADSR
- Attack: 0
- Decay: short
- Sustain: 0
- Release: short
- Time Range: L or M

### Sound
Each note has a small pitch kick at the start, great for punchy bass melodies.

---

# How the time range switch changes musical behavior

The **Time Range** switch is very important for melodic use.

## L (low)
Very fast envelopes.

Best for:
- clicks
- plucks
- percussive bass
- sharp filter attacks
- tight sequencer lines

## M (medium)
General-purpose melodic work.

Best for:
- leads
- basses
- normal keyboard articulation
- standard synth phrasing

## H (high)
Very slow envelopes.

Best for:
- swelling notes
- ambient melody
- slow filter sweeps tied to note events
- long releases between phrases

---

# How to think about the inverted output musically

The inverted output is easy to overlook, but it can be very useful in melodic design.

## Example uses
- Normal out -> VCA, inverse out -> negative filter modulation
- Normal out -> oscillator pitch rise, inverse out -> second oscillator pitch fall
- Normal out -> open one VCA, inverse out -> close another VCA

## Melodic result
This allows:
- timbral crossfades
- push-pull movement
- note-dependent contrast
- more complex phrase articulation

It’s especially good when building a melody voice from multiple oscillators or parallel signal paths.

---

# Limitations to keep in mind

From the manual, the A-140 is an **envelope generator only**. So to create full melodic components, you still need other modules such as:

- **VCO** for pitch/audio generation
- **VCA** for amplitude control
- **VCF** for tone shaping
- **Sequencer / keyboard / MIDI-CV** for pitch and gate

So the A-140 is not the melody source, but rather the module that makes a melody **musical, shaped, and expressive**.

---

# Best “used together” roles in a melodic system

If you are combining this module with standard Eurorack voice modules, the strongest pairings are:

## A-140 + VCA
For note articulation and dynamics

## A-140 + VCF
For brightness contour and expressive phrasing

## A-140 + VCO PWM
For animated timbre per note

## A-140 + VCO pitch/FM
For pitch attack and synth-style transient shaping

## A-140 + clock/LFO via Retrig
For repeated articulation inside sustained melodic notes

## A-140 normal + inverse outputs together
For complex counter-moving modulations in a melody voice

---

# Bottom line

The **Doepfer A-140 ADSR** is one of the core modules for turning a raw pitch sequence into an actual melodic performance.

Its biggest strengths for melodic patching are:

- shaping **volume** with a VCA
- shaping **brightness** with a VCF
- adding **pitch attack** to a VCO
- animating **PWM**
- using **retriggering** for rhythmic internal motion
- using **normal and inverted outputs** for richer note behavior

If you patch it into both the **VCA and VCF** of a voice, you already have the foundation of a very playable melodic synthesizer voice. Add a sequencer or keyboard CV, and the A-140 becomes the articulation engine that gives your melodies life.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)