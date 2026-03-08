# Bastl Instruments — Cinnamon VCF

- [Manual PDF](../../manuals/manual-cinnamon-web-v1.4.pdf)

---

[Manual PDF](about:blank)

# Bastl Cinnamon — using it for melodic components

Based on the attached manual, the module here is:

- **Bastl Cinnamon** — a **state-variable filter** that can also **self-oscillate as a sine/special waveform oscillator**

This means Cinnamon is not just a tone-shaping filter. It can act as a **melodic voice source** when driven into self-oscillation, and it can also shape other oscillators into more animated melodic lines.

## What Cinnamon does well melodically

Relevant functions from the manual:

- **V/Oct input** for pitch control
- **Cutoff control** sets the oscillation frequency
- **Resonance** at maximum makes it **self-oscillate**
- **LP / BP / HP outputs** provide phase-shifted outputs
- **Character switches** alter the resonance response and self-oscillating waveform
- **Drive + Input Level** strongly affect tone when filtering external audio
- **FM CV input with attenuator** for modulation of cutoff

Important caveat from the manual:

- **V/Oct tracking works reliably when the Character switches are off**
- The **Character switches may disrupt tracking**

So for the most stable melodic use, start with:

- **Resonance high enough to self-oscillate**
- **Character switches off**
- Send sequencer pitch CV to **V/Oct**
- Take audio from **LP**, **BP**, or **HP**

---

# Main melodic use cases

## 1. Cinnamon as a sine oscillator voice

This is the most direct melodic patch.

### Patch
- Set **Resonance** fully clockwise until it self-oscillates
- Keep **Character switches off** for best pitch tracking
- Send sequencer or keyboard CV to **V/Oct**
- Use **Cutoff** to tune the base pitch range
- Patch one output to your VCA/mixer:
  - **LP** = sine-like, 0°
  - **BP** = phase-shifted, 90°
  - **HP** = phase-shifted, 180°

### Musical result
- Clean, minimal melodic tones
- Great for:
  - basslines
  - sine leads
  - sub melodies
  - tuned percussion

### Tip
Because the outputs are phase-related versions of the self-oscillation, you can mult them for interesting stereo or layered patches if your system allows.

---

## 2. Cinnamon as a character oscillator for rougher melodies

The manual notes that the **Character switches change waveform when self-oscillating**.

### Patch
Start from the self-oscillating patch above, then:

- Engage the **upper Character switch** for a sharper, edgy waveform
- Engage the **lower Character switch** for a saw-like character
- Try one or both while sequencing pitch

### Musical result
- More aggressive or harmonically rich melodic material
- Better for:
  - acid-like lines
  - cutting leads
  - unstable, expressive melodies
  - industrial or experimental sequences

### Caution
These switches can **disrupt V/Oct tracking**, so this mode is often best for:

- short repeating sequences
- drone melodies
- looser intonation
- recording and tuning by ear

---

## 3. FM-style animated melodic lines

Cinnamon has a second CV input for cutoff/frequency modulation with an **attenuator**.

### Patch
In self-oscillation mode:

- Pitch CV to **V/Oct**
- Send an LFO, envelope, or another oscillator to the **FM/right CV input**
- Use the **Attenuator** to control modulation amount

### Musical result
Depending on modulation source:

- **Envelope to FM input**:
  - per-note pitch sweeps
  - plucky attacks
  - punchy bass articulation
- **LFO to FM input**:
  - vibrato
  - slow melodic drift
- **Audio-rate oscillator to FM input**:
  - clangorous or metallic tones
  - animated leads
  - unstable bell-like melodic colors

### Best practice
For tonal melodies, keep FM amount low at first. Cinnamon can get wild quickly.

---

## 4. Filtering another oscillator into a melodic voice

If you already have another VCO in the rack, Cinnamon becomes a strong melodic sculptor.

### Patch
- Patch oscillator audio into **Input**
- Use **Input Level** to set gain
- Use **Drive** on/off to control saturation
- Send sequencer melody to the other oscillator’s pitch
- Modulate Cinnamon’s cutoff with:
  - envelope
  - sequencer CV
  - random stepped voltage
  - keyboard CV
- Take one or more outputs: **LP**, **BP**, **HP**

### Musical result
- **LP**: rounded bass/lead shaping
- **BP**: vocal, nasal melodic emphasis
- **HP**: thinner, cutting melodic parts

Because Cinnamon is a state-variable filter, the three outputs are especially useful for creating complementary melodic layers from one source.

---

# How to use the outputs musically

## Low-pass output
- Best for:
  - warm bass
  - smooth leads
  - sub-heavy melodic lines
- In self-oscillation:
  - closest to a pure sine feel

## Band-pass output
- Best for:
  - focused melodic mids
  - plucks
  - “talking” or nasal lead lines
- Excellent when cutoff is sequenced rhythmically

## High-pass output
- Best for:
  - bright melodic accents
  - thin cutting counter-melodies
  - removing low-end clutter

A very useful strategy is to treat the outputs as **three tonal perspectives of the same pitch movement**.

---

# Drive and Input Level as melodic tools

The manual emphasizes that the filter response is **highly affected by input level**.

## With Drive off
- Input gain ranges from **0 to 2**
- More controllable
- Better for cleaner filtering of melodic content

## With Drive on
- Input gain ranges from **0 to 10**
- Easily overdrives the filter input
- Great for:
  - acid bass
  - distorted leads
  - harmonically enhanced arpeggios

### Melodic application
If you send a simple waveform from another oscillator into Cinnamon:

- low gain = smoother tone
- high gain = richer harmonics
- high gain + Character switches = dramatic timbral movement across a melody

This is especially good when a simple sequence needs more personality without changing notes.

---

# Strong melodic patch ideas

## Patch 1: Pure sine bassline
- Resonance max
- Character switches off
- Sequencer CV to V/Oct
- LP out to VCA
- Envelope to VCA

**Result:** stable, round bass voice

---

## Patch 2: Dirty resonant lead
- External oscillator into Input
- Drive on
- Input Level fairly high
- Resonance medium-high
- Sequenced envelope to FM/right CV
- BP out to mixer

**Result:** expressive, biting lead with pronounced vowel-like motion

---

## Patch 3: Lo-fi tuned percussion
- Self-oscillation on
- Sequence to V/Oct
- Short envelope into FM/right CV for pitch blip
- Character switch on for rougher waveform
- Fast VCA envelope after output

**Result:** toms, bleeps, synthetic marimba-like phrases

---

## Patch 4: Dual-layer melody from one filter
- Self-oscillation on
- Pitch sequence to V/Oct
- LP out to one VCA/voice channel
- BP or HP out to another VCA/voice channel
- Different envelopes on each

**Result:** one pitch source producing two coordinated melodic layers

---

## Patch 5: Acid-style sequence
- Saw or pulse oscillator into Input
- Drive on
- Resonance high
- Sequencer runs melody to oscillator pitch
- Envelope or accent CV to FM/right CV
- LP output to VCA/mixer

**Result:** animated squelchy sequence with strong note articulation

---

# Best practices for melodic tuning

From the manual, the **rear trimmer** adjusts **V/Oct tracking**.

## Use this if:
- You want Cinnamon to play more accurately across several octaves in self-oscillation mode
- You mainly use it as an oscillator rather than just a filter

## For best pitch stability
- Keep **Character switches off**
- Let the module warm up
- Tune using the **Cutoff** knob
- Use the **trimmer** only if necessary and carefully

---

# Most useful “together” interactions inside the module

Since only one module manual was provided, the key “used together” relationships are the internal functions of Cinnamon itself:

- **V/Oct + self-oscillation** = oscillator voice
- **FM input + attenuator** = melodic articulation and vibrato
- **Character switches + resonance** = alternate oscillator timbres
- **Drive + Input Level + filter core** = harmonically rich external melodic processing
- **LP/BP/HP outputs together** = layered melodic voicings

So Cinnamon can cover multiple melodic roles in a Eurorack patch:

1. **Primary oscillator**
2. **Timbre shaper for another oscillator**
3. **Secondary tuned sine/special-tone voice**
4. **Source of layered melodic outputs**
5. **Experimental pitched resonant voice**

---

# Bottom line

**Bastl Cinnamon** is unusually useful for melody because it is both:

- a **filter for shaping pitched sources**, and
- a **trackable self-oscillating sound source**

If you want the cleanest melodic behavior, use it as a self-oscillating sine oscillator with:

- **Resonance max**
- **V/Oct input**
- **Character off**

If you want more personality, use:

- **Character switches**
- **FM modulation**
- **Drive + Input Level**

That shifts it from accurate pitch utility into expressive, unstable, and very musical territory.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)