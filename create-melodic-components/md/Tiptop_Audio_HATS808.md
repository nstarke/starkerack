# Tiptop Audio — HATS808

- [Manual PDF](../../manuals/Tiptop_Audio_HATS808_ns.pdf)

---

[Manual PDF](https://www.tiptopaudio.com/808-2)

# Tiptop Audio HATS808 — melodic use analysis

Although the **HATS808** is fundamentally a drum/hi-hat voice, the manual reveals several ways it can be pushed into **pitched, quasi-pitched, and melodic territory** inside a Eurorack patch.

## What the module gives you

From the manual, the key features relevant to melodic use are:

- **Open Hat (OH) and Closed Hat (CH)** voices with separate outputs
- **Accent inputs** for dynamic articulation
- **Open Hat decay control**
- **Q / VC-Q** control over the main internal band-pass filter resonance
- **Band-Pass OUT** tapping the raw filtered source
- A **choke interaction** between CH and OH
- Very **hot output levels**, useful for driving other modules

These are important because melody in modular does not always mean “1V/oct oscillator into VCF/VCA.” It can also mean:
- tuned percussive lines,
- resonant pings,
- accent-shaped motifs,
- filter self-oscillation,
- and extracting raw spectral material for further pitch processing.

---

## The most important melodic takeaway: the Q circuit

The manual’s biggest clue is the **Q / VC-Q** section:

- At minimum Q, the module is closest to the original 808 sound.
- Increasing Q makes the hats more **metallic** and **retuned**.
- At high settings, the filter saturates into a crushed sound.
- At maximum, the filter can **become an oscillator and generate a constant tone**.
- **VC-Q accepts 0–5V CV**, and the Q knob offsets that CV.

This means the HATS808 is not just a cymbal voice — it can behave like a **resonant sound source** whose timbre and apparent pitch are voltage-variable.

### Melodic implications
You can use **VC-Q** with:
- sequencer CV
- envelopes
- stepped random voltages
- audio-rate modulation

to create:
- repeating tuned metallic motifs
- pseudo-melodic percussion
- shifting harmonic textures
- droning tones when pushed into self-oscillation

It is unlikely to behave as a precise **1V/oct oscillator**, so think:
- **expressive tuned percussion**
- **atonal or scale-constrained metallic melody**
- **industrial lines**
- **FM-like animated tones**

rather than traditional keyboard tracking.

---

## Best melodic strategies

## 1) Use self-oscillation as a tone source

When Q is maxed, the filter may oscillate continuously. That gives you a pitched tone source.

### Patch idea
- Turn **Q** high until oscillation begins.
- Monitor **Band-Pass OUT**.
- Send a stepped CV sequence to **VC-Q**.
- Use an external VCA and envelope to shape notes.
- Optionally trigger OH or CH alongside it for transient attack.

### Result
A **metallic sine-ish / resonant tone** with unstable analog character.  
This can become:
- a lead line,
- drone bass,
- background harmonic layer,
- or a noisy bell sequence.

### Best use
- experimental melody
- dark techno hooks
- industrial arps
- tuned drones

---

## 2) Sequence VC-Q for quasi-pitched percussion

Because increasing Q alters the tuning/metallicity of the hat sound, you can use CV to create a sequence that reads as melodic even though it is still a drum.

### Patch idea
- Trigger **OH GATE IN** from a clocked rhythm.
- Patch a sequencer row or sample & hold into **VC-Q**.
- Keep Q in the mid-to-high range.
- Use **DECAY** to lengthen the OH so pitch character is more audible.
- Use **ACCENT IN** to emphasize selected notes.

### Result
The open hat becomes a **pitched metallic percussion voice**.  
With the right sequence, it can function like:
- tuned cymbal melody,
- bell line,
- top-line hook,
- percussive ostinato.

### Why it works
Longer decay gives the ear more time to perceive the resonant center of the sound. Accent gives contour, which helps the pattern feel melodic rather than purely percussive.

---

## 3) Use the Band-Pass OUT as a raw oscillator bank texture

The manual explains that the HATS808 sound source begins as a mix of **six analog square oscillators**, then goes into the main band-pass filter. The **Band-Pass OUT** gives access to this filtered harmonic material.

This is especially useful for melodic patching because it separates the timbral core from the normal hat envelope behavior.

### Patch idea
- Take **Band-Pass OUT** into:
  - an external VCA,
  - another band-pass filter,
  - a low-pass gate,
  - wavefolder,
  - resonator,
  - pitch shifter,
  - or delay.
- Shape amplitude with your own envelopes.
- Modulate **VC-Q** slowly or with sequences.

### Result
You get a **metallic harmonic source** that can be turned into:
- synthetic bells
- tuned noise leads
- chord-like drones through resonators
- melodic textures after external filtering

### Why this is powerful
The Band-Pass OUT is effectively the module’s **raw spectral material**, which means you can build your own melodic voice around it using standard modular tools.

---

## 4) Create melodic articulation with accents

The manual makes clear that **accent** is not just volume; in this analog circuit it also changes **attack character**. That makes accent highly useful for phrasing melodic lines.

### Patch idea
- Send one trigger pattern to **GATE IN**.
- Send a sparser trigger pattern to **ACCENT IN**.
- Sequence **VC-Q** in tandem.
- Use accent on key notes of the phrase.

### Result
Even if pitch is only approximate, the pattern reads as musical because:
- louder notes feel important,
- stronger attack marks phrase boundaries,
- repetition plus selective emphasis creates motif.

### Good musical role
- melodic percussion
- syncopated hooks
- call-and-response top lines

---

## 5) Use choke as note-length control

The **choke** function is extremely musical. The CH envelope can cut off the OH, effectively shortening the OH note.

That means you can think of:
- **OH = sustained note**
- **CH = note terminator / articulator**

### Patch idea
- Send OH triggers on the melodic phrase.
- Send CH triggers where you want shorter note lengths.
- Modulate OH decay for variation.
- Sequence VC-Q so each OH hit has a different “pitch color.”

### Result
The choke acts like a primitive **gate length editor** for a percussive melodic voice.

### Musical uses
- staccato vs sustained pattern shaping
- syncopated phrasing
- dynamic hi-hat melodies
- pseudo-legato interruption effects

If desired, the manual says the choke can be disabled via an internal PCB header, but for melodic patching it is often more interesting left on.

---

## 6) Drive other modules with its hot outputs

The manual emphasizes that the outputs can be **very hot** and useful for overdriving downstream modules.

This matters melodically because a hot, bright source into external processing can become much richer.

### Patch idea
Send **OH OUT**, **CH OUT**, or **Band-Pass OUT** into:
- resonant filters
- LPGs
- wavefolders
- distortion
- resonators
- frequency shifters
- granular samplers
- delays with feedback
- phasers/flangers

### Result
The HATS808 becomes an excitation source for:
- Karplus-like plucks
- metallic basses
- resonator melodies
- tuned feedback systems

A very effective trick is to feed the Band-Pass OUT into a resonator tuned to a scale, then sequence accents and VC-Q.

---

## Concrete melodic patch recipes

## Patch 1: Metallic lead voice
**Goal:** turn the HATS808 into a playable lead-ish voice.

- Monitor **Band-Pass OUT**
- Turn **Q** high, near oscillation
- Patch stepped CV from sequencer to **VC-Q**
- Send Band-Pass OUT to external **VCA**
- Trigger external envelope from same rhythm source
- Use VCA output to mixer/effects

**Enhancements**
- Add slow modulation to Q offset
- Use CH accents to mark phrase endings
- Add delay/reverb for pitch illusion

---

## Patch 2: Tuned hat ostinato
**Goal:** melodic top-line from hat triggers.

- Trigger **OH GATE IN** with 8th or 16th note rhythm
- Set **DECAY** medium-long
- Sequence **VC-Q** with 4–8 step pattern
- Use **OH ACCENT IN** for selected notes
- Mix **OH OUT** with moderate level

**Result**
A repetitive metallic motif that sits between percussion and melody.

---

## Patch 3: Choked melodic phrasing
**Goal:** use CH to articulate OH like note lengths.

- Send sparse sequence to **OH GATE IN**
- Send syncopated shorter rhythm to **CH GATE IN**
- Keep choke enabled
- Sequence **VC-Q**
- Use OH for “long notes,” CH to truncate them

**Result**
Complex note-length interplay without a traditional envelope/gate setup.

---

## Patch 4: Raw source into resonator
**Goal:** extract harmonic material and impose pitch externally.

- Patch **Band-Pass OUT** into a resonator or tuned filter bank
- Trigger OH or CH separately for transient energy
- Modulate **VC-Q** slowly
- Use resonator tuning for actual melodic scale

**Result**
The HATS808 becomes the excitation source while the resonator supplies the stable pitch center.

This is one of the best ways to make the module contribute to clearly melodic material.

---

## Patch 5: Self-oscillating drone melody
**Goal:** drone/ambient harmonic layer.

- Turn **Q** to self-oscillation
- Patch slow sequencer or random stepped CV to **VC-Q**
- Feed Band-Pass OUT into delay/reverb
- Use external VCA for fade-ins
- Optionally add OH/CH triggers occasionally for attacks

**Result**
A drifting metallic drone with melodic movement.

---

## What kind of melody is this module best at?

The HATS808 is best for:

- **metallic melodies**
- **atonal or semi-pitched lines**
- **industrial hooks**
- **percussive motifs**
- **bell-like sequences**
- **resonant drones**
- **accented top-line rhythmic melody**

It is less suitable as:
- a precision tonal oscillator,
- a calibrated bass/lead voice,
- or a conventional subtractive synth VCO.

Think of it as a **spectral percussion source that can be pushed into pitch-adjacent behavior**.

---

## Performance suggestions

## Use OH and CH as two “voices”
Since OH and CH have separate outputs and accents, you can create:
- one brighter, longer “melodic” voice from OH
- one shorter answering voice from CH

This can create call-and-response patterns that feel melodic even if both are percussion-derived.

## Sequence accent separately from pitch
This is especially effective with the HATS808 because accent also affects attack, not only volume. A simple 4-step VC-Q sequence can sound far more musical if the accent pattern is different from the gate pattern.

## Exploit analog instability
The manual notes oscillator tolerances and slight variation between units. For melodic use, that is not a flaw — it is the charm. It gives:
- natural drift
- organic high-end motion
- less static repetition

---

## Summary

The **Tiptop Audio HATS808** can contribute melodic material in several strong ways:

1. **VC-Q sequencing** creates quasi-pitched metallic note changes.
2. **High Q / self-oscillation** turns the filter into a tone source.
3. **Band-Pass OUT** provides raw harmonic material for external melodic shaping.
4. **Accent** adds phrase definition and dynamic contour.
5. **Choke** acts like note-length articulation for OH phrases.
6. **Hot outputs** make it excellent for driving resonators, filters, distortion, and other modules that can impose stronger pitch identity.

So while it begins as a hi-hat module, in a Eurorack context it can absolutely serve as a source for **melodic percussion, resonant leads, metallic drones, and tuned textures**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)