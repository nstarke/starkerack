# Omnitone — Beatsi

- [Manual PDF](../../manuals/Beatsi_Information_Package.pdf)

---

[Beatsi Manual PDF](attachment)

# Using Beatsi to Create Melodic Components

Beatsi is primarily a **digital drum synth voice**, not a dedicated melodic oscillator. But as a eurorack musician, I’d absolutely still use it for **pitched percussion, tuned tom lines, pseudo-basslines, and animated tonal textures**. Its architecture gives you enough pitch control and CV assignment flexibility to pull melodic material out of a drum module.

## What the module gives you

Beatsi has 5 drum voices:

- Kick
- Snare
- Hi-hat
- Tom
- Crash

Each piece has controllable:

- **Timbre**
- **Pitch**
- **Decay**
- **Level**

It also provides:

- **Two assignable CV inputs**: CV1 and CV2
- Per-parameter **attenuversion**
- **Tom CV input** with **V/Oct** behavior for pitch
- Smoothly morphing timbres within 3 kits:
  - **Orange** = acoustic/basic
  - **Blue** = lo-fi
  - **Green** = alien

## Most melodic use: the Tom voice

The **Tom** is the clearest path to melody because it has a dedicated **TOM CV** input labeled for **Pitch (V/Oct)**.

### Why this matters
That means you can patch a sequencer, keyboard, quantizer, or precision CV source into the Tom and play it as a tuned percussion voice.

### Patch idea: tuned tom melody
- Send a trigger sequence into **TOM**
- Send 1V/Oct pitch CV from a sequencer into **TOM CV**
- Set **Decay** medium to long
- Tune **Pitch** to a musically useful base range
- Adjust **Timbre** until it behaves more like a conga, bongo, electronic tom, or synthetic pluck

This gives you:
- melodic tom riffs
- tuned tribal patterns
- marimba-like synthetic percussion
- bass-percussion lines

If the timbre is clean and the decay is short, it can act like a **pitched pluck**. With longer decay, it can become a **percussive lead**.

## CV-mapped pitch modulation on other voices

The manual says any parameter can be assigned to **CV1** or **CV2**, and specifically notes:

> If a pitch parameter is assigned to a CV source, it will follow the v/oct protocol if the attenuverting settings are at gain of 1.

That is a big deal.

## What this means musically
You can potentially make **Kick, Snare, Hi-hat, Tom, or Crash pitch track melodically**, as long as:
- you assign that voice’s **Pitch** parameter to CV1 or CV2
- set attenuversion to **+1 gain**
- feed proper pitch CV into that CV input

So Beatsi is not just one melodic voice—it can become a **multi-part tuned percussion system**.

## Patch idea: tuned drum ensemble
- Assign **Kick Pitch** to CV1
- Assign **Snare Pitch** to CV1
- Assign **Tom Pitch** to CV1 or use TOM CV
- Send a quantized melodic sequence to CV1
- Trigger each voice with different rhythmic gates

Result:
- Kick plays the root note
- Tom plays the fifth or melody accents
- Snare becomes a tuned electro-snare stab
- Crash/hat can become metallic tuned punctuation

This works especially well for:
- IDM
- electro
- minimal techno
- gamelan-like percussion lines
- experimental tonal rhythm

## Best voices for melodic use

### 1. Tom
Best for:
- basslines
- tuned percussion
- plucks
- melodic ostinatos

### 2. Kick
Useful for:
- sub-bass pulses
- acid-adjacent low percussion
- tuned thumps

A kick with longer decay and stable pitch can work as a **bass voice**, especially in sparse arrangements.

### 3. Snare
Useful for:
- tuned zaps
- rimshot-like stabs
- pitched noise hits

This won’t be “melodic” in a pure sine-wave way, but in the right patch it creates very musical tonal accents.

### 4. Hi-hat and Crash
Useful for:
- metallic tuned textures
- pseudo-chords through resonance implication
- high-register tonal punctuation

These are more useful for **atonal or inharmonic melodic color** than conventional notes.

## Timbre morphing as melodic expression

Because timbres blend smoothly within each kit, and rolling past the ends changes kits, you can use **Timbre** almost like a wavetable position or macro tone control.

That means melody doesn’t have to come only from pitch. You can create **melodic phrasing through timbral movement**.

### Patch idea: timbre melody
- Keep pitch static or simple
- Sequence **Timbre** via CV1 or CV2
- Trigger the same voice repeatedly
- Use different timbre zones as if they were different “notes”

This works especially well on:
- Tom
- Snare
- Hi-hat

In a mix, changing timbre per step can read like a melodic phrase even if the pitch is barely moving.

## Decay as a phrase-shaping tool

