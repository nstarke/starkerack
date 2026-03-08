# 2hp — MMF

- [Manual PDF](../../manuals/2hp_MMF.pdf)

---

[Manual PDF](#)

# Using the 2hp MMF to create melodic components

The attached manual is for the **2hp MMF**, a **voltage-controlled analog multimode filter**. On its own, this is not a sound source or pitch generator, but in a Eurorack system it is extremely useful for shaping harmonics into **melodic voices, animated sequences, and resonant tuned lines**.

## What the module does

The MMF provides:

- **Audio input**
- **Cutoff frequency control** with CV input
- **Resonance control** with CV input
- Three simultaneous outputs:
  - **LP**: low-pass
  - **HP**: high-pass
  - **BP**: band-pass

Key specs from the manual:

- **12 dB/octave** slope
- **Analog multimode filter**
- **2HP**
- **Freq CV range:** `-8V to +8V`
- **Reso CV range:** `-5V to +5V`

## What this means musically

A multimode filter like this is one of the main tools for turning simple raw oscillator signals into something that feels melodic and expressive.

You can use it to:

- emphasize the fundamental for **round basslines**
- carve harmonics into **lead sounds**
- animate timbre rhythmically so a repeated note feels like a melody
- create **acid-like movement** with resonance
- isolate moving frequency bands for pseudo-melodic textures
- derive multiple related tonal layers from one source using the three outputs

---

## Best melodic uses of the MMF

## 1. Classic subtractive melodic voice

This is the most straightforward use.

### Patch
- Oscillator saw or square output → **MMF Input**
- **MMF LP output** → VCA → mixer/output
- Sequencer CV → oscillator 1V/oct
- Envelope → VCA CV
- Another envelope or modulation source → **Freq CV**

### Result
This gives you a standard synth voice:
- oscillator determines the pitch
- MMF shapes brightness
- modulation of cutoff adds articulation and contour

### Why it works melodically
Even if the pitch sequence is simple, filter motion makes each note feel distinct. Short envelopes into cutoff create plucks; longer envelopes create expressive lead lines.

---

## 2. Acid-style bass and lead lines

The manual specifically suggests it can do **“squelchy acid lines.”**

### Patch
- Saw or pulse oscillator → **Input**
- **LP output** → VCA
- Sequencer → oscillator pitch
- Envelope with fast decay → **Freq CV**
- Manually raise **Reso**
- Optionally modulate resonance slightly with CV

### Result
You get:
- per-note cutoff sweeps
- emphasized harmonics
- pronounced resonant character

### Musical tip
For acid-style phrasing:
- use slides from your sequencer if available
- accent certain notes by increasing cutoff CV amount
- keep resonance high, but back off if the fundamental disappears too much

---

## 3. Tuned band-pass melodies from rich audio

The **BP output** is especially useful for melodic work.

### Patch
- Rich harmonic source (saw, supersaw, detuned oscillator, noise mixed with tone, chord source) → **Input**
- **BP output** → VCA
- Slow or sequenced CV → **Freq CV**
- Moderate to high **Reso**

### Result
The band-pass output isolates a narrower spectral region. Sweeping cutoff across harmonics can create the impression of changing pitches or formants, especially when the source is rich.

### Musical applications
- vocal-like leads
- narrow, reedy melodies
- moving harmonic lines from static drones
- pseudo-sequenced melodies even without changing oscillator pitch much

This is a great trick if you want melodic motion from timbre rather than only from pitch CV.

---

## 4. Dual or triple melodic layers from one oscillator

Because the module outputs **LP, HP, and BP simultaneously**, you can create multiple related parts from one source.

### Patch
- One oscillator → **MMF Input**
- **LP output** → VCA/mixer channel 1
- **BP output** → VCA/mixer channel 2
- **HP output** → VCA/mixer channel 3

### Result
You can treat the three outputs as separate voices:

- **LP** = body / bass / warm lead
- **BP** = focused melodic midrange line
- **HP** = bright accent layer or percussive top line

### Musical benefit
All three layers track the same filter movement, so they feel connected, but each occupies a different spectral role. This is excellent for creating a more complex melodic texture from minimal patching.

---

## 5. Resonant filter as a pitched voice

The manual doesn’t explicitly say the MMF self-oscillates, so this cannot be guaranteed from the documentation alone. However, many analog filters with resonance can approach sine-like ringing at high resonance.

### Practical approach
- Send a simple source into **Input**
- Turn **Reso** up high
- Use **BP** or **LP** output
- Modulate **Freq** carefully with sequencer or keyboard CV

### Possible result
At high resonance, cutoff becomes very prominent and can behave in a quasi-pitched way. Even if it does not fully self-oscillate, it can still produce tuned resonant tones when excited by incoming audio.

### Musical use
- tuned pings
- filtered percussion with melodic tuning
- sine-ish supporting lines if resonance is strong enough

If your system includes trigger envelopes, you can ping the filter with very short transients from another module and tune the cutoff for melodic percussion.

---

## 6. Melodic articulation through cutoff tracking

The Freq CV range is wide: **-8V to +8V added to knob position**. That means the filter cutoff can be animated dramatically.

### Patch idea
Mult the same pitch sequence:
- one copy to oscillator 1V/oct
- another copy, attenuated, to **Freq CV**

### Result
As notes go up, the filter opens too. This creates a natural brightening with pitch, similar to acoustic instruments and many classic synth patches.

### Why this matters
A melodic line often sounds more alive when timbre loosely follows pitch. The MMF can do that very effectively with the right attenuation.

---

## 7. High-pass output for melodic definition

High-pass filters are often overlooked in melodic patching.

### Patch
- Rich oscillator or chord source → **Input**
- **HP output** → VCA
- Sequence pitch normally
- Modulate cutoff with envelope or LFO

### Result
The HP output strips low fundamentals and emphasizes upper harmonics. This can create:
- thin, cutting leads
- airy arpeggios
- supporting countermelodies that sit above a bass part

### Good use case
If your patch is muddy, use HP for the melodic layer while another voice handles the low end.

---

## 8. Formant and vowel-like melodic lines

The MMF is only one filter, but the **BP output** with resonance can create vocal-like emphasis.

### Patch
- Saw oscillator → **Input**
- **BP output** → VCA
- Sequencer → oscillator pitch
- Slow LFO, stepped CV, or manual performance gestures → **Freq CV**
- Moderate resonance

### Result
Instead of hearing only note changes, you hear timbral “mouth shapes” moving with the melody.

### Musical roles
- expressive solo lines
- organic hooks
- evolving mono leads

---

## 9. Sequenced timbre as melody

A melody does not always need to be purely pitch-based. You can make a repeated note feel melodic by sequencing the filter.

### Patch
- Oscillator held on one note or simple drone → **Input**
- Any output, usually LP or BP → VCA
- Stepped CV sequence → **Freq CV**
- Optional second sequence or modulation → **Reso CV**

### Result
Each step emphasizes different harmonics, creating the sensation of contour and phrase. This is especially effective with rich waveforms.

### Why it works
Our ears often interpret changing spectral emphasis as a musical line, especially when resonance adds a distinct peak.

---

## Good pairings with other module types

Since the MMF is a filter, it works best in a melodic patch when paired with:

- **Oscillator/VCO**: provides pitch and harmonics
- **Sequencer**: provides melodic CV
- **Envelope generator**: shapes cutoff and amplitude
- **VCA**: controls note articulation
- **LFO**: creates movement in cutoff or resonance
- **Mixer or mult**: lets you combine LP/BP/HP outputs
- **Attenuator/offset**: very useful for controlling filter CV depth

If you have only one oscillator, the MMF still greatly expands your melodic possibilities by creating multiple timbral variants of the same line.

---

## Example melodic patch recipes

## Warm bassline
- Saw VCO → MMF Input
- LP out → VCA
- Medium resonance
- Short envelope to cutoff
- Sequencer to VCO pitch

Use this for solid mono bass with dynamic note articulation.

## Nasal lead
- Pulse or saw VCO → MMF Input
- BP out → VCA
- Higher resonance
- Moderate envelope to cutoff
- Slight vibrato from LFO to oscillator pitch

Good for focused melodic leads that cut through a mix.

## Bright arpeggio layer
- Rich oscillator → MMF Input
- HP out → VCA
- Fast envelope to amplitude
- Clocked modulation to cutoff

Useful for sparkly top-end melodic texture above a bass voice.

## One-source three-layer melody
- Oscillator → MMF Input
- LP, BP, and HP each to separate VCAs or mixer channels
- Different amplitude envelopes for each path

Creates a complex, mix-ready layered voice from one oscillator.

---

## Important practical notes from the manual

### Installation / power
- **2HP**
- **42 mm depth**
- **+12V: 55 mA**
- **-12V: 55 mA**
- Ribbon cable red stripe goes to **-12V**
- Manual notes that in most systems **-12V is at the bottom**
- The power cable should connect to the module with the **red band facing the front**

### Control voltages
- **Freq CV:** `-8V to +8V`
- **Reso CV:** `-5V to +5V`

In practice, attenuating modulation into these inputs will help you keep melodic patches controllable and musical.

---

## Bottom line

The **2hp MMF** is best thought of as a **melodic tone-shaping module** rather than a melody generator. It shines when used with an oscillator and sequencer to produce:

- classic subtractive basses and leads
- acid lines
- resonant band-pass melodies
- layered parts using simultaneous LP/HP/BP outs
- timbre-driven melodic motion from static or simple sources

If you pair it with even a basic VCO + envelope + VCA + sequencer, it can become a central part of highly expressive melodic patching.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)