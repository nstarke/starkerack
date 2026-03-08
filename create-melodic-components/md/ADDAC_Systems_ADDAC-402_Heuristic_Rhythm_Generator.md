# ADDAC Systems — ADDAC-402 Heuristic Rhythm Generator

- [Manual PDF](../../manuals/ADDAC402_UsersGuide_A_0_web_6500.pdf)

---

[ADDAC402 User Manual (PDF)](http://addacsystem.com/uploads/files/ADDAC402_manual.pdf)

# ADDAC402: using it for melodic components

The ADDAC402 is **not a pitch sequencer**. It is a **4-channel trigger/gate rhythm generator** with multiple algorithmic modes. So its role in melody-making is indirect but very powerful: it can become the **timing brain** that drives pitch events, phrase resets, transpositions, note length changes, and probabilistic articulation.

If you pair it with quantizers, sample & holds, sequential switches, precision adders, envelope generators, oscillators, or other melodic sequencers, it can generate surprisingly rich melodic structures.

## What the module actually gives you

From the manual, the ADDAC402 provides:

- 4 independent gate/trigger outputs
- 4 inverted outputs
- multiple rhythm modes:
  - Euclidean
  - Gate Sequencer
  - Game of Life
  - Golomb Rulers
  - Probabilistic
  - Footwork
  - Pong
- per-channel resets and skips
- global swing / assign CV
- trigger/gate selection per channel
- clocked operation

That means it’s ideal for controlling **when notes happen**, **which melodic lane is active**, and **how phrases evolve over time**.

---

# Best ways to use the ADDAC402 for melody

## 1. Trigger a quantized random melody
A classic patch.

### Patch idea
- Send one ADDAC402 gate output to a **sample & hold trigger** or **quantizer trigger**.
- Feed random CV, noise, or a slow modulation source into the sample & hold.
- Send the resulting CV into a **quantizer** and then to an oscillator’s 1V/oct.

### Result
The 402 determines the rhythm of the melody; the random source determines pitch.

### Why it works well
Different 402 modes create very different melodic feels:
- **Euclidean** = balanced, musical ostinatos
- **Probabilistic** = semi-random note entrances
- **Game of Life** = evolving phrase structures
- **Pong** = playful cyclic accents

---

## 2. Use the 4 channels as four melodic voices
Since the ADDAC402 has 4 outputs, it can drive:

- 4 separate oscillators
- 4 separate envelopes/VCA chains
- 4 voices of a polyphonic patch
- 4 different pitch sources into one mixer

### Example
- Gate 1 triggers bass notes
- Gate 2 triggers mid melody
- Gate 3 triggers high counterline
- Gate 4 triggers accent or ornament voice

If each voice has its own pitch source or quantized CV stream, the 402 becomes a **polyrhythmic melodic ensemble conductor**.

---

## 3. Use outputs to clock multiple pitch sequencers at different rates
Instead of using the 402 only as note gates, use its outputs to **advance pitch sequencers**.

### Patch idea
- Gate 1 clocks Sequencer A
- Gate 2 clocks Sequencer B
- Gate 3 resets a sequencer every so often
- Gate 4 triggers an envelope for accents

### Result
Pitch motion becomes rhythmically non-uniform. Notes do not advance every master beat; they advance only when the 402 says so.

This is excellent for:
- generative melodies
- asymmetrical phrase lengths
- shifting motifs

---

## 4. Use resets to create melodic phrasing
The manual makes clear that individual and master reset functions are central in many modes.

If one 402 output is used as a **reset signal** for:
- a pitch sequencer
- a quantizer with internal pattern memory
- a shift register melody source
- a sequential switch

then you can create repeating melodic phrases with controlled interruptions.

### Example
- Gate 1 = note trigger
- Gate 2 = sequencer advance
- Gate 3 = sequencer reset every 5 or 7 beats
- Gate 4 = transpose envelope or accent trigger

This creates a melody that feels composed rather than merely random.

---

## 5. Use the inverted outputs for off-beat melodic echoes
The manual notes the inverted outputs are literal inversions of the normal gate outputs, effectively creating complementary timing relationships.

### Melodic use
Take:
- main gate output -> primary melody voice
- inverted output -> second voice, pluck, echo, harmonizer, or transposed clone

### Result
You get:
- call-and-response phrasing
- off-beat harmonies
- interlocking melodic lines

This is one of the most musically useful features on the module.

---

# Mode-by-mode melodic applications

## 1. Euclidean mode
This is the most immediately useful for melody.

### Controls
- Steps = pattern length
- Fills = number of active events
- Skip = rotates pattern
- CV on fills available

### Melodic uses
- Trigger a quantized voice with mathematically even note placement
- Use different step/fill settings per channel for interlocking arpeggios
- Rotate channels with skip to create phase-shifted melodic clones

### Good patch
- Channel 1: low voice, 8 steps / 3 fills
- Channel 2: mid voice, 11 steps / 4 fills
- Channel 3: high voice, 13 steps / 5 fills
- Channel 4: accent trigger to transpose a precision adder

This produces evolving melodic counterpoint from simple materials.

---

## 2. Gate Sequencer mode
This turns the 402 into a direct step gate sequencer.

### Controls
- Steps = number of bars
- Fills = move edit cursor
- Skips = activate/clear step

### Melodic uses
This mode is best if you want to **compose note rhythms manually** while leaving pitch generation elsewhere.

### Patch ideas
- Program note on/off patterns for 4 melodic lines
- Use one channel to trigger pitch changes, another to trigger envelopes
- Use one channel only for ornament notes or ratchet-like accents

Because presets are available in this mode, it’s useful for structured live melodic sets.

---

## 3. Game of Life mode
This produces cellular automata patterns.

### Controls
- Fills = number of bars
- Skip = move pattern forward
- Individual reset = new initial pattern
- Master reset = calculate next pattern

### Melodic uses
Excellent for:
- generative ambient melodies
- evolving canons
- long-form algorithmic composition

### Patch idea
- 4 outputs trigger 4 separate quantized pitch paths
- Hit master reset occasionally to evolve to a related phrase
- Use one channel’s output to transpose another voice

This creates melody that feels organic and self-transforming.

---

## 4. Golomb Rulers mode
These patterns are based on unique interval spacing.

### Melodic uses
This is ideal when you want:
- sparse melodic events
- non-repeating accents
- unusual phrase spacing

### Patch idea
Use Golomb outputs to trigger:
- a plucked voice
- a shift register advance
- a sample & hold refresh
- a second oscillator for occasional harmony notes

This can generate pointillistic melodic textures.

---

## 5. Probabilistic mode
Each channel outputs events based on probability.

### Melodic uses
Perfect for:
- varied note density
- humanized phrasing
- uncertain ornamentation

### Patch idea
- One voice gets low probability for occasional melodic punctuation
- One voice gets medium probability for main line
- One voice gets high probability for trills or repeated notes

The manual notes that higher settings on earlier channels may “eat up” probability for later ones, so treat the channels as somewhat interdependent. That can actually be musically useful for melody: denser lead lines naturally suppress decorations.

---

## 6. Footwork mode
This mode is based on a bug, but intentionally musical.

### Controls
- Steps = trigger length
- other fill functions shown on main screen
- skip/reset/gate-trigger switches inactive

### Melodic uses
This is best for **hyperactive rhythmic articulation** of melody:
- stuttering leads
- fast repeated note bursts
- glitch arpeggios
- rapid gate patterns into LPGs or envelopes

### Important note from manual
If Steps is too high, you may get no output; start low.

### Patch idea
Use Footwork to trigger:
- a fixed pitch voice for rhythmic riffs
- a quantizer receiving slow-changing CV
- a sequential switch cycling through pitch rows

This produces complex rhythmic melody from a simple pitch structure.

---

## 7. Pong mode
Ball collisions with the 4 walls generate the 4 outputs.

### Melodic uses
Very playable for melodic interaction.

### Mapping from manual
- Left wall = Gate 1
- Top wall = Gate 2
- Right wall = Gate 3
- Bottom wall = Gate 4

### Patch idea
Assign each wall to:
- a note in a chord
- a different transposition lane
- a different voice register

Because collisions depend on simulated motion, this mode gives semi-predictable melodic phrasing that feels animated.

---

# Practical melodic patch recipes

## Patch 1: Euclidean arpeggiator network
### Modules needed
- ADDAC402
- quantizer
- random CV or sequencer
- 1–2 oscillators
- envelopes + VCAs

### Patch
- Clock into ADDAC402
- Ch1 gate -> S&H trigger -> quantizer -> oscillator 1 pitch
- Ch2 gate -> envelope for oscillator 1
- Ch3 gate -> transpose input via precision adder
- Ch4 gate -> reset random source or sequencer

### Result
A melody with independent note timing, articulation, and phrase transposition.

---

## Patch 2: Four-lane melodic canon
### Patch
- Each ADDAC402 channel triggers a separate envelope/VCA voice
- Feed all voices related pitch CVs:
  - same sequence, different octave offsets
  - same random source, separately sampled
  - same quantizer scale

### Result
The 402 creates a canon-like polyphonic texture. Euclidean or Game of Life work especially well here.

---

## Patch 3: Triggered sequential switch melody
### Modules needed
- sequential switch
- 4 stored voltages or 4 sequencer rows
- quantizer
- oscillator

### Patch
- Use ADDAC402 outputs to:
  - advance switch
  - reset switch
  - trigger envelope
  - trigger sample & hold

### Result
The melody moves through different pitch sources according to 402 rhythm logic.

---

## Patch 4: Complementary melody using inverted outs
### Patch
- Main output 1 -> lead voice trigger
- Inverted output 1 -> second oscillator trigger
- Send second oscillator through a different octave or interval

### Result
Every gap in the lead becomes an answering note. Great for contrapuntal melodic lines.

---

## Patch 5: Probabilistic ornament generator
### Patch
- Ch1 = steady main melody trigger source
- Ch2 = low-probability grace notes
- Ch3 = medium-probability transposition trigger
- Ch4 = rare reset of melody sequencer

### Result
A stable melodic line with occasional embellishments and phrase variation.

---

# How swing/assign helps melodic patches

The manual makes clear that the **Swing/Assign** control can be assigned to several functions, and multiple assigns can be active.

Possible melodic uses:

- **Swing**: add lilt to note timing
- **Assign to steps**: dynamically alter rhythmic cycle length, affecting phrase length
- **Assign to skip**: rotate patterns for melodic displacement
- **Assign to reset**: externally force phrase restarts
- **Assign via CV**: automate these changes with LFOs, envelopes, gates, or another sequencer

This is especially valuable for melodies because it lets you animate structure without repatching.

### Good trick
Feed gates into the Swing/Assign CV input after assigning **SKIP** or **RESET** to selected channels. Then another rhythmic source can periodically rotate or restart melodic timing patterns.

---

# Best companion modules for melody

The ADDAC402 works especially well with:

## Quantizers
To convert random or stepped CV into scale-locked melody.

## Sample & hold / track & hold
To capture new notes only when the 402 triggers them.

## Sequencers
Use the 402 to advance or reset them irregularly.

## Precision adders
For transposition controlled by one of the rhythm channels.

## Sequential switches
For selecting among pitch rows or melodic sources.

## Envelope generators and VCAs
To shape note articulation from gate patterns.

## Logic modules
Combine 402 outputs for more complex melodic triggers.

## Clock dividers/multipliers
To produce layered phrase structures around the 402 clock.

---

# Strongest musical roles for the ADDAC402 in a melodic system

## 1. Phrase rhythm designer
It decides when notes occur.

## 2. Melody structure modulator
It resets, rotates, and spaces melodic events.

## 3. Polyphonic trigger source
It runs multiple melodic voices at once.

## 4. Articulation engine
Gate/trigger mode changes note length behavior.

## 5. Generative composition core
In Game of Life, Pong, Probabilistic, and Euclidean modes, it can generate evolving musical timing that keeps melodies alive.

---

# Limitations to understand

To use it melodically, remember:

- It does **not directly output pitch CV**
- You will usually need:
  - a pitch source
  - a quantizer
  - or another sequencer
- Some modes are more useful for melody than others
- Footwork and Pong are more characterful than precise
- Gate Sequencer mode handles rhythm, not note values

So think of the 402 as the **rhythmic intelligence layer** of a melodic patch, not the complete melody module.

---

# Recommended melodic use ranking by mode

For most melodic applications, I’d rank the modes like this:

1. **Euclidean** — best all-around melodic rhythm source  
2. **Gate Sequencer** — best for manually composed melodic rhythms  
3. **Game of Life** — best for evolving generative melodies  
4. **Probabilistic** — best for variable melodic density  
5. **Pong** — best for playful semi-deterministic melodic motion  
6. **Golomb Rulers** — best for sparse abstract melodic accents  
7. **Footwork** — best for glitch/stutter melodic articulation  

---

# Bottom line

The ADDAC402 becomes a strong melodic module when you stop thinking of melody as just pitch and start thinking of it as:

- **event timing**
- **phrase length**
- **repetition vs variation**
- **density**
- **articulation**
- **reset behavior**
- **counterpoint between voices**

Used with quantizers, sample & holds, switches, and pitch sequencers, it can drive:

- arpeggios
- melodic canons
- generative lead lines
- probabilistic ornamentation
- contrapuntal voices
- evolving phrase structures

In a Eurorack system, this module is best seen as an **algorithmic rhythmic composer for melody**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)