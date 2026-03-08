# Moog — Mavis

- [Manual PDF](../../manuals/MAVIS_MANUAL_V2_06.27.2022.pdf)

---

[Moog Mavis User Manual (PDF / product page)](https://www.moogmusic.com/media/2022/06/Mavis_Manual.pdf)

# Using Moog Mavis to Create Melodic Components in Music

The **Moog Mavis** is a compact semi-modular analog synth voice that can generate a surprising range of **melodic material** on its own or as part of a Eurorack system. From the manual, its key melodic building blocks are:

- **VCO** for pitch generation
- **Keyboard / KB CV / 1V-OCT** for note control
- **EG** for note articulation
- **VCF** for timbral shaping
- **VCA** for amplitude contour
- **LFO** for cyclic modulation or even second-oscillator audio use
- **Sample + Hold** for stepped voltages and pseudo-random melodies
- **Mixer / Attenuator / Mult / Wavefolder** for shaping and routing pitch and timbre control

Below is a practical analysis of how these modules work together specifically for **melodic synthesis**.

---

## 1. Core melodic voice architecture

At its simplest, Mavis already contains a normalled melodic signal path:

**Keyboard / external pitch CV → VCO → VCF → VCA → output**

And for note triggering:

**Keyboard / external gate → EG → VCA**

This means Mavis naturally behaves like a classic monosynth voice. For melody writing, this gives you three essential layers:

1. **Pitch source**  
   - Internal keyboard via **KB CV**
   - External sequencer via **1V/OCT**
2. **Note articulation**
   - Gate into **EG**
   - EG shapes note onset and duration through the **VCA**
3. **Tone shaping**
   - VCO waveform and pulse width define harmonic base
   - VCF cutoff/resonance define brightness and contour

This is the foundation for basslines, lead lines, arps, and sequenced motifs.

---

## 2. Melodic pitch generation

## A. Internal keyboard as a melodic controller

The onboard one-octave button keyboard outputs pitch through the internal routing and also via **KB CV out**.

Useful melodic behaviors from the manual:

- **KB SCALE** changes the voltage span of the keyboard  
  - Full CCW: one octave across low C to high C
  - Full CW: five octaves across the same keys

This is unusual and musically powerful. It means the keyboard can act as:

- a normal one-octave melodic keyboard
- a **compressed pitch map** for wide melodic leaps
- an expressive CV source for transposition and interval experiments

### Musical use
- Set KB SCALE low for traditional melodies
- Increase KB SCALE for larger interval jumps and wide-register riffs
- Use GLIDE to turn discrete notes into portamento phrases

---

## B. External sequencer or Eurorack pitch CV

The **1V/OCT input** allows Mavis to be driven from any sequencer, keyboard, quantizer, or CV source.

This makes Mavis ideal as a **complete analog melodic voice** in a modular system.

### Common melodic patch
- External sequencer pitch CV → **1V/OCT**
- External gate/trig → **GATE**
- Audio out from **/VCA** to mixer or interface

This gives you:
- precise melodic sequences
- synchronized timing
- classic analog note articulation

---

## C. Sample + Hold as a melody generator

The **S+H** circuit is one of the most useful melodic tools in Mavis.

By default:
- **VCO** is the sample source
- **LFO** is the gate source

The result is a stepped voltage output at **S+H out**, which can be patched to pitch destinations like **1V/OCT**.

### Why this creates melodies
When S+H samples a changing waveform, it outputs discrete voltage steps. Those steps can become pitches when sent to the oscillator pitch input.

### Patch idea
- **S+H out → 1V/OCT**

Now the oscillator pitch jumps in stepped intervals. If the VCO source waveform is saw, the values vary more continuously and produce broader pitch variety.

### Make it musical
Because raw S+H can be too wide or erratic:
- use the **Attenuator**
- use **KB CV** as a transposition source
- use the **Mixer** to combine offsets and pitch voltages

This is one of the best ways to create:
- generative melodies
- pseudo-random riffs
- Berlin-school stepping patterns
- experimental lead lines

---

## 3. Controlling melodic range and transposition

Mavis includes several utilities that are extremely useful for turning raw control voltage into musical pitch material.

## A. Attenuator for pitch interval control

Patch:
- **S+H out → ATTN (+5)**
- **ATTN out → 1V/OCT**

Now the **ATTENUATOR** knob scales the pitch movement.

### Musical result
- low attenuation = small interval melody
- high attenuation = wide leaps

This is essential for making random voltages feel more musical.

---

## B. Mixer for pitch offsets and combining sources

The **ONE/TWO mixer** can combine voltages, not just audio. This means it can build more complex melodic CV.

Examples:

### 1. Add transposition offset
- Put a CV into **TWO**
- Use **ONE LVL** with nothing at ONE input for offset behavior described in the manual

This can shift a melodic line up/down.

### 2. Combine two melodic sources
- Sequencer CV → **TWO**
- S+H or LFO CV → **ONE**
- **ONE+TWO out → 1V/OCT**

This creates:
- melody plus ornament
- pitch drift
- interval modulation
- semi-random note variation over a structured sequence

---

## C. Mult for parallel melodic control

The **MULT** lets one pitch source affect several destinations at once.

### Example
- **KB CV → MULT**
- **MULT 1 → 1V/OCT**
- **MULT 2 → LFO RATE**

Now the keyboard pitch also changes LFO rate. If the LFO is in audio range, this enables pitch-linked harmonic behavior. If the LFO is in low range, it gives note-dependent modulation speeds, which can make melody lines feel more animated.

---

## 4. Articulation: turning pitches into notes

Pitch CV alone is not enough for melody. The note needs time-shaping. On Mavis, this is mainly handled by:

- **GATE**
- **EG**
- **VCA**
- optionally **VCF modulation**

## A. EG to VCA = note shape

By default the envelope generator shapes the VCA. This creates note contours:

- **Attack**: slow or sharp onset
- **Decay**: fall from peak
- **Sustain**: held note level
- **Release**: tail after key/gate ends

### Musical uses
- Fast attack / short decay / low sustain = pluck, sequence blip, bass stab
- Fast attack / medium decay / medium sustain = lead line
- Slow attack / long release = melodic pad-like phrasing
- Long release + glide = lyrical mono lead

---

## B. EG to filter for melodic expressiveness

The **VCF MOD MIX** and **VCF MOD AMT** let the EG shape filter cutoff.

This is critical for melody because it makes each note dynamically “speak.”

### Musical results
- positive filter EG: classic synth pluck
- negative filter EG: darker attack and opening tail
- higher resonance: vowel-like melodic articulation
- moderate envelope amount: expressive phrasing without overpowering pitch

For melodies, filter envelopes are often as important as note pitch.

---

## 5. Using modulation to enrich melodies

## A. LFO vibrato

Use the VCO modulation section:
- **VCO MOD MIX toward LFO**
- raise **PITCH MOD AMT**

This creates pitch modulation.

### Musical result
- low amount, medium rate = vibrato
- slow rate = drifting melodic line
- fast rate = FM-like brightness or instability

For leads, subtle vibrato adds life.

---

## B. PWM for animated melodic timbre

If using pulse wave:
- set **VCO WAVE** toward pulse
- raise **PWM AMT**
- choose EG or LFO with **VCO MOD MIX**

This creates melodic tones that evolve over time.

### Musical result
- LFO PWM = classic animated lead/pad character
- EG PWM = every note has its own timbral attack
- useful for melody lines needing movement without filter overuse

---

## C. Filter modulation as phrasing engine

Use:
- **VCF MOD MIX** to choose EG/LFO blend
- **VCF MOD AMT** to define depth and polarity

This can create:
- repeating brightness pulses across a sequence
- note-by-note contour
- syncopated tonal motion if driven externally

A melody becomes much more compelling when timbre moves with it.

---

## 6. LFO as a second oscillator for richer melodic voices

One of the most musically important manual examples is using the **LFO in audio rate** as a second oscillator.

Patch:
- **LFO out → ONE (-5)**
- **VCO out → TWO**
- **ONE+TWO out → FOLD IN**
- optionally **KB CV → LFO RATE**

### Why this matters melodically
A second oscillator thickens a melody dramatically:
- intervals
- beating
- richer harmonics
- more presence for bass or lead lines

Without the **KB CV → LFO RATE** patch, the LFO stays at fixed pitch while the VCO tracks the keyboard. That creates drone-against-melody effects.

With **KB CV → LFO RATE**, both oscillators track together more like a classic dual-osc monosynth.

### Musical applications
- fat basslines
- harmonically dense lead sounds
- metallic melodic phrases when slightly detuned
- aggressive solos when combined with wavefolder

---

## 7. Wavefolder for melodic timbre design

Mavis is notable for including a **wavefolder**, and this can strongly affect melodic presence.

Patch:
- **VCO out → FOLD IN**

Now the oscillator is routed through the folder, then onward to filter/VCA.

### Musical role in melody
Wavefolding adds harmonic complexity before the filter. This is especially effective for:
- cutting leads
- acid-adjacent bass timbres
- expressive solo voices
- brighter melodic motifs that stay audible in a mix

The manual notes the folder is especially pronounced with **saw wave**.

### Best melodic use
- saw wave into folder
- moderate fold amount
- filter cutoff partially open
- envelope on filter
- slight glide

This produces a very playable, vocal, aggressive monosynth lead.

---

## 8. Sample + Hold for structured melodic variation

S+H doesn’t need to be fully random. It can create **rhythmic melodic motifs** when carefully constrained.

## A. Stepped pitch sequence
- **S+H out → 1V/OCT**
- LFO provides clocking
- adjust **LFO RATE**
- use **ATTENUATOR** to reduce range

Result:
- a repeating but quasi-random stepped melody

## B. Stepped filter melody accent
- **S+H out → CUTOFF**
- keyboard still controls pitch

Result:
- stable melody pitch with evolving timbral accents

## C. Parallel pitch + filter melody
- **S+H out → MULT**
- **MULT 1 → 1V/OCT**
- **MULT 2 → CUTOFF**

Result:
- pitch and brightness move together
- creates highly animated melodic lines with internal coherence

This is especially effective for generative music.

---

## 9. Glide as a melodic expression tool

The **GLIDE** control affects transitions between notes.

### Melodic uses
- no glide: precise sequenced lines
- short glide: legato funk bass or lead phrasing
- medium glide: classic monosynth solos
- long glide: experimental interval smears

Because glide also affects **KB CV out**, it can be part of larger patch behavior if KB CV is used elsewhere.

This makes Mavis good for:
- portamento leads
- acid-style slides
- expressive legato phrases
- animated CV interactions

---

## 10. Patch strategies for different melodic roles

## A. Bassline voice

**Goal:** tight, punchy low-end melody

Suggested setup:
- VCO: saw or pulse
- Filter: low-pass, medium cutoff
- Resonance: low to medium
- EG: fast attack, short decay, medium/low sustain, short release
- VCF EG: moderate positive amount
- Glide: very low or subtle
- Optional: wavefolder lightly engaged

Patch ideas:
- external sequencer → **1V/OCT**, **GATE**
- **VCO out → FOLD IN** for extra bite
- subtle **PWM** or filter LFO modulation

---

## B. Lead voice

**Goal:** expressive monophonic melody

Suggested setup:
- VCO: saw/pulse blend
- Pulse width adjusted for body
- Filter: medium cutoff, some resonance
- EG: fast attack, medium decay, medium sustain, medium release
- Glide: moderate
- LFO to pitch: subtle vibrato
- Filter EG: moderate

Patch ideas:
- **VCO out → FOLD IN**
- **KB CV → MULT**
- one copy to pitch path, another to LFO rate for note-dependent vibrato speed or dual oscillator tracking
- audio-rate LFO mixed with VCO for thicker tone

---

## C. Generative melody source

**Goal:** self-running melodic component

Suggested patch:
- **S+H out → ATTN in**
- **ATTN out → 1V/OCT**
- LFO as default S+H gate
- VCO as default sample source
- EG with medium attack/decay
- VCA in EG mode
- S+H optionally also to filter via MULT

Refinements:
- slow LFO for sparse melodic notes
- faster LFO for arpeggio-like stepping
- attenuate pitch range for tonal consistency
- use external quantizer downstream if desired in a bigger Eurorack system

---

## D. Drone-plus-melody patch

**Goal:** melody against a fixed internal harmonic reference

Patch:
- LFO in audio range
- **LFO out → ONE (-5)**
- **VCO out → TWO**
- **ONE+TWO → FOLD IN**
- no KB CV to LFO RATE

Result:
- VCO follows played notes
- LFO stays fixed
- creates interval beating and drone tension

This is excellent for:
- modal melodies
- experimental techno hooks
- cinematic motifs

---

## E. Sequence with animated timbre

**Goal:** melody that evolves without changing note content

Patch:
- sequencer pitch → **1V/OCT**
- sequencer gate → **GATE**
- **S+H out → CUTOFF** or LFO → CUTOFF
- use EG on VCF also
- pulse wave with PWM

Result:
- steady melodic pattern
- constantly shifting articulation and brightness
- useful for minimalist and modular-style repetition

---

## 11. Best module combinations for melody inside Mavis

Here are the most important “musician’s combinations” from the manual.

## 1. Keyboard + VCO + EG + VCA
The basic playable melody path.

Best for:
- immediate lead/bass playing
- testing melodic ideas
- expressive manual performance

---

## 2. External 1V/OCT + GATE + VCF EG
Turns Mavis into a full Eurorack melodic voice.

Best for:
- sequenced basslines
- modular lead voice
- DAW/CV controlled melodies

---

## 3. S+H + Attenuator + 1V/OCT
Turns Mavis into a generative pitch machine.

Best for:
- random melodies
- evolving motifs
- self-playing patches

---

## 4. LFO audio rate + Mixer + VCO + FOLD IN
Makes a richer two-oscillator melodic synth.

Best for:
- thick leads
- harmonically rich riffs
- aggressive melodic material

---

## 5. VCO + Wavefolder + Filter
Adds harmonic complexity before subtractive shaping.

Best for:
- cutting melodies
- expressive solo tones
- modern, brash analog voices

---

## 6. Mult + one CV source to multiple destinations
Couples pitch with timbre/modulation.

Best for:
- melodies that “open up” as they rise
- pitch-dependent modulation behavior
- more organic phrasing

---

## 12. Practical melodic patch recipes

## Patch 1: Classic analog lead
- Use default signal path
- VCO wave between saw and pulse
- Filter cutoff around mid position
- Resonance low-medium
- EG: fast attack, medium decay, medium sustain, medium release
- VCF MOD MIX toward EG
- VCF MOD AMT positive
- slight glide
- slight LFO vibrato via VCO mod

Result: singing Moog-style mono lead

---

## Patch 2: Acid-ish melodic bass
- saw wave
- **VCO out → FOLD IN**
- cutoff fairly low
- resonance medium-high
- EG with fast attack, short decay, low sustain, short release
- VCF EG amount fairly high
- glide short

Result: sharp, articulate melodic bassline

---

## Patch 3: Generative stepped melody
- **S+H out → ATTN (+5)**
- **ATTN out → 1V/OCT**
- leave default S+H source/gate
- LFO rate sets melody speed
- VCO wave to saw for broader pitch values
- EG short-medium for percussive notes if externally gated, or use drone methods with filter animation

Result: autonomous modular melody source

---

## Patch 4: Dual oscillator solo
- LFO rate to audio range
- **LFO out → ONE (-5)**
- **VCO out → TWO**
- **ONE+TWO out → FOLD IN**
- **KB CV → LFO RATE**
- tune LFO by rate knob
- shape with filter and EG

Result: fuller, more powerful melodic voice

---

## Patch 5: Pitch + brightness linked melody
- **KB CV → MULT**
- **MULT 1 → 1V/OCT** or let internal keyboard handle pitch
- **MULT 2 → CUTOFF**

Attenuate if needed via utility rerouting.

Result: higher notes naturally get brighter, mimicking acoustic behavior

---

## 13. What makes Mavis especially good for melody

From a Eurorack musician’s perspective, Mavis is especially effective for melodic work because it combines:

- a **true analog voice**
- a **playable keyboard**
- **1V/oct and gate I/O**
- internal utility modules usually missing from small synth voices
- **wavefolder** for additional harmonic expression
- **audio-rate LFO** that doubles as second oscillator
- **sample & hold** for generative pitch material

So it can function as:

- a self-contained melodic monosynth
- a Eurorack lead/bass voice
- a generative melody module
- a modulation-rich timbre engine for repeating note patterns

---

## 14. Final musician’s take

If your goal is to create **melodic components**, think of Mavis in three layers:

### 1. Pitch layer
Use:
- keyboard
- external 1V/oct
- S+H
- attenuated CV
- mixed CV sources

### 2. Articulation layer
Use:
- gate
- EG
- VCA
- glide

### 3. Character layer
Use:
- waveform selection
- pulse width / PWM
- filter envelope
- resonance
- wavefolder
- audio-rate LFO mixing

The most musical patches usually come from combining all three layers:
- **stable pitch source**
- **dynamic envelope**
- **moving timbre**

That’s where Mavis becomes much more than a starter synth—it becomes a very capable **melodic modular voice**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)