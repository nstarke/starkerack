# 2hp — Freez

- [Manual PDF](../../manuals/Freez_Manual.pdf)

---

[Freez Manual PDF](#)

# Using the 2hp Freez to Create Melodic Components

The attached manual covers the **2hp Freez**, a **voltage-controlled locked looper** that captures a short slice of incoming audio and repeats it. While it is not a pitch-tracking oscillator or traditional sampler, it can absolutely be used to generate **melodic material** when paired with other Eurorack modules.

## What Freez Does Musically

Freez records incoming audio into a buffer and then "freezes" that buffer for looping playback.

Key behavior from the manual:

- **SIZE** sets loop/buffer length
  - Fully CCW = longest buffer
  - Fully CW = shortest buffer
  - Range: roughly **9 ms to 3 s**
- **S. RATE** sets sample rate
  - Range: **2.36 kHz to 96 kHz**
- Changing **SIZE** after freezing alters the captured material's **pitch and timbre**
- Changing **S. RATE** affects both:
  - the incoming audio fidelity
  - the time/pitch character of the frozen loop
- **FREEZ** can be controlled by:
  - front-panel button
  - **TRIG** input
  - **momentary or latching** toggle

That makes Freez useful as a hybrid of:

- micro-looper
- beat repeater
- pseudo-granular voice
- pitch-warped sample fragment player
- crude wavetable-ish sound source

## The Core Idea for Melody

To get melodic results, think of Freez less like a recorder and more like a **tiny captured waveform engine**.

If you freeze:

- a single cycle or near-single-cycle waveform,
- a short pluck,
- a vocal consonant/vowel fragment,
- a filtered noise burst,
- or a transient-rich sound,

then modulating **SIZE** and **S. RATE** can push the frozen sound into stable-ish pitches or stepped note-like changes.

## Best Ways to Use Freez for Melodic Material

## 1. Freeze a Simple Oscillator Waveform

Patch:

- VCO sine/triangle/saw -> **IN**
- **OUT** -> VCA -> filter/mixer
- Use button or **TRIG** to capture a tiny fragment
- Set **SIZE** toward shorter settings
- Tune with **S. RATE**

### Why this works
If the buffer becomes very short, Freez begins behaving like a repeating waveform fragment. The looped cycle can produce a pitched tone. You can then "play" it by altering:

- **S. RATE** for broad pitch movement
- **SIZE** for more radical pitch/timbre changes

### Best musical result
A sine or triangle input usually gives the cleanest melodic tone. Saws and complex waves give harsher, more digital pitched textures.

## 2. Use a Quantized CV Source on S. RATE CV

The manual says **S. RATE CV** accepts **±5V** and is added to the knob position.

Patch:

- sequencer CV -> quantizer -> **S. RATE CV**
- manually freeze a short buffer first
- use the sequencer to step through note values

### Result
This is one of the strongest ways to get actual melodic lines out of Freez. Since sample rate changes alter playback character, stepped voltages can create note-like intervals. It may not track in exact 1V/oct fashion, but quantized stepped CV can still produce musically coherent melodies.

### Tip
Use the front-panel **S. RATE** knob as your base tuning, then let the quantized CV define the melody contour.

## 3. Sequence the SIZE CV for Interval Jumps

The **SIZE CV input** also accepts **±5V** and is summed with the knob.

Patch:

- random stepped CV or sequencer -> attenuator -> **SIZE CV**
- freeze a buffer
- carefully limit modulation depth

### Result
SIZE changes can shift both **pitch and timbre**, often more dramatically than S. RATE. This is excellent for:

- alien arpeggios
- metallic melodies
- vowel-like interval shifts
- broken digital lead lines

### Tip
Small SIZE modulation amounts work best if you want recognizable pitches. Larger modulation becomes more granular and textural.

## 4. Clocked Triggering for Rhythmic Melodic Re-Sampling

Use **TRIG** to repeatedly capture new snippets in time with your patch.

Patch:

- melodic source or chord source -> **IN**
- clock division or gate pattern -> **TRIG**
- **MODE TOGGLE** in **momentary** or **latching** depending behavior desired

### Result
Instead of one stable pitch, Freez can grab rhythmic slices of an already-pitched sound. This creates:

- stuttering lead phrases
- glitch arpeggios
- repeated note fragments
- pseudo-granular melodic riffs

### Mode behavior from the manual
- **Momentary mode**:
  - freeze lasts while gate is high / button is held
- **Latching mode**:
  - each rising edge toggles freeze on/off

### Musical use
- **Momentary** is better for rhythmic repeats and gated melodic textures
- **Latching** is better when you want to capture one note and continue "playing" it with CV

## 5. Feed Freez with Filter Pings or Percussive Tones

Instead of a steady oscillator, feed it short resonant sounds:

- LPG plucks
- self-oscillating filter pings
- tuned percussion voices
- Karplus-Strong patches

Patch:

- resonant voice -> **IN**
- freeze very short sections after the transient
- modulate **S. RATE**

### Result
You get expressive, unusual melodic tones with a natural attack baked into the sampled material. This often sounds more organic than freezing a plain waveform.

## 6. Turn Speech or Field Recordings into Pitched Leads

The manual emphasizes sound mangling and buffer warping. This makes Freez excellent for melodic extraction from non-musical audio.

Patch:

- microphone preamp / sample player / radio / field recording -> **IN**
- freeze very short vocal or noisy fragment
- tune using **S. RATE**
- optionally sequence **SIZE CV**

### Result
This can yield:

- vocal-like synth leads
- haunted choirs
- granular pads
- melodic glitch hooks

A tiny vowel fragment often creates especially playable melodic content.

## 7. Use Freez as a Crude Drone Oscillator

Freeze a tiny loop and leave it latched.

Patch:

- sound source -> **IN**
- latch a short buffer
- **OUT** -> filter -> VCA
- sequence VCA with envelopes
- vary **S. RATE** slowly or with stepped CV

### Result
Freez becomes its own unstable digital oscillator voice. Even without precise pitch tracking, this works well for:

- bass drones
- pad roots
- monophonic lead parts
- supporting tonal textures

## Patch Recipes for Melodic Use

## Patch 1: Lo-Fi Lead Voice

**Modules needed**
- VCO
- Freez
- quantizer
- sequencer
- VCA
- envelope
- filter optional

**Patch**
- VCO saw -> Freez **IN**
- Freeze a short buffer manually
- Sequencer CV -> quantizer -> **S. RATE CV**
- Gate sequencer -> envelope -> VCA CV
- Freez **OUT** -> VCA -> mixer

**What happens**
The frozen buffer acts like a rough oscillator, while the sequencer creates note changes. This gives a crunchy, digital lead.

## Patch 2: Glitch Arpeggiator

**Modules needed**
- melodic source
- clock
- trigger sequencer
- Freez
- reverb/delay

**Patch**
- melodic source -> **IN**
- trigger sequencer -> **TRIG**
- Set **MODE** to momentary
- Short **SIZE**, medium-low **S. RATE**
- **OUT** -> delay/reverb

**What happens**
Freez repeatedly grabs tiny slices of the input and spits out rhythmic, melodic repeats. Great for IDM-style hooks.

## Patch 3: Vocal Fragment Keyboard

**Modules needed**
- sampler or external audio
- Freez
- quantized CV source
- VCA/filter

**Patch**
- vocal sample -> **IN**
- latch-freeze a very short vowel segment
- Quantized CV -> **S. RATE CV**
- Slow CV or manual movement -> **SIZE**
- **OUT** -> filter/VCA

**What happens**
You get a playable vocal-ish synth line from a frozen speech fragment.

## Patch 4: Harmonic Resampling Voice

**Modules needed**
- chord oscillator or submix of oscillators
- Freez
- sequencer or S&H
- attenuator

**Patch**
- mixed harmonic signal -> **IN**
- freeze a medium-short buffer
- Stepped CV -> attenuator -> **SIZE CV**
- Optional second CV -> **S. RATE CV**

**What happens**
The harmonically rich source produces complex melodic tones. CV over SIZE and S. RATE makes it behave like a digital wavetable/granular synth voice.

## Strengths for Melody

Based on the manual, Freez is especially good at:

- **short-loop pitch generation**
- **timbral note variation**
- **rhythmic melodic repetition**
- **lo-fi digital lead sounds**
- **captured micro-sample drones**
- **pseudo-granular arpeggios**

## Limitations to Keep in Mind

Freez is not described as a precision pitch module. So for melodic use:

- it likely will **not track 1V/oct accurately**
- tuning may be approximate
- note intervals may need to be found by ear
- extreme SIZE/S. RATE changes may alter timbre more than pitch

That said, those limitations are also its musical strength. It excels at:

- unstable melody
- degraded digital pitch
- expressive resampling
- unusual tonal artifacts

## Practical Performance Tips

## Use attenuation on CV
Both CV inputs accept **±5V**, and both are added to the knob setting. A full-strength sequencer may be too wide. Attenuation helps narrow the response into a more playable range.

## Capture carefully
The exact frozen slice matters a lot. Tiny changes in when you press freeze can dramatically alter pitch, stability, and harmonic content.

## Start clean, then get weird
For easier tuning:
- start with a simple waveform
- high **S. RATE**
- short **SIZE**

Then lower sample rate or widen size modulation for more character.

## Pair with envelopes and filters
Freez becomes much more "musical" as a melodic voice when shaped downstream by:
- VCA + envelope
- lowpass filter
- LPG
- delay/reverb

These help turn its static loop into articulated notes.

## Use latching for drone, momentary for articulation
- **Latching mode**: best for creating a sustained frozen source
- **Momentary mode**: best for rhythmic phrasing and beat-repeat style melodic fragments

## Bottom Line

The **2hp Freez** is not a conventional melodic module, but it can absolutely serve as a **melodic sound generator** when used as a tiny captured waveform looper. The most effective strategies are:

1. **freeze a very short pitched sound**
2. **sequence S. RATE CV for note movement**
3. **use SIZE for timbral/pitch variation**
4. **trigger freezing rhythmically for glitch melodies**
5. **shape the result with VCAs, filters, and effects**

In a Eurorack system, Freez works best as a **character voice** for:
- lo-fi leads
- granular melodies
- vocal-like synth lines
- broken arps
- digital drones

If you want, I can also turn this into:
- a **"patch ideas" cheat sheet**
- a **beginner-friendly explanation**
- or a **module pairing guide** listing the best companion module types for Freez.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)