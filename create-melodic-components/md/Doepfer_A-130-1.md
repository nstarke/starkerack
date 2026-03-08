# Doepfer — A-130-1

- [Manual PDF](../../manuals/A1301_man.pdf)

---

[Manual PDF](attachment)

# Doepfer A-130 / A-131 VCA: using them for melodic patching

The manual covers two closely related VCAs:

- **A-130** = **linear VCA**
- **A-131** = **exponential VCA**

They are otherwise functionally the same:
- 2 audio inputs, each with its own level control
- 2 CV inputs, one with an attenuator
- gain control
- output level control

For melodic music, these modules are not pitch sources by themselves, but they are extremely important for shaping **notes, articulation, dynamics, timbre motion, and keyboard tracking**. In practice, they help turn oscillators, envelopes, LFOs, and sequencer CV into playable melodic voices.

---

## What each module is best at musically

## A-131 (exponential VCA): best for note loudness

The manual explicitly says this is the one you’d **normally use for audio signals**. That makes it the more natural choice for:

- final amplitude shaping of a melodic voice
- plucky or expressive envelope-controlled notes
- natural-feeling loudness response
- dynamic accents from envelopes or velocity-like CV

### Typical melodic role
Patch:
- **VCO audio** → **A-131 Audio In**
- **ADSR envelope** → **A-131 CV**
- **A-131 Out** → mixer / filter / output

This gives you the classic synthesizer note shape:
- keyboard or sequencer determines pitch
- gate triggers ADSR
- ADSR opens the VCA
- each note gets a distinct contour

That is the foundation of most melodic patches.

---

## A-130 (linear VCA): best for control voltages and modulation depth

The manual says this is the one you’d **normally use for control voltages**. For melodic work, that makes it especially useful for controlling things like:

- vibrato depth
- filter envelope amount
- tremolo amount
- keyboard tracking amount
- modulation scaling from sequencers or random sources

Because it is linear, it behaves more predictably when scaling CV.

### Typical melodic role
Use it to control how much modulation reaches another module:
- **LFO** → **A-130 Audio/CV In**
- **envelope or macro control CV** → **A-130 CV input**
- **A-130 Out** → VCO FM input, filter CV input, or another VCA’s CV input

This lets modulation appear only on certain notes or only at certain strengths.

---

# Important features from the manual and what they mean musically

## 1. Two audio inputs per VCA

Each VCA has:
- **Audio In 1**
- **Audio In 2**

Both are mixed and then amplified together.

### Musical uses
This is useful for melodic patches because you can combine:
- two oscillators in an interval
- oscillator + noise for attack transient
- sub oscillator + main oscillator
- two different waveforms for richer note tone

Example:
- VCO 1 saw → In 1
- VCO 2 pulse tuned a fifth up → In 2
- envelope to CV
- output gives one articulated melodic sound with both oscillators under the same amplitude contour

This is a very efficient way to make harmonically richer melodic voices.

---

## 2. Gain control acts like an offset

The **Gain** knob sets overall gain. The manual notes that if gain is above zero, amplification can happen even with no CV present.

### Musical implications
This matters a lot in melodic patches:

- With **Gain at 0**, notes only sound when CV opens the VCA
- With **Gain above 0**, some sound may pass all the time, or negative/bi-polar modulation can still be heard

### Good uses
- create drones beneath melodies
- let tremolo continue smoothly with a bipolar LFO
- add a constant bed under a sequenced line
- make modulation audible even when the modulating CV swings below 0 V

This is especially useful if you want a melodic part that is partly percussive and partly sustained.

---

## 3. CV response: linear vs exponential

The manual emphasizes the difference:

- **A-130 linear**: amplification changes directly with control voltage
- **A-131 exponential**: more natural loudness behavior for audio

### Musical interpretation
For melodic lines:
- use **A-131** when you care about how loudness feels to the ear
- use **A-130** when you care about accurate scaling of modulation/control signals

A strong patching strategy is:
- **A-130** for shaping modulation
- **A-131** for shaping the audible voice

