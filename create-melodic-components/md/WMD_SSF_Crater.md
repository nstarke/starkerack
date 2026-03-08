# WMD SSF — Crater

- [Manual PDF](../../manuals/Kick_Manual.pdf)

---

[Manual PDF](attachment)

# WMD Crater — using it for melodic components

Based on the attached manual, **Crater** is primarily a **hybrid kick drum voice**, but it can absolutely contribute to **melodic material** in a Eurorack patch when treated as a **pitched oscillator/percussive bass voice** rather than only a drum.

## What in the manual suggests melodic use

A few features make Crater useful beyond simple kick duties:

- **PITCH** ranges from **5 Hz to 100 Hz**
- **1V/OCT input** is present
- **SUSTAIN** allows the sound to hold while the **TRIGGER remains high**
- The manual explicitly says:  
  > “Hit those dirty deep kick drum basslines by setting the sustain level and sending a gate to the TRIGGER input. Make it even hotter by sending a sequence to the 1V/OCT input.”
- **Pitch envelope amount and decay** can be controlled, which lets you move from a stable bass note to more tom-like, expressive transients
- **Saturation** and **clipping** can turn a plain low sine-like body into something harmonically richer and easier to hear as a note in a mix

So while this is not a conventional full-range melodic oscillator, it is very usable for:

- **basslines**
- **tuned kick melodies**
- **acid-adjacent low-end riffs**
- **tom-like tuned percussion**
- **drone/sub notes with attack**
- **accented rhythmic melodic motifs**

---

## Core melodic behaviors of Crater

## 1. Tuned bass voice

The clearest melodic use is as a **monophonic bass synth voice**.

### Patch idea
- Send a **pitch sequencer** to **1V/OCT**
- Send a **gate sequence** to **TRIGGER**
- Raise **SUSTAIN**
- Adjust **DECAY** so notes either pluck or hold
- Set **PITCH DECAY AMOUNT** low for more stable pitch
- Use **PITCH DECAY** short if you want punch without obvious pitch dive

### Result
This gives you a bass voice with:
- strong transient
- deep fundamental
- built-in drive options
- expressive gate-length response

Because the oscillator sustains while the trigger is high, **gate length matters**, which is very useful for actual note phrasing.

---

## 2. Tuned toms / melodic percussion

The pitch envelope section is ideal for making **pitched percussion lines**.

### Patch idea
- Sequence **1V/OCT**
- Use shorter **DECAY**
- Set **SUSTAIN** low or off
- Increase **PITCH ENVELOPE AMOUNT**
- Tune **PITCH DECAY** to taste

### Result
You can get:
- disco toms
- electro tuned drum riffs
- tribal melodic percussion
- short “doof” notes that still carry pitch

This is especially effective if the sequence repeats a tonal center, because the ear hears the drum hits as melodic events.

---

## 3. Distorted sub-leads

Crater includes both **SATURATION CV** and a **3-position clipping section**:
- left: clipping off
- middle: restricted clipping that fades to cleaner as amplitude decays
- right: full clipping

### Why this matters melodically
A pure low kick fundamental can be hard to perceive as a note on small speakers. Distortion adds upper harmonics, which makes the pitch more audible.

### Patch idea
- Sequence **1V/OCT**
- Open **SUSTAIN**
- Use medium **DECAY**
- Apply some **SATURATION**
- Set **CLIPPING** to middle or full
- Keep **CLICK LEVEL** lower if you want a more synth-like note

### Result
You get:
- gritty basslines
- gabber-style tuned low-end riffs
- distorted one-note drones with rhythmic articulation

The middle clipping mode is especially musical because the attack is more distorted and the tail cleans up.

---

## 4. Click-based pseudo-melodic articulations

Crater has:
- **14 sampled clicks**
- **CLICK TIMBRE**
- **CLICK DECAY**
- **CLICK LEVEL**

The click is not “pitched” in the same sense as the body oscillator, but it changes note articulation a lot. Different click choices can make repeated notes sound like separate melodic phrases.

### Patch idea
Use the kick body for the actual pitch, and shape melody perception by:
- changing **CLICK TIMBRE**
- changing **CLICK DECAY**
- using accents on selected notes

### Result
Even a simple two-note bassline can sound more musical because each note has a distinct front edge.

This is great for:
- techno bass hooks
- syncopated low-end motifs
- call-and-response between accented and unaccented notes

---

## 5. Accent as melodic emphasis

The module has separate **TRIGGER** and **ACCENT** behavior:
- normal trigger for standard hit
- accent to “beef up” the hit
- plugging into **ACCENT only** always triggers accented kick

### Melodic use
Accent is not pitch, but it is a major part of phrasing. In melodic sequencing, emphasis often matters as much as note choice.

### Patch idea
- Main gate stream to **TRIGGER**
- A second rhythmic lane to **ACCENT**
- Pitch CV to **1V/OCT**

### Result
This creates:
- emphasized notes in a bassline
- pseudo-acid phrasing
- rhythmic variation inside repetitive tonal patterns

---

# Best melodic patch strategies

