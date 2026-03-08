# 2hp — Kick

- [Manual PDF](../../manuals/2hp_Kick.pdf)

---

[Manual PDF](#)

# Using the 2hp Kick for Melodic Components

The attached manual appears to cover a single module:

- **2hp Kick** — bass drum synthesizer / percussive voice with **1V/Oct tracking across five octaves**

Even though it’s presented as a drum module, **Kick can absolutely be used melodically** because it has:

- **V/Oct input**
- **Pitch control**
- **Long decay times** up to **15 seconds**
- **Tone shaping** that moves from clean sine-based hits to more aggressive, overdriven timbres

That combination makes it more than a drum voice: it can function as a **pitched percussion voice**, **bass synth**, **sub voice**, or even a **minimal lead/pluck source**.

---

## What the module does musically

## 2hp Kick as a melodic voice

From the manual:

- **Trig** accepts gate signals to fire the sound
- **Tone** changes timbre and pitch modulation behavior
- **Decay** ranges from **80 ms to 15 s**
- **V/Oct** tracks pitch over **five octaves**
- **Pitch** sets base frequency
- **Out** is **10 Vpp**

This means the module can be patched like a compact synthesized oscillator/voice that is internally shaped into a percussive envelope.

---

# Best melodic use cases

## 1. Tuned kick basslines

This is the most obvious melodic application.

### Patch idea
- Send a **sequencer pitch CV** to **V/Oct**
- Send the sequencer’s **gate/trigger** to **Trig**
- Set **Decay** medium to long
- Use **Pitch** to place the sequence in bass range
- Keep **Tone** near center for a cleaner, more sine-like low end

### Result
You get:
- tuned kick notes
- 808-style basslines
- electro and hip-hop sub patterns
- acid-adjacent percussive bass if sequenced tightly

Because the decay can get very long, notes can blur into a sustained low-end line rather than isolated drum hits.

---

## 2. 808-style gliding sub melodies

Since the module responds to **1V/Oct**, you can program melodic movement instead of just drum transients.

### Patch idea
- Sequence pitch into **V/Oct**
- Trigger every note with **Trig**
- Set **Decay** fairly long
- Tune **Pitch** low
- Use **Tone** around center or slightly right for cleaner body
- If your sequencer or CV source supports it, use **slewed pitch CV** before the **V/Oct** input for glide

### Result
This creates:
- singing sub bass
- trap/808 melodic lines
- legato-feeling descending bass phrases
- tonal kick patterns that sit between percussion and bass synth

Even without true internal portamento, slewed incoming pitch can create a gliding effect between triggered notes.

---

## 3. Pitched toms and melodic percussion

Because it tracks well over a wide pitch range, Kick can behave like a **tuned drum synth**.

### Patch idea
- Sequence notes into **V/Oct**
- Trigger with rhythmic patterns
- Use shorter **Decay**
- Move **Pitch** into low-mid or mid range
- Sweep **Tone** left or right for different drum colors

### Result
You can create:
- tuned tom lines
- melodic percussive riffs
- IDM-style pitch-bouncing drums
- marimba-like synthetic thuds at shorter settings

This is especially strong for music where drums carry harmonic motion.

---

## 4. Sine-pluck melodies

The manual says that at the middle position of **Tone**, the source is a **clean sine wave** with minimum pitch modulation. That is very useful for tonal work.

### Patch idea
- Put **Tone** at center
- Set **Decay** short-to-medium
- Send melodic CV to **V/Oct**
- Trigger from a clocked sequence
- Tune **Pitch** up into mid range

### Result
You get:
- soft sine plucks
- minimal techno bleeps
- rounded mallet-like phrases
- simple melodic motifs that stay very clean

This is probably the most “musical note” application if you want recognizable pitches instead of obvious kick drums.

---

## 5. Distorted mono lead or industrial melody

Moving **Tone** left introduces **overdrive** and increased pitch modulation. That makes the module more aggressive and less purely sinusoidal.

### Patch idea
- Sequence **V/Oct** melodically
- Use rapid triggers for repeated notes
- Set **Decay** medium
- Push **Tone** left for overdriven character
- Raise **Pitch** into upper bass / low-mid / mid range

### Result
You can get:
- distorted plucked leads
- industrial bass stabs
- EBM-style mono riffs
- noisy melodic percussion

Because the waveform gets more complex, this use is especially good when you want the line to cut through a mix.

---

# How to think about the controls melodically

## Trig
This is the articulation input.

For melodic use:
- use a **trigger sequencer** for rhythmic note events
- use a **gate sequencer** if the module responds happily to longer pulses
- experiment with sparse triggers for bass punctuation or dense triggers for riffs

The trigger pattern defines phrasing as much as the note CV does.

---

## Tone
This is the key timbral macro.

### Center
- cleanest
- most sine-like
- best for tonal bass and plucks

### Right
- still clean sine source
- more pitch modulation
- more snap/impact
- useful for punchy melodic bass

### Left
- overdriven source
- maximum modulation
- rougher harmonics
- useful for aggressive melodic percussion and distorted bass

For melodic clarity, start at **center** and then move outward until you get enough character.

---

## Decay
This strongly affects whether the module reads as a drum or a note.

### Short decay
- clicky
- tom-like
- percussive melodic use
- better for busy patterns

### Medium decay
- bass plucks
- 808-like notes
- good note separation

### Long decay
- sustained subs
- droning low melodies
- pseudo-legato bass
- can overlap into harmonic texture

A very long decay combined with slow sequences can create a surprisingly lyrical bass voice.

---

## V/Oct + Pitch
These together determine musical pitch.

- **Pitch** sets the base register
- **V/Oct** adds accurate note control from your sequencer, keyboard, or quantizer

A good workflow:
1. Put **Tone** around center
2. Set **Decay** to medium
3. Tune **Pitch** by ear into the desired octave
4. Send quantized melodic CV into **V/Oct**
5. Refine the register with the **Pitch** knob

Because the manual states tracking over five octaves, the module should be usable for more than just sub-bass.

---

# Practical melodic patch recipes

## Patch 1: 808 bassline
**Goal:** classic melodic sub bass

- Sequencer pitch CV → **V/Oct**
- Sequencer gate/trigger → **Trig**
- **Pitch**: low
- **Decay**: medium-long
- **Tone**: center to slightly right
- **Out** → mixer / VCA / saturation / compressor

**Musical effect:** deep, tuned kick-bass notes with strong fundamental.

---

## Patch 2: Minimal sine melody
**Goal:** soft tuned plucks

- Quantized CV → **V/Oct**
- Trigger pattern → **Trig**
- **Pitch**: mid range
- **Tone**: center
- **Decay**: short-medium

**Musical effect:** simple pure-tone phrases, great for minimal techno, ambient pulses, or interlocking melodic percussion.

---

## Patch 3: Melodic tom sequence
**Goal:** drum line with pitch content

- Sequencer CV → **V/Oct**
- Euclidean or stepped trigger pattern → **Trig**
- **Pitch**: low-mid
- **Decay**: short
- **Tone**: left or right depending on brightness/aggression

**Musical effect:** tuned drum riffs that carry both rhythm and melody.

---

## Patch 4: Distorted bass riff
**Goal:** aggressive mono bass

- Bass sequence CV → **V/Oct**
- Gate/trigger sequence → **Trig**
- **Pitch**: bass range
- **Decay**: medium
- **Tone**: left
- Optional external filtering after output

**Musical effect:** gritty bass stabs with strong attack and character.

---

## Patch 5: Drone pulses
**Goal:** sparse tonal low-end atmosphere

- Slow sequencer or random quantized CV → **V/Oct**
- Slow clock triggers → **Trig**
- **Decay**: very long
- **Tone**: center
- **Pitch**: low to mid-low

**Musical effect:** resonant sub pulses that imply harmony with very little patching.

---

# How it works in a larger melodic Eurorack system

Even though only one module is shown in the provided manual, here’s how it integrates with common melodic utilities.

## With a sequencer
A pitch sequencer turns Kick into:
- bassline voice
- tuned percussion voice
- simple mono lead

Best pairing:
- quantized CV for tonal accuracy
- trigger lane for articulation

---

## With a quantizer
If your pitch source is random or unquantized:
- random CV → quantizer → **V/Oct**
- trigger source → **Trig**

This gives musically scaled percussive melodies.

---

## With a slew limiter
Put slew before **V/Oct** for:
- glides
- sliding 808 lines
- more vocal melodic movement

---

## With a VCA or LPG after the output
Although Kick has its own internal decay contour, external amplitude shaping can:
- shorten long tails
- add dynamics
- help it sit more like a synth voice

---

## With filters
Filtering the output is very effective.

### Low-pass filter
- smoother bass
- removes click/high transient
- emphasizes sub

### Band-pass or resonant filter
- turns it into a more tonal midrange percussion voice
- useful for melodic riffs

### High-pass
- thinner plucks and synthetic toms

---

## With distortion/saturation/compression
Since the output is **10 Vpp**, it is healthy and strong.

Further processing can make it:
- more present in a mix
- more sustained
- more harmonically rich
- more “record-like” for bass music

Compression especially helps long-decay 808-style melodic lines.

---

# Strengths for melodic composition

## Why this module works well melodically
- **True V/Oct input**
- **Wide pitch tracking**
- **Very long decay**
- **Clean sine option**
- **Overdriven option**
- **Compact size**

So despite being labeled a kick drum module, it is really a **compact synth voice specialized for percussive articulation**.

---

# Limitations to keep in mind

## It is still a drum-oriented voice
Compared to a full oscillator + envelope + VCA voice, melodic use is somewhat specialized.

Potential limitations:
- articulation is always based on its internal drum envelope behavior
- no separate waveform outputs
- no separate envelope outputs
- timbre is macro-controlled rather than deeply patch-programmable
- melodic phrasing may always retain some percussive identity

But that “limitation” is also its charm: it excels at **pitched, punchy, memorable melodic lines** that ordinary subtractive voices don’t naturally produce.

---

# Best musical roles for this module

If you’re writing melodic music, the 2hp Kick is especially strong for:

- **808/sub basslines**
- **tuned kicks**
- **pitched tom sequences**
- **sine plucks**
- **industrial bass stabs**
- **IDM percussive melodies**
- **minimal techno tonal percussion**

---

# Bottom line

The **2hp Kick** can be used as a melodic module by treating it as a **triggered, pitch-trackable synth voice** rather than only a drum.

Its most useful melodic approaches are:

1. **Tuned kick basslines**
2. **808-style sub melodies**
3. **Pitched tom and percussive sequences**
4. **Clean sine plucks**
5. **Overdriven bass and lead stabs**

The key controls for melody are:

- **V/Oct** for note pitch
- **Pitch** for register
- **Decay** for note length
- **Tone** for timbral identity
- **Trig** for phrasing and rhythm

So if you pair it with a sequencer, quantizer, and optionally slew/filter/saturation, this module can contribute real melodic content—not just rhythm.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)