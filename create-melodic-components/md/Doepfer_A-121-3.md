# Doepfer — A-121-3

- [Manual PDF](../../manuals/A-121-3 12dB Multimode Filter (slim version).pdf)

---

[Manual PDF / Source](https://doepfer.de/a1213.htm)

# Doepfer A-121-3 12dB Multimode Filter: using it for melodic patching

The attached manual page is for the **Doepfer A-121-3 12dB Multimode Filter (Slim Line Series)**. Since only this module is included here, I’ll explain how **this filter can be used with other typical Eurorack building blocks** to create melodic material, and how its internal features support pitch-like and musical behavior.

## What this module gives you musically

The A-121-3 is a **12 dB/oct multimode VCF** with:

- **4 simultaneous outputs**
  - **LP** low-pass
  - **HP** high-pass
  - **BP** band-pass
  - **N** notch
- **Cutoff control** (`Frequ.`)
- **Two frequency CV inputs**
  - `CV1` without attenuator, about **1V/oct**
  - `CV2` with attenuator `FCV2`
- **Resonance control** (`Q`)
- **Resonance CV input** (`CQ`)
- **Self-oscillation**, meaning it can act like a **sine oscillator**
- **Audio input with level control**, including intentional overdrive/distortion at higher settings

That means this filter is not just for tone shaping — it can be used as:

1. a **melody voice** by self-oscillation  
2. a **timbre shaper** for another oscillator’s melody  
3. a **multi-output tone splitter** for layered melodic lines  
4. a **dynamic, playable resonant processor** for sequenced patches

---

## 1. Use it as a sine-wave melodic oscillator

The most important melodic feature in the manual is:

- **resonance up to self-oscillation**
- **CV1 has about 1V/oct sensitivity**

This means the A-121-3 can generate its own tone even **without any audio input**, and that tone can be played melodically.

### Basic patch

- Leave **audio input In unpatched**
- Turn up **Q** until the filter starts **self-oscillating**
- Send your sequencer or keyboard pitch CV to **CV1**
- Take audio from **LP** or **BP** output
- Send that to a **VCA**
- Use an **envelope** to control the VCA
- Clock your sequencer as normal

### Result

You get a **clean sine-like melodic voice**, great for:

- basslines
- sub melodies
- FM sources
- minimal techno tones
- soft lead lines

### Musical character

Because it’s a self-oscillating filter, the pitch tracking may be **usable rather than precision-VCO perfect**. That’s often musically excellent for:

- short melodic loops
- drones with tonal centers
- acid-adjacent bass tones
- percussion tuned to scale degrees

---

## 2. Filter another oscillator to create expressive melodies

A more common use is to run a VCO through the A-121-3 and sequence the oscillator normally, while using the filter to add movement.

### Patch idea

- VCO saw or pulse → **In**
- Sequencer pitch CV → VCO 1V/oct
- Gate → envelope
- Envelope → VCA CV
- Another envelope or the same envelope → **CV2**
- Set `FCV2` to taste
- Output from **LP** or **BP**

### Why this is melodic

The melody comes from the oscillator pitch, but the A-121-3 adds:

- note articulation
- brightness contour
- vowel-like emphasis
- resonant emphasis at musical partials

A 12 dB/oct filter tends to sound **more open and less severe** than a 24 dB ladder-style filter, which is very nice for:

- melodic sequences that need clarity
- chords or interval patches
- arpeggios that shouldn’t get too muffled
- animated leads

---

## 3. Exploit the four simultaneous outputs for layered melodic voices

One of the best features here is that **LP, HP, BP, and Notch are all available at once**.

That means one source can become **multiple melodic layers**.

### Patch idea: one sequence, three tones

- VCO → **In**
- Main sequence controls VCO pitch
- Send:
  - **LP** → one VCA/mixer channel
  - **BP** → second VCA/mixer channel
  - **HP** → third VCA/mixer channel

Then:

- use separate envelopes on each VCA, or
- pan them differently, or
- add different effects to each output

### Musical result

You can turn one monophonic melody into:

- a body layer (LP)
- a nasal/midrange layer (BP)
- a thin attack/air layer (HP)

This is especially effective for:

- melodic techno
- Berlin school sequences
- IDM-style timbral counterpoint
- pseudo-polyphonic texture from one source

### Bonus use: interval illusion

If resonance is high, different outputs can emphasize different harmonics. By balancing outputs separately, you can make a single melody feel harmonically richer and more “composed.”

---

## 4. Use band-pass mode for focused melodic lines

The **BP output** is especially strong for melodic work.

Why:

- it removes excessive lows and highs
- it creates a very “voiced” center
- it sits in a mix well
- it can sound vocal or reed-like with resonance

### Good uses

- plucky sequences
- woody basslines
- tuned percussion
- expressive lead sounds

### Patch tip

Send an envelope to **CV2** and keep resonance moderately high. This gives each note a defined center frequency sweep and helps melodies speak more clearly.

---

## 5. Sequence the filter cutoff itself as a melodic layer

Since `CV1` is approximately **1V/oct**, the filter cutoff can be treated as a **pitched parameter**, even when processing incoming sound.

### Patch idea

- Rich oscillator or noise source → **In**
- Sequencer pitch CV or a second sequencer row → **CV1**
- Moderate-to-high resonance
- Take **BP** output

### Result

The filter “picks out” frequencies according to the sequenced CV, creating:

- tuned resonant lines
- pseudo-formant melodies
- spectral arpeggios
- tonal percussion from noise

This is a classic way to make melodies from otherwise non-melodic material.

### Especially useful sources

- white or pink noise
- saw wave
- supersaw-ish mixed oscillators
- chord source
- external audio loops

With noise into a resonant BP filter and sequenced cutoff, you can get **flute-like or whistling melodic phrases**.

---

## 6. Voltage-control the resonance for animated note behavior

The A-121-3 includes **CV control over resonance (`CQ`)**, which is a big musical advantage.

The manual notes that unlike the A-121-2, the A-121-3 has **no attenuator** for this resonance CV input, so you’ll often want an external attenuator or a carefully sized modulation source.

### Musical uses of resonance CV

#### Per-note emphasis
- Send an envelope to `CQ`
- Each note becomes more resonant at the attack
- Great for plucks and accented melodies

#### Accent programming
- Send an accent trigger/envelope to `CQ`
- Some notes become sharper, more vocal, more “speaking”
- Excellent for acid-style sequencing

#### Slow macro-expression
- Send an LFO or slow random CV to `CQ`
- The melody stays the same, but the timbre becomes more or less focused over time

### Why this matters melodically

Resonance determines how much the filter emphasizes the cutoff area. In melodic patches, that often acts like **articulation**, almost like changing embouchure or vowel shape on a wind instrument.

---

## 7. Drive the input for harmonically rich melodic distortion

The manual mentions that above about **Level position 5**, distortion/clipping can occur with normal A-100 levels.

This is very useful for melodic parts because distortion before/inside filtering can add:

- more harmonics
- stronger resonance interaction
- greater note definition
- aggressive lead and bass character

### Patch idea

- VCO triangle/saw → **In**
- Turn **Level** up into mild clipping
- Use **LP** or **BP**
- Sequence normally
- Add envelope to **CV2**

### Result

Compared with a clean input, you’ll hear:

- more bite
- stronger filter sweeps
- more audible resonance
- more attitude in bass or lead lines

This is especially good for:

- EBM bass
- acid-like riffs
- industrial sequences
- synthwave leads

---

## 8. Use the notch output for moving melodic space

The **Notch output** is less commonly the “main voice” output, but it can be very musical.

A notch filter removes a narrow band, creating a moving hollow character. In a melodic context this works well when:

- the source is harmonically rich
- the melody is already established by the oscillator
- you want motion without losing low and high content

### Patch idea

- Saw VCO → **In**
- Pitch CV to VCO
- Envelope or LFO to **CV2**
- Use **N** output

### Musical effect

You get a timbre that shifts around the spectrum in a subtle but very alive way — ideal for:

- pads playing melodic phrases
- secondary lead layers
- dubby or psychedelic sequences
- stereo pairing with LP or BP

---

## 9. Build tuned percussion and struck melodies

Because the filter can self-oscillate and respond to CV, it can be used for **tuned percussion**.

### Patch idea A: self-oscillating ping
- No audio input
- Raise `Q` to self-oscillation edge
- Send short envelopes to `CV2`
- Pitch sequence to `CV1`
- Output from LP or BP

### Patch idea B: resonant ping from impulse
- Short trigger/click/noise burst → **In**
- High `Q`
- Pitch CV to `CV1`
- Short modulation envelope to cutoff

### Musical applications

- marimba-like lines
- tom melodies
- tuned bleeps
- West Coast-ish plucked sequences

This works especially well in minimal or percussive melodic composition.

---

## 10. Pair it with common module types for full melodic systems

Since the manual only covers the A-121-3, here’s how it fits into a larger melodic Eurorack patch.

### With a VCO
Use the A-121-3 as the main subtractive voice shaper.

Best for:
- basslines
- leads
- arps
- drones

### With an envelope generator
Patch envelope to `CV2` for classic note contour.

Best for:
- plucks
- swells
- acid movement
- expressive articulation

### With a sequencer
- pitch CV to VCO or directly to `CV1` in self-oscillation mode
- gate to envelope
- accent row to `CQ`

Best for:
- evolving sequences
- accented patterns
- melodic repetition with variation

### With an LFO
- subtle LFO to `CV2` for vibrato-like timbre movement
- slow LFO to `CQ` for evolving resonance

Best for:
- animated sustained notes
- ambient melodies
- moving ostinatos

### With a VCA
Essential if using the A-121-3 as a self-oscillating voice, since the filter itself does not provide amplitude shaping.

### With a mixer
Because all four outputs are simultaneous, a mixer lets you create blended timbres:
- LP + BP = focused but warm
- HP + BP = thin, vocal, cutting
- LP + N = rich but animated

---

## Example melodic patch recipes

## Patch 1: Simple sine bass voice
- No input to filter
- `Q` up to self-oscillation
- Sequencer CV → `CV1`
- LP output → VCA → mixer
- Gate → envelope → VCA

Sound:
- pure, rounded bassline
- good for minimal techno or electro

---

## Patch 2: Acid-adjacent lead
- Saw VCO → `In`
- Pitch CV → VCO
- Envelope → `CV2`
- Accent envelope → `CQ`
- BP or LP out to VCA/mixer
- Input `Level` pushed above 5 for drive

Sound:
- squelchy, articulate, dynamic
- especially good with step sequencer accents

---

## Patch 3: Noise-to-melody patch
- Noise source → `In`
- Sequencer CV → `CV1`
- High resonance
- BP output → VCA
- Envelope to VCA and/or `CV2`

Sound:
- whistling, breathy, tuned melodic figures
- excellent for experimental melodies

---

## Patch 4: One melody, three layers
- Saw VCO → `In`
- Pitch CV → VCO
- LP, BP, HP each to separate VCA or mixer channels
- Different envelopes or effects per output

Sound:
- one sequence becomes a complete melodic texture

---

## Patch 5: Resonant tuned percussion
- Short trigger pulse or click → `In`
- High `Q`
- Sequencer CV → `CV1`
- BP output to mixer
- Optional envelope to `CV2`

Sound:
- tuned hits, woodblock/tom-style melodic percussion

---

## Performance notes

A few practical takeaways from the manual:

- **CV1 is the main pitch-relevant input** because it has about **1V/oct sensitivity**
- **CV2** is best for controlled modulation because it includes the **FCV2 attenuator**
- **CQ has no attenuator**, so use care; external attenuation is helpful
- The module reaches **self-oscillation**, making it a valid sound source on its own
- The **input level control** can intentionally add musical distortion
- The **12 dB/oct slope** tends to sound musical and less overly closed-in than steeper filters

---

## Bottom line

The Doepfer **A-121-3** is more than a compact filter. For melodic music, it can function as:

- a **sine oscillator voice**
- a **sequenced resonator**
- an **expressive subtractive filter**
- a **multi-output tone layer generator**
- a **per-note articulation tool** via resonance CV
- a **distortion-plus-filter lead/bass processor**

If you build around it with a **sequencer, envelope, VCA, and one oscillator**, it becomes a very capable melodic centerpiece. If you use **self-oscillation**, it can even become the oscillator itself for pure and focused melodic lines.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)