# 2hp — Grain

- [Manual PDF](../../manuals/2hp_Grain_Manual.pdf)

---

[Manual PDF](#)

# 2hp Grain — creating melodic components

Based on the attached manual, this module is:

- **2hp Grain**
- A **granular audio processor**
- Designed to turn an incoming audio signal into **pitched grains, clouds, microsound phrases, and textures**
- Particularly useful for deriving **melodic material from existing sound sources**

## What Grain does musically

Grain is not a traditional oscillator. It needs an **audio input** and then creates grains from that incoming sound. The melodic strength comes from two things:

1. **Pitch control over the grains**
   - The **Freq** knob shifts grain pitch from **-4 octaves to +4 octaves**
   - The **V/Oct** input allows **pitch-accurate sequencing**

2. **Controllable grain generation**
   - **Density** determines how often grains are created and how they behave:
     - **Left side**: periodic grains
     - **Center**: no grains
     - **Right side**: stochastic grains
   - Higher **Freq** also makes grains **smaller** and increases **generation speed**

That means Grain can act like a hybrid of:

- a pitch shifter
- a granular voice
- a texture-to-melody converter
- a sampled microsound instrument driven by external audio

---

## Panel summary

From top to bottom:

- **In** — audio input
- **Density CV** — CV control of grain density, **-5V to +5V**
- **Density knob** — periodic ↔ stop ↔ stochastic grain behavior
- **Mix CV** — CV control of dry/wet mix, **-5V to +5V**
- **Mix knob** — dry input ↔ fully granular output
- **V/Oct** — pitch control for grains, **1V/oct**, range **-1.5V to +5.5V**
- **Freq** — pitch shift amount and indirect grain-size/speed behavior
- **Out** — audio output

---

## How to use Grain for melodic parts

## 1. Turn any oscillator into a granular lead voice

### Patch
- Patch a basic oscillator, wavetable oscillator, or harmonically rich voice into **Grain In**
- Patch a sequencer or keyboard CV into **V/Oct**
- Take **Out** to your VCA/filter/output chain
- Set **Mix** mostly or fully wet

### Why it works
The incoming oscillator provides a stable harmonic source. Grain then re-pitches and re-articulates slices of it. Because **V/Oct** tracks pitch, you can sequence melodic lines while the granular engine adds motion and texture.

### Best settings
- **Density** slightly left of center for regular grain pulses
- **Freq** near center for recognizable pitch, or above center for brighter, smaller grains
- **Mix** 75–100% wet for a clear granular melody

### Result
- crystalline lead lines
- digital plucks
- shimmering arpeggios
- “frozen” melodic textures

---

## 2. Derive melody from a drone

### Patch
- Send a sustained drone, chord, or noise-rich source into **In**
- Sequence **V/Oct**
- Put **Mix** fully wet
- Set **Density** left of center for periodic grain generation

### Why it works
A static sound source becomes raw material for granular extraction. The sequence on **V/Oct** imposes melodic contour onto the grains, even though the source itself may not be playing notes.

### Musical use
This is excellent for:
- ambient melodies
- ghostly countermelodies
- evolving intros
- melodic overdubs derived from one sustained sound

### Tip
If the source is harmonically dense, the melody will feel more spectral and complex. If the source is simple, the melody will sound clearer and more tonal.

---

## 3. Use percussion as a melodic grain source

### Patch
- Feed a hi-hat loop, click track, snare, or short percussive sound into **In**
- Sequence **V/Oct**
- Set **Density** around the periodic side
- Increase **Freq** for tighter, faster grains

### Why it works
Granular processing of percussive sound often produces tiny pitched fragments that feel like mallets, bells, or glitch plucks.

### Result
- melodic glitch lines
- pointillistic arps
- IDM-style micro-melodies
- tuned percussion textures

This is one of the most interesting melodic uses of Grain because it lets rhythm become pitch.

---

## 4. Crossfade between original note and granular harmony

### Patch
- Input a melodic source into **In**
- Send the same pitch CV used by the original voice to **V/Oct**
- Modulate **Mix CV** slowly
- Send Grain output alongside or instead of the original voice

### Why it works
The **Mix** control blends dry source and granular-processed material. If your source is already melodic, Grain can add a pitched parallel layer that moves between recognizable note and transformed note-cloud.

### Result
- melody with shadow harmonics
- call-and-response between dry and granular versions
- expressive morphing lead tones

### Good modulation idea
Use a slow triangle or envelope into **Mix CV** so phrases bloom from dry to granular.

---

## 5. Build stochastic melodic textures

### Patch
- Send a sustained or looping sound into **In**
- Sequence **V/Oct** with a sparse melody
- Turn **Density** to the right of center for stochastic grain behavior
- Keep **Mix** wet or mostly wet

### Why it works
On the right side, Grain generates grains stochastically. The pitch can still be guided by **V/Oct**, so you get melodies that are recognizable but unstable and alive.

### Result
- fluttering melodic clouds
- unstable generative lines
- aleatoric upper voices
- “particle” melodies

This is especially effective in ambient, experimental, and soundtrack-oriented patches.

---

## 6. Make octave-shifted melodic doubles

### Patch
- Feed a melodic line or oscillator into **In**
- Sequence **V/Oct**
- Use **Freq** to shift the grain pitch up or down in octave ranges
- Blend with **Mix**

### Why it works
Since **Freq** spans **-4 to +4 octaves**, you can create upper or lower pitched doubles from the source material.

### Musical uses
- sub-octave granular bass reinforcement
- high octave sparkle above a melody
- layered “12-string” type shimmer
- artificial harmonics and register spreads

### Tip
Keep **Density** moderate so the pitch remains legible if you want clearly melodic results.

---

## 7. Use Grain as a playable microsound voice

### Patch
- Feed in a complex audio source
- Set **Mix** fully wet
- Sequence **V/Oct** from a keyboard or sequencer
- Fine tune **Freq**
- Use external envelopes/VCA after Grain for articulation

### Why it works
At full wet, Grain becomes less like an effect and more like a voice derived from captured audio. Because pitch is externally controllable, you can “play” the buffer material melodically.

### Result
- playable sample-cloud voice
- expressive digital lead
- granular pseudo-sampler
- unusual tuned textures without a dedicated sampler

---

## Important behavior to exploit

## Density is not just “more or less”
It changes the *character* of note production:

- **Far left**: grains become periodic, increasingly fast as you move further left
- **Center**: grain generation stops
- **Right**: grains become stochastic, increasingly fast as you move further right

So for melody:

- use **left side** for rhythmic, clock-like note definition
- use **right side** for loose, animated, probabilistic melody
- avoid center if you want continuous grain output

## Freq affects more than pitch
The manual states that as **Freq increases**:

- **grain size decreases**
- **grain generation speed increases**

So high Freq settings give:
- brighter
- smaller
- more active
- more sparkling melodic output

Low Freq settings give:
- larger
- slower
- heavier
- often more smeared output

This interaction is key to shaping whether a melody feels like:
- a clean plucked line
- a shimmery cluster
- a stretched, spectral phrase

---

## Best input sources for melodic use

Since Grain depends on incoming sound, source choice matters a lot.

### Best for clear melodies
- saw or pulse oscillator
- simple FM tones
- tuned percussion
- vocal phrases
- plucked strings or string-like synths

### Best for textural melodies
- filtered noise
- pads and drones
- field recordings
- percussion loops
- chords or full mixes

### Best for strange but musical results
- speech
- metallic percussion
- resonant filter pings
- feedback tones
- wavefolded audio

---

## Practical melodic patch recipes

## Patch 1: Granular lead
- Oscillator → **In**
- Sequencer CV → **V/Oct**
- **Mix** full wet
- **Density** slightly left of center
- **Freq** slightly above center

**Sound:** articulate digital lead with sparkle

---

## Patch 2: Ambient melody from noise
- Filtered noise or drone → **In**
- Slow sequencer → **V/Oct**
- **Density** right of center
- **Freq** around center or slightly high
- **Mix** full wet

**Sound:** drifting, unstable, airy melody

---

## Patch 3: Tuned glitch percussion
- Hi-hat/snare loop → **In**
- Fast sequencer or random quantized CV → **V/Oct**
- **Density** left of center
- **Freq** high
- **Mix** full wet

**Sound:** tiny tuned clicks and glassy percussive notes

---

## Patch 4: Morphing melody layer
- Main melodic voice → **In**
- Same pitch CV → **V/Oct**
- LFO or envelope → **Mix CV**
- **Density** moderate
- **Freq** to taste

**Sound:** melody that fades between natural and granular versions

---

## Patch 5: Granular bass accent
- Bass oscillator → **In**
- Bass pitch sequence → **V/Oct**
- **Freq** below center
- **Density** moderate left
- **Mix** 50–100% wet

**Sound:** gritty, broken, sub-rich bass ornamentation

---

## Performance tips

- **Use Mix as a phrase control**: dry for clarity, wet for transformation
- **Sequence V/Oct conventionally** if you want actual note lines
- **Modulate Density CV** for evolving articulation
- **Keep Density on the periodic side** for more rhythmically readable melodies
- **Push Density stochastic** for fills, transitions, and generative passages
- **Raise Freq for smaller, more agile grains**
- **Lower Freq for heavier, slower, more smeared notes**

---

## Limits and workflow notes

From the manual, Grain has:

- one **audio input**
- one **audio output**
- CV over **Density** and **Mix**
- **V/Oct** for pitched control

That means Grain works best in a larger melodic patch when paired with:

- a sound source to feed it
- a sequencer or keyboard for **V/Oct**
- envelopes and a VCA after the output
- possibly a quantized random source for semi-generative melodies

By itself, it is **not a complete standalone melodic voice**. It becomes one when supplied with:
1. source audio
2. pitch CV
3. downstream articulation/amplitude shaping

---

## Bottom line

**2hp Grain** is excellent for making melodic material out of almost any sound. Its strongest melodic roles are:

- **granular lead voice**
- **pitched texture generator**
- **melodic layer derived from drones or loops**
- **glitch arp / microsound instrument**
- **wet/dry morphing harmony processor**

If you patch it with a stable source and a sequencer into **V/Oct**, it can produce very playable and musical melodic lines. If you feed it noisier or more complex material, it excels at creating **organic, unstable, and highly characterful melodic fragments**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)