The **Decay** parameter can also create the impression of melody by changing note length and resonance.

### Example
For a tom melody:
- short decay on passing notes
- long decay on phrase endings
- medium decay on accented steps

This makes the pattern feel composed rather than mechanical.

If Decay is CV-controlled, you can create:
- call-and-response phrases
- accents
- ratcheted-sounding dynamic contours
- pseudo-legato vs staccato behavior

## Hi-hat as a melodic gate voice

The manual notes that the **Hi-hat input accepts trigger/gate**, and the decay starts on the **falling edge** of the gate/trigger.

That means you can shape open/closed hat behavior with gate length. While this is mainly rhythmic, it also gives a way to make upper-register tonal gestures.

### Musical use
If you tune the hi-hat pitch through CV assignment:
- short gates = closed, tight bright ticks
- long gates = open metallic sustained notes

This can create:
- high melodic counterlines
- shimmering ostinatos
- pseudo-arpeggios in the treble

## Using the kits for harmonic role

The three kits can be treated as different tonal vocabularies.

### Orange kit
Best for:
- natural tuned drums
- grounded bass/percussion lines
- acoustic-ish melodic support

### Blue kit
Best for:
- chiptune-like percussion
- lo-fi leads
- crunchy bass motifs
- stepped digital melodies

### Green kit
Best for:
- alien plucks
- unstable lead percussion
- strange metallic tonal gestures
- sci-fi counter-melody

Switching kits via Timbre rollover is especially useful for performance. A phrase can move from acoustic to synthetic to alien while preserving the same trigger structure.

## Using CV1 and CV2 musically

Since multiple parameters can be assigned to a single CV source simultaneously, one CV can create complex “melodic macros.”

## Patch idea: one sequencer, many destinations
Send a sequenced CV into **CV1**, then assign it to:
- Tom Pitch
- Tom Timbre
- Kick Pitch
- Snare Decay

Now one melodic line controls:
- note pitch
- brightness
- low-end support
- accent shape

That’s a very modular way to get a whole drum system to “sing” together.

## Great companion modules for melodic use

If using Beatsi in a larger melodic eurorack patch, pair it with:

- **Quantizer**: to keep pitch-based modulation musical
- **Sequencer**: for TOM CV or assigned pitch CV
- **Precision adder / offset**: to transpose drum melodies
- **Envelope or function generator**: to animate timbre/decay
- **Sample & hold / random CV**: for generative tuned percussion
- **Filter or LPG after the output**: to carve tones into more clearly melodic shapes
- **Delay/reverb**: to turn percussive notes into ambient melodic material

## Important limitation

Beatsi has only **one mixed output** listed in the manual:
- **OUT**: all sounds are output here

So if multiple voices are triggered at once, their pitches and tonal identities will blend in the same output. That is fine for melodic percussion ensembles, but it means:
- less control over separate processing
- melodic clarity is best when arrangements are sparse
- the Tom is the cleanest dedicated melodic lane

## Best practical melodic strategies

## 1. Use Tom as your main melodic voice
This is the easiest and strongest option.

## 2. Use Kick as tuned bass
Short sequence, low register, restrained decay.

## 3. Use CV assignment to pitch-track other drum voices
Great for electro and experimental styles.

## 4. Sequence Timbre, not just Pitch
This creates melodic identity even with noisy sounds.

## 5. Keep arrangements sparse
Because of the summed output, fewer simultaneous voices means stronger note definition.

## 6. Use external quantization
Especially if using CV1/CV2 for pitch duties.

## Example full melodic patch

### “Tuned percussion groove”
- Trigger sequencer to:
  - Kick on 1 and 9
  - Snare on 5 and 13
  - Tom on a 16-step melody
  - Hi-hat on offbeats
- Pitch sequencer to **TOM CV**
- CV1 from quantizer assigned to:
  - Kick Pitch
  - Snare Pitch
- CV2 from slow triangle LFO assigned to:
  - Tom Timbre
  - Snare Decay
  - Hi-hat Timbre

### Result
- Tom carries melody
- Kick reinforces root movement
- Snare adds tuned accents
- Hi-hat provides animated top-end color
- Timbres evolve across the pattern for a living melodic rhythm section

## Bottom line

Beatsi is a drum module first, but it can absolutely be used for **melodic percussion synthesis**. The strongest melodic tools are:

- **Tom CV input for V/Oct melodic control**
- **Assignable CV over pitch on other voices**
- **Smooth timbre morphing**
- **Decay shaping for phrase articulation**
- **Three kits that act like different tonal palettes**

In practice, I’d treat it as a **compact tuned percussion ensemble** capable of:
- basslines
- tom melodies
- tuned drum riffs
- metallic counter-melodies
- animated electro percussion hooks

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)