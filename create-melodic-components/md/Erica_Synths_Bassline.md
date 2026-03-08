# Erica Synths — Bassline

- [Manual PDF](../../manuals/BASSLINE_web.pdf)

---

[Manual PDF: BASSLINE_web.pdf](BASSLINE_web.pdf)

# Erica Synths Bassline — using it for melodic parts

From the manual pages provided, this is a **full analog synth voice** meant for acid/bass lines, but it can absolutely be used as a **melodic voice** in a larger Eurorack system.

## What the module gives you

The manual describes Bassline as having:

- **VCO** with good **1V/oct tracking**
- **Three waveforms**
- **Triangle, square, and master outputs**
- **Suboscillator**
- **Detune circuit** that emulates multiple VCOs / BBD-style detune
- **VCF** with **LP/BP** modes
- **Separate VCF and VCA decay envelopes**
- **Accent input**
- **FM input** for the oscillator
- **VCF cutoff CV input**

That means this module already contains most of what you need for a complete melodic monosynth line:
- pitch source
- tone source
- filter shaping
- amplitude shaping
- articulation

---

## Main musical role

This module is best understood as a **complete mono lead / bass / sequence voice**.

Because it includes:
- oscillator
- filter
- VCA
- envelopes

…you can patch just:
- **1V/oct pitch CV**
- **gate**
and get a playable melodic synth line from **MAIN OUT**.

So in a system with sequencers, quantizers, keyboards, random CV, clocking, modulation, delay/reverb, etc., Bassline becomes the **sound-generating core** for melody.

---

## Important controls and jacks for melodic use

## Pitch and note control

### 1V/OCT
The manual states this is the oscillator pitch input and tracks well over several octaves.

**Use it for:**
- sequencer pitch CV
- keyboard CV
- quantized random voltages
- transposition from a precision adder

This is the main entry point for making the module play actual melodies.

### GATE
The gate input triggers both the VCF and VCA envelopes simultaneously.

**Use it for:**
- step sequencer gates
- keyboard gate
- trigger sequencer for plucky lines

This gives each note its articulation.

### ACCENT
The manual says +10V here increases volume and opens the VCF slightly.

**Use it for:**
- emphasizing selected steps in a melody
- making repeated notes feel dynamic
- classic acid-style rhythmic phrasing

For melodic writing, accent is very useful because it creates **phrased notes**, not just equal notes.

---

## Tone shaping for melody

### TUNE
Sets the base pitch range. Use this to place the voice in:
- bass register
- tenor register
- lead register

### WAVE
Selects the waveform sent to the master output.

This will strongly affect melodic character:
- **triangle**: softer, flute-like, rounded
- **square**: hollow, woody, more prominent in mixes
- **master output waveform options**: likely your core timbral choice for the line

If you want a melody to sit above percussion without sounding harsh, try triangle or filtered square. For a more obvious lead, use brighter wave settings.

### SUBOSC LVL
Adds low octave weight through the suboscillator.

For melody:
- use **small amounts** to thicken a lead
- use **higher amounts** for bass melodies
- keep it restrained if you want clearer higher-register note definition

Too much sub on upper-register melodic lines can blur intervals, but it is excellent for hooks that need body.

### DETUNE
The manual describes this as a detuned multi-VCO style effect with BBD-like behavior.

For melody, detune is one of the most useful expressive controls:
- slight detune = wider, chorused lead
- medium detune = vintage unstable mono synth tone
- high detune = aggressive, animated acid/solo texture

Use it carefully if the melody must remain pitch-clear in dense arrangements. A little goes a long way.

### FM LEVEL and FM IN
This is oscillator FM.

For melodic use:
- subtle FM gives extra harmonic motion
- audio-rate FM can create more aggressive lead timbres
- envelope or LFO into FM IN can animate notes over time

For tonal melodies, keep FM moderate unless you want dissonant or metallic sounds.

---

## Filter and articulation for melodic phrasing

### CUTOFF
Sets the filter cutoff manually.

This is one of the most important melodic controls because filter brightness often reads as musical emphasis just as much as pitch does.

### RESONANCE
The manual notes the filter can do extreme resonance sweeps.

