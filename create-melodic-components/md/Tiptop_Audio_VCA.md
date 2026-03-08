# Tiptop Audio — VCA

- [Manual PDF](../../manuals/Tiptop Audio VCA user manual_6.pdf)

---

[Tiptop Audio VCA Manual PDF](http://tiptopaudio.com/vca/)

# Using the Tiptop Audio VCA to Create Melodic Components

The attached manual is for the **Tiptop Audio VCA**, a single-channel **variable-response voltage controlled amplifier** with:

- **LEVEL**: output gain / post-VCA volume
- **SHAPE**: CV response morphing from **logarithmic -> linear -> exponential**
- **OFFSET**: manual bias to open the VCA / shift incoming CV behavior
- **CV IN attenuator**
- **CV IN / Audio IN / Audio OUT**
- Clip LEDs for both CV and audio

Although a VCA is often thought of as “just volume control,” this module is actually a core melodic utility because it can shape:

- note articulation
- modulation depth
- FM index
- filter movement amount
- effect-send animation
- ducking and dynamic phrasing

In a melodic system, that means it helps turn a plain oscillator pitch sequence into a **performed line**.

---

## What this VCA is especially good at

The standout feature in this module is the **SHAPE** control. It changes how incoming CV opens the amplifier:

- **Logarithmic**: faster perceived opening at lower CV; can feel punchy or snappy
- **Linear**: accurate proportional response; ideal for CV processing
- **Exponential**: more natural for audio loudness; often best for musical envelopes

This makes the module useful in two major melodic roles:

1. **Final note amplitude shaping**
2. **Dynamic control of another modulation source**

That second role is where a lot of melodic expression comes from.

---

# Best melodic uses described in the manual

## 1. Standard voice articulation
The manual’s most important melodic patch is the classic:

**VCO -> VCF (optional) -> VCA -> output**  
**Envelope -> VCA CV input**

This is the basic architecture for turning a raw oscillator into playable notes.

### Why it matters musically
Without the VCA, a pitched oscillator is just a constant drone.  
With the VCA controlled by an envelope, each note gets:

- attack
- sustain contour
- release
- phrasing
- separation between notes

### Recommended settings from the manual
For typical audio amplitude shaping:

- **SHAPE**: toward **logarithmic** or **exponential**
- **OFFSET**: off
- **LEVEL**: adjusted to taste
- **CV IN attenuator**: high enough for full envelope range, but not clipping

### Musical result
This gives you:

- plucks
- pads
- bass notes
- leads
- staccato or legato phrasing depending on envelope and gate timing

If you are building melodic content, this is the first job of the VCA.

---

## 2. Voltage-controlled modulation depth
The manual shows using the VCA to control the amount of an LFO going to filter cutoff.

Patch concept:

**LFO or modulation oscillator -> VCA audio/signal in**  
**Envelope -> VCA CV in**  
**VCA out -> filter FM / cutoff CV**

### Why this is melodic
For melodic lines, static modulation often sounds repetitive.  
This patch lets each note have a different amount of movement over time.

For example:

- note begins pure, then vibrato fades in
- note starts dull, then filter wobble grows
- longer notes bloom with modulation while short notes remain clean

### Best SHAPE setting
The manual suggests **linear** for CV processing, which makes sense here because you want predictable modulation scaling.

### Musical applications
Use this for:

- delayed vibrato on leads
- animated filter sweeps on arpeggios
- expressive movement on sustained notes
- per-note timbral change tied to articulation

This is one of the most useful ways to make a melodic patch feel alive.

---

## 3. FM index control for melodic timbre animation
The manual includes a patch where one oscillator modulates another through the VCA:

**VCO2 sine -> VCA IN**  
**Envelope -> VCA CV**  
**VCA OUT -> VCO1 FM input**  
**VCO1 audio -> mixer/output**

### Why this is powerful for melody
This patch gives you **time-varying FM amount per note**.

That means a note can:

- start bright and noisy, then settle
- begin pure and grow complex
- have different harmonic intensity depending on envelope shape

### Melodic uses
This is excellent for:

- bell tones
- evolving leads
- electric piano-ish sounds
- metallic arpeggios
- expressive bass attacks

### Important controls
- **OFFSET** around middle can help with bipolar modulation behavior
- **CV IN attenuator** controls maximum FM depth
- **LEVEL** affects how much modulation gets sent onward
- **SHAPE** changes how quickly FM depth grows with the envelope

For melodies, this is one of the best uses of a VCA beyond basic loudness.

---

## 4. AM / ring-mod-like melodic textures
The manual notes that the CV input can accept audio, letting the VCA act as an **amplitude modulator**.

Patch concept:

**Carrier oscillator -> Audio IN**  
**Modulator oscillator -> CV IN**  
**OUT -> mixer/filter/output**

### Why it helps melodic composition
Amplitude modulation can create:

- tremolo at low modulator rates
- clangorous sidebands at audio rates
- harmonic complexity tied to oscillator tuning

If both oscillators are tuned musically, you can get:

- chimes
- metallic intervals
- animated drones with pitch center
- bright melodic overlays

### Practical note
Because the response curve is variable, you can experiment with **SHAPE** to hear how the modulation contour changes.

---

# How the VCA helps build full melodic voices

## A. Lead voice
Patch:

- VCO saw or pulse -> filter -> VCA -> output
- envelope -> VCA CV
- optional LFO -> second VCA -> filter cutoff
- pitch CV from sequencer -> VCO 1V/oct

Result:

- envelope shapes note volume
- second modulation path adds expressive timbre movement
- SHAPE lets you fine-tune how “played” the lead feels

### Tips
- Use **exponential-ish** VCA shape for natural note loudness
- Use **logarithmic** for punchier attack feeling
- Keep CV LED just below clipping for full dynamic range

---

## B. Bass voice
Patch:

- VCO triangle/saw -> optional filter -> VCA -> output
- short envelope -> VCA CV
- optional second oscillator/LFO through VCA into filter FM or FM input

Result:

- tight articulation
- dynamic thump
- controlled bite on note onset

### Tips from the manual behavior
Avoid unwanted clipping on rounded bass sounds unless distortion is desired.  
The manual specifically notes clipping may hurt “nicely rounded bass drums or bass lines.”

So for melodic bass:

- watch the red audio clip LED
- use LEVEL to match gain rather than overdrive by accident

---

## C. Plucked sequence
Patch:

- bright oscillator -> filter -> VCA
- short decay envelope -> VCA CV
- SHAPE toward logarithmic or exponential
- optional slow modulation amount through a second VCA into filter

Result:

- articulate plucks
- sharper transient
- per-note filter animation if modulation depth is enveloped

This is great for:

- Berlin-school patterns
- minimal techno hooks
- melodic ostinatos

---

## D. Evolving melodic pad or drone with note emphasis
Patch:

- oscillator or mixed oscillators -> VCA -> output
- envelope with slow attack/release -> VCA CV
- OFFSET raised slightly so sound never fully closes
- modulation source through VCA into filter or FM

### Why OFFSET matters
The manual explains OFFSET can keep the VCA partially open so notes don’t fall to total silence.  
For melodic work, that means:

- drones with articulated accents
- legato bed textures
- notes that rise out of a sustained tone

This is very useful if you want melody embedded inside an ambient texture.

---

# Musically important controls from the manual

## SHAPE
This is the main “feel” control.

### For melodic audio loudness
Use:
- **center to right** for more natural or exponential amplitude feel
- **left** for punchier or unusual behavior

### For modulation CV processing
Use:
- **center / linear**

### Creative melodic trick
Sweep SHAPE while looping a sequence.  
This changes how the envelope translates into loudness or modulation amount, giving:

- more pluck
- smoother swells
- more abrupt FM bursts
- softer note entry

It’s almost like changing the playing technique of the sequence.

---

## OFFSET
The manual gives three key uses that are highly relevant musically:

1. **Manually open the VCA**
2. **Keep some sound present between notes**
3. **Correctly handle bipolar sources like LFOs**

### Melodic application ideas
- add sustain floor to a sequence
- create legato phrasing without changing the envelope
- center a bipolar vibrato/modulation source so both halves affect the destination

This is especially useful when controlling melodic modulation depth.

---

## CV IN attenuator
This sets how strongly the incoming envelope/LFO/audio modulates the VCA.

### Melodic use
It acts like a **performance depth control** for:

- note loudness range
- vibrato amount
- FM brightness
- filter movement intensity

A small reduction here can make a sequence sit better in a mix or become more subtle and expressive.

---

## LEVEL
Post-VCA gain.

### Musically
Use it to:

- balance voices
- compensate for different SHAPE settings
- set FM send level
- set effect send amount

The manual notes different SHAPE settings can produce different gain, so LEVEL often becomes part of the tone-shaping workflow.

---

# Five strong melodic patch ideas based on the manual

## 1. Classic subtractive melody voice
- Sequencer pitch CV -> oscillator 1V/oct
- Gate -> envelope trigger
- Oscillator -> filter -> VCA -> mixer
- Envelope -> VCA CV

Use SHAPE near exponential.  
This gives a standard melodic synth voice.

---

## 2. Envelope-controlled vibrato lead
- LFO sine -> VCA IN
- Envelope -> VCA CV
- VCA OUT -> oscillator FM input or pitch modulation attenuator input

Now vibrato appears only after the note starts.  
This is one of the most expressive lead techniques possible with a VCA.

---

## 3. Per-note filter animation
- LFO or second oscillator in LFO mode -> VCA IN
- Envelope -> VCA CV
- VCA OUT -> filter cutoff CV

Each note opens with a different modulation depth contour.  
Excellent for arpeggios and repeating melodic figures.

---

## 4. FM lead with dynamic brightness
- Modulator oscillator sine -> VCA IN
- Envelope -> VCA CV
- VCA OUT -> carrier oscillator FM input
- Carrier oscillator out -> filter or directly out

You get per-note harmonic evolution.  
Great for modern melodic techno, IDM, electro, and ambient leads.

---

## 5. Semi-legato drone melody
- Oscillator -> VCA -> output
- Envelope -> VCA CV
- OFFSET slightly up
- Long release

This leaves a low-level tone between notes while still accenting each step.  
Very effective for ambient melodic work.

---

# Notes on gain staging and clipping

The manual emphasizes both **CV clipping** and **audio clipping** LEDs.

## CV clipping
If the CV LED flashes, peaks are clipped.

For melody, this matters because clipped envelopes can make dynamics feel flattened and harsh.  
If notes feel like they all hit the same loudness too abruptly, back off the **CV IN** control.

## Audio clipping
If the red audio LED flashes, the signal is clipping.

Sometimes this is desirable, but for melodic clarity:

- keep basses cleaner
- keep FM signals controlled
- avoid accidental distortion unless it supports the musical role

---

# How this module works with a larger melodic Eurorack system

Even though this manual is just for the VCA, it clearly pairs well with:

- **oscillators** for pitched sources
- **envelopes** for note articulation
- **filters** for subtractive tone shaping
- **LFOs** for vibrato and animated movement
- **sequencers** for pitch and trigger information
- **effects** for automated sends

In practical melodic patching, this VCA is not the “sound source,” but it is often the module that makes the source feel like a playable instrument.

---

# Best musical roles summary

## Most direct melodic roles
- final amplitude shaping for notes
- dynamic control of filter modulation depth
- dynamic control of FM index
- audio-rate amplitude modulation
- effect-send automation for melodic phrases
- ducking/accent shaping

## Best settings by task
- **Audio loudness control**: exponential / right side
- **CV processing**: linear / center
- **Punchy experimental articulation**: logarithmic / left
- **Legato or drone phrasing**: add OFFSET
- **Subtle modulation depth**: lower CV IN attenuator
- **Full articulation**: raise CV IN to just below clipping

---

# Bottom line

The Tiptop Audio VCA is much more than a utility. In a melodic patch, it can control:

- when a note speaks
- how strongly it speaks
- how its timbre evolves
- how its modulation blooms over time
- how effects and movement are introduced per note

If you’re building melodic voices, the most important combinations are:

1. **Oscillator + Envelope + VCA** for note articulation  
2. **LFO/oscillator + VCA + Envelope** for dynamic modulation depth  
3. **Modulator oscillator + VCA + Envelope + carrier oscillator** for FM-based melodic expression

That combination turns static pitch sequences into phrases with contour, expression, and musical motion.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)