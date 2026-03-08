# 2hp — Tune

- [Manual PDF](../../manuals/Tune_Manual_2023.pdf)

---

[Manual PDF](https://www.twohp.com/manuals/tune)

# 2hp Tune — using it for melodic patching

The **2hp Tune** is a **voltage quantizer**. Its job is simple but very musical: it takes an incoming CV and forces it onto notes from a chosen scale, then outputs a **quantized 1V/oct melodic CV**.

Since this manual set only includes **one module**, the main question is not really “how do these modules work together,” but rather:

- how **Tune** works with the rest of a Eurorack system, and
- how to use it to generate **melodic components** like basslines, arps, leads, modal riffs, and constrained random melodies.

---

## What the module does

### Inputs and controls
- **Input**
  - CV to be quantized
  - Range: **0V to +5V**
- **Scale knob**
  - Selects the scale
- **Scale LEDs**
  - Show the selected scale
- **Bias knob**
  - Diatonically shifts the note range inside the selected scale
- **Bias CV input**
  - Positive CV control for Bias
  - Range: **0V to +5V**
- **Output**
  - Quantized **V/Oct** output
  - Range: **0V to +5V**

### Available scales
The module provides these 11 scales/modes:

1. Chromatic  
2. Major  
3. Major Pentatonic  
4. Minor  
5. Minor Pentatonic  
6. Harmonic Minor  
7. Egyptian Minor  
8. Whole Tone  
9. Octatonic (0, 2)  
10. Diminished  
11. Octatonic (0, 1)

This is a very useful set for melody writing because it covers:
- conventional tonal material
- pentatonic “safe” note sets
- darker harmonic minor colors
- symmetric scales for abstract or cinematic lines

---

# How Tune creates melody in a Eurorack patch

A quantizer becomes melodic when you feed it **changing voltage**.

Typical CV sources:
- sequencer row
- random stepped voltage
- sample & hold
- LFO
- envelope
- joystick/manual voltage
- pressure or touch controller
- a second melodic CV source you want constrained to a scale

Then:
1. Send that CV into **Tune Input**
2. Select a **scale**
3. Patch **Tune Output** to an oscillator’s **1V/oct**
4. Gate/envelope/VCA handle articulation

So Tune sits between **raw CV generation** and **pitched sound generation**.

---

# Best musical uses

## 1. Turn random voltages into usable melodies
One of the most common uses.

### Patch concept
- Random stepped CV → **Tune Input**
- **Tune Output** → oscillator 1V/oct
- Clocked gate → envelope → VCA
- Choose **Major Pentatonic**, **Minor Pentatonic**, or **Major**

### Result
You get melodies that feel intentional instead of totally atonal.

### Why it works
Random voltage by itself often lands between semitones and in notes outside a tonal center. Tune snaps everything onto scale tones, so even chaotic CV becomes musically coherent.

---

## 2. Constrain a sequencer to a scale
If you have a CV sequencer without built-in quantization, Tune gives it harmonic structure.

### Patch concept
- Sequencer CV row → **Tune Input**
- **Tune Output** → oscillator 1V/oct
- Sequencer gate row → envelope/gate destination

### Result
You can freely adjust sequence voltages by ear or by slider position, and Tune keeps pitches in key.

### Good scale choices
- **Major** for bright pop/house/ambient
- **Minor** for darker lines
- **Harmonic Minor** for dramatic/eastern/classical tension
- **Pentatonic** for very forgiving melodic movement

---

## 3. Create transposable melodic patterns with Bias
The **Bias** control is the most interesting performance feature on this module.

The manual says Bias adjusts the base voltage level **diatonically within the selected scale**. That means it shifts the note set in musically relevant steps rather than arbitrary semitone offsets.

### Musical use
Think of Bias like a **scale-aware melodic offset**.

### Patch concept
- Sequencer or random CV → **Tune Input**
- **Tune Output** → oscillator 1V/oct
- Slow CV or manual knob movement → **Bias CV Input**

### Result
The same melodic contour can be shifted to different note centers within the scale.

This is excellent for:
- phrase variation
- modal movement
- chord-tone cycling
- making one sequence feel like it’s evolving harmonically without rewriting the sequence

### Performance trick
Use the **Bias knob** manually while the patch plays. This can “rotate” the available note range in a very musical way and produce evolving melodies from static source material.

---

## 4. Build basslines from simple modulation sources
You don’t need a dedicated sequencer.

### Patch concept
- Triangle or stepped LFO → **Tune Input**
- **Tune Output** → VCO 1V/oct
- Clock divider / trigger source → envelope/VCA
- Select **Minor**, **Major**, or **Minor Pentatonic**

### Result
The LFO shape becomes a repeating melodic contour. Quantization makes it a proper riff.

### Tip
- Smooth LFO in gives rising/falling lines
- Stepped random in gives discrete note movement
- Slow envelope in gives contour-based phrase motion

---

## 5. Generate arpeggio-like lines
Tune doesn’t create arpeggios by itself, but it can convert repeating modulation into arpeggio-style note movement.

### Patch concept
- Ascending saw LFO or sequencer ramp → **Tune Input**
- **Tune Output** → oscillator 1V/oct
- Fast clocked gates → envelope/VCA
- Use **Major**, **Minor**, or **Harmonic Minor**

### Result
As the input voltage rises, Tune steps through notes in the chosen scale, often creating scalar or arpeggio-adjacent patterns.

### Make it more arpeggio-like
Keep the incoming CV range narrow so it cycles through a compact note cluster instead of traversing many octaves.

---

## 6. Make lead melodies more stable and tonal
If you use a ribbon controller, joystick, pressure source, or another expressive CV source, Tune can preserve performance feel while keeping you in key.

### Patch concept
- Performance CV source → **Tune Input**
- **Tune Output** → lead oscillator 1V/oct
- Manual scale selection for song section changes

### Result
You can improvise freely without falling outside the chosen harmonic language.

This is especially useful live.

---

## 7. Use exotic and symmetric scales for cinematic or experimental melody
The scale list is unusually good for non-standard melodic material.

### Interesting options
- **Whole Tone**
  - Dreamlike, floating, ambiguous
- **Diminished**
  - Tense, angular, suspenseful
- **Octatonic**
  - Great for horror, fusion, modern classical, techno weirdness
- **Egyptian Minor**
  - Open, modal, pseudo-folk flavor
- **Harmonic Minor**
  - Immediate dramatic pull

### Patch concept
- Random or sequenced CV → Tune
- Slow Bias modulation
- Long envelopes and delay/reverb after voice

### Result
Strong melodic identity with minimal patch complexity.

---

# How Bias affects melody

Bias deserves special attention because it is not just a coarse transpose in the usual sense.

According to the manual:
- fully left = no bias
- fully right = the last note of the selected scale becomes the starting point where the scale begins

Practically, this means:
- the available quantization map is shifted **within the scale**
- this changes which diatonic notes are emphasized by the same incoming voltage
- the melodic contour can remain similar while the tonal gravity changes

## Why this matters musically
If your source CV has a recognizable shape, Bias lets you keep that shape but hear it from a new scalar perspective.

That is extremely useful for:
- verse/chorus variation
- bassline mutation
- call-and-response
- evolving ambient melody
- pseudo-harmonic progression from one CV source

## Best sources for Bias CV
- slow LFO
- stepped random
- sequencer lane
- manual offset from another module
- envelope for phrase-based note shifts

---

# Patch recipes

## Patch 1: Simple tonal melody
**Goal:** easy in-key lead

- Stepped sequencer CV → **Tune Input**
- **Tune Output** → oscillator 1V/oct
- Gate sequencer → envelope → VCA
- Scale: **Major**
- Bias: low or centered

**Musical outcome:** clear, stable melody in key

---

## Patch 2: Generative ambient melody
**Goal:** evolving ambient notes

- Sample & hold random CV → **Tune Input**
- **Tune Output** → oscillator 1V/oct
- Sparse random gates → envelope/VCA
- Scale: **Minor Pentatonic** or **Egyptian Minor**
- Slow LFO → **Bias CV Input**

**Musical outcome:** drifting but coherent generative melodic line

---

## Patch 3: Dark cinematic sequence
**Goal:** tense melodic motion

- 8-step sequencer CV → **Tune Input**
- **Tune Output** → oscillator 1V/oct
- Trigger sequencer → envelope/VCA
- Scale: **Harmonic Minor** or **Diminished**
- Manual Bias changes at phrase boundaries

**Musical outcome:** dramatic line with controlled harmonic tension

---

## Patch 4: Scalar bass riff from an LFO
**Goal:** melody without a sequencer

- Ramp LFO → **Tune Input**
- **Tune Output** → bass oscillator 1V/oct
- Clocked trigger → short envelope → VCA
- Scale: **Minor**
- Tune oscillator low

**Musical outcome:** repeating bass riff that sounds sequenced

---

## Patch 5: Controlled chaos
**Goal:** random melody that still works musically

- Chaos/random CV source → **Tune Input**
- **Tune Output** → oscillator 1V/oct
- Irregular gates → envelope/VCA
- Scale: **Major Pentatonic** for consonance or **Octatonic** for tension
- Stepped random → **Bias CV Input**

**Musical outcome:** unpredictable but scale-locked melody

---

# Scale selection advice for songwriting

## Safest scales for immediate musical results
- **Major Pentatonic**
- **Minor Pentatonic**
- **Major**
- **Minor**

These are best when:
- you want melodic success quickly
- your input CV is very wild
- you’re improvising live

## Most colorful scales
- **Harmonic Minor**
- **Egyptian Minor**

These are best when:
- you want stronger character
- the melody should feel modal or dramatic

## Most abstract scales
- **Whole Tone**
- **Diminished**
- **Octatonic**

These are best when:
- tonal ambiguity is desirable
- you’re making experimental, soundtrack, IDM, or dark techno material

---

# Practical patching notes from the manual

## Voltage ranges
- **Input:** 0V to +5V
- **Bias CV:** 0V to +5V
- **Output:** 0V to +5V

So this module expects **unipolar positive CV**. That matters.

### Practical implication
If your modulation source is bipolar, like:
- -5V to +5V LFO
- centered random
- audio-rate bipolar signal

you’ll usually want to:
- offset it upward, or
- attenuate and bias it into the **0V to +5V** range

Otherwise, part of the source behavior may be outside the intended operating range.

---

# Strengths of Tune in a melodic system

## 1. It makes non-musical voltages musical
This is the core benefit.

## 2. It allows free-form sequencing
You can use crude control sources and still end up with organized pitch material.

## 3. Bias adds melodic development
Not just quantization, but controllable note-set shifting.

## 4. The scale set is performance-friendly
There are enough scales to cover:
- traditional melodies
- modal writing
- pentatonic safety
- experimental harmony

## 5. Great for small systems
Because one compact module can add melodic structure to:
- random systems
- utility-driven systems
- minimalist techno rigs
- portable skiffs

---

# Limitations to keep in mind

## 1. No explicit root-note control described
The manual describes scale selection and Bias, but not a dedicated root/key selector. So the module is best understood as quantizing around its internal scale mapping and incoming voltage range.

## 2. Positive CV ranges only
You may need external offset/attenuation utilities.

## 3. It is a quantizer, not a sequencer
It shapes pitch, but does not itself generate rhythm or gates.

So for complete melody voices you still need:
- CV source
- gate/trigger source
- oscillator
- envelope
- VCA
- optional filter/effects

---

# Best “used together” interpretation in a system context

Since only **2hp Tune** is included here, the best way to think about “used together” is:

### Tune + CV source
creates note choices

### Tune + gate source
creates rhythmic note articulation

### Tune + oscillator
creates actual melody pitch

### Tune + envelope/VCA
creates phrasing

### Tune + Bias modulation
creates melodic evolution

In other words, Tune is the **harmonic intelligence layer** in a melodic patch.

---

# Summary

The **2hp Tune** is ideal for building melodic content from almost any changing control voltage. Its strongest uses are:

- quantizing sequencers into scales
- turning random voltages into musical lines
- creating scalar basslines and leads
- generating evolving melodies via **Bias**
- exploring tonal, modal, and symmetric scales in compact systems

If you want melody in Eurorack without needing a full-featured pitch sequencer, this module is extremely effective. It is especially powerful in patches where the raw CV source is unpredictable or loosely controlled, because it turns that unpredictability into something compositionally useful.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)