For melody:
- low resonance = fuller, more stable tone
- medium resonance = clearer vowel-like tone, better note articulation
- high resonance = acid, nasal, focused lead sound

Resonance can help a simple sequence become more “speaking” and melodic.

### VCF mode: LP / BP
The panel shows LP/BP selection.

- **LP (low-pass)**: best for classic basses, rounded leads, warm melodies
- **BP (band-pass)**: more focused, narrower, reedy, and often very good for cutting melodic riffs in a mix

Band-pass can be especially effective when you want a melody that occupies a clear spectral lane without overwhelming bass and highs.

### CUTOFF CV
External CV for filter cutoff.

Use this with:
- an LFO for motion
- a sequencer row for per-step timbre changes
- random CV for evolving melodies
- velocity/accent-style CV for expression

### VCF ENV
Controls filter envelope decay amount/behavior according to the manual text.

This shapes how each note “opens” in brightness:
- short decay = plucky notes
- longer decay = more vocal or swelling phrases
- more envelope depth = stronger attack bite

### VCA ENV
Controls amplitude decay time.

This is central for melody:
- short = staccato/plucked sequences
- medium = synth bass or articulated lead
- long = legato-ish sustained notes if gates support it

Together, **VCF ENV** and **VCA ENV** define note shape. For melodic music, this matters as much as pitch selection.

---

## Outputs and how to use them musically

### MAIN OUT
This is the primary full voice output.

Use it when you want the complete Bassline sound:
- VCO
- filter
- VCA
- envelopes

This is the easiest way to use the module melodically.

### TRI OUT and SQR OUT
The manual says these are additional VCO outputs and are not affected by VCF/VCA.

These are very useful in a larger patch.

You can use them:
- as raw oscillator sources into external filters/VCA/envelopes
- to layer with the main output
- as tuning references
- as extra voices if processed elsewhere

This means Bassline can function both as:
1. a self-contained melodic voice, and
2. an oscillator source for more complex melodic patching

---

# How to use Bassline with other Eurorack modules for melody

Since only this manual was attached, I can describe how it pairs with the typical module categories in a Eurorack system.

## 1. With a sequencer
Patch:
- sequencer pitch CV → **1V/OCT**
- sequencer gate → **GATE**
- sequencer accent row / trigger row → **ACCENT**
- audio from **MAIN OUT** → mixer / effects

This gives you:
- basslines
- hooks
- repeating motifs
- acid-style phrases

Best use:
- short VCA decay
- moderate resonance
- some VCF envelope
- selective accent steps

---

## 2. With a quantizer and random source
Patch:
- random stepped CV → quantizer → **1V/OCT**
- clocked trigger → **GATE**
- optional random gate stream → **ACCENT**
- slow CV or LFO → **CUTOFF CV**

This creates:
- evolving melodic patterns
- generative hooks
- semi-controlled tonal lines

Best use:
- keep detune low for pitch clarity
- use LP mode for stable tonal center
- use BP mode for more characterful patterns

---

## 3. With a keyboard or touch controller
Patch:
- keyboard CV → **1V/OCT**
- keyboard gate → **GATE**
- pressure/aux CV → **CUTOFF CV** or **FM IN**
- velocity/accent output if available → **ACCENT**

This turns Bassline into a performance monosynth.

Great for:
- solos
- expressive leads
- bass parts with articulation
- live acid improvisation

Pressure to cutoff CV is especially musical.

---

## 4. With external modulation
Patch modulation sources into:
- **CUTOFF CV** for tonal movement
- **FM IN** for harmonic animation

Examples:
- LFO to cutoff = cyclic phrase movement
- envelope to FM = brighter attack
- sequencer CV row to cutoff = per-step timbral melody
- sample-and-hold to cutoff = shifting note color

This is how you make a repeated pitch sequence feel more melodic and less static.

---

## 5. With external filters and VCAs
Use:
- **TRI OUT** or **SQR OUT**

Then patch to:
- external filter
- external VCA
- separate envelope

Why do this?
- create a second articulation from the same oscillator
- layer a raw oscillator melody with the internal processed main output
- split one pitch line into multiple parallel timbral voices

Example:
- **MAIN OUT** = short plucky acid line
- **TRI OUT** through external LPG = softer supporting melodic layer

