# 2hp — Blur

- [Manual PDF](../../manuals/2hp_Blur.pdf)

---

[Manual PDF](https://www.twohp.com/modules/blur)

# 2hp Blur — using it with other modules for melodic music

Based on the manual, **2hp Blur** is a **spectral processor** that can turn short, harmonically rich sounds into stretched, smeared, pad-like material. It is not a pitch source by itself, but it is very useful for creating **melodic layers, sustained harmonic beds, and transformed lead voices** when paired with oscillators, voices, or pitch-related modules.

## What Blur does musically

Blur has:

- **Audio In / Out**
- **Time** knob + CV  
  - At far left: shorter, quicker playback
  - Center: roughly original playback speed
  - Far right: stretched up to **16x**
- **Vibe** knob + CV  
  - Low: timbre stays close to the input
  - High: the sound spreads into a washed, reverb-like spectral pad
- **Mix** knob + CV  
  - Dry/wet blend

### Musical implication
Blur is best thought of as a **melody transformer**:
- it can turn **plucks into pads**
- make **single-note lines bloom into ambient tails**
- smear **chords or intervals into harmonic textures**
- create **sustained accompaniment** from short melodic material

---

## The module pairings from the manual and how they help melodic writing

The manual suggests pairing Blur with:

- **2hp Pluck**
- **2hp Pitch**
- **2hp Swarm**
- **2hp Verb**

Below is how each pairing contributes to melodic components.

---

## 1. Blur + Pluck: turning notes into melodic ambience

The manual specifically says **Pluck** is a great candidate because it produces **sharp transients and intriguing harmonics** that Blur can turn into a wash.

### Why this works
Pluck likely gives you:
- a clearly pitched sound
- a strong attack
- rich harmonics

That is perfect input for Blur, because Blur’s spectral processing has something harmonic to stretch and smear.

### Melodic use cases
#### A. Pad from a sequence
Patch:
- Sequencer CV -> **Pluck V/OCT**
- Gate/trigger -> **Pluck TRIG**
- **Pluck OUT -> Blur IN**
- **Blur OUT -> mixer/output**

Set:
- **Time** around 1–3 o’clock for longer note bloom
- **Vibe** around noon to high for harmonic spreading
- **Mix** to taste

Result:
- Your sequenced pluck becomes a **soft sustained melodic bed**
- Good for ambient, downtempo, soundtrack, intro sections

#### B. Ghost harmony behind an arpeggio
Use a fast arpeggio into Pluck, then process through Blur with:
- medium-high **Time**
- medium **Vibe**
- wet-heavy **Mix**

Result:
- the original rhythm can disappear into a **harmonic cloud**
- useful as a background layer under a dry lead voice

#### C. Expressive call-and-response
If you can modulate Blur:
- use CV into **Time CV** or **Vibe CV**
- lower the mix for verses, raise it for transitions

Result:
- same melody can alternate between **defined plucks** and **blurred sustain**

### Best melodic role
- accompaniment
- harmonic wash
- supportive countermelody layer

---

## 2. Blur + Pitch: playable blurred melodies

The manual explicitly recommends putting **Pitch after Blur**:
> Pitch shift your blurred spectral signal ... turn any audio source into a v/oct tracking bed of sound.

This is probably the most directly melodic pairing in the document.

### Why this works
Blur creates:
- sustained spectral material
- a harmonically rich signal

Pitch then allows that material to be:
- shifted melodically
- played as a pitched voice
- tracked with **V/Oct**

### Patch idea
- Sound source or Pluck -> **Blur IN**
- **Blur OUT -> Pitch IN**
- Sequencer CV -> **Pitch V/OCT**
- **Pitch OUT -> mixer/output**

### Melodic use cases
#### A. Turn texture into a lead
Feed any harmonically rich source into Blur, then into Pitch.

Set Blur for:
- center to high **Time**
- medium/high **Vibe**

Then sequence **Pitch** melodically.

Result:
- an ethereal, sustained, pitch-tracked voice
- useful for leads that feel halfway between synth and sampled choir

#### B. Harmonized drones
Use a static or repeating input into Blur and sequence only a few notes in Pitch.

Result:
- a drone can become a **slow melody line**
- excellent for modal or minimal composition

#### C. Layered intervals
If you mult the source:
- dry source to one mixer channel
- blurred + pitch-shifted source to another

Tune Pitch to:
- octave
- fifth
- third, if the patch tolerates it

Result:
- instant melodic doubling or pseudo-harmony

### Best melodic role
- lead voice
- octave/interval support
- playable ambient top line

---

## 3. Blur + Swarm: lush melodic oscillator textures

The manual says **Swarm**’s hyper-saws and pulse waves are ideal for Blur to smear.

### Why this works
Swarm likely generates:
- very rich harmonic content
- supersaw-like density
- synth-friendly stable pitch

Blur turns that into:
- lush sustained pads
- softened chordal or monophonic textures
- evolving melodic timbres

### Melodic use cases
#### A. Big mono lead
Patch:
- Sequencer CV -> **Swarm pitch/freq**
- **Swarm OUT -> Blur IN**
- **Blur OUT -> output**

Set:
- lower **Vibe** for clearer pitch definition
- moderate **Time**
- moderate **Mix**

Result:
- melodic clarity remains, but the edges soften
- great for cinematic melodies

#### B. Pad bass or low-register melody
Sequence Swarm in a lower octave and use Blur conservatively.

Result:
- bass notes gain body and sustain
- useful for slow melodic basslines

#### C. Chord illusion from single notes
Because Blur spreads spectral content, a rich single oscillator voice can feel wider and more chord-like.

Result:
- monophonic melodic lines feel larger and more harmonically complex

### Performance tip
For melody, don’t always max **Vibe**.  
Too much can reduce note definition. For articulate melodic parts:
- **Vibe low to medium**
- **Time medium**
- **Mix around 30–60% wet**

### Best melodic role
- lush lead
- melodic bass texture
- pad-like mono voice

---

## 4. Blur + Verb: expanding melodic space

The manual suggests using **Verb** to make Blur even bigger, and notes that because Verb is stereo, two Blurs could be used before or after it.

### Why this matters melodically
Verb doesn’t create melody, but it helps place melodic material in space.

### Use cases
#### A. Blur before Verb
Patch:
- voice -> **Blur -> Verb**

Result:
- Blur shapes the harmonic smear first
- Verb adds room/stereo depth afterward
- best for **pads, melodic washes, sustained hooks**

#### B. Verb after a melodic lead
A dry melody can be layered with a blurred-then-reverbed duplicate.

Result:
- the dry signal keeps note definition
- the wet chain creates emotional size

#### C. Two-Blurs-into-Verb concept
The manual mentions using **2 Blurs** with stereo Verb.

Possible approach:
- Left melodic source -> Blur 1
- Right melodic source or duplicate -> Blur 2
- Both into Verb stereo inputs

Result:
- wide stereo melodic pad field
- especially useful if you have two related sequences or interval voices

### Best melodic role
- spatial enhancement
- ambient accompaniment
- stereo widening of melodic material

---

# Practical melodic patch recipes

## Patch 1: Plucked melody into ambient pad
**Goal:** convert a simple sequence into a sustained melodic layer

Patch:
- Sequencer CV -> **Pluck V/OCT**
- Trigger pattern -> **Pluck TRIG**
- **Pluck OUT -> Blur IN**
- **Blur OUT -> mixer**

Blur settings:
- **Time:** 2 o’clock
- **Vibe:** 1–3 o’clock
- **Mix:** 60–80% wet

Musical result:
- notes retain pitch center
- phrase becomes legato and atmospheric
- ideal under vocals or another lead

---

## Patch 2: Ambient lead with pitch tracking
**Goal:** playable blurred lead voice

Patch:
- Oscillator/Pluck/Swarm -> **Blur IN**
- **Blur OUT -> Pitch IN**
- Sequencer keyboard CV -> **Pitch V/OCT**
- **Pitch OUT -> mixer**

Settings:
- **Blur Time:** noon to 2 o’clock
- **Blur Vibe:** noon
- **Blur Mix:** 50–70%

Musical result:
- smooth and melodic
- less percussive than the original source
- good for hooks and slow lead lines

---

## Patch 3: Dry melody + blurred melodic shadow
**Goal:** keep note clarity while adding emotion

Patch:
- Voice output multed to:
  - mixer channel 1 dry
  - **Blur IN** on channel 2
- Blend dry and Blur return externally or with Blur’s own Mix

Settings:
- **Time:** medium-high
- **Vibe:** medium
- **Mix:** moderate

Musical result:
- clear main melody
- blurred tail acts like a harmonic shadow
- excellent for melodic techno, ambient house, filmic electronica

---

## Patch 4: Swarm pad melody
**Goal:** lush synth melody

Patch:
- Sequencer CV -> **Swarm pitch**
- **Swarm OUT -> Blur IN**
- **Blur OUT -> Verb IN** if available
- **Verb OUT -> mixer**

Settings:
- **Vibe:** low-medium for pitch clarity
- **Time:** medium-high
- **Mix:** 40–70%

Musical result:
- supersaw-style melodic line becomes polished and cinematic
- can function as the main musical statement in sparse arrangements

---

# CV strategies for more expressive melodies

Blur has CV over:
- **Time**
- **Vibe**
- **Mix**

All CV inputs accept **-5V to +5V**.

## Good modulation ideas
### 1. Modulate Mix by phrase section
- lower mix during busy passages
- increase mix at phrase endings

This makes melodies “open up” musically.

### 2. Modulate Time slowly
A slow LFO or envelope into **Time CV** can make notes stretch differently over time.

Effect:
- evolving sustain
- less repetitive melodic loop feel

### 3. Modulate Vibe with dynamics
If you have a related modulation source, push **Vibe** higher on accented notes.

Effect:
- certain melody notes bloom more than others
- very expressive in slow lines

---

# Best practices if you want clearly melodic results

Because Blur is a spectral smearing effect, it can reduce pitch definition if pushed too far. For melodies:

## Keep pitch recognizable by:
- starting with a **strongly pitched source**
- using **moderate Vibe** instead of maximum
- keeping **Time near center to moderate stretch**
- blending some **dry signal** with Mix

## Push it further when you want:
- pads instead of leads
- harmonic fog
- transitions, breakdowns, intros, outros

---

# Installation / technical notes from the manual

## Specs
- **Width:** 2HP
- **Depth:** 46mm
- **Power:** +12V = 85mA, -12V = 7mA, +5V = 0mA

## Signal ranges
- **Audio In:** 10Vpp
- **Audio Out:** 10Vpp
- **Time CV / Vibe CV / Mix CV:** -5V to +5V

## Power cable note
For 2hp modules, the red stripe on the ribbon should align with the **white marker line** on the PCB above the power header.

---

# Overall musical takeaway

**2hp Blur is best used as a melodic enhancer rather than a melody generator.**  
It excels at turning:
- **Pluck** into ambient pitched textures
- **Swarm** into lush melodic pads/leads
- **Pitch** into a way to make blurred material track musically
- **Verb** into the final spatial polish for melodic beds

If your goal is to build melodic components, Blur is especially strong for:

- **sustained harmony from short notes**
- **cinematic lead textures**
- **background melodic layers**
- **pitch-shifted ambient voices**
- **melodic transitions and phrase tails**

In a patch, I’d think of it as the module that gives your notes **memory and atmosphere**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)