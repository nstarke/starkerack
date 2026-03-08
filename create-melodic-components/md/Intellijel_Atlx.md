# Intellijel — Atlx

- [Manual PDF](../../manuals/Atlx - intellijel.pdf)

---

[Atlx / Atlantix product page & manual link](https://intellijel.com/shop/eurorack/atlx/)

# Intellijel Atlx + Atlantix: making melodic parts together

Based on the attached pages, **Atlx** is a **passive 6HP expander** for **Atlantix** that breaks out a lot of otherwise internal sound sources and processing points:

- **Dedicated oscillator outputs** for **A** and **B**
  - Sine
  - Triangle
  - Saw
  - Square
  - **Sub Square on A only**
- **Filter outputs**
  - Lowpass
  - Highpass
  - Bandpass
  - Phazor
- **Ring mod section**
  - **X in**
  - **Y in**
  - **Ring out**

Atlantix itself is the main voice:
- **Dual analog VCO**
- **Multimode VCF**
- **VCA with drive**
- **ADSR envelope**
- Extensive internal routing and patch points

So musically, the pairing gives you a **complete analog melodic voice** plus a way to extract multiple simultaneous tones from inside it for **layered, harmonically rich, and patch-programmable melodic material**.

---

## What Atlx adds for melodic use

Atlantix alone is already a playable synth voice, but **Atlx makes it much better for melody writing** because it lets you treat one played pitch as **multiple coordinated melodic signals**:

1. **Multiple waveforms at once**
   - You can use one oscillator pitch to generate:
     - a bass layer from **sub square**
     - a lead layer from **saw**
     - a softer doubling voice from **sine**
   - These can go to other VCAs, filters, effects, or mixers.

2. **Parallel filtered melody voices**
   - The same note line can appear as:
     - warm **lowpass**
     - nasal **bandpass**
     - bright **highpass**
     - more characterful **phazor**
   - Great for splitting one sequence into several melodic colors.

3. **Ring modulation as an extra pitched source**
   - Using oscillator A and B as ring mod inputs can create:
     - metallic intervals
     - bell tones
     - animated countermelodies
   - If A and B are tuned musically, ring mod can become a melodic voice in its own right.

4. **Self-patching possibilities**
   - Since Atlx exposes more outputs, you can route Atlantix’s own oscillators/filter responses back into external utilities and then back into Atlantix or other modules.
   - This is useful for creating **controlled melodic complexity** without losing the central pitch relationship.

---

# Best melodic roles for this combo

## 1. Classic mono lead voice
Use Atlantix as the main synth voice and Atlx for parallel tone extraction.

### Patch idea
- Sequence **Pitch A/B** from your sequencer/keyboard
- Gate to Atlantix envelope
- Main audio from Atlantix out for the lead
- Also patch from Atlx:
  - **A saw** to an external VCA/effect for a bright doubled lead
  - **A sine** for a tucked-under pure fundamental layer

### Why it works
You get a focused lead from the main voice while simultaneously generating cleaner or brighter layers that follow the exact same melody.

---

## 2. Bassline plus upper melodic doubling
This is one of the most useful melodic applications.

### Patch idea
- Tune **Osc A** as your main pitch source
- Use **A sub square** from Atlx as the bass foundation
- Use **A saw or square** as the midrange bass articulation
- Use Atlantix’s main filtered output for the expressive top of the bass sound

### Result
One sequence creates:
- **sub weight**
- **body**
- **filter-shaped attack/presence**

This is ideal for techno, electro, synthpop, and cinematic pulse lines.

---

## 3. Two-oscillator interval melodies
Atlantix has dual oscillators, so you can tune A and B in intervals.

### Patch idea
- Osc A = root
- Osc B = tuned to:
  - fifth
  - octave
  - third
  - detuned unison
- Mix in Atlantix for one main melodic voice
- Use Atlx outputs from A and B separately to process each oscillator independently

### Melodic advantage
You can create:
- harmonized leads
- octave melodies
- pseudo-duophonic textures
- interval-based riffs

For example:
- **A triangle** = clean root
- **B square** = octave or fifth above
- Main Atlantix output = filtered blended lead

That gives a melody with internal harmony.

---

## 4. Countermelody from the ring mod
The **ring mod** is especially interesting melodically if the two oscillators are tuned deliberately.

### Patch idea
- Send **A waveform** to **X in**
- Send **B waveform** to **Y in**
- Take **Ring out**
- Tune A and B to musically related intervals

### What you hear
Ring modulation emphasizes the **sum and difference frequencies** between the two inputs. With careful tuning, this creates:
- bell-like melodic accents
- clangorous but pitched side tones
- a separate line that tracks your oscillator interval relationship

### Musical use
Use it quietly behind the main melody for:
- shimmer
- harmonic tension
- a “ghost melody” effect

Or run the ring mod out through filtering to isolate sweeter partials.

---

## 5. Parallel filter voices from one sequence
The filter outputs are a huge gift for melodic composition.

### Patch idea
Take from Atlx:
- **LP**
- **BP**
- **HP**
- **PHZ**

Then send each to:
- separate VCAs
- a mixer
- stereo effects
- different rhythmic gates

### Musical outcome
A single melodic line can become:
- lowpass = warm center voice
- bandpass = nasal singing layer
- highpass = airy transient line
- phazor = character/animation layer

This is excellent for:
- evolving arpeggios
- melodic techno sequences
- animated ostinatos
- stereo melodic textures

You can even rhythmically mute/unmute these different filter responses to make one line feel like several interacting parts.

---

# Strong melodic patch strategies

## Strategy A: “One sequence, three melodic layers”
Use one CV/gate sequence to make a complete melodic stack.

### Example
- **Atlantix main out** = expressive lead
- **Atlx A sub** = bass reinforcement
- **Atlx bandpass out** = narrow, vocal-like upper line

This gives a full melodic arrangement from one voice.

---

## Strategy B: “Root + interval + metallic overtone”
A very musical Atlantix/Atlx patch.

### Example
- Osc A = root
- Osc B = perfect fifth
- Main out = blended lead
- **A sine out** = pure fundamental support
- **Ring out** = metallic overtone voice

This produces a rich melodic tone that sounds arranged rather than merely layered.

---

## Strategy C: “Pseudo-polyphonic melodic spread”
Not true polyphony, but very effective.

### Example
Use separate outputs to make different voices occupy different frequency bands:
- **Sub square** = bass note
- **Lowpass** = main body
- **Highpass** = top sparkle
- **Ring mod** = accent layer

All follow one pitch structure, but the ear interprets them as a larger melodic ensemble.

---

## Strategy D: “Call and response from the same voice”
Use different Atlantix/Atlx outputs with switched or sequenced VCAs.

### Example
- Step 1–4: open lowpass output
- Step 5–8: open bandpass output
- occasional ring mod accents

Same melody, but changing timbral routing creates the feeling of phrase variation and response.

---

# Practical melodic patch examples

## 1. Acid-style melodic line
- Sequence pitch into Atlantix
- Use saw/square oscillator source
- Filter resonance up
- Envelope to filter
- Take:
  - main out for the acid line
  - **Atlx sub out** for low-end support
  - **Atlx highpass out** into distortion/delay for top bite

This gives a stronger, more mix-ready melodic riff.

---

## 2. Berlin-school sequence
- Clocked pitch sequence to both oscillators
- Slight detune or interval on B
- Slow modulation to filter
- Use:
  - **LP out** for body
  - **BP out** for a narrow repeating melodic stripe
  - **Ring out** for occasional metallic motion

Pan/filter these separately for width and movement.

---

## 3. Bell melody / glass arpeggio
- Tune A and B to a consonant interval
- Patch them into **X in** and **Y in**
- Take **Ring out**
- Filter it and apply a snappy envelope

The ring mod output can become a beautiful melodic percussive voice, especially for:
- ambient arps
- soundtrack motifs
- IDM-style tuned percussion

---

## 4. Bass + lead from one performance
- Use the main Atlantix output as the lead
- Use **A sub square** externally as bass reinforcement
- If possible, process bass and lead separately with different VCAs/effects

Even without separate pitch sequencing, this creates a convincing dual-role melodic performance.

---

# How to think compositionally with these two modules

## Atlantix = the performer
Atlantix is the central playable instrument:
- pitch
- articulation
- filtering
- envelope dynamics
- main timbral identity

## Atlx = the orchestrator
Atlx lets you “orchestrate” the internals of Atlantix:
- expose hidden layers
- split one note into multiple spectral roles
- derive secondary melodic material
- create harmonically related side voices

That makes this pair especially strong for:
- **lead hooks**
- **bass motifs**
- **arpeggiated figures**
- **harmonic doubling**
- **metallic melodic accents**
- **evolving mono-synth arrangements**

---

# Limitations to keep in mind

From the provided pages, Atlx appears to be an **expander only**, not a standalone voice:
- **Passive**
- Designed specifically for **Atlantix**

So:
- It does not generate notes on its own
- Its melodic usefulness depends on Atlantix being the source
- To fully exploit the extra outputs, you’ll likely want additional:
  - VCAs
  - mixers
  - effects
  - possibly external envelopes/modulators

That said, even with minimal support, the expander substantially improves Atlantix’s melodic range.

---

# Best musical use cases

This combo is especially good for:

- **Mono leads with layered articulation**
- **Basslines with integrated sub reinforcement**
- **Single-sequence arrangements with multiple timbral voices**
- **Interval and detuned melodic hooks**
- **Ring-mod chimes and metallic melodies**
- **Parallel filter-based melodic animation**

If your goal is to get **more melody, harmony, and arrangement depth out of one synth voice**, Atlx makes Atlantix much more composition-friendly.

---

# Summary

**Atlantix** gives you the playable analog synth voice.  
**Atlx** turns that voice into a **multi-output melodic ecosystem**.

Together, they can produce:
- a main lead or bass voice,
- parallel oscillator layers,
- multiple simultaneous filter colors,
- and ring-mod-derived pitched overtones,

all locked to the same melodic material. In practice, that means you can turn one sequence into a **fuller, more arranged melodic part** with bass, body, brightness, and harmonic shimmer.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)