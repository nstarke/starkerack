# Bastl Instruments — ABC Mixer

- [Manual PDF](../../manuals/manual-abc-web.pdf)

---

[Manual PDF](#)

## Bastl Instruments ABC — using it for melodic work in a Eurorack system

The attached manual is for the **Bastl Instruments ABC**, a **6-channel mixer**. By itself, ABC does **not generate pitch, gates, envelopes, or sound**, so it is not a melodic voice on its own. But in a melodic patch, it is very useful as a **utility mixer** for combining the control voltages and audio signals that make melodies expressive and playable.

## What the module does

ABC provides:

- **6 inputs**: A, B, C, D, E, F
- **2 outputs**:
  - **A+B+C**
  - **D+E+F**
- If nothing is patched into **A+B+C out**, that mix is **normalled into D+E+F out**, so the module can act as:
  - **two 3-channel mixers**, or
  - **one 6-channel mixer**
- Each channel has a **gain knob**
- **Maximum gain is 1** per channel
- By default the inputs are **AC-coupled** for audio
- There are **solder jumpers** on the back to change it for **DC-coupled CV mixing**
- There are **3 normalization jumpers** on the back:
  - A normalled to D
  - B normalled to E
  - C normalled to F

## Why this matters for melody

Melody in Eurorack usually comes from combining:

- **pitch CV**
- **sequence transposition**
- **modulation**
- **clocked variation**
- **layered audio voices**

ABC is ideal for the **combining** part.

---

## Best melodic uses for ABC

### 1. Mix multiple audio voices into one melodic line or harmony bus
If you have several oscillators or full voices playing related notes:

- Voice 1 audio → A
- Voice 2 audio → B
- Voice 3 audio → C
- Output from **A+B+C** → filter / VCA / effects / final mix

This is the most direct melodic use:
- combine a **lead oscillator**
- a **sub octave**
- a **FM layer**
- or several voices playing chords or counterpoint

Because each channel has its own level control, ABC works well for balancing:
- root note vs fifth
- lead vs harmony
- dry oscillator vs processed layer

### 2. Build a 6-oscillator chord or unison stack
Since A+B+C can cascade into D+E+F, you can use all six channels as one mix bus:

- Osc 1 → A
- Osc 2 → B
- Osc 3 → C
- Osc 4 → D
- Osc 5 → E
- Osc 6 → F
- Take output from **D+E+F**

This is excellent for:
- supersaw-style unison
- chord stacks
- layered sine partials
- combining multiple plucked or struck voices into one harmonic texture

For melodic music, this is especially good if the oscillators are:
- tuned to chord tones
- slightly detuned
- spread across octaves

### 3. Use it as a stereo melodic mixer
The rear jumpers can normalize:
- A → D
- B → E
- C → F

This lets you patch the same melodic sources into left and right groups and adjust each side separately. For example:

- Melody voice 1 → A
- Melody voice 2 → B
- Melody voice 3 → C
- Use **A+B+C** as Left
- Use **D+E+F** as Right

Then you can create stereo width by setting different levels on D/E/F than on A/B/C.

This is useful for:
- stereo chord voices
- left/right balance of arp layers
- pseudo-stereo melodic textures before effects

### 4. Mix pitch CV sources for transposition and variation
The manual says ABC can be modified for **CV mixing** by closing the solder jumpers on the back, which bypass the capacitors and make it suitable for **DC-coupled** signals.

Once modified for CV, ABC becomes very useful for melodic control.

Example:
- Sequencer pitch CV → A
- Precision offset or keyboard CV → B
- Slow modulation or random stepped CV → C
- **A+B+C out** → oscillator 1V/oct

This lets you create:
- transposed sequences
- evolving melodies
- offset pitch structures
- controlled randomness

Important note:
because this is just a mixer, not a precision adder, pitch mixing may be musically useful but may not be as exact as a dedicated precision adder for strict tonal tracking over many octaves.

Still, for:
- small transpositions
- melodic drift
- layering sequence sources
- experimental tonal work

…it can be very effective.

### 5. Mix modulation sources that shape melody indirectly
Even if you don’t use it for pitch CV, ABC is very useful for combining modulations that affect melodic articulation:

- Envelope + LFO + velocity CV → filter cutoff
- Envelope + random CV → wavefolder amount
- Sequencer row + LFO → FM index
- Accent CV + envelope → VCA control path

This helps create more musical phrasing:
- brighter notes on accents
- timbre changes across a sequence
- evolving harmonic content
- rhythmic movement in melodic lines

Again, this requires the **CV modification** if you want proper DC-coupled CV behavior.

---

## Patch ideas for melodic components

### Patch 1: Layered lead voice
Use ABC as an audio mixer for one melody built from several sources.

- VCO saw → A
- VCO pulse → B
- Sub oscillator → C
- A+B+C out → filter → VCA → output
- Sequencer pitch CV controls all oscillators

Result:
- one melody
- richer timbre
- easy balancing of harmonic layers

### Patch 2: Harmony stack
Create a chord from several independently tuned oscillators.

- Root oscillator → A
- Third → B
- Fifth → C
- Seventh or octave → D
- Ninth or doubled root → E
- Noise/transient layer → F
- Final output from D+E+F

Result:
- a full harmonic bed or stab voice
- useful for pads, chord hits, and drone harmony

### Patch 3: Stereo arpeggio mixer
With rear normalization jumpers set:

- Arp voice 1 → A
- Arp voice 2 → B
- Arp voice 3 → C
- Left = A+B+C
- Right = D+E+F

Set different right-side levels for a stereo image.

Result:
- wider melodic field
- clearer separation of lines
- more polished stereo presentation

### Patch 4: CV melody shaping mixer
After CV mod:

- Main sequencer CV → A
- Transpose CV from keyboard or sequencer row → B
- Stepped random CV → C
- A+B+C → oscillator pitch input

Use small amounts on B and C.

Result:
- melody stays recognizable
- but gains movement and variation
- great for generative tonal patches

### Patch 5: Two parallel melodic buses
Use ABC as two separate 3-channel mixers.

Bus 1:
- Lead voice layers → A/B/C
- A+B+C → lead processing chain

Bus 2:
- Harmony / counter-melody layers → D/E/F
- D+E+F → second processing chain

Result:
- one module handles both lead and accompaniment summing

---

## Things to keep in mind

### 1. Default behavior is for audio
Out of the box, the inputs are **AC-coupled**, so it is intended primarily for **audio mixing**.

If you want to mix:
- pitch CV
- envelopes
- gates
- offsets
- LFOs used as steady CV

you should use the rear **solder jumpers** to convert it for **DC-coupled CV mixing**.

### 2. Maximum gain is 1
This means it is a **unity-gain style mixer**, not a boost mixer. It combines signals, but does not amplify channels above their incoming level.

### 3. It is not a precision adder
For exact melodic pitch operations, especially 1V/oct transposition over large ranges, a dedicated precision adder is often better. ABC is best for:
- practical utility mixing
- approximate CV blends
- experimental melodic control
- audio layering

### 4. It is especially strong in small systems
In a compact rack, ABC is great because melodic patches often need simple summing:
- several oscillators into one voice
- several voices into one harmony bus
- modulation sources combined for expressive articulation

---

## Bottom line

The **Bastl ABC** is best thought of as a **support module for melodic patching** rather than a melody generator.

It helps create melodic components by letting you:

- **layer multiple oscillators** into richer leads and chords
- **combine several melodic voices** into one submix
- **build stereo melodic mixes**
- **mix CV sources** for transposition and variation, if modified for DC coupling
- **combine modulation signals** that make melodies more expressive

So if your system already has:
- sequencers
- quantizers
- oscillators
- envelopes
- filters
- VCAs

then ABC becomes very useful as the glue that turns separate melodic ingredients into a coherent musical line or harmonic texture.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)