This is a strong strategy for richer melodic arrangements.

---

## 6. With effects
After **MAIN OUT**, add:
- delay for repeating melodic motifs
- reverb for ambient lead lines
- chorus for widening
- distortion/saturation for aggressive acid hooks

The Bassline module seems particularly effective before:
- delay
- spring reverb
- tape-style echo
- stereo chorus

Subtle detune plus delay is especially good for memorable lead phrases.

---

# Practical melodic patch ideas

## Patch 1: Classic acid melody
- pitch sequencer → **1V/OCT**
- gate sequencer → **GATE**
- accent triggers on selected steps → **ACCENT**
- **MAIN OUT** → distortion → delay

Settings:
- square-ish waveform
- medium resonance
- moderate VCF envelope
- short-to-medium VCA decay
- slight detune

Result:
- tight, articulate melodic sequence
- strong phrasing from accent
- ideal for techno/electro/acid

---

## Patch 2: Warm mono lead
- keyboard CV → **1V/OCT**
- keyboard gate → **GATE**
- mod wheel / pressure → **CUTOFF CV**
- **MAIN OUT** → chorus → reverb

Settings:
- triangle or softer waveform
- low resonance
- slight suboscillator
- longer VCA decay
- minimal detune

Result:
- expressive lead line
- smoother melodic contour
- good for synth-pop, ambient, melodic techno

---

## Patch 3: Animated generative melody
- random stepped CV → quantizer → **1V/OCT**
- clock divider rhythm → **GATE**
- occasional trigger pattern → **ACCENT**
- slow LFO → **CUTOFF CV**
- very slow CV → **FM IN**
- **MAIN OUT** → delay

Settings:
- LP or BP depending on mix
- medium resonance
- moderate envelope amount
- moderate VCA decay

Result:
- evolving, musical sequence
- timbral variation across repeating motifs
- useful for ambient or experimental rhythmic pieces

---

## Patch 4: Layered melodic voice from one module
- sequencer pitch → **1V/OCT**
- sequencer gate → **GATE**
- **MAIN OUT** → mixer channel 1
- **TRI OUT** → external LPG/filter/VCA → mixer channel 2

Settings:
- main output brighter and resonant
- triangle layer soft and lower in volume

Result:
- one module supplies both:
  - articulated foreground melody
  - supporting body layer

This is a very efficient use of rack space.

---

# Best melodic strengths of this module

## 1. It is a complete voice
You do not need to build a voice from separate VCO/VCF/VCA/EG modules.

## 2. Accent makes sequences musical
Accent is not just louder notes; it creates phrasing and contour.

## 3. Separate filter and amp decays
This gives strong control over pluck, bite, sustain feel, and note definition.

## 4. Extra oscillator outputs expand it
You can use the raw VCO outputs for layering or parallel signal paths.

## 5. Detune and FM add expressiveness
Even a simple melody can become lively and complex.

---

# Things to watch out for in melodic use

## Keep detune under control
Too much can smear pitch clarity, especially in faster melodies.

## Use suboscillator sparingly for upper melodies
It can overpower the fundamental and make lines muddy.

## Resonance affects perceived pitch character
At high settings, the filter peak becomes a major part of the sound, which can be amazing, but more demanding in a mix.

## FM can push you away from tonal clarity
Very useful for expressive color, but subtle settings work best when the melody must stay singable.

---

# Summary

The **Erica Synths Bassline** is best used as a **monophonic melodic synth voice** for:

- basslines
- leads
- acid sequences
- generative melodic patterns
- layered mono synth parts

Its most melodic features are:

- accurate **1V/oct**
- direct **gate** control
- expressive **accent**
- separate **VCF/VCA envelope decay**
- flexible **filter mode and resonance**
- **detune** and **FM** for animated tone
- raw **triangle/square outputs** for layering with other modules

In a Eurorack system, this module works especially well with:
- sequencers
- quantizers
- keyboards/controllers
- modulation sources
- effects
- external VCAs/filters for parallel layers

If you want, I can also turn this into:
1. a **“patch recipes” guide**,  
2. a **signal-flow diagram**, or  
3. a **“best module pairings” list** for melodic composition.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)