# Bastl Instruments — Dark Matter

- [Manual PDF](../../manuals/manual-dark-matter.pdf)

---

[Manual PDF: manual-dark-matter.pdf](manual-dark-matter.pdf)

# Casper/Bastl Dark Matter — using it for melodic components

Based on the attached manual, this PDF is for **Casper Electronics / Bastl Instruments – Dark Matter: Feedback Observatory**.  
Dark Matter is not a conventional oscillator or filter voice by itself. It is a **feedback instrument / processor** built around:

- **Input/Drive**
- **Dynamics** envelope follower
- **Tone** section with **Bass** and **Treble** EQ/boost
- **Feedback (FBK)** loop with internal and external routing
- **X-Fade** crossfader between input and feedback
- CV control over drive, tone boosts, x-fade, and feedback amount

Its core strength for melody is that it can turn simple material—drums, tones, VCOs, external effects—into **pitched resonances, sub-octaves, screaming harmonics, unstable drones, and animated tuned feedback**.

---

## What the module does musically

Dark Matter creates melodic content in three main ways:

1. **It extracts pitch from feedback**
   - The manual explicitly mentions using the feedback loop to reach **resonant oscillation** and to tune the “pitch” of the loop.
   - The **FBK** control and **FBK fader** determine how close the system is to self-resonance.

2. **It reshapes incoming audio into pitched material**
   - The **Drive** section adds gain/soft clipping and optional **Hyper Drive**.
   - The **Tone** section boosts bass/treble into the feedback path, which emphasizes different frequency regions and can make a loop behave more like a tuned instrument.

3. **It animates melody/rhythm with control signals**
   - The **Dynamics** section is an envelope follower from the input signal.
   - That envelope is internally normalled to the **X-FADE CV**, so transients and dynamics can “play” the feedback balance.
   - CV inputs for **Drive**, **Bass Boost**, **Treble Boost**, **X-Fade**, and **FBK** let sequencers/LFOs shape pitch-like behavior over time.

---

# Key sections relevant to melody

## 1. Drive
The manual describes **Drive** as a VCA/preamp with soft clipping. This is important melodically because:

- more drive excites the feedback network harder
- it increases harmonics, helping a tone cut through
- with **Hyper Drive** on, the signal can push into hotter saturation and more aggressive pitched feedback

### Melodic use
- Use lower Drive for more stable, sine-ish/rounded resonances
- Use higher Drive for harmonically rich, lead-like shrieks
- Modulate **Drive CV** with a sequence or envelope for accent patterns

---

## 2. Dynamics
This is an **envelope follower** tracking the input signal and generating a CV.

The manual notes:
- output is approximately **0–5 V**
- it is internally normalled to **X-FADE CV**
- it has **pre/post drive** source selection
- **Decay** sets envelope speed from snappy to sluggish

### Melodic use
This is one of the most powerful musical features in the module.

You can use Dynamics to:
- make drum hits excite tuned feedback like a playable percussion synth
- make melodic inputs “duck/push” the feedback amount
- derive phrasing from a source and apply it to the feedback voice

If you patch a rhythmic or melodic signal into Dark Matter, Dynamics can convert articulation into a control shape, so feedback opens in time with the source.

---

## 3. Tone
The manual describes Tone as a **2-band EQ** feeding the feedback section.

Controls:
- **Bass fader / Bass boost / Bass boost CV**
- **Treble fader / Treble boost / Treble boost CV**

### Melodic use
Tone is effectively part of the “tuning” and “voicing” of the feedback instrument.

- **Bass emphasis** encourages lower resonances and sub-octave behavior
- **Treble emphasis** encourages harmonics, edge, and upper partials
- the balance between Bass and Treble can make the feedback read as:
  - bassline
  - lead
  - metallic overtone texture
  - unstable drone

For melody, think of Tone as both:
- a timbre shaper
- a coarse pitch-behavior shaper

---

## 4. FBK
This is the heart of the module.

The manual states that the FBK section:
- controls the intensity of the feedback loop
- can be pushed into **resonant oscillation**
- has **FBK fader**, **FBK CV**, and an **ENV** indicator
- includes **FBK OUT** and **FBK IN** for external insertion
- has **CV control routing** between input and output side of the external loop
- has **Out Polarity** invert switch for external loops

### Melodic use
This is the section that makes Dark Matter capable of producing pitched material even from simple sources.

