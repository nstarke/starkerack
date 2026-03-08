# Mutable Instruments — Ripples

- [Manual PDF](../../manuals/Manual - Mutable Instruments Documentation.pdf)

---

[Manual PDF](#)

## Module: Mutable Instruments Ripples 2020

Ripples 2020 is a **voltage-controlled multimode filter** with built-in **low-pass VCA behavior**, which makes it very useful for shaping raw oscillators into playable, melodic voices.

### What it does musically
Ripples gives you:

- **Low-pass, band-pass, and high-pass outputs**
- **Switchable 2-pole / 4-pole response** on BP and LP outputs
- **Voltage-controlled resonance**
- **V/Oct tracking**, so the filter can **self-oscillate as a sine oscillator**
- A **VCA on the low-pass output**, controlled by CV

That combination means Ripples can work in multiple melodic roles:

1. **Classic subtractive voice shaper**
2. **Sine oscillator for melodies/basslines**
3. **Dynamic tone shaper for sequenced material**
4. **Final LPG/VCA-like stage for a voice**

---

## Best melodic uses

### 1. Turn an oscillator into a melodic subtractive synth voice
Patch a harmonically rich oscillator into Ripples and use it as the main tone-shaping stage.

**Patch idea**
- Oscillator saw or pulse -> **IN 1** or **IN 2**
- Pitch sequence -> oscillator V/Oct
- Envelope or modulation -> **FREQ CV**
- Envelope or gate-derived CV -> **LEVEL**
- Use **LP out** as your main audio output

**Why it works**
- The **cutoff** sets brightness
- **Resonance** emphasizes harmonics and adds character
- The **LEVEL CV** on the low-pass output acts like an integrated VCA, so Ripples can serve as both **filter and amplitude control**
- This is ideal for **basslines, leads, arps, and plucks**

**Musical tip**
- Use **IN 1** when you want saturation/soft clipping and more aggressive melodic lines
- Use **IN 2** when you want a cleaner, more classic tone

---

### 2. Use self-oscillation as a sine voice
Ripples self-oscillates at higher resonance settings and tracks **V/Oct** over about 4 octaves.

**Patch idea**
- Turn **RES** high until it self-oscillates
- Send pitch CV from a sequencer/keyboard into **V/OCT**
- Take audio from **LP out** or experiment with other outputs
- Use **LEVEL CV** for note articulation

**Why it works**
- In self-oscillation, Ripples becomes a **pure melodic sine oscillator**
- Great for:
  - **sub-bass**
  - **sine leads**
  - **FM-like support tones**
  - **minimal melodic lines**

**Musical tip**
- Because the module is **not temperature stabilized**, treat it as a characterful tracking oscillator rather than a precision VCO in all situations
- It’s especially strong for **short melodic phrases**, **bass parts**, and **doubled lines**

---

### 3. Create animated melodic timbre with cutoff modulation
For melody, movement matters as much as pitch. Ripples excels at making repeated notes feel alive.

**Patch idea**
- Sequence a VCO normally
- Send a slow or rhythmic CV into the **cutoff modulation input**
- Set the **FM attenuverter** to control depth and polarity
- Use **BP output** for nasal, vocal-like melodic phrasing

**Results**
- Slight modulation creates expressive phrasing
- Stronger modulation creates:
  - acid-like motion
  - talking lead tones
  - lively arpeggios
  - evolving ostinatos

**Musical tip**
- Positive modulation opens notes dynamically
- Negative modulation can create more percussive or “ducked” phrases

---

### 4. Use the band-pass output for focused melodies
The **band-pass** output is especially useful for melodies that need to sit in a mix.

**Why BP is useful**
- Removes excessive low-end and top-end
- Gives a more **focused, reedy, vocal** sound
- Helps melodic parts cut through dense arrangements

**Good for**
- sequenced arps
- midrange hooks
- techno riffs
- counter-melodies

**Slope switch use**
- **12 dB/oct**: more open, lively, less severe
- **24 dB/oct**: smoother, more rounded, more sculpted

---

### 5. Use the low-pass LEVEL CV as the note-shaping VCA
A standout feature of Ripples is that the **LP output has voltage-controlled gain**.

**Behavior from manual**
- **0V** = silence
- **5V** = unity gain
- above **5V** = progressively compressed
- if nothing is patched, **7V** is internally applied

**Why this matters melodically**
You can patch an envelope directly into **LEVEL** and get:
- note articulation
- dynamics
- plucks
- swells
- accents

This means a minimal melodic voice can be:

- **Oscillator -> Ripples**
- **Pitch CV -> Oscillator**
- **Envelope -> LEVEL**
- **Envelope or modulation -> FREQ**

That is enough for a complete playable monosynth voice.

---

## Input character and melodic implications

### IN 1
- Gain from **0 to 5**
- Can **soft-clip**
- Great for:
  - aggressive bass
  - driven leads
  - thicker sequences
  - more pronounced harmonics before filtering

### IN 2
- Always clean
- Better for:
  - pure melodic content
  - delicate sequences
  - cleaner subtractive sounds
  - preserving waveform identity

### Combined use
Because both inputs are mixed together, you can build richer melodic timbres:
- Saw in **IN 2** for body
- Square or sub in **IN 1** for grit
- Then shape both together through the filter

This is excellent for **big mono leads** or **weighty basslines**.

---

## Resonance as a melodic tool
Resonance is not only for sweeps. In melodic contexts it can:

- emphasize note attacks
- tune the brightness contour of a sequence
- create vowel-like peaks
- push tones toward self-oscillation for a hybrid oscillator/filter sound

**Practical melodic ranges**
- **Low resonance**: warm, stable melodic tone
- **Medium resonance**: expressive, classic subtractive phrasing
- **High resonance**: sharp, acid-like melodies
- **Self-oscillation**: pure sine melody source

---

## Output choice for different melodic roles

### LP output
Best for:
- basslines
- warm leads
- classic subtractive patches
- patches needing amplitude control via LEVEL CV

### BP output
Best for:
- riffs
- arps
- cutting midrange melodic lines
- vocal or nasal textures

### HP output
Best for:
- thin melodic layers
- bright plucks
- parallel processing
- removing low-end from secondary melodic parts

A useful technique is multing the same source into Ripples and recording or mixing multiple outputs for layered melody design.

---

## Example melodic patches

### Patch 1: Simple bass voice
- Saw oscillator -> **IN 1**
- Sequencer pitch -> oscillator V/Oct
- Envelope -> **LEVEL**
- Envelope -> cutoff CV
- Output from **LP**
- Set slope to **24 dB**

**Sound**
A rounded, punchy bass with controllable drive.

---

### Patch 2: Clean melodic lead
- Triangle or saw oscillator -> **IN 2**
- Pitch sequence -> oscillator
- Envelope -> **LEVEL**
- LFO or envelope -> cutoff modulation
- Output from **BP** or **LP**

**Sound**
Focused and expressive, especially for melodic hooks.

---

### Patch 3: Sine sequence without a VCO
- No audio input
- Increase **RES** until self-oscillation
- Sequencer -> **V/OCT**
- Envelope -> **LEVEL**
- Output from **LP**

**Sound**
Minimal sine bass or pure melodic line.

---

### Patch 4: Acid-style phrase generator
- Saw wave -> **IN 1**
- Sequencer -> oscillator pitch
- Accent envelope -> cutoff CV
- Gate/envelope -> **LEVEL**
- Higher **RES**
- Use **LP** at 24 dB

**Sound**
Squidgy, resonant melodic sequences with built-in drive.

---

### Patch 5: Dual-source melodic timbre
- Saw oscillator -> **IN 2**
- Square/sub oscillator -> **IN 1**
- Same pitch CV to both oscillators
- Envelope -> **LEVEL**
- Modulation -> cutoff CV
- Take **BP** out

**Sound**
Complex, mix-ready melodic tone with body plus grit.

---

## Strengths of Ripples in a melodic system
Ripples is especially good in a melodic Eurorack setup because it combines several voice-building functions:

- **Filter**
- **Sine-capable oscillator via self-oscillation**
- **CV-controlled resonance**
- **Built-in VCA on the LP output**
- **Drive option on input 1**
- **V/Oct tracking**

So even by itself, it can become the core of a compact melodic voice. Paired with:
- a **sequencer**
- a **sound source**
- an **envelope**
- optionally an **LFO**

it easily produces complete musical lines.

---

## Bottom line
Ripples 2020 is most effective for melodic work as either:

1. a **subtractive voice-finishing filter/VCA**
2. a **self-oscillating sine voice**
3. a **resonant timbre animator** for sequences and arpeggios

Its biggest advantage is that it can make a melodic patch both **expressive and compact**: one module handles tone shaping, resonance character, and low-pass amplitude control all at once.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)