# 2hp — Pitch

- [Manual PDF](../../manuals/2hp_Pitch.pdf)

---

[Manual PDF](https://www.twohp.com/modules/pitch)

# Using 2hp Pitch to create melodic components

From the attached manual, the module shown is:

- **2hp Pitch** — a **time-domain pitch shifter with wow & flutter**

It’s a compact utility/effect, but it can absolutely be used to generate or expand **melodic material** in a Eurorack patch. The manual also suggests pairings with:

- **2hp VCO**
- **2hp Loop**
- **2hp Play**
- **2hp Freez**

Below is a musician-focused analysis of how these can work together for melody, harmony, and tuneful textures.

---

## What 2hp Pitch does musically

2hp Pitch takes an incoming audio signal and shifts its pitch:

- **Pitch knob**: transposes the signal **up/down 2 octaves**
- **1V/OCT input**: adds CV control over pitch shift, tracking **1 octave further than the knob in either direction**
- **Mix knob / Mix CV**: blends **dry** and **wet**
- **W&F knob / W&F CV**: adds **wow and flutter**, i.e. random tape/turntable-style pitch fluctuation

### Key musical implication
This means Pitch is not just an “effect” — it can act like:

- a **harmony generator**
- an **octaver**
- a **parallel voice maker**
- a **lo-fi melody destabilizer**
- a way to derive **new pitched layers from a single source**

If you already have one melodic line, Pitch can turn it into two or more perceived melodic parts.

---

## Important I/O and ranges

From the manual:

- **Audio In / Audio Out**: **10 Vpp**
- **1V/OCT CV input**: **+5 V**
- **Mix CV input**: **+5 V**
- **W&F CV input**: **+5 V**

### Practical patching note
The **1V/OCT input** here is for controlling the **pitch shifting amount**, not turning Pitch into a standalone oscillator. So you’ll usually want to feed it:

- an oscillator
- a sample player
- a looper
- a frozen audio texture

Then use Pitch to derive musical intervals from that audio.

---

# Best ways to use it melodically

## 1. Turn one melody into harmony

This is the most immediate use.

### Patch
- Patch a melodic source into **Pitch IN**
  - e.g. VCO, sampled vocal, plucked voice, looped phrase
- Set **Mix** somewhere between dry and wet
- Tune the **Pitch** knob to an interval:
  - **+12 semitones** for octave up
  - **-12 semitones** for octave down
  - other positions by ear for fifths, fourths, etc.

### Result
You get:

- original melody = dry
- shifted copy = wet

This creates instant **two-part harmony** from a single monophonic source.

### Good musical uses
- octave doubling basslines
- fifth-above leads
- shimmer-like upper melodies
- thickened arpeggios

---

## 2. Use 1V/OCT to sequence interval changes

The manual states the **1V/OCT input tracks one octave further than the knob in either direction**. That means you can apply melodic or stepped CV to dynamically change the shift amount.

### Patch
- Send your audio source into Pitch
- Send a sequencer, quantized CV, or keyboard CV into **1V/OCT**
- Keep the dry/wet mixed

### Result
The shifted copy moves in musically related steps, creating:

- counter-melodies
- moving harmonies
- pseudo-duophonic lines from one source

### Why this is powerful
Instead of static transposition, the harmony itself can become animated. For example:

- root note dry
- wet signal follows a second sequencer lane of interval offsets

This gives the impression of two coordinated melodic voices.

---

## 3. Create octave melodies from non-oscillator sources

Pitch doesn’t care whether the source is a VCO or recorded audio. So you can make melodic content from:

- drum loops
- vocal chops
- sampled instruments
- frozen ambient textures

### Patch
- Feed **Play**, **Loop**, or **Freez** into Pitch
- Shift by octaves or intervals
- Blend dry/wet
- Optionally modulate **Mix CV** to bring in harmony only at certain moments

### Result
Even simple or noisy source material can become a recognizable melodic layer.

This is especially useful for:

- lofi hooks
- degraded leads
- ghost harmonies behind vocals
- tape-like chord fragments

---

# How it pairs with the modules mentioned in the manual

---

## 2hp VCO + 2hp Pitch

The manual explicitly says Pitch can turn one oscillator into two.

### Musical role
This is the cleanest way to build melodic material.

### Patch idea: single oscillator, dual melody
- **VCO OUT** → **Pitch IN**
- Sequence the **VCO** normally with your pitch CV
- Set Pitch:
  - **Mix** around 50%
  - **Pitch** to octave, fifth, or another consonant interval

### What you get
- one oscillator melody
- one pitch-shifted parallel voice

This can sound like:

- octave lead stack
- bass + upper melody
- faux interval duet

### Better still
If the VCO has multiple outputs, as the manual suggests, you can do more:

- send one VCO output dry to your mixer/filter/VCA chain
- send another output to Pitch
- separately process the shifted signal

Now the original and shifted voices can have different:

- filters
- envelopes
- effects
- stereo positions

That turns one oscillator into a much richer melodic instrument.

### Melodic applications
- **Octave bass reinforcement**
- **Fifth-above acid line**
- **Detuned lead-like motion** using subtle W&F
- **Call-and-response phrasing** by modulating Mix CV

---

## 2hp Loop + 2hp Pitch

The manual notes Pitch works well before or after Loop.

This is very important, because **order changes the musical behavior**.

---

### A. Pitch before Loop

#### Patch
- Source → **Pitch** → **Loop**

#### What happens
You record the already-shifted material into Loop.

#### Musical use
This is great when you want to:

- build harmonized overdubs
- record lofi transposed phrases
- capture unstable wow/flutter melodies as part of the loop itself

#### Melodic outcome
You can perform with the Pitch controls while recording into Loop, then capture:

- rising pitch gestures
- harmonized phrases
- tape-warbled motifs

This is good for evolving melodic ostinatos.

---

### B. Pitch after Loop

#### Patch
- Source → **Loop** → **Pitch**

#### What happens
Loop stores the original phrase, and Pitch transforms playback.

#### Musical use
This is better for:

- re-harmonizing the same loop in real time
- making one loop serve multiple harmonic roles
- changing octave placement live

#### Melodic outcome
A single recorded phrase can become:

- bassline
- countermelody
- octave shimmer
- degraded warped hook

This is especially strong in live sets because one recorded line can be repurposed across sections.

---

### Best melodic strategy with Loop + Pitch
Record a simple monophonic phrase into Loop, then use Pitch to create:

- octave-up choruses
- lower bass doubles
- unstable cassette-like repeats with W&F
- interval changes via 1V/OCT for evolving harmonies

---

## 2hp Play + 2hp Pitch

The manual highlights sample processing as a major strength.

### Musical role
This combo is excellent for creating melody from audio that wasn’t originally melodic.

### Patch
- **Play OUT** → **Pitch IN**
- Use Play for:
  - vocal samples
  - plucks
  - synth notes
  - drum fragments
  - found sound snippets

### Musical results
Pitch can transform sample playback into:

- pitched vocal hooks
- octave-stacked stabs
- eerie detuned melodies
- tuned glitch motifs

### Strong melodic use cases

#### 1. Vocal lead creation
- Put a short vocal phrase in Play
- Send it to Pitch
- Blend dry/wet
- Add a small amount of W&F

Result: a tape-like doubled vocal lead.

#### 2. Tuned percussion melody
- Use short percussive samples in Play
- Pitch shift them to different registers
- Sequence the shift amount through 1V/OCT

Result: a strange but musical pseudo-melodic percussion line.

#### 3. Harmonic sample layering
- Trigger one sample from Play
- Use Pitch to make a transposed layer
- Modulate Mix CV so the harmony only appears on some notes

Result: accents and hooks that feel composed, not static.

---

## 2hp Freez + 2hp Pitch

The manual describes this as an “ultimate lo-fi combo.”

### Musical role
Freez likely provides held or frozen audio slices, while Pitch turns those static textures into playable melodic material.

### Patch
- **Freez OUT** → **Pitch IN**
- Freeze a harmonic or noisy moment
- Use Pitch to transpose it

### Musical result
You can derive:

- drones with melodic movement
- pad-like intervals
- frozen grains that become tonal centers
- haunted lead tones

### Why this works
Freez gives you a sustained sound bed; Pitch gives you register and interval control. Together they can create melody from otherwise static audio.

### Patch approaches

#### 1. Frozen drone melody
- Capture a frozen sound
- Send to Pitch
- Use 1V/OCT to step through melodic transpositions

Result: a melody made from one sustained frozen timbre.

#### 2. Lo-fi chord illusion
- Use dry + wet mix
- Shift by octave or consonant interval
- Add some W&F

Result: a chorusy, degraded chord-like layer from one frozen source.

#### 3. Unstable ambient lead
- Freeze a bright source
- Shift upward
- Apply moderate wow/flutter

Result: wavering melodic lines with strong cassette/tape character.

---

# The role of Wow & Flutter in melody

The manual defines wow and flutter as pitch wavering caused by irregular playback speed. On this module, W&F introduces **random fluctuation** into the shifted signal.

## Musically, this is not just “vintage flavor”
It changes how a melody behaves.

### At low settings
You get:

- gentle detune
- chorusing feel
- tape softness

This is useful for:
- making doubled melodies wider
- making octave layers less sterile
- adding movement to sustained melodic notes

### At medium settings
You get:

- drifting intonation
- unstable harmonies
- seasick cassette character

Useful for:
- ambient leads
- Boards-of-Canada-style motifs
- nostalgic sampled melodies

### At high settings
You get:

- more random pitch instability
- less precise harmony
- expressive degradation

Useful for:
- broken tape melodies
- haunted loops
- unstable melodic textures rather than exact interval work

### Best practice
If you want clearly tonal melodic parts:

- keep **W&F low**
- use it more as a “humanizing” or “aging” layer

If you want more expressive lo-fi character:

- raise W&F on sustained notes or loops
- modulate it with CV for transitions

---

# Melodic patch recipes

## 1. Simple octave lead
**Goal:** make a lead line bigger

- VCO or sample source → Pitch
- Pitch knob: **+1 octave**
- Mix: **50–70% wet**
- W&F: low

**Result:** clear octave doubling for lead melodies.

---

## 2. Bass + upper voice from one sequence
**Goal:** derive two melodic registers from one line

- Oscillator sequence → split signal
- One copy dry to mixer
- One copy to Pitch
- Set Pitch to **+1 octave** or **+5th**
- Pan dry and wet separately if possible

**Result:** one sequenced line becomes a layered melodic part.

---

## 3. Evolving harmonized loop
**Goal:** create a melodic motif that changes over time

- Record phrase into Loop
- Loop out → Pitch
- Send stepped CV into Pitch **1V/OCT**
- Modulate Mix CV slowly

**Result:** the same phrase continuously re-harmonizes.

---

## 4. Lo-fi sample hook
**Goal:** create a memorable melodic motif from samples

- Play sample → Pitch
- Set Mix around halfway
- Add medium W&F
- Trigger sample rhythmically

**Result:** warped doubled sample hooks with melodic identity.

---

## 5. Frozen ambient melody
**Goal:** turn a drone into notes

- Freez captures sustained sound
- Freez out → Pitch
- Sequencer or keyboard CV → Pitch 1V/OCT
- Low-to-medium W&F

**Result:** a playable melodic voice from frozen audio.

---

# Performance strategies

## Use Mix CV for arrangement
The manual gives a dedicated **Mix CV input**. This is great for performance.

You can use Mix CV to:

- bring harmony in only on choruses
- make every fourth note bloom into a double
- create transitions from monophonic to harmonized material

This is one of the best ways to keep melodic patches dynamic.

---

## Sequence Pitch intervals, not just notes
A powerful idea is:

- one sequencer controls the original melody
- another CV lane controls Pitch’s 1V/OCT interval movement

This creates structured harmony motion without needing a second voice architecture.

---

## Add W&F only where emotion is needed
Use W&F sparingly for:

- phrase endings
- sustained notes
- intros and breakdowns

That keeps the melody intelligible while still giving you character.

---

# Strengths and limitations for melodic use

## Strengths
- Makes **instant harmonies** from any audio source
- Great for **octaves, interval doubling, and lo-fi melodic coloration**
- Works with **oscillators, loops, samples, and frozen textures**
- CV over **pitch shift, mix, and wow/flutter** adds movement
- Excellent in very small systems because it multiplies the usefulness of one sound source

## Limitations
- It is still fundamentally an **audio processor**, not a complete melodic voice by itself
- For clean tonal harmony, settings may need to be tuned by ear
- Heavy wow/flutter can reduce pitch precision
- Best results come when paired with a stable source and external sequencing

---

# Best overall melodic use cases

If your goal is to create melodic components, the strongest combinations from the manual are:

## Best for clean melodic harmony
- **VCO + Pitch**

## Best for evolving melodic phrases
- **Loop + Pitch**

## Best for hooks and sample melody
- **Play + Pitch**

## Best for ambient/lo-fi melodic textures
- **Freez + Pitch**

---

# Conclusion

Based on the manual, **2hp Pitch** is best thought of as a **melodic multiplier**. It takes one sound source and turns it into:

- harmony
- octave reinforcement
- counter-lines
- degraded tape-like melodic textures

Used with the suggested pairings:

- **VCO** gives you classic melodic doubling and interval harmony
- **Loop** gives you repeatable phrases that can be re-harmonized
- **Play** gives you pitched sample hooks and tuneful texture
- **Freez** gives you frozen material that can be shaped into melodic drones and leads

If you want the most musically useful results, start with:
1. a simple melodic source,
2. Pitch mixed 50/50,
3. low wow/flutter,
4. then add CV to **1V/OCT** and **Mix** for motion.

That will get you from “effect module” territory into genuinely expressive melodic patching very quickly.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)