- Turn up **FBK** until the system starts “locking” onto a pitch region
- Adjust **Bass/Treble** and **X-Fade** to find a stable note-like resonance
- Feed external processors into **FBK OUT → effect/module → FBK IN** to create more controllable tuned loops

The manual specifically mentions:
- creating **sub octave tones and harmonic fills**
- using an external VCO in relation to the feedback path
- using the feedback loop almost like an instrument to be tuned

---

## 5. X-Fade
This crossfades between the **dry/input path** and the **feedback path**.

The manual notes:
- the **Dynamics** output is internally patched to **X-FADE CV**
- there is an **Input/Feedback switch**
- it can crossfade audio and interact deeply with the envelope follower

### Melodic use
X-Fade lets you decide whether the listener hears:
- the original played note/drum/source
- the resonant feedback result
- a hybrid of both

This is crucial for melody because it lets you create:
- **attack from the source, sustain from the feedback**
- ghost harmonies behind a sequence
- pseudo-duophonic textures, where dry signal carries pitch center and feedback adds tuned overtones

---

# Best melodic applications from the manual

The manual includes quick-starts and patches for:

- **Drums**
- **Tones**
- **External feedback**
- **Loops**

These strongly suggest the most useful melodic workflows.

---

# 1. Melodic percussion from drums

The manual’s **Drums** quick start says to:

- feed **Drive** with the drum signal
- set **X-Fade** to medium and raise **FBK**
- adjust **Bass** and **Treble** to shape feedback distortion and tone
- use **Dynamics CV → FBK CV** type interaction to apply the drum envelope to feedback
- optionally enable **Hyper Drive**
- bonus: use gates/LFOs synced to the drum sequencer on CV inputs

## What this gives you
A drum hit becomes an exciter for a tuned resonant body. That means:

- kick → subby pitched boom
- snare/rim → tuned bark
- hi-hat/noise burst → metallic note cloud

## How to turn it melodic
Use a sequenced or tuned source elsewhere in the system alongside the drum excitation:

### Patch concept
- Patch a kick, tom, or click into **Input**
- Raise **FBK** until the loop begins to sing
- Shape the resonant region with **Bass/Treble**
- Sequence **FBK CV** or **X-Fade CV** for note-like stepping
- Mult the same clock/gate pattern to modulation sources for repeatable phrasing

This creates percussive melodies, tuned tom lines, and rhythmic ostinatos.

---

# 2. Tones → sub-octaves and harmonics

The manual’s **Tones** quick start says to:

- connect an audio waveform to **Input**
- keep **Drive** low and **Hyper Drive** off
- adjust **Bass** and **Treble** to shape waveform
- adjust **Drive, Tone, and FBK** to bring in **sub octave tones and harmonic fills**
- connect **LFOs to CV inputs** to animate wave shape and tone

Bonus suggestions:
- patch external waveform into **FBK CV**
- keep **FBK CV** around middle
- with a bit of fine tuning, sync the feedback to an **external VCO**
- use **FBK OUT** as a special audio out

## Why this matters
This is the clearest melodic application in the manual. Dark Matter can act like a **harmonic companion** to a pitched oscillator.

## Musical result
If you feed it a plain VCO waveform:
- it can add subharmonics under the note
- generate unstable upper harmonics
- create a pseudo second voice around the original pitch
- produce animated distortion that tracks or quasi-tracks the source

## Best use together with other modules
Dark Matter pairs especially well with:
- a basic analog VCO
- a sequencer sending 1V/oct to that VCO
- a VCA/envelope before or after it
- delay/reverb after Dark Matter

In that role, the VCO supplies exact pitch, while Dark Matter supplies **musical complexity**.

---

# 3. External feedback loop as a melodic resonator

The **External Feedback** section of the manual is especially important.

It explains:
- use **FBK OUT** and **FBK IN** to insert modules/effects into the loop
- external modules may invert polarity; use **Out Polarity**
- **CV Control** chooses whether the FBK VCA responds before or after the external processor
- examples shown include **echo, reverb, filter, phaser, distortion**

## Why this is huge for melody
Once you place modules in the loop, Dark Matter becomes a resonant ecosystem. You can bias the loop toward stable pitches or harmonically useful resonances.