---

## 4. VCA control range

The manual states the effective CV range is:
- **0 V = no amplification**
- **+5 V = maximum amplification**

### Why that matters
Many envelopes, sequencers, and modulation sources in Eurorack exceed 5 V. So in melodic patches:
- use the **CV2 attenuator** to tame hot modulation
- use the **input attenuators** to avoid distortion
- use the **Out** knob for final level balancing

This helps keep your melodic voice clean and controlled.

---

# Melodic patch ideas using these modules

## 1. Basic subtractive melodic voice

This is the most direct use.

### Patch
- VCO pitch controlled by keyboard/sequencer
- VCO audio → A-131 In 1
- ADSR → A-131 CV1 or CV2
- A-131 Out → mixer/output
- Gate from keyboard/sequencer → ADSR gate

### Result
A standard melodic synth line with proper note articulation.

### Why A-131 here
Its exponential response gives a more musically natural volume contour.

---

## 2. Two-oscillator lead voice

Use the VCA’s two inputs to combine oscillators before amplitude shaping.

### Patch
- VCO 1 saw → A-131 In 1
- VCO 2 pulse → A-131 In 2
- tune VCO 2:
  - unison for thickness
  - octave for body
  - fifth for harmonic brightness
- ADSR → A-131 CV
- A-131 Out → output

### Result
A richer melodic line with one envelope controlling both oscillators.

### Musical advantage
The two input attenuators let you balance the interval and waveform mix.

---

## 3. Add attack transient to notes

The second input can also add percussive brightness.

### Patch
- VCO → A-131 In 1
- Noise source → A-131 In 2
- ADSR to VCA CV
- set noise input low

### Result
Each melodic note gets a sharper attack, useful for:
- plucks
- brass-like patches
- pseudo-piano attacks
- more defined sequence articulation

---

## 4. Tremolo on melodic lines

The manual specifically describes amplitude modulation using an LFO.

### Patch
- VCO → A-130 In 1 or A-131 In 1
- LFO → CV input
- set **Gain above 0**
- output to mixer

### Result
At low LFO rates, you get **tremolo**.

### Melodic application
Excellent for:
- sustained lead lines
- animated pads playing chords/arpeggios
- expressive pulsing on held notes

### Best choice
- **A-130** is ideal if you want precise amplitude modulation behavior
- **A-131** can sound more ear-natural as final loudness control

---

## 5. Audio-rate AM for metallic melodic tones

The manual notes that with audio-rate modulation, sidebands appear and interesting timbres emerge.

### Patch
- carrier VCO → A-130 In 1
- second VCO or audio-rate LFO → CV input
- set Gain above 0
- output to mixer
- pitch the carrier from your sequence
- optionally pitch the modulator musically too

### Result
Complex, clangorous, or bell-like melodic tones.

### Musical use
This is great for:
- metallic leads
- tuned percussion
- experimental melodic motifs
- evolving harmonics in repeated sequences

The A-130 is especially suitable here because linear response tends to be more predictable for modulation duties.

---

## 6. Voltage-controlled vibrato depth

This is where the A-130 really shines.

### Patch
- LFO → A-130 In 1
- envelope or performance CV → A-130 CV input
- A-130 Out → VCO FM input (lightly)
- VCO audio → A-131 for final amplitude shaping

### Result
Vibrato amount changes over the life of each note.

### Musical examples
- no vibrato at attack, more at sustain
- stronger vibrato on accented notes
- modulation wheel-like expressiveness if a controller provides the CV

This makes melodic lines feel much more alive.

---

## 7. Voltage-controlled filter envelope amount

You can also use the A-130 to scale an envelope before it reaches a filter.

### Patch
- ADSR → A-130 In 1
- sequencer accent CV / controller / second envelope → A-130 CV
- A-130 Out → filter cutoff CV input
- VCO audio → filter → A-131 → output

### Result
Some notes open the filter more than others.

