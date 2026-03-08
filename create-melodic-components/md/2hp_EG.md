# 2hp — EG

- [Manual PDF](../../manuals/EG_Manual-7ja4.pdf)

---

[Manual PDF](#)

# Using the 2hp EG to Create Melodic Components

The attached manual describes the **2hp EG**, a compact **two-stage envelope generator**. On its own, EG does not generate pitch or sound, but in a Eurorack system it is very useful for shaping melodic events by controlling:

- **VCA amplitude** for note articulation
- **filter cutoff** for timbral melody movement
- **oscillator pitch** for pitch envelopes
- **wavefolder / FM depth / effect parameters** for animated melodic phrasing

Because this module has:
- **trigger/gate input**
- **attack and decay CV**
- **linear/exponential response switching**
- **output attenuation**
- **0–10V envelope output**
- **very wide time range: 3 ms to 11 minutes per stage**

it can be used as a highly flexible modulation source for melodic patching.

---

## Manual Summary

### Main functions
- **TRIG input**: accepts trigger or gate signals, threshold **2.5V**
- **ATTACK CV input**: 0–5V control over attack time
- **ATTACK knob**: sets rise time
- **DECAY CV input**: 0–5V control over decay time
- **DECAY knob**: sets fall time
- **RESPONSE toggle**:
  - **Up = Linear**
  - **Down = Exponential**
- **AMP knob**: attenuates output from **0V to 10V**
- **OUT**: envelope output
- **LED**: visual indication of envelope activity

### Specs
- **2hp**
- **45 mm deep**
- **+12V: 26mA**
- **-12V: 7mA**

---

# What This Module Contributes to Melody

A melodic part usually needs a few things:

1. **Pitch information**
2. **Timing / note triggers**
3. **Articulation / dynamics**
4. **Timbre movement**

The **EG** covers items **3 and 4** directly, and can also contribute to **1** indirectly by modulating pitch-sensitive inputs.

So when used with:
- a **sequencer**
- a **quantizer**
- an **oscillator**
- a **VCA**
- optionally a **filter**

the EG becomes the part of the system that makes notes feel musical rather than mechanical.

---

# Best Ways to Use EG for Melodic Patches

## 1. Classic note envelope for a melodic voice
This is the most direct use.

### Patch
- Sequencer/gate output → **EG TRIG**
- Oscillator audio → **VCA input**
- **EG OUT** → **VCA CV input**
- Sequencer pitch CV → oscillator 1V/oct

### Result
Each trigger creates an attack-decay contour controlling note volume. This gives every note a defined beginning and end.

### Musical use
- **Fast attack, medium decay**: plucky synth lines
- **Fast attack, long decay**: ringing melodic notes
- **Slow attack, medium decay**: swelling lead lines

### Tips
- Use **exponential mode** for more natural, punchy note shapes
- Use **linear mode** for more even, synthetic-sounding articulation
- Use the **AMP knob** to match your VCA’s preferred CV range

---

## 2. Create plucks and percussive melodies
EG is especially strong for short attack/decay envelopes.

### Patch
- Trigger sequencer → **TRIG**
- **EG OUT** → VCA CV
- Optional: mult **EG OUT** to filter cutoff CV

### Settings
- **Attack**: near minimum
- **Decay**: short to medium
- **Response**: exponential
- **AMP**: to taste

### Result
A plucked synth voice with strong transient definition.

### Why it works
The manual states each stage can go as short as **3 ms**, which is ideal for:
- acid-like plucks
- marimba-like synth tones
- arpeggios
- short bass melodies

---

## 3. Use the same envelope for both loudness and brightness
A very musical approach is to send the same envelope to both VCA and filter.

### Patch
- **EG OUT** → VCA CV
- Mult **EG OUT** → filter cutoff CV attenuator/input

### Result
Every note opens in both amplitude and timbre at once, making simple pitch sequences sound expressive.

### Musical effect
- Short decay = tight, muted notes
- Longer decay = brighter, singing phrases
- Exponential response = more acoustic-like contour
- Linear response = more electronic/precise movement

This is one of the best ways to turn a plain sequence into a melodic phrase.

---

## 4. Add pitch envelopes for melodic accent
Because **EG outputs 0–10V**, it can be used carefully to modulate oscillator pitch.

### Patch
- **EG OUT** → attenuator or pitch modulation input on oscillator
- Trigger source → **TRIG**

### Result
At note onset, pitch briefly rises or falls depending on modulation polarity and routing.

### Uses
- subtle attack bend on lead notes
- kick-drum-like pitch drops
- expressive acid-style accents
- ornamentation at the beginning of notes

### Important note
The raw envelope range is large, so for pitch modulation you usually want **heavy attenuation** before the oscillator pitch input unless the oscillator has a very small-depth FM/mod input.

---

## 5. Animate melodic phrasing with CV over attack and decay
A standout feature of EG is **CV over both attack and decay**.

This means another modulation source can vary articulation over time, so your melody breathes and evolves.

### Patch ideas
- Slow LFO → **ATTACK CV**
- Random stepped CV → **DECAY CV**
- Sequencer row / modulation lane → **ATTACK CV** or **DECAY CV**

### Result
Different notes can have:
- different lengths
- different sharpness
- different emotional character

### Musical examples
- ascending notes with longer attack
- accented notes with longer decay
- randomized phrasing in generative melodies
- evolving ambient melody contours

### Why this is powerful
Even with a fixed pitch sequence, changing envelope shape creates the perception of a more composed, expressive melody.

---

## 6. Turn gates into dynamic note lengths
Since EG responds to **trigger or gate signals**, you can use rhythmic gate streams to articulate melodic lines.

### Patch
- Gate sequencer / keyboard gate → **TRIG**
- **EG OUT** → VCA CV

### Result
The EG converts timing information into shaped note gestures.

If your sequencer produces different rhythmic patterns, the envelope can turn them into:
- short stabs
- swelling notes
- legato-like overlaps, depending on settings downstream

This is especially useful when melodic interest comes from rhythm more than pitch complexity.

---

## 7. Make melodic accents in a sequence
Use EG on only part of a patch to create dynamic note emphasis.

### Patch
- Main sequence runs normally
- Accent trigger pattern → **EG TRIG**
- **EG OUT** → filter cutoff CV or wavefolder amount

### Result
Only accented steps receive extra brightness or harmonic intensity.

### Musical use
This is excellent for:
- techno sequences
- acid lines
- bass melodies
- repeating ostinatos that need variation

Instead of changing the pitch, you change the **expression** of selected notes.

---

## 8. Use long envelopes for slow melodic motion
The manual gives a maximum stage length of **11 minutes per stage**, which is unusually long.

### Patch
- Occasional trigger source → **TRIG**
- **EG OUT** → oscillator FM depth, filter cutoff, or wave shaping amount

### Result
Extremely slow rises and falls can shape an ambient melodic texture over long time spans.

### Musical uses
- evolving drones with slow pitch color changes
- gradual opening of harmonics during a melodic layer
- long-form phrasing in ambient or generative pieces

This makes EG useful not only for note-level articulation, but also for macro-level melodic development.

---

# Linear vs Exponential: Which to Use for Melody

The response toggle is one of the most musically significant controls.

## Linear
Best for:
- precise, synthetic shapes
- even modulation sweeps
- patching to pitch or parameter CV where you want predictable movement

### Sound
More neutral, straight, and controlled.

## Exponential
Best for:
- plucks
- natural-feeling note articulation
- punchy melodic accents
- VCA and filter shaping

### Sound
More lively and “acoustic” in feel, with stronger perceived transients.

### Practical advice
For most melodic voice articulation:
- start with **exponential**
- switch to **linear** if you want a cleaner or less punchy contour

---

# Example Melodic Patches

## Patch 1: Basic synth lead
- Pitch sequencer → oscillator 1V/oct
- Gate sequencer → **EG TRIG**
- Oscillator → filter → VCA
- **EG OUT** → VCA CV
- Optional mult of **EG OUT** → filter CV

**Suggested settings**
- Attack: low
- Decay: medium
- Response: exponential
- AMP: around 50–75%

**Result**
Playable, expressive mono lead voice.

---

## Patch 2: Plucked sequence
- Sequencer pitch CV → oscillator
- Clocked trigger pattern → **EG TRIG**
- Oscillator → LPG or VCA
- **EG OUT** → LPG/VCA CV

**Suggested settings**
- Attack: minimum
- Decay: short
- Response: exponential

**Result**
Tight, melodic plucks ideal for arps and basslines.

---

## Patch 3: Evolving ambient melody
- Quantized random CV → oscillator pitch
- Sparse trigger stream → **EG TRIG**
- **EG OUT** → VCA CV
- Slow LFO → **DECAY CV**
- Optional second slow CV → **ATTACK CV**

**Suggested settings**
- Attack: medium to long
- Decay: long
- Response: linear for smoothness

**Result**
Melodic notes with constantly shifting articulation, ideal for ambient or generative music.

---

## Patch 4: Acid-style melodic accenting
- Pitch sequencer → VCO
- Main gate sequence → VCA envelope elsewhere or same EG
- Accent trigger pattern → **EG TRIG**
- **EG OUT** → filter cutoff CV and slight pitch mod

**Suggested settings**
- Attack: very short
- Decay: short-medium
- Response: exponential

**Result**
Selected notes snap brighter and slightly bend, creating animated acid-like phrasing.

---

# Strengths of This Module in a Melodic System

## 1. Tiny footprint
At **2hp**, it adds expressive control without consuming valuable rack space.

## 2. Extremely wide timing range
From **very fast transient shaping** to **ultra-slow phrase development**.

## 3. CV control over both attack and decay
This is especially helpful for melodic variation and generative patching.

## 4. Useful output attenuation
The built-in **AMP** control makes it easier to dial modulation depth without needing another attenuator in some patches.

## 5. Switchable contour type
Linear/exponential switching gives you two very different articulation feels from one compact module.

---

# Limitations to Keep in Mind

Based on the manual, this is a **two-stage attack-decay envelope**, so:

- there is **no sustain stage**
- it is not a full ADSR
- it is best for:
  - plucks
  - simple note articulation
  - triggered or gated shapes
  - modulation gestures

For sustained keyboard-style melodic phrasing, another envelope type might be better, but for sequenced melodic lines this AD design is often perfect.

---

# Best Companion Modules

To build full melodic functionality around EG, pair it with:

- **oscillator** for pitch generation
- **sequencer** or **keyboard controller** for notes
- **quantizer** if using random CV melodically
- **VCA** for amplitude shaping
- **filter** for timbral shaping
- **mixer/attenuator** for controlling modulation depth
- **clocked trigger source** for rhythmic articulation

---

# Bottom Line

The **2hp EG** is a compact but powerful tool for making melodic patches feel alive. It does not create melody by itself, but it is excellent for shaping the expressive side of melody:

- **how notes start**
- **how long they bloom**
- **how bright they feel**
- **how accents behave**
- **how phrases evolve over time**

If used with a sequencer, oscillator, VCA, and optionally a filter, it can produce:
- plucked melodies
- expressive leads
- accented basslines
- evolving ambient phrases
- generative articulation changes

Its biggest melodic strengths are the **wide time range**, **CV over attack/decay**, and **linear/exponential switch**, all of which help transform simple note sequences into more musical performances.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)