### Good external modules for melody
- **Filters**: narrow resonance and emphasize pitch centers
- **Delays**: Karplus-ish pitched plucks, repeats that lock into note-like resonances
- **Phasers**: moving comb-like tones
- **Distortion/waveshapers**: harmonic lead textures
- **BBD/echo**: ghost melodies and self-playing lines

### A particularly useful setup
- **FBK OUT → filter → delay → FBK IN**
- Input a short pluck/click/noise burst
- Raise FBK until the loop becomes semi-self-sustaining
- Tune the filter cutoff and resonance for pitch center
- Use X-Fade to blend attack from input with sustained pitched loop

That produces very musical plucked or droning melodic material.

---

# 4. Loops and drone melody

The manual’s **Loops** page shows several routing examples involving:
- LFO
- audio
- VCO
- drums
- echo

This implies Dark Matter excels as a **hub** where modulation, external sound, and feedback all cross-influence.

## Melodic use
For drones and long-form melody:
- feed a VCO or loop into Input
- use an LFO on **X-Fade CV** or **FBK CV**
- optionally put echo in the FBK loop
- tune Bass/Treble/FBK for a pitch cluster
- then slowly modulate around that “note”

This yields:
- evolving drone melodies
- overtone shifts
- unstable chord-like beating
- semi-autonomous melodic phrases

---

# How to use Dark Matter with other eurorack modules for melody

Since you asked how these modules can be used together, here’s the practical answer in eurorack terms:  
Dark Matter works best as a **melodic enhancer / resonant voice shaper** alongside more conventional melodic modules.

---

## A. With a VCO + sequencer
### Goal
Turn a plain mono sequence into a richer melodic voice.

### Patch
- Sequencer 1V/oct → VCO
- VCO audio → Dark Matter **Input**
- Set **Drive** low to medium
- Set **X-Fade** around center
- Slowly raise **FBK**
- Use **Bass** for body, **Treble** for overtone detail
- Add slow modulation to **FBK CV** or **X-Fade CV**

### Result
- fundamental pitch stays readable
- Dark Matter adds subharmonics, extra harmonics, and resonant sustain
- sequence feels more alive and less static

Best for:
- acid-like lines
- industrial leads
- unstable basslines
- psychedelic monosynth phrases

---

## B. With a drum voice + sequencer
### Goal
Create tuned percussion and melodic hits.

### Patch
- Triggered drum/click/noise source → **Input**
- Dynamics source set to track that input
- Dynamics internally affects X-Fade, or patch Dynamics output elsewhere
- Raise **FBK** until each hit excites a pitched burst
- Sequence **FBK CV** or **Bass Boost CV**
- Optionally send a synced LFO to **Treble Boost CV**

### Result
- percussive notes instead of plain drum hits
- tom-like lines
- electro/IDM metallic melodies
- feedback “singing” per trigger

---

## C. With an external filter in the loop
### Goal
Make the feedback act more like a tuned voice.

### Patch
- **FBK OUT → filter input**
- Filter output → **FBK IN**
- Audio source → Dark Matter Input
- Adjust filter cutoff/resonance while increasing FBK
- Use **Out Polarity** if the loop cancels or dies
- Switch **CV Control** to find the more stable/musical feedback behavior

### Result
- stronger pitch center
- easier to find singable notes
- more controllable melodic resonance

This is one of the best ways to use Dark Matter musically.

---

## D. With delay/reverb in the loop
### Goal
Create ghost melodies and ambient tonal feedback.

### Patch
- **FBK OUT → delay or reverb → FBK IN**
- Feed short notes, plucks, or vocal-like tones into Input
- Use X-Fade to bring in feedback tail
- Modulate FBK slowly

### Result
- shimmering note trails
- decaying harmonized repeats
- self-generating ambient melody fragments

---

## E. With LFOs and envelopes
### Goal
Animate static notes into musical phrases.

### Patch ideas
- Envelope → **Drive CV** for accents
- LFO → **Bass Boost CV** for vowel-like low movement
- Another LFO → **Treble Boost CV** for shimmer
- Clocked stepped voltage → **FBK CV** for phrase changes
- Slow triangle → **X-Fade CV** for dry/wet melodic breathing

### Result
Dark Matter becomes less an effect and more a **performance voice**.

---

# Techniques for actual melodic writing

## 1. Treat the source as pitch, Dark Matter as articulation
Use a properly tuned oscillator or synth voice as the note source.  
Let Dark Matter provide:
- overtone cloud
- grit
- pseudo-resonance
- feedback sustain

This is the easiest way to keep melody intelligible.

---

## 2. Use feedback as a second voice
Blend dry and feedback with **X-Fade** so the original note is still there.  
Now the feedback behaves like:
- a shadow melody
- octave/sub layer
- unstable harmony

This works very well for bass and lead lines.

---

## 3. Excite it with short transients
Short clicks, pings, hats, rims, or noise bursts often produce the most playable resonances.  
That gives you:
- plucks
- tuned hits
- pseudo-Karplus behavior
- acoustic-like attacks

---

## 4. Sequence the CV, not just the note
Dark Matter is highly responsive to modulation.  
Instead of only sequencing pitch elsewhere, also sequence:
- **FBK CV**
- **X-Fade CV**
- **Bass/Treble boost CV**
- **Drive CV**

This creates melodic variation even if the note itself is static.

---

## 5. Use external loop modules to “tune” the behavior
The external feedback loop is where Dark Matter gets much more compositionally useful.

A filter, EQ, phaser, delay, or resonator in the loop can turn chaotic feedback into:
- a stable bass growl
- tuned comb tones
- repeating melodic figures
- spectral drones

---

# Practical patch recipes

## Patch 1: Harmonic lead enhancer
**Use when:** you already have a lead sequence

- VCO saw → Dark Matter Input
- Keep Drive moderate
- Hyper Drive off initially
- X-Fade at 40–60%
- FBK just below self-oscillation
- Treble slightly boosted
- Slow LFO to FBK CV

**Result:** animated lead with harmonic bloom and occasional resonant flare

---

## Patch 2: Sub bass companion
**Use when:** you want a bassline to feel larger

- Square or sine-ish VCO → Input
- Bass boosted, Treble reduced
- FBK raised until sub-octave behavior appears
- X-Fade toward feedback
- Small envelope to Drive CV for punch

**Result:** bassline with dirty sub undertow and controlled feedback weight

---

## Patch 3: Tuned drum melody
**Use when:** you want melodic percussion

- Short drum/click → Input
- Dynamics source pre or post drive, depending punch desired
- X-Fade medium
- FBK raised until each hit rings
- Sequence FBK CV with stepped modulation
- Optional filter in external FBK loop

**Result:** tom-like or metallic melodic pattern from percussion

---

## Patch 4: External resonant loop voice
**Use when:** you want Dark Matter to become a semi-autonomous instrument

- FBK OUT → resonant filter → delay → FBK IN
- VCO or noise burst → Input
- Raise FBK
- Tune filter cutoff
- Use Out Polarity switch if needed
- Use CV Control switch to decide whether feedback VCA behaves best before or after the inserted processor

**Result:** plucked/drone hybrid voice with tunable resonance and evolving melody fragments

---

## Patch 5: Ambient melody cloud
**Use when:** you want cinematic textures

- Sparse VCO or sample loop → Input
- FBK OUT → reverb or delay → FBK IN
- X-Fade mostly toward feedback
- Slow LFO to X-Fade CV
- Another slow CV to Treble Boost
- Modest FBK, not maximum

**Result:** blurred melodic halos and floating overtone movement

---

# Things to watch out for

The manual repeatedly implies this is a **wild feedback device**, so musically:

- small knob changes can matter a lot
- external modules in the feedback loop may invert polarity or radically change gain
- feedback can go from silent to explosive quickly
- use speakers/ears carefully and start levels low

For melody specifically:
- if you want **clear notes**, keep some dry signal in the mix
- if you want **chaotic but musical**, push FBK and shape with Tone
- if the loop disappears, try **Out Polarity**
- if it squeals too much, lower FBK or reduce Treble/Drive

---

# Bottom line

**Dark Matter is best used for melody as a feedback-based harmonic instrument layered around another sound source.**  
It excels at:

- adding **sub-octaves**
- generating **harmonic fills**
- creating **pitched resonant feedback**
- turning **drums into tuned hits**
- making **oscillators into unstable, expressive leads**
- building **external feedback loops** that function like semi-tuned voices

If you pair it with:
- a **VCO + sequencer**
- a **drum trigger/audio source**
- a **filter/delay/reverb in the FBK loop**
- some **LFOs/envelopes for CV**

then Dark Matter becomes a very strong tool for **melodic basses, leads, tuned percussion, drones, and evolving harmonic textures**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)