### Musical benefit
This creates:
- accents
- phrase dynamics
- stronger articulation on selected notes
- expressive melodic contour beyond simple pitch changes

---

## 8. Keyboard tracking for brighter/louder high notes

The manual specifically includes **keyboard tracking** patches.

### Patch concept from the manual
Use keyboard CV to control a VCA so pitch affects amplification.

### Example
- VCO audio → VCA 1 → VCA 2
- ADSR controls VCA 1 for normal note articulation
- keyboard pitch CV goes to VCA 2 CV
- adjust VCA 2 gain/CV amount to determine how much louder higher notes become

### Result
Higher notes are louder than lower notes.

### Musical use
This is useful when:
- you want leads to “speak” more in the upper range
- you want a keyboard-like dynamic contour across pitch
- you want patches that cut through more at the top

The manual also shows the inverse version using a voltage inverter:
- lower notes louder than higher notes

That can be great for:
- bass-focused sequences
- mellow top-end behavior
- psychoacoustic balancing of melodic runs

---

## 9. Controlled modulation depth for evolving phrases

The manual’s three-VCA example is especially good for melodic development.

### Structure
- **VCA 1**: applies AM to the sound
- **VCA 2**: final volume control
- **VCA 3**: controls modulation depth

### Melodic interpretation
You can adapt this concept to any modulation:
- vibrato depth
- tremolo depth
- filter modulation amount
- wavetable position movement
- FM amount

### Result
A phrase can evolve over time:
- first notes dry
- later notes more animated
- chorus stronger than verse
- accents push modulation deeper

This is one of the most musically powerful uses of VCAs in a melodic system.

---

# Practical “voice architecture” ideas

## Voice architecture 1: classic mono lead
- VCO → filter → A-131
- ADSR → A-131 CV
- sequencer/keyboard pitch → VCO
- gate → ADSR

Use the A-130 to scale:
- vibrato depth
- filter envelope amount
- accent CV

---

## Voice architecture 2: expressive dual-oscillator voice
- VCO 1 → A-131 In 1
- VCO 2 → A-131 In 2
- ADSR → A-131 CV
- keyboard CV also routed through A-130 for keyboard tracking of filter or amplitude

This gives a solid melodic lead with dynamic response across the keyboard.

---

## Voice architecture 3: animated sequence voice
- sequenced VCO → A-131
- ADSR → A-131 CV
- LFO → A-130
- envelope or accent CV → A-130 CV
- A-130 Out → filter cutoff or vibrato FM

This creates repeated melodic patterns that subtly evolve note by note.

---

# Best practices from the manual

## Keep levels under control
The manual warns that if the output distorts undesirably:
- reduce **In 1**
- reduce **In 2**

This is especially important when combining two oscillators or strong modulation signals.

---

## Use Gain carefully with bipolar modulation
If using an LFO that swings negative and positive:
- set **Gain > 0**

Otherwise, only the positive half of the modulation may open the VCA, producing chopped or asymmetric behavior.

That can be useful creatively, but if you want smooth tremolo or AM, a little gain offset helps.

---

## Use A-130 and A-131 together, not as alternatives
The most musical takeaway from this manual is that these modules complement each other:

- **A-131** shapes the audible note
- **A-130** shapes the behavior of modulation that makes the note expressive

That combination is ideal for melodic music.

---

# Summary

These Doepfer VCAs are core melodic utility modules.

## Use the **A-131** for:
- final loudness shaping of notes
- envelope-controlled articulation
- dual-oscillator melodic voices
- plucks, leads, basses, pads

## Use the **A-130** for:
- scaling CV
- vibrato depth control
- filter modulation amount
- tremolo and AM
- keyboard tracking
- dynamic modulation of melodic phrases

## Most musical combined use
A very effective setup is:

1. **VCO(s)** provide pitch and harmonic content  
2. **A-130** controls expressive modulation depth  
3. **A-131** controls final note loudness  

That gives you melodic patches that are not just pitched, but also **phrased, articulated, and dynamically shaped**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)