## A. Simple bassline patch

**Connections**
- Sequencer pitch CV → **1V/OCT**
- Sequencer gate → **TRIGGER**
- Crater **OUTPUT** → mixer / filter / VCA / effects

**Settings**
- **PITCH** around low-mid region
- **SUSTAIN** at 10–2 o’clock
- **DECAY** medium
- **PITCH ENV AMOUNT** low
- **PITCH DECAY** short
- **CLICK LEVEL** low-medium
- **CLIPPING** off or middle

**Use**
- Deep techno bass
- EBM bass sequence
- industrial low-end line

---

## B. Tuned kick melody patch

**Connections**
- Pitch sequence → **1V/OCT**
- Trigger pattern → **TRIGGER**
- Occasional accents → **ACCENT**

**Settings**
- **SUSTAIN** low
- **DECAY** short-medium
- **PITCH ENV AMOUNT** medium-high
- **PITCH DECAY** medium
- **CLICK LEVEL** medium
- **CLICK TIMBRE** chosen for attack character

**Use**
- melodic tom runs
- percussive riffs
- classic drum-synth tuned fills

---

## C. Sustained drone/sub patch

**Connections**
- Quantized CV source → **1V/OCT**
- Long gate or manual gate → **TRIGGER**
- Slow CV → **SATURATION** if available

**Settings**
- **SUSTAIN** high
- **DECAY** medium-long
- **CLICK LEVEL** very low
- **PITCH ENV AMOUNT** very low
- **CLIPPING** middle or off

**Use**
- held root notes
- sub drones under melodies
- dark ambient low fundamentals

---

## D. Aggressive gabber bass sequence

**Connections**
- Sequencer → **1V/OCT**
- Trigger pattern → **ACCENT** or **TRIGGER**
- Optional modulation → **SATURATION**

**Settings**
- **SUSTAIN** medium
- **DECAY** medium
- **PITCH ENV AMOUNT** medium
- **PITCH DECAY** short
- **SATURATION** up
- **CLIPPING** full/right position

**Use**
- hardcore/gabber riffs
- distorted industrial bass
- overdriven mono hooks

---

# How it combines with other modules in a Eurorack system

Since only this manual is attached, I can’t describe specific interactions with additional modules from other manuals. But in a typical system, Crater pairs especially well with the following categories to create melodic components:

## 1. Sequencers and quantizers
Crater becomes melodic as soon as you feed its **1V/OCT** from:
- step sequencers
- keyboard controllers
- quantized random voltages
- arpeggiators

A quantizer is especially helpful because Crater is naturally a drum voice; quantized pitch CV pushes it into clearer tonal use.

## 2. Filters
Even though Crater already has tone-shaping via saturation, clipping, and click controls, a **low-pass or band-pass filter** can help transform it from “kick” into “bass synth.”

Use a filter to:
- tame click brightness
- emphasize a note’s fundamental
- create movement with envelope or LFO modulation

## 3. VCAs and envelopes
If you want more standard synth-note articulation than the built-in drum envelope provides, send Crater through an external VCA.

This helps with:
- tighter note lengths
- dynamic shaping
- sidechain-like arrangements
- better integration with melodic voices

## 4. Distortion / wavefolding / saturation
Crater already distorts internally, but external processing can make it read more like a lead or bass synth.

Useful for:
- bringing out harmonics
- making pitch more audible
- fitting into dense arrangements

## 5. Delay and reverb
Short delay or reverb can turn tuned percussion into a melodic texture.

Best for:
- dubby tom phrases
- atmospheric kick melodies
- sparse low-end motifs in ambient or experimental work

---

# Musical roles Crater can fill

## Bassline voice
Probably the most straightforward non-drum use.

## Root-note anchor
It can reinforce the tonic or root beneath more complex melodic voices.

## Melodic percussion
Excellent for tuned toms and note-like drum phrases.

## Riff generator
With sequencing and accenting, it can create memorable low-register hooks.

## Transitional fills
Pitch-sequenced fills between phrases are a strong use case.

---

# Practical tips

- **Lower click level** if you want the ear to hear “note” instead of “drum.”
- Use **some sustain** and **longer gates** for actual bassline phrasing.
- Keep **pitch envelope amount modest** when tracking melodies; too much can obscure note center.
- Use **middle clipping** for a more musical distorted contour.
- Use **accent rhythmically**, not constantly, to create phrase structure.
- If tracking across a wider range, test pitch response practically; as a kick voice, it may be most convincing over a focused low register rather than as a full melodic lead.

---

# Bottom line

**Crater is not a traditional melodic oscillator, but it is definitely capable of melodic work**—especially in the roles of:

- **tuned kick bass**
- **sustained sub bass**
- **melodic tom percussion**
- **distorted low-end riffs**

Its most important melodic features are the **1V/OCT input**, **sustain behavior**, **pitch envelope controls**, and **harmonic enhancement via saturation/clipping**. In a Eurorack system, that makes it a strong choice for **bass-driven melodic content**, especially in techno, electro, industrial, EBM, hardcore, and experimental patches.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)