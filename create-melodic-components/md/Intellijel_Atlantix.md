# Intellijel — Atlantix

- [Manual PDF](../../manuals/atlantix_manual_2024.09.12.pdf)

---

[Atlantix Manual PDF](#)

# Intellijel Atlantix + ATLX Expander: using them to create melodic parts

The **Intellijel Atlantix** is essentially a complete **dual-oscillator analog voice** in Eurorack:  
- **VCO A** = main melodic oscillator  
- **VCO B** = second oscillator or modulation source  
- **Mixer** = blends waves and auxiliary signals  
- **VCF** = tone shaping / articulation  
- **Envelope + VCA** = note dynamics  
- **Mods / S&H** = motion, variation, pseudo-sequencing  
- **ATLX expander** = extra waveform/filter outs + ring mod access

For melodic music, this means Atlantix can function as:

1. a **full monosynth voice**  
2. a **two-layer melodic source**  
3. a **bass / lead / arp voice**  
4. a **self-patching melodic generator**  
5. a **hub for external sequencers, envelopes, and utilities**

---

## What the module gives you for melody

## 1. A complete playable voice
Atlantix already contains the full chain you need:

**Pitch CV → Oscillator(s) → Mixer → Filter → VCA → Output**

Specifically:
- Send **1V/oct** pitch to **PITCH A IN [1.A]**
- Send gates to **GATE [5.A]**
- Take audio from **OUT [5.G]**

With no extra patching, the internal normals already connect:
- Mixer → VCF
- VCF → VCA
- Envelope → VCA
- Envelope → filter modulation
- Mod sources → oscillator/filter FM destinations

So for melody, this behaves much like a semi-normalled analog synth voice.

---

## 2. Strong oscillator relationships for harmonic melody
### VCO A
VCO A is the main melodic oscillator:
- octave + fine tune
- saw + pulse in the mixer
- PWM
- sync
- exponential FM
- thru-zero linear FM

This makes it great for:
- classic lead lines
- bass lines
- sync leads
- expressive FM timbres
- evolving melodic tones

### VCO B
VCO B can be:
- another audio oscillator
- an LFO
- a pitch-following harmonic partner
- a modulation source

The key melodic feature is the **PITCH SOURCE [2.3]** switch:
- **A+B**: VCO B can follow PITCH A, optionally offset by PITCH B input
- **B**: VCO B is independent

This is extremely useful for melody because you can make VCO B:
- track the main melody in unison
- track it at an interval
- run independently as a second melodic line
- act as a synced/fm modulator tied to the same keyboard/sequencer pitch

---

# Best melodic use cases

## 1. Classic mono lead voice
This is the most straightforward patch.

### Patch
- Sequencer/keyboard pitch → **PITCH A [1.A]**
- Gate → **GATE [5.A]**
- Audio out → **OUT [5.G]**

### Settings
- Bring up **SAW [3.2]** or **PULSE [3.1]**
- Set filter to **LP**
- Use envelope on filter with **ENV [4.3]**
- Set VCA mode to **ADSR [5.6]**

### Why it works
Atlantix has the classic subtractive architecture for melodic leads:
- harmonically rich oscillator
- resonant multimode filter
- ADSR contour
- optional drive at the VCA

### Variations
- Add **SUB [3.3]** for a thicker lead
- Add **NOISE [3.4]** very subtly for breath/grit
- Use **SYNC A SOURCE = VCO B saw** and **SYNC TYPE = HARD** for classic sync leads
- Use **DRIVE [5.7]** in SYM or ASYM for more aggressive solos

---

## 2. Basslines
Atlantix looks especially strong for bass.

### Why
- VCO A has **sub oscillator** options:
  - -1 octave
  - -2 octaves
  - logical OR pulse-style sub
- Filter can be lowpass and resonant
- VCA drive gives weight
- Envelope can be very snappy in **FAST** mode

### Patch
Same as mono lead:
- Pitch → **PITCH A**
- Gate → **GATE**
- Audio → **OUT**

### Suggested settings
- Mixer:
  - **SAW** medium-high
  - **SUB** medium-high
  - maybe a little **PULSE**
- Filter:
  - **LP**
  - moderate resonance
  - medium envelope amount
- Envelope:
  - fast attack
  - short/medium decay
  - low sustain
  - short release
- VCA:
  - **ADSR**
  - maybe **SYM** drive

### Musical result
You get:
- Moog-ish rounded bass
- acid-like resonant bass
- punchy techno bass
- sync bass with bite

---

## 3. Dual-oscillator interval leads
Since VCO B can follow pitch from VCO A, you can build richer melodic voices.

### Method A: use VCO B as audio via AUX inputs
The mixer has two normalized AUX paths:
- **AUX 1** can default to **VCO A triangle** or **VCO B square**
- **AUX 2** can default to **VCO A sine** or **VCO B saw**

So you can bring VCO B into the main signal path without needing the expander.

### Patch idea
- Pitch CV → **PITCH A**
- Leave **PITCH B** unpatched
- Set **VCO B PITCH SOURCE [2.3] = A+B**
- Tune **PITCH B [2.2]** to an interval:
  - slight detune = thick unison
  - +7 semitones ≈ fifth
  - +12 semitones = octave
- Set **AUX 1 Source [3.10]** to VCO B square and raise **AUX 1 [3.5]**
- Or set **AUX 2 Source [3.11]** to VCO B saw and raise **AUX 2 [3.6]**

### Result
One incoming melodic pitch controls both oscillators, but VCO B can be offset to create:
- octave leads
- fifth-based heroic leads
- detuned unison leads
- tuned drone-plus-lead combinations

This is one of Atlantix’s strongest melodic features.

---

## 4. Cross-modulated melodic timbres
For more advanced melodic parts, use VCO B to modulate VCO A.

### Internal normal advantage
If nothing is plugged into **FM 1 IN [1.D]**, VCO A’s FM 1 source defaults to **MOD X**.  
MOD X can select VCO B waveforms.

So you can:
- choose VCO B sine/triangle/saw/square as MOD X source
- send that to VCO A FM1 internally
- choose **TZFM** or **EXP**
- control modulation depth with **INDEX [1.4]**
- control dynamic FM amount with **IM [1.3]**

### Melodic applications
#### Linear FM melodies
Use **TZFM**
- good pitch stability
- better for tuned melodic playing
- rich but still musical harmonic movement

#### Exponential FM melodies
Use **EXP**
- wilder and more vintage
- pitch/timbre change together
- better for expressive, unstable lines

### Great musical setup
- VCO B follows VCO A pitch with **A+B**
- Tune VCO B to a simple ratio (unison, octave, fifth-ish)
- Use **MOD X = VCO B sine**
- Raise **INDEX**
- Modulate index with the envelope via the internal IM normal

This creates notes that start bright/complex and settle into a purer pitch—excellent for:
- plucked FM tones
- metallic melodic motifs
- expressive synth leads

---

## 5. Oscillator sync leads
VCO A supports both **hard** and **soft** sync.

### Default normal
If nothing is patched to **SYNC A [1.B]**, VCO A can sync either to:
- **VCO B saw**
- or **GATE**
depending on **SYNC A SOURCE [1.13]**

### Melodic uses
#### VCO B as sync master
- Gives classic ripping sync lead sounds
- Sequence pitch into VCO A
- Let VCO B follow or offset pitch
- Sweep VCO A tuning for the signature sync harmonics

#### Gate sync
- Each note can restart the oscillator phase
- Great for percussive/plucky consistency
- Useful for tight bass or plucked melodies

### Hard sync
Sharper, more aggressive, classic lead tone.

### Soft sync
Smoother, less abrasive, still harmonically rich.

For melodic content, sync is especially useful when you want:
- one-note leads with lots of movement
- repeated sequences that need timbral animation
- expressive filterless or lightly filtered solo lines

---

## 6. PWM melodies
Atlantix gives VCO A pulse width and pulse width modulation.

### Internal PWM normals
If nothing is plugged into **PWM IN [1.F]**, the source can be:
- **VCO B sine**
- **Envelope**

### Melodic applications
#### Envelope PWM
- each note opens/closes pulse width
- great for plucks, brass-like leads, animated bass

#### VCO B PWM
- slow VCO B in LFO mode for moving pulse texture
- audio-rate VCO B for more aggressive harmonic animation

Because pulse width changes harmonic content dramatically, this is one of the easiest ways to make a repeating melody feel alive without changing notes.

---

# Using the filter melodically

Atlantix’s filter is not just a tone control—it can become part of the melodic identity.

## 1. Pitch-tracking filter
If nothing is patched into **FM 2 [4.B]**, the filter defaults to tracking **VCO A pitch**.

This is very useful for melody because:
- higher notes can stay bright
- lower notes remain warm
- the voice feels more “played” across the keyboard

Use this for:
- bass patches
- expressive mono leads
- patches with significant resonance

## 2. Envelope-shaped articulation
The envelope is normalled to the filter and scaled by **ENV [4.3]**.

This gives classic melodic articulations:
- pluck
- sweep
- punch
- vowel-like attacks

## 3. Multimode filtering for different melodic roles
- **LP**: best for basses and classic leads
- **BP**: focused, nasal, sequence-friendly
- **HP**: thinner melodic lines, useful in dense mixes
- **PHZ**: very interesting animated melodic textures

### Phaser mode for melody
The **PHZ** mode can make repeating melodic parts more animated and spatial without needing a separate phaser module. Good for:
- arps
- sequences
- hovering melodic ostinatos

---

# Using the envelope and VCA for phrasing

Atlantix’s ADSR and VCA determine how “played” your melody feels.

## Envelope ranges
Three rates:
- **FAST**
- **MED**
- **SLOW**

This makes Atlantix suitable for:
- short staccato basslines
- medium synth leads
- long evolving drones or ambient melodies

## VCA modes
### ADSR mode
Best for traditional melodic phrasing.

### GATE mode
Makes the voice behave like an organ:
- immediate on
- immediate off

Great for:
- chiptune-ish lines
- mechanical sequences
- external envelope control

## Drive
The VCA has:
- **SYM**
- **X**
- **ASYM**

For melody:
- **SYM** = tighter, more centered saturation
- **ASYM** = dirtier, more characterful harmonics

This can help a lead or bass cut through without extra modules.

---

# How the MOD section helps melody

This section is where Atlantix becomes much more than a basic voice.

## MOD X and MOD Y
Two assignable modulation outputs with:
- 8 source choices each
- unipolar/bipolar switching
- polarity inversion

Defaults:
- **MOD X → VCO A FM1**
- **MOD Y → VCF FM1**

That means the module is already set up for dynamic self-patched melodic timbres.

## Useful melodic modulation sources
You can choose for MOD X/Y:
- VCO B sine/triangle/saw/square
- sample & hold
- noise
- VCF
- VCA or MIX depending on X/Y

### Musical use cases
#### VCO B as LFO
Set **VCO/LFO [2.4] = LFO**
Then MOD X or MOD Y can become:
- vibrato
- filter wobble
- slow timbral drift

#### Audio-rate modulation
Set VCO B to audio
Use MOD X/Y for:
- FM tones
- filter FM brightness
- harsh or glassy melodic timbres

#### Using VCF or MIX as modulation
This creates feedback-like self-referential motion.
Very useful for:
- unstable evolving melodic tones
- animated drones
- living, semi-chaotic sequence timbres

---

# Sample & Hold for melodic variation

Atlantix includes S&H/T&H and noise, which can create melodic motion even without a traditional sequencer.

## S&H basics
- **HOLD [6.A]** determines when sampling occurs
- **SAMP [6.B]** is the source being sampled
- **S&H OUT [6.C]** is the stepped result

If nothing is plugged in:
- HOLD can default to **VCO B square** or **Gate**
- SAMP defaults to **white noise**

## Melodic applications
### 1. Random note generator
Patch:
- **S&H OUT [6.C]** → **PITCH A [1.A]**

Then use:
- quantizer externally if you want tonal notes
- HOLD from gate for one new pitch per note
- HOLD from VCO B square for clocked random stepping

This creates random melodies.

### 2. Per-note timbre variation
Instead of pitch, patch S&H to:
- **VCF FM**
- **Q**
- **PWM**
- **IM**
- **FM 2**

This is often musically better than random pitch because the melody stays stable while each note gets a slightly different color.

### 3. Semi-random ornamentation
Use **Track & Hold** instead of Sample & Hold for more fluid, less rigid movement.

---

# How Atlantix and ATLX work together musically

The **ATLX expander** adds significant melodic flexibility because it exposes many internal signals as dedicated outputs.

## Extra oscillator waveform outputs
ATLX gives dedicated outputs for:
- VCO A sine / triangle / saw / pulse
- VCO B sine / triangle / saw / square
- sub out
- multiple filter outputs
- ring mod out

This matters for melody because you can use Atlantix as a **voice plus source bank**.

## 1. Parallel melodic layers
Use the main **OUT [5.G]** as one complete melodic voice, while also taking:
- **A SAW**
- **B SIN**
- **SUB**
- dedicated filter outs

These can go to:
- external VCAs
- extra filters
- effects
- wavefolders
- stereo processing

So one Atlantix sequence can become:
- dry bass in the center
- filtered sine octave layer
- effected saw lead in parallel
- sub reinforcement on another path

## 2. Multiple filter-output melodies
The expander gives:
- **LP**
- **HP**
- **BP**
- **PHZ**

This is excellent for building melodic texture:
- use **OUT** as your main voice
- send **BP out** to delay/reverb for a second melodic shadow
- send **HP out** to distortion for bright harmonics
- send **PHZ out** to stereo effects for width

A single melody line becomes a layered arrangement.

## 3. Ring modulation for tuned melodic overtones
The ring mod section has:
- **X in**
- **Y in**
- **RING out**

Defaults:
- X = Osc A sine
- Y = Osc B sine

If VCO B tracks VCO A at a fixed interval, the ring mod can produce very musical sidebands.

### Melodic use
- Tune VCO B to octave/fifth/other interval
- Use **RING out** as a second audio layer
- Mix it externally with the main voice

This can produce:
- bell-like melodic doubles
- metallic leads
- tuned shimmer on bass notes
- inharmonic but repeating melodic color

For melodic composition, the best approach is often not to use ring mod alone, but to blend it under the main voice.

---

# Practical melodic patch ideas

## Patch 1: Simple analog lead
**Connections**
- Pitch CV → PITCH A
- Gate → GATE
- OUT → mixer/audio interface

**Settings**
- SAW up
- LP filter
- ENV to filter moderate
- ADSR mode
- slight resonance

**Result**
Classic subtractive mono lead.

---

## Patch 2: Thick bass with sub
**Connections**
- Pitch CV → PITCH A
- Gate → GATE
- OUT → output

**Settings**
- SAW medium
- SUB high
- LP 4-pole
- fast envelope
- drive ON
- filter tracking active via FM2 normal

**Result**
Solid melodic bassline with good low-end focus.

---

## Patch 3: Dual-oscillator interval melody
**Connections**
- Pitch CV → PITCH A
- Gate → GATE

**Settings**
- VCO B pitch source = A+B
- Tune VCO B to fifth or octave
- AUX 1 source = B square or AUX 2 source = B saw
- bring up AUX level
- blend with VCO A waves

**Result**
One-note melody with harmonic interval layering.

---

## Patch 4: Sync lead
**Connections**
- Pitch CV → PITCH A
- Gate → GATE

**Settings**
- SYNC A source = VCO B saw
- SYNC TYPE = HARD
- VCO B tracks A+B
- Sweep VCO A pitch knob while playing
- use filter sparingly

**Result**
Classic tearing sync lead for melodic solos.

---

## Patch 5: Musical FM pluck
**Connections**
- Pitch CV → PITCH A
- Gate → GATE

**Settings**
- MOD X source = VCO B sine
- FM1 uses MOD X normal
- TZFM selected
- VCO B tracks A+B
- INDEX moderate
- IM raised so envelope affects FM index
- short envelope

**Result**
Bright attack with harmonically rich but playable melodic notes.

---

## Patch 6: Animated PWM melody
**Connections**
- Pitch CV → PITCH A
- Gate → GATE

**Settings**
- Pulse up in mixer
- PWM source = envelope or VCO B sine
- moderate PWM amount
- LP or BP filter
- medium ADSR

**Result**
Warm animated sequence or lead with organic motion.

---

## Patch 7: Melodic voice plus parallel shimmer using ATLX
**Connections**
- Pitch CV → PITCH A
- Gate → GATE
- Main OUT → main mix
- ATLX RING OUT → reverb/delay return or second VCA
- Optionally ATLX BP OUT → stereo effect path

**Settings**
- VCO B tuned to interval from VCO A
- Ring mod defaults to A sine and B sine

**Result**
Main melody stays grounded, while ring mod and filter outs create a second melodic halo.

---

# Best strategies for writing melodic music with Atlantix

## 1. Keep VCO A as the “pitch anchor”
For the clearest melodic result:
- send your main sequence to **PITCH A**
- let the rest of the module orbit around that pitch

This preserves musical coherence while allowing rich timbral movement.

## 2. Use VCO B for one of three jobs
VCO B is most effective when you commit it to a role:
- **harmonic partner**
- **LFO/modulator**
- **audio-rate FM/sync source**

Trying to do all three at once can get chaotic.

## 3. Use modulation for articulation, not just complexity
For melodic parts, the best modulation destinations are often:
- filter cutoff
- PWM
- FM index
- resonance in small amounts

These preserve note identity while adding expression.

## 4. Use S&H for timbre, not only pitch
Random pitch can be fun, but random timbral variation often sits better musically.
Try S&H to:
- filter cutoff
- Q
- pulse width
- FM depth

## 5. Use the expander for arrangement
ATLX is especially useful for taking one melodic part and splitting it into:
- core voice
- upper texture
- sub reinforcement
- effected duplicate

That is powerful for composition and mixing.

---

# Summary

The **Atlantix** is very well suited to melodic music because it combines:
- a playable main oscillator
- a secondary oscillator that can track, offset, sync, or modulate
- an internal mixer with useful waveform normals
- a flexible multimode filter
- ADSR/VCA articulation
- self-patching modulation tools
- random/held voltage generation
- optional expander outputs for layering

In practice, it excels at:
- **basslines**
- **mono leads**
- **sync solos**
- **FM plucks**
- **dual-oscillator interval melodies**
- **self-evolving sequences**
- **layered melodic textures with the ATLX expander**

If you want, I can also turn this into:
1. a **set of 10 specific melodic patches**,  
2. a **quick-start cheat sheet**, or  
3. a **signal-flow diagram showing how to patch Atlantix as a lead/bass voice**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)