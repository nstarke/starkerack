# Blue Lantern Modules — Voks Analog Filter

- [Manual PDF](../../manuals/BLM Voks Analog Filter.pdf)

---

[Manual PDF / Source](https://www.bluelanternstore.com/store/p133/BLM_Voks_Analog_Filter.html#/)

# Using These Modules Together for Melodic Eurorack Patches

From the provided manual pages, the module shown is:

- **Blue Lantern Modules BLM Voks VCF**
  - 6hp
  - Analog filter based on the **Polivoks** filter
  - Modes:
    - **Normal**
    - **Unstable Brite**
  - Switchable **internal limiter diode**
  - Outputs:
    - **12 dB Low Pass**
    - **6 dB Band Pass**
  - Inputs:
    - **Attenuated audio input**
    - **Direct audio input**
    - **CV direct input**
    - **Bi-polar FM input**

This is a **filter**, not a complete melodic voice by itself, so its role in melodic patching is to shape harmonics, emphasize note articulation, and create animated timbral movement that makes melodies feel alive.

## What this module contributes to melody

A melodic Eurorack patch usually needs:

- a **pitch source**: sequencer, keyboard, quantizer, random voltage
- a **sound source**: VCO, wavetable oscillator, noise into resonant filter, etc.
- a **contour source**: envelope/LFO
- a **VCA**
- and often a **filter** for tone shaping

The **Voks VCF** is most useful in the melodic chain as the **timbre shaper**. Because it has both LPF and BPF outputs, plus normal vs unstable/bright behavior, it can make a simple oscillator line become:

- smooth and rounded
- nasal and vocal
- aggressive and unstable
- expressive under CV control

That is especially valuable for leads, basslines, arpeggios, and pseudo-formant melodies.

---

## Core melodic patch roles

## 1. Basic subtractive melodic voice

**Patch idea:**
- VCO saw or pulse output -> **Voks audio input**
- **LPF output** -> VCA -> mixer/output
- Pitch CV from sequencer/keyboard -> VCO 1V/oct
- Gate from sequencer -> envelope
- Envelope -> VCA CV
- Optional second envelope or modulation source -> **Voks CV input**

**What happens:**
- The oscillator provides the note pitch
- The VCA envelope gives note articulation
- The Voks shapes brightness over time

**Musical result:**
- Basslines
- Leads
- Arpeggios
- Classic synth phrases with more character than a clean modern filter

The **12 dB low-pass** response should preserve some edge while still taming harmonics, which is often great for melodic parts that need presence without becoming dull.

---

## 2. Use the filter as the “expression” layer for melodies

A melody becomes expressive when its tone changes from note to note, not just its pitch.

**Patch idea:**
- Sequence pitch to oscillator normally
- Send a second CV lane from your sequencer to the **Voks CV input** or **bi-polar FM input**
- Use that lane to open/close the filter differently per step

**Why it works:**
- Notes can have different timbral emphasis
- Repeated notes no longer sound static
- Accent patterns become much more musical

**Good uses:**
- Acid-style phrasing
- Evolving techno sequences
- Melodies where every step has a different emotional weight

If your sequencer offers **accent**, route accent voltage to the filter CV so accented notes get brighter or more aggressive.

---

## 3. Band-pass melodies for vocal or reed-like lead tones

The **6 dB band-pass output** is especially interesting for melody.

**Patch idea:**
- VCO triangle, saw, or rich digital oscillator -> Voks input
- **BPF output** -> VCA
- Moderate resonance
- Slow or envelope-based filter motion

**What it sounds like:**
- More focused mids
- Thinner but characterful lead tones
- Vocal, nasal, or “speaking” textures

This is excellent for:
- solo lead lines
- counter-melodies
- folk-ish or experimental melodic parts
- melodies that must cut through a dense mix

Compared with the LPF output, the BPF can sit in a mix with less low-frequency clutter.

---

## 4. Parallel melodic timbres from both outputs

Since the module has separate **LPF** and **BPF** outputs, you can use both at once.

**Patch idea:**
- Oscillator -> Voks input
- **LPF output** -> VCA 1 -> mixer left
- **BPF output** -> VCA 2 -> mixer right or second mixer channel
- Modulate the two VCAs differently

**Musical benefit:**
- One oscillator becomes two complementary melodic layers
- LPF provides body
- BPF provides edge and presence

This can create:
- stereo melodic voices
- layered unison leads
- dynamic morphing tones
- “main note + ghost note” style textural doubling

If you envelope the two paths differently, one note can have a warm body with a sharper midrange transient.

---

## 5. Resonant filter as a near-voice source

Polivoks-inspired filters often excel at strong resonance and unstable behavior.

Even though the manual does not explicitly say it tracks 1V/oct, you can still use the Voks in a **quasi-oscillating or resonant melodic** role.

**Patch idea:**
- Feed a harmonically rich source or even a click/impulse into the filter
- Raise resonance
- Tune cutoff carefully
- Send sequenced CV to the filter cutoff

**Result:**
- The perceived pitch center can follow the cutoff
- You get whistle-like, vocal, or unstable melodic tones

This is not guaranteed to be precise tonal tracking, but it can be musically excellent for:
- industrial melodies
- unstable leads
- strange bells
- eerie counterpoint

Use a quantizer before the filter CV if you want more stable melodic intervals.

---

## 6. “Unstable Brite” mode for animated melodic lines

The manual mentions **Normal Mode and Unstable Brite Mode**.

That strongly suggests you can switch between:
- a more expected filter response
- a brighter, less stable, more characterful one

**Melodic application:**
- Use **Normal** for foundational bass or lead phrases
- Use **Unstable Brite** for chorus sections, fills, or higher-register hooks

This can function almost like a performance macro:
- verse = normal
- chorus = unstable brite
- breakdown = band-pass unstable modulation

On repeated melodies, this helps create arrangement contrast without changing notes.

---

## 7. Internal limiter diode for soft clipping and tone shaping

The module includes an **internal limiter diode selected by switch**.

That likely alters how the filter saturates or limits internally, which is very useful musically.

**For melody:**
- Use the limiter to make peaks feel more compressed and aggressive
- Push oscillator level into the filter for harmonically richer lines
- Use it on bass melodies to add growl
- Use it on lead sequences to add edge without external distortion

This is especially effective if you:
- send a hot saw wave into the **direct audio input**
- use moderate resonance
- animate the cutoff with an envelope or step CV

The melody will feel more “spoken” and forward in the mix.

---

## 8. Attenuated input vs direct input as performance tools

The module provides both:
- **attenuated audio input**
- **direct audio input**

That means you can change how hard the signal drives the filter.

### Practical use:
- **Attenuated input**: cleaner, more controlled melodic shaping
- **Direct input**: stronger drive, more saturation, more aggression

For melodic composition:
- route a delicate waveform or high melody through the attenuated input
- route basslines or acid lines through the direct input

This gives you two distinct tonal personalities from the same oscillator/sequence concept.

---

## 9. Bi-polar FM for melodic motion

The **bi-polar FM input** is one of the most interesting features for melody.

Because it is bipolar, modulation can move the cutoff above and below the set point, making the filter movement more animated and centered.

**Patch ideas:**
- Slow triangle LFO -> bi-polar FM for gentle melodic timbre drift
- Envelope -> bi-polar FM for plucky articulation
- Second sequencer row -> bi-polar FM for per-note harmonic animation
- Audio-rate oscillator -> bi-polar FM for metallic or vocalized lead tones

**Melodic uses:**
- animated arpeggios
- growling basslines
- pseudo-formant leads
- expressive phrase shaping

If you use audio-rate FM lightly, you can make the melody sound more alive without fully destroying pitch clarity.

---

# Musical patch recipes

## 1. Acid-adjacent bassline

**Patch:**
- Saw VCO -> direct input
- LPF output -> VCA
- Step sequencer pitch -> VCO
- Gate -> snappy envelope -> VCA
- Accent or second CV row -> filter CV input
- Moderate resonance
- Try limiter diode engaged
- Try unstable brite mode for more edge

**Result:**
- Aggressive, rubbery melodic bassline
- Best for EBM, techno, electro, industrial

---

## 2. Vocal lead

**Patch:**
- Rich oscillator -> attenuated input
- BPF output -> VCA
- Sequencer pitch -> oscillator
- Envelope -> VCA
- Slow LFO + subtle envelope mixed into filter FM

**Result:**
- Nasal, singing lead tone
- Great for melodic hooks that must stand out

---

## 3. Dual-output melody layering

**Patch:**
- Oscillator -> filter
- LPF output -> main voice path
- BPF output -> second VCA with longer envelope
- Both mixed together

**Result:**
- One note generates a core body plus a spectral halo
- Excellent for ambient, soundtrack, and melodic techno

---

## 4. Percussive tuned sequence

**Patch:**
- Short pulse or click source -> filter
- Resonance up
- Sequenced CV -> filter CV
- BPF output preferred
- Fast decay envelope to VCA

**Result:**
- Bongos, zaps, tuned percussion
- Can become a melodic ostinato line

---

## 5. Melodic drone with evolving harmonics

**Patch:**
- Drone oscillator -> Voks
- LPF and BPF both used
- Very slow LFO to bi-polar FM
- Manual switching between normal/unstable brite
- Quantized stepped modulation to filter CV

**Result:**
- The pitch source stays stable while harmonics imply shifting melodic contours
- Very useful for ambient and experimental music

---

# Best module pairings for creating melody

Since this module is a filter, it works best when paired with:

- **VCOs**: for the actual pitched source
- **sequencers/quantizers**: for melody notes
- **envelopes**: for articulating brightness
- **VCAs**: for note dynamics
- **LFOs/random CV**: for variation
- **mixers/attenuators**: to control how much CV hits the filter

If you have multiple oscillators, the Voks can also be used after a small oscillator mix to create richer melodic voices with interval stacking.

---

# Performance advice

## For bass melodies
- Use **LPF**
- Use **direct input**
- Add envelope to cutoff
- Use limiter if you want growl

## For leads
- Use **BPF** or mix LPF+BPF
- Modulate with a gentle bipolar source
- Try unstable brite mode for expressive peaks

## For arpeggios
- Use sequencer accent into filter CV
- Keep resonance moderate
- Add subtle FM for movement

## For experimental melody
- Push resonance
- Use unstable brite mode
- Send stepped random CV through a quantizer into filter CV
- Treat the filter cutoff as a secondary melodic dimension

---

# Bottom line

The **BLM Voks VCF** is best used in a melodic system as a **character filter** that adds articulation, aggression, and vocal-like spectral movement to otherwise simple pitched material. Its strongest melodic advantages are:

- **distinct low-pass and band-pass outputs**
- **Polivoks-style character**
- **normal vs unstable bright behavior**
- **switchable internal limiting**
- **CV and bipolar FM control for animated note timbre**

It will not generate a full melodic line by itself, but in combination with any oscillator, sequencer, envelope, and VCA, it can make melodies feel much more vivid, expressive, and alive.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)