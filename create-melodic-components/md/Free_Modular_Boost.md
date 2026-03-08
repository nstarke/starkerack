# Free Modular — Boost

- [Manual PDF](../../manuals/boost_manual.pdf)

---

[Manual PDF](attachment)

# Free Modular Boost — melodic use analysis

This manual shows **one module: Boost** by Free Modular. It is **not a voice, oscillator, filter, envelope, sequencer, or VCA**, so by itself it does **not generate melody**. Instead, it is a **signal-conditioning / coloration module** that can help melodic parts cut through, gain harmonic richness, and interface better with quieter sources.

## What Boost does
Boost is an **all-analog gain and soft-ish diode clipping stage** with:

- **Drive**: from roughly **unity gain** up to **+26 dB**
- **Tone**: tilts the high-frequency content after clipping
- **AC-coupled input**: intended for **line-level or Eurorack audio**
- **No CV control**
- Output typically limited to about **13 Vpp** with neutral tone, though high tone boost can push toward rails and cause **severe distortion**

## What that means musically
For melodic material, Boost is best thought of as:

- an **overdrive** for basslines, leads, plucks, and arps
- a **harmonic enhancer** to make simple waveforms sound richer
- a **level booster** for quieter external audio before further modular processing
- a way to make a melodic part feel more **present**, **aggressive**, or **forward in the mix**

Because it is **input-level sensitive**, you can indirectly “animate” the distortion by changing signal level before it.

---

## Best ways to use Boost in melodic patches

## 1. Add harmonics to a simple oscillator voice
A plain sine, triangle, or mellow saw can become more melodically expressive with Boost.

### Patch idea
- **VCO** → **Boost input**
- **Boost output** → **VCA / filter / mixer**
- Sequence pitch normally with your **sequencer + quantizer**

### Result
- Low Drive: subtle thickening
- Medium Drive: more upper harmonics, more presence
- High Drive: overdriven lead or acid-like aggression

### Why this helps melody
Extra harmonics make pitch content easier to hear in a mix, especially for:
- mono leads
- basslines
- arpeggios
- repetitive sequenced motifs

---

## 2. Use it after a filter for expressive lead tones
Putting Boost **after** a filter gives you a more performance-oriented melodic voice.

### Patch idea
- **VCO** → **VCF**
- **VCF** → **Boost**
- **Boost** → **VCA**
- Envelope to VCF and VCA as usual

### Result
- The filter shapes the tone first
- Boost adds saturation to the already-shaped sound
- Resonant peaks can clip in a pleasing way

### Musical use
Great for:
- techno leads
- electro bass
- saturated plucks
- expressive monosynth lines

This placement often feels more controlled than driving the filter input.

---

## 3. Put it before a filter for dynamic timbral motion
Putting Boost before a filter gives a different character.

### Patch idea
- **VCO** → **Boost**
- **Boost** → **VCF**
- **VCF** → **VCA**

### Result
- Boost generates harmonics first
- Filter then sculpts those harmonics
- Sweeping the filter creates richer melodic movement

### Musical use
Useful when a melody needs to evolve over time:
- acid sequences
- animated ostinatos
- bright plucks with controllable harshness

---

## 4. Animate distortion by controlling level before Boost
The manual specifically suggests using a **VCA before Boost** if you want to automate distortion amount.

### Patch idea
- **VCO** → **VCA**
- Envelope / CV → **that VCA**
- **VCA output** → **Boost**
- **Boost output** → mixer

### Why this is important
Since Boost has **no CV over Drive**, pre-level control becomes your “distortion CV.”

### Musical result
You can make individual notes in a melody:
- cleaner when quieter
- dirtier when accented
- more aggressive on strong beats

This is extremely useful for:
- accented step sequences
- velocity-style dynamic phrasing
- call-and-response lead articulation

If you have a sequencer with accent outputs, patch accent CV to the pre-Boost VCA.

---

## 5. Preserve melody but add edge with parallel processing
For melodic clarity, parallel distortion works very well.

### Patch idea
- Mult your melodic voice
- Path A: dry signal to mixer
- Path B: signal → **Boost** → mixer
- Blend dry and boosted versions

### Result
- Dry path keeps pitch and articulation clear
- Boosted path adds bite and harmonics
- Combined sound stays musical and intelligible

### Best for
- lead lines
- bass melodies
- arpeggios
- sampled melodic loops

---

## 6. Thicken external melodic sources
Since Boost can bring **line-level or mic-level** signals up, it is useful with non-modular melodic material.

### Patch idea
- External synth / groovebox / sampler / voice → **Boost**
- Boost output → modular effects / filter / VCA / mixer

### Use cases
- saturate a desktop synth melody
- push a vocal phrase into modular processing
- add grit to a sampled piano or loop
- integrate quiet melodic sources into Eurorack level

For vocals or melodic samples, keep Drive moderate if you want intelligibility.

---

## 7. Make bass melodies more audible
Basslines often need upper harmonics to be heard on smaller speakers. Boost is very useful here.

### Patch idea
- Bass oscillator or sub-mixed voice → **Boost**
- Optional filter after
- Then to final VCA/mix

### Settings
- Drive: low to medium
- Tone: slightly right of center if you need definition
- Avoid too much top end if the bass gets fizzy

### Result
The root notes and rhythmic motion of a bass melody become easier to perceive.

---

## 8. Use Tone as a melodic placement control
The Tone knob is more than brightness; it changes how a melodic line occupies space.

### Tone left of center
- smoother
- less harsh
- better for warm basses and rounded leads

### Tone right of center
- more bite
- more attack presence
- better for cutting leads, plucks, and arps

Because tone shaping happens **after clipping**, boosting highs can get extreme quickly. That can be excellent for aggressive leads, but it may also make pitch sound less stable if overdone.

---

## Patch roles in a melodic system

## With an oscillator
Boost turns a basic oscillator into a more harmonically complex melodic voice.

## With a sequencer
Boost won’t affect pitch sequencing directly, but it can make repeated sequences feel more alive through accent-driven pre-gain changes.

## With a quantizer
No direct interaction, but once pitches are quantized, Boost helps those notes speak more clearly.

## With envelopes
Use envelopes on a VCA placed **before** Boost to create note-dependent saturation.

## With filters
- **Before filter**: richer harmonic source for subtractive shaping
- **After filter**: polished, driven synth voice

## With VCAs
This is the most important pairing from the manual’s perspective:
- **VCA before Boost** = dynamic distortion control
- **VCA after Boost** = control final loudness

## With wavefolders / digital distortion
Boost can be the gentler first stage before more extreme processors.

---

## Concrete melodic patch recipes

## A. Saturated mono lead
- VCO saw → VCF → Boost → VCA → output
- Sequencer CV to VCO pitch
- Gate to envelope for VCA
- Envelope to filter cutoff

**Why it works:** filter gives shape, Boost adds bite and sustain-like presence.

---

## B. Accent-sensitive acid line
- VCO square/saw → VCA → Boost → VCF → VCA
- Sequencer pitch to VCO
- Gate to amp envelope
- Accent CV to pre-Boost VCA CV

**Why it works:** accented notes hit Boost harder and distort more, creating expressive variation across the sequence.

---

## C. Warm bass melody
- Triangle or sine+sub → Boost → low-pass filter → VCA
- Drive low to medium
- Tone slightly left of center

**Why it works:** adds enough harmonics for note definition while staying full and rounded.

---

## D. Parallel lead enhancer
- Main melodic voice multed
- Dry path to mixer
- Second path to Boost, then mixer
- Blend to taste

**Why it works:** preserves note clarity while adding aggression and mix presence.

---

## E. External synth melody into modular
- External synth output → Boost → modular filter/delay/reverb
- Keep Drive near low or medium at first

**Why it works:** level-matches and colors external melodic material for modular integration.

---

## Practical cautions
- **AC-coupled input** means this is for **audio**, not for processing pitch CV or slow modulation in a meaningful way.
- At high **Tone** and high **Drive**, harsh upper harmonics can dominate and obscure melodic clarity.
- Since there is **no CV**, any rhythmic or note-by-note change in distortion needs to come from **input amplitude changes** before the module.
- If you want distortion without a large output jump, **attenuate after Boost** as the manual suggests.

---

## Bottom line
**Boost is a supporting melodic utility, not a melody generator.**  
Its strongest role in melodic music is to make existing pitched material more vivid by adding:

- gain
- saturation
- harmonic density
- presence
- accent-responsive overdrive when paired with a pre-VCA

If you share the other module manuals too, I can analyze **how the modules work together as a full melodic system** and propose complete patches for leads, basslines, arps, and chordal textures.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)