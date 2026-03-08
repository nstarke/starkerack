# SSF — Autodyne

- [Manual PDF](../../manuals/Autodyne - Steady State Fate.pdf)

---

# [Autodyne manual / product page](https://steadystatefate.com/products/autodyne)

From the material provided, only **one module** is documented here: **Steady State Fate Autodyne**. So I can’t analyze inter-module patch relationships from multiple manuals, but I *can* explain how **Autodyne** can be used **with other Eurorack building blocks** to create and shape **melodic components**.

## Module identified
- **Steady State Fate Autodyne**
  - 4hp
  - Auto-compressor / distortion
  - Parallel compression blend
  - Switchable sidechain filter
  - External sidechain input
  - Designed for clean-to-character dynamics control

## What Autodyne does musically
Autodyne is **not a pitch source, oscillator, sequencer, or quantizer**. It won’t generate melodies by itself. Instead, it is a **dynamics and tone-shaping module** that helps melodic parts become:
- more present
- more even in level
- punchier
- more saturated
- more expressive
- more mix-ready

That means it works best **after** a melodic voice or **on a melodic bus**.

## Core controls and how they affect melodic material

### COMP
According to the page, **ratio, threshold, and gain behavior are combined into one control**.
- **Below center**: gentler compression, more traditional leveling
- **Past center**: more aggressive compression
- Useful for:
  - evening out inconsistent note levels
  - adding sustain to plucks
  - gluing legato phrases
  - making arpeggios feel more “forward”

### GAIN
This trims output level, but can also push into **heavy distortion**.
- Low/moderate use: compensates level after compression
- High use: adds harmonics and aggression
- Useful for melody:
  - brighten dull waveforms
  - add edge to leads
  - turn simple sine/triangle voices into more audible foreground lines

### BLEND
Parallel compression mix between dry and compressed signal.
- Minimum: effectively bypasses compression
- Increasing blend: mixes in compressed character
- Very useful for melodic work because you can:
  - keep transients from a pluck
  - add body/sustain underneath
  - preserve articulation while increasing density

### Side Chain Filter
The sidechain can be filtered with a **high-pass response** so low frequencies don’t over-trigger compression.
- This matters if your melodic line has:
  - strong bass content
  - resonant low mids
  - filter sweeps
- For melody, this helps compression react more to the **articulation and upper tone** rather than low-end energy.

### External Side Chain Input
An external signal can drive the compressor detector.
- This opens up rhythmic and phrase-shaping possibilities for melodic lines:
  - duck melodies under kick
  - pulse a drone with a trigger pattern
  - shape a sustained lead from an unrelated rhythmic source

---

## Best ways to use Autodyne for melodic components

## 1. Make a plucked sequence sound bigger
**Patch idea**
- VCO → VCF → VCA/envelope → **Autodyne** → mixer
- Use a sequencer + quantizer for pitch

**Settings**
- COMP: just below or around noon
- BLEND: 10–1 o’clock
- GAIN: unity or slight boost

**Result**
- Short notes gain body and sustain
- Quiet notes become more audible
- The sequence feels more polished without losing attack

This is especially good for:
- acid-style lines
- marimba/pluck voices
- filtered saw arpeggios

---

## 2. Turn a simple oscillator line into a lead
If your melodic voice is too plain:
- oscillator → wavefolder/filter → VCA → **Autodyne**
- push **GAIN** for harmonic enhancement
- add some **COMP** and a moderate **BLEND**

**Result**
- more upper harmonics
- greater perceived loudness
- lead cuts through a mix better

This works well on:
- triangle leads
- sine FM lines
- softly filtered saws

---

## 3. Add sustain to sparse melodies
Some melodic phrases feel too thin when notes decay quickly.

**Patch**
- voice → **Autodyne** → delay/reverb

**Settings**
- COMP above noon
- BLEND moderate
- GAIN adjusted to match output

**Result**
- note tails become more audible
- sustained ambience feeds delay/reverb more evenly
- melodic phrases sound more connected

This is useful for:
- ambient sequences
- slow generative melodies
- fragile west-coast style plucks

---

## 4. Use parallel compression to keep articulation
Autodyne’s **BLEND** is especially useful for melody because fully compressed melodic material can lose expression.

**Approach**
- Start with stronger compression than you think you need
- Then back off with **BLEND**

**Why**
- dry path preserves note attack and pitch clarity
- compressed path adds body and sustain

**Result**
- melodic line stays expressive
- dynamics become controlled
- phrase remains intelligible in dense arrangements

This is one of the strongest uses of Autodyne on melodic voices.

---

## 5. Create rhythmic melodic pumping with external sidechain
**Patch**
- melodic voice audio → Autodyne IN
- kick drum, trigger-derived envelope, or percussion bus → sidechain input

**Result**
- the melodic line ducks rhythmically
- sustained notes become animated
- static harmonies feel syncopated

For melodic music, this can make:
- pads pulse with groove
- basslines stay out of the kick’s way
- drones become rhythmically musical

If using a kick as sidechain:
- enable sidechain filtering as needed
- tune response by ear so ducking supports the groove rather than flattening the phrase

---

## 6. Keep bass melodies controlled
For bass melodies or low-register sequenced lines, compression can overreact to the fundamental. The **sidechain filter** is important here.

**Patch**
- bass voice → Autodyne
- sidechain filter engaged

**Result**
- compression responds less to huge low-end swings
- pitch definition improves
- bass melody stays firmer and more even

Great for:
- sequenced monosynth bass
- low LPG plucks
- resonant filter bass phrases

---

## 7. Add “glue” to a layered melodic bus
If you have multiple melodic voices mixed together externally or through a submixer:
- lead + countermelody + arpeggio → submix → **Autodyne**

**Result**
- parts feel like one musical object
- peaks are controlled
- harmonic density increases

This is probably the most “studio-like” use:
- one module can make several melodic layers feel unified

---

## How Autodyne fits in a melodic signal chain

## A. After the full voice
**Typical melodic use**
- pitch CV → oscillator → filter → VCA → **Autodyne**

Best when you want:
- overall note leveling
- sustain
- character
- final polish

## B. Before time effects
- voice → **Autodyne** → delay/reverb

Best when you want:
- more consistent sends into effects
- richer echoes
- smoother ambient tails

## C. On a melodic subgroup
- several voices → mixer → **Autodyne** → final mix

Best when you want:
- ensemble cohesion
- “glue”
- bus compression flavor

---

## Pairing ideas with common module types

Even though only Autodyne is shown, here’s how it works with typical melody-generating modules:

### With sequencers
Use sequencers for pitch and rhythm, then Autodyne to:
- even note accents
- increase sustain on short gate patterns
- make step sequences feel more finished

### With quantizers
Quantizers produce stable pitch structure; Autodyne helps those pitches feel:
- more connected
- louder in a mix
- more expressive dynamically

### With oscillators
Autodyne can make oscillator voices:
- more harmonically rich via gain/distortion
- more stable in level via compression
- more lead-like via saturation

### With filters
After a resonant filter, Autodyne can tame peaks and emphasize tone.
Useful when:
- resonance causes some notes to jump out
- envelope sweeps are too uneven
- filter pings need more body

### With VCAs and envelopes
VCA + envelope create the articulation; Autodyne reshapes the result.
- fast envelope + Autodyne = punchy plucks with more density
- long envelope + Autodyne = smoother, sustained melodic lines

### With wavefolders / distortion
Autodyne after tone-shaping can help manage wild dynamics.
- folded timbres often vary a lot in level
- compression makes them more playable melodically

---

## Practical melodic patch recipes

## Patch 1: Compressed analog lead
- Quantizer/sequencer → VCO pitch
- VCO saw → lowpass filter
- Envelope → filter + VCA
- VCA out → **Autodyne** → reverb

**Autodyne**
- COMP: 1 o’clock
- GAIN: slight boost
- BLEND: noon

**Sound**
- stable, present mono lead with body and sustain

---

## Patch 2: Rhythmic ducked pad melody
- Oscillator chord or pad voice → VCA → **Autodyne**
- Kick or trigger envelope → sidechain input

**Autodyne**
- COMP: noon to 2 o’clock
- BLEND: to taste
- Sidechain filter: experiment based on trigger source

**Sound**
- breathing/pumping harmonic bed with strong groove

---

## Patch 3: Distorted bass melody
- Sequencer → quantizer → bass oscillator
- Filter → VCA → **Autodyne**

**Autodyne**
- COMP: moderate
- GAIN: pushed into character/distortion
- BLEND: retain some dry signal
- Sidechain filter: on

**Sound**
- aggressive but controlled bass sequence with better note consistency

---

## Patch 4: Glue for arpeggio + lead
- Arp voice and lead voice into mixer
- Mixer out → **Autodyne** → stereo FX / output

**Autodyne**
- COMP: mild
- BLEND: low to moderate
- GAIN: unity

**Sound**
- layered melodic lines feel unified and mix-ready

---

## Strengths of Autodyne for melody
- Very compact at **4hp**
- Good for **final voice shaping**
- Parallel compression is excellent on articulate melodic content
- Sidechain input enables musical rhythmic interaction
- Can move from transparent control to obvious color/distortion

## Limitations for melody
- Does **not** generate pitch, gates, or CV
- No evidence in the provided material of voltage control over parameters
- More of a **processor** than a melodic source
- Best paired with oscillators, filters, envelopes, sequencers, and quantizers

## Bottom line
**Autodyne is a finishing and character module for melodic material.** It won’t create melodies on its own, but it can make melodic voices:
- louder without simply turning them up
- more sustained
- more harmonically rich
- rhythmically animated via sidechaining
- better glued into a complete track

If you want, I can also turn this into:
1. a **“best patch ideas” cheat sheet**, or  
2. a **signal-flow diagram** showing exactly where Autodyne fits in melodic Eurorack patches.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)