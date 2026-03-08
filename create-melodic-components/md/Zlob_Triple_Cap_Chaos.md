# Zlob — Triple Cap Chaos

- [Manual PDF](../../manuals/Zlob Modular - Triple Cap Chaos.pdf)

---

[Manual PDF / Product Page: Zlob Modular Triple Cap Chaos](https://zlobmodular.com/product/triplecapchaos/)

# Using the Zlob Modular Triple Cap Chaos for melodic music

The **Triple Cap Chaos** is not a conventional melodic oscillator. It is a **2hp chaotic analog audio-rate module** that behaves as:

- a **chaotic oscillator**
- an **audio mangler**
- a **pseudo ring modulator / harmonics generator**
- a source of **two related outputs**: **X** and **Y**

From the manual text, the key point is that this module is **not 1V/oct** and has a **fairly narrow operating frequency range** intended to preserve chaotic behavior. So if your goal is “melody,” the best approach is usually **indirect**: use it to generate pitched-ish material, harmonic variation, animated timbres, and stereo/interval relationships rather than expecting precise keyboard tracking.

---

## What the module gives you

### Controls
- **Emanate**
  - Coarse control over the overall chaotic spectrum
  - Counterclockwise = more activity / more chaos
  - Clockwise = less chaos / more steady oscillation

- **Width / CV Att**
  - Fine control over the chaotic behavior
  - If nothing is patched to **CV**, this acts as a manual fine control
  - If **CV** is patched, the knob becomes an **attenuator** for the incoming modulation

### Inputs
- **CV**
  - Expects roughly **-5V to +5V max**
  - Modulates the chaos behavior / oscillation region

- **IN**
  - **AC-coupled input**
  - Intended for audio, but both CV and audio may produce interesting results
  - External signals interact with the onboard oscillator

### Outputs
- **X**
  - “windy,” noisier, more sinusoidal character

- **Y**
  - more squared-off, aggressive, harsher

### Useful specs / behavior
- Both outputs are generally around **10 Vpp**
- Frequency range is limited, roughly around **150–250 Hz** depending on settings
- Extreme settings or certain input signals can push it out of its desired operating region and cause oscillation to cut out

---

# Best melodic roles for Triple Cap Chaos

Because this is chaotic and not trackable, think of it in these roles:

## 1. A drone voice with implied pitch
Set the module in a less chaotic regime and treat it like a semi-pitched drone source.

### Patch idea
- Turn **Emanate** more clockwise to reduce chaos
- Use **Width** to find a stable-ish resonant zone
- Take **X** output into:
  - a **VCA**
  - then a **filter**
  - then your output mixer
- Use a sequencer or keyboard to control the **filter cutoff** and **VCA envelope**

### Why this works musically
Even if the oscillator itself is not tracking pitch, your ear can still hear melody when:
- notes are articulated rhythmically
- spectral emphasis changes per note
- the timbre stays in a controllable pitched region

This is especially effective for:
- industrial melodies
- sci-fi lead lines
- unstable bass drones
- dark ambient motifs

---

## 2. Harmonic layer on top of a proper VCO
This is one of the strongest uses for melodic music.

### Patch idea
- Use a **standard 1V/oct oscillator** as your main melodic voice
- Send that oscillator into the **IN** jack of Triple Cap Chaos
- Take **X** or **Y** out and mix it with the dry oscillator
- Envelope the mixed result with a VCA

### Result
The Triple Cap adds:
- ring-mod-like sidebands
- extra harmonics
- unstable upper partials
- “bit-crushed” or broken digital-like texture while still being analog

### Musical use
This gives you a melody that is still clearly controlled by the main oscillator, but with a much more animated and distinctive timbre.

Use:
- **X** for softer, ghostly, airy melodic enhancement
- **Y** for aggressive, metallic, more percussive lines

---

## 3. Animated parallel voice for interval-like motion
Because **X** and **Y** are related but different, you can use them as two correlated voices.

### Patch idea
- Send **X** to the left channel and **Y** to the right
- Or send **X** and **Y** into two separate VCAs/filters
- Shape each path differently:
  - X → lowpass filter
  - Y → wavefolder or highpass filter
- Trigger both with related but different envelopes

### Musical use
This can create:
- stereo melodic motion
- call-and-response textures
- pseudo-intervals
- evolving doubled lead lines

Even without exact pitch control, the shared chaotic core makes the two outputs feel musically connected.

---

## 4. Chaos as a melodic accent processor
Rather than using Triple Cap as the whole voice, use it only on selected notes or phrases.

### Patch idea
- Main melody from a standard oscillator
- Mult the oscillator:
  - one copy stays dry
  - one copy goes into **Triple Cap IN**
- Put Triple Cap output through its own VCA
- Open that VCA only on specific sequencer steps

### Result
You get a stable melody with occasional chaotic note accents:
- fills
- transitions
- phrase endings
- chorus lift
- glitch emphasis

This is one of the most practical “musical” uses in a melodic system.

---

# Creating melodic behavior with modulation

## 5. Step-sequence the CV input
The manual says the **CV** input modulates the chaos and expects up to about **±5V**.

That means you can send:
- sequencer voltages
- offset/random stepped voltages
- envelopes
- LFOs
- quantized random

### Important caveat
This will **not** behave like 1V/oct pitch input. Instead, it moves the circuit through different chaotic states and frequencies.

### How to make it musical
Use:
- a **quantized stepped CV**
- a **small attenuation amount**
- a **clocked sequence**

This can create repeating “note-like” changes in:
- density
- timbre
- apparent pitch center
- aggressiveness

### Tip
Keep the CV depth modest. Too much modulation may push the oscillator into unstable or silent regions.

---

## 6. Use a quantizer upstream for repeatable “chaos melodies”
A quantizer can still help even though Triple Cap is not pitch-trackable.

### Patch idea
- Random source or sequencer → **quantizer**
- Quantizer output → attenuator → **CV input**
- Tune **Emanate** and **Width** until the module sits in a musically useful zone

### What you get
Not exact notes, but **repeatable islands of tone behavior** that correspond to scale steps. This can sound like:
- broken arpeggios
- unstable acid lines
- mutated motifs
- “alive” melodic fragments

This works especially well if you are making:
- IDM
- experimental techno
- electro-acoustic music
- horror soundtrack cues

---

## 7. Envelope-based note shaping
A classic way to force melodic phrasing onto a nontraditional sound source.

### Patch idea
- Triple Cap **X** or **Y** → VCA
- ADSR or function generator → VCA CV
- Trigger envelopes from a sequencer rhythm
- Optionally send the same envelope, attenuated, into **CV**

### Musical result
Each note has:
- a clean start and finish
- a dynamic contour
- a timbral sweep tied to articulation

This helps the ear perceive events as “notes” even if the source pitch is unstable.

---

# Using external oscillators for stronger melodic control

## 8. Process a tuned oscillator for melodic mangling
This is probably the easiest way to get clearly melodic output.

### Patch idea
- 1V/oct VCO or complex oscillator plays the melody
- Send VCO sine/triangle/saw into **IN**
- Use Triple Cap output as the audible voice
- Try sequencing or slowly modulating **Emanate** and **Width**

### What happens
The incoming pitched audio interacts with the chaotic core, producing:
- sidebands
- distorted pitch shadows
- metallic upper harmonics
- unstable ring-mod style tones

If the source oscillator is very simple, the results can remain surprisingly musical.

### Best source waveforms
- **Sine**: most controlled, best for subtle enhancement
- **Triangle**: still musical, slightly richer
- **Saw**: more dramatic and abrasive
- **Pulse**: aggressive, good for industrial leads

---

## 9. Use it after a sequenced sub-oscillator or bass voice
For basslines, instability can actually help.

### Patch idea
- Sequenced bass oscillator → **IN**
- Triple Cap **Y** out → lowpass filter → VCA
- Envelope on filter and VCA
- Blend some dry bass back in

### Result
You keep low-end pitch identity while adding:
- growl
- tearing harmonics
- chaotic edge
- note-to-note variation

This is excellent for:
- EBM
- industrial
- broken electro
- experimental acid

---

# X and Y as melodic materials

## 10. X for lyrical material, Y for rhythmic aggression
From the manual:

- **X** = more sinusoidal, windy, noisy
- **Y** = squarer, harsher, more aggressive

That naturally suggests different melodic roles.

### Use X for
- ghost melodies
- drones
- filtered lead tones
- softer counterlines
- atmospheric arpeggios

### Use Y for
- bass stabs
- metallic hooks
- rhythmic ostinatos
- distorted lead accents
- pseudo-digital riffs

### Combined patch
- X → long envelope, reverb, delay
- Y → short envelope, distortion, sequenced gate

You get one chaotic source doing both:
- melodic atmosphere
- rhythmic melodic punctuation

---

# Practical melodic patch recipes

## Patch 1: Unstable lead voice
**Goal:** expressive lead that feels melodic but alive

- Triple Cap **X out** → lowpass filter → VCA
- Envelope → VCA CV
- Keyboard/sequencer → filter cutoff tracking input if available
- Slow LFO → CV input, lightly attenuated
- Emanate set toward more stable oscillation
- Width adjusted for the sweet spot

**Sound:** eerie, vocal, unstable lead tone

---

## Patch 2: Chaotic harmonics over a normal melody
**Goal:** preserve exact notes while adding character

- VCO (1V/oct melody) → mult
- Copy 1 → mixer
- Copy 2 → Triple Cap **IN**
- Triple Cap **Y** → mixer
- Mixer → filter/VCA/output
- Optional envelope to bring the Triple Cap layer in only on accents

**Sound:** articulate melody with metallic, animated overtone layer

---

## Patch 3: Stereo melodic texture
**Goal:** one source becomes a wide melodic field

- Triple Cap **X** → left VCA/filter
- Triple Cap **Y** → right VCA/filter
- Same gate triggers both envelopes
- Slightly different envelope times or filter settings per side
- Reverb after both channels

**Sound:** wide, shifting melodic image with natural chaotic motion

---

## Patch 4: Quantized chaos motif
**Goal:** repeating note-like pattern from chaos

- Sequencer or random source → quantizer
- Quantizer → attenuator → Triple Cap **CV**
- Triple Cap **X** → VCA
- Clocked envelope → VCA
- Tune Emanate/Width for a stable center region

**Sound:** semi-pitched repeating figure, excellent for experimental melodies

---

## Patch 5: Chaotic bass enhancer
**Goal:** make a bassline more unique without losing impact

- Bass VCO → mult
- Dry path → mixer
- Second path → Triple Cap **IN**
- Triple Cap **Y** → lowpass filter → mixer
- Envelope controls filter/VCA downstream
- Blend wet subtly

**Sound:** bass remains musical but gains shredded harmonic texture

---

# Performance tips

## Find “islands” of stability
The manual suggests there are operating zones where it behaves more like a steady oscillator and others where it is much more chaotic. For melodic use, spend time finding those **stable islands**.

A good workflow:
1. Set **Emanate** high enough for steadier tone
2. Sweep **Width** slowly
3. Listen for regions with a definite pitch center
4. Then add only small CV modulation

---

## Don’t overdrive the CV input
Since large modulation can push the circuit out of its useful operating range, use:
- attenuators
- offset generators
- VCAs for modulation depth control

Small modulation often sounds more musical than large swings here.

---

## Let filtering do some of the “pitch clarification”
If the sound is too unruly, a filter can help emphasize a pitch center. Try:
- lowpass for bass/lead
- bandpass for nasal melodic focus
- resonant filter for quasi-formant note shaping

---

## Use rhythm to make chaos feel melodic
Even when pitch is unstable, the ear hears melody better if there is:
- repeated timing
- phrase structure
- accents
- consistent envelope shapes

So clocked gates and phrase repetition are your friend.

---

# Bottom line

The **Triple Cap Chaos** is best used for melody in these ways:

1. **As a semi-pitched chaotic voice** in its more stable settings  
2. **As a timbral processor** for a normal 1V/oct oscillator  
3. **As a dual-output melodic texture source** using X and Y together  
4. **As an accent layer** added only to certain notes or phrases  
5. **As a sequenced chaos circuit** where CV creates repeating note-like states rather than exact pitches

If you expect precise tuning, it will fight you. If you treat it as a **melodic instability generator**, it becomes extremely useful and distinctive.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)