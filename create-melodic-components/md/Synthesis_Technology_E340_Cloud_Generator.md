# Synthesis Technology — E340 Cloud Generator

- [Manual PDF](../../manuals/E340_manual.pdf)

---

[Manual PDF](https://www.synthtech.com/euro/e340)

# Synthesis Technology E340 Cloud Generator — melodic use in a Eurorack patch

The E340 is best understood as a **single oscillator voice that internally stacks 2, 4, or 8 detuned oscillators**. It gives you two simultaneous outputs:

- **SAW OUT**
- **SINE OUT**

That makes it especially strong for **thick melodic lines, drones with pitch focus, chord-like unison textures, and animated lead/bass parts**.

## What this module contributes melodically

### 1. A playable pitched oscillator
The E340 accepts:

- **1V/OCT** for note pitch
- **FM CV** for pitch modulation
- **SYNC** for hard sync effects

So at its core, it can be used exactly like a melody oscillator:
- sequence pitch into **1V/OCT**
- use **COARSE** and **FINE** to tune range
- send the output to a filter/VCA/envelope chain

### 2. “Unison melody” generator
The special melodic feature is **SPREAD**, which detunes the internal oscillators around the center pitch.

This means one incoming pitch CV can become:
- a subtle, wide **supersaw-style lead**
- a soft chorused **sine ensemble**
- an unstable, swarm-like **animated note cloud**

For melodic music, this is useful because it adds **size and movement without needing multiple VCOs**.

### 3. Motion around a note
The **CHAOS** and **CHAOS BW** controls add filtered random FM-like movement to the detuned voices.

Musically, that means:
- **small CHAOS** = lively pitch drift, like analog instability
- **higher CHAOS** = more animated shimmer
- **high CHAOS + wide BW** = noisy, unstable, nearly effects-style pitch cloud

For melody, keep CHAOS low to moderate if you want notes to remain clearly tonal.

---

# Important behavior that affects patching

The manual notes:

- CV inputs are effectively designed around about **-5V to +5V**
- There are **no built-in CV attenuators** for most modulation destinations
- Any incoming CV is **added to the panel knob position**
- If using a full-scale bipolar CV, the relevant panel knob should often be around **12 o’clock**
- Overdriving CV can cause **pitch changes** or clamping

So in musical patches:
- attenuate external modulation before patching when possible
- use modest modulation depth for SPREAD/CHAOS if you want stable intonation
- be especially careful with pitch-related FM and large spread modulation

---

# Best melodic roles for the E340

## 1. Huge lead voice
Use **SAW OUT** with:
- low or medium **SPREAD**
- **DENSITY** at 4 or 8
- low **CHAOS**
- into a lowpass filter and VCA

Result:
- wide, glossy lead
- classic supersaw-inspired melodic sound
- good for trance, synthwave, cinematic hooks

### Patch idea
- Sequencer CV → **1V/OCT**
- Gate → envelope → VCA
- **SAW OUT** → filter → VCA
- Envelope or slow LFO → filter cutoff
- Small CV modulation to **SPREAD CV** for chorus-like expansion on held notes

---

## 2. Soft ensemble sine melody
Use **SINE OUT** instead of saw.

Result:
- organ-like or choir-like melodic tone
- less buzzy, more pure
- useful for ambient lines, counter-melodies, basses, and tuned drones

### Good settings
- **DENSITY** = 4 or 8
- **SPREAD** very low
- **CHAOS** low
- **CHAOS BW** low to medium

This gives a very elegant “many oscillators gently drifting together” character.

---

## 3. Animated bassline
The E340 can also do bass, especially if you keep it more controlled.

### Suggested approach
- **DENSITY** = 2 or 4
- **SPREAD** very low
- **CHAOS** almost off
- choose **SINE OUT** for sub-heavy bass, or **SAW OUT** for more aggressive bass

Because amplitude drops as density increases, **DENSITY 2** can feel punchier and louder for bass parts.

---

## 4. Chord-like unison without actual chords
The E340 does not quantize internal voices to chord intervals; it detunes them around a central pitch. Still, melodically it can create a **quasi-harmonic cloud**.

This works well when:
- notes are held longer
- **SPREAD** is moderate
- filtering shapes the brightness
- reverb/delay is added

You get the emotional effect of harmonic width even though the module is technically still centered on one pitch.

---

# How the controls shape melody

## COARSE and FINE
These set the base tuning range.

Use:
- **COARSE** for register
- **FINE** for exact tuning with the rest of your system

If tracking is off, the manual notes a **blue multiturn trimmer** on the PCB for calibrating **1V/OCT**.

---

## FM amount + FM input
This is pitch modulation of the fundamental frequency.

For melodic purposes:
- tiny modulation from an envelope can add attack punch
- vibrato from an LFO can be expressive
- audio-rate FM can make notes more metallic, but may reduce tonal clarity

Use cautiously if your goal is a clean melody line.

---

## SPREAD
This is the most important musical control.

It detunes oscillators around the center pitch, and the detune amount is **exponential**:
- very small at first
- then rapidly wider

So the sweet spots for melodic use are often in the lower part of the knob range.

### Musical interpretation
- very low: subtle thickening
- low-medium: unison lead / chorus
- medium: dramatic supersaw cloud
- high: swarm, less precise pitch center

---

## CHAOS
Adds independent random movement to the spread voices.

For melody:
- use a little for life
- use more for unstable ambient or experimental lines
- too much can make tuned passages feel blurred

---

## CHAOS BW
Changes the speed character of that random motion in **6 steps**.

Think of it as:
- **narrow BW** = slow drift
- **wide BW** = faster flutter

For musical phrasing:
- slow drift is better for pads and lyrical melodies
- faster motion is better for nervous textures and special effects

---

## DENSITY
Selects **2, 4, or 8 oscillators**.

Manual note: more oscillators means **automatic amplitude reduction** to avoid clipping.

### Musical use
- **2** = clearer, stronger, more direct
- **4** = balanced width and definition
- **8** = widest, richest, most washed-out

For melodies that need to cut through a mix, **4** is often a sweet spot.

---

## SYNC
A positive voltage over **+0.25V** hard-syncs the VCOs.

This can create:
- harmonically rich synced leads
- aggressive timbral changes while keeping melodic pitch anchored
- unusual textures when combined with SPREAD

For melodic use, sync is excellent if another oscillator is driving the sync input. You can then sequence the E340 as the “slave” oscillator and get animated harmonic movement while the note pitch remains playable.

---

# Using both outputs together

A major strength of the E340 is having **SAW and SINE available at the same time**.

## Layered melodic patch
Use:
- **SINE OUT** for body/fundamental
- **SAW OUT** for brightness

Possible routing:
- SINE → one VCA/filter path
- SAW → separate filter/VCA path
- mix them later

This gives a more produced, layered sound from one module.

### Example
- SINE path: lowpass filtered, strong low mids
- SAW path: brighter, maybe highpass or bandpass filtered
- both controlled by the same sequencer and envelopes

Result:
- polished lead or bass with weight and air

---

# Practical melodic patch recipes

## Patch 1 — Supersaw melody
**Goal:** big, modern melodic line

- Pitch sequencer → **1V/OCT**
- Gate sequencer → envelope
- **SAW OUT** → lowpass filter → VCA
- Envelope → VCA CV
- Slow LFO or envelope → filter cutoff
- Small attenuated LFO → **SPREAD CV**
- Settings:
  - DENSITY: 8
  - SPREAD: low-medium
  - CHAOS: low
  - CHAOS BW: low

This makes a classic wide lead while staying tuneful.

---

## Patch 2 — Floating ambient melody
**Goal:** soft, shifting notes with motion

- Quantized CV source → **1V/OCT**
- **SINE OUT** → VCA → reverb/delay
- Slow random or envelope modulation → **CHAOS CV**
- Very slow CV → **SPREAD CV**
- Settings:
  - DENSITY: 4 or 8
  - SPREAD: low
  - CHAOS: low-medium
  - CHAOS BW: low

This creates an ensemble-like melodic line that breathes.

---

## Patch 3 — Expressive mono bass
**Goal:** thick but controlled bass melody

- Sequencer → **1V/OCT**
- **SINE OUT** or **SAW OUT** → filter → VCA
- Envelope → VCA and slight filter modulation
- Optional tiny LFO → **FM input** via FM amount for subtle vibrato
- Settings:
  - DENSITY: 2
  - SPREAD: near minimum
  - CHAOS: off or barely on
  - CHAOS BW: low

This keeps the bass centered while still fuller than a normal VCO.

---

## Patch 4 — Sync lead with motion
**Goal:** more aggressive melodic tone

- Another oscillator → **SYNC input**
- Sequencer → E340 **1V/OCT**
- **SAW OUT** → filter → VCA
- Moderate **SPREAD**
- Low **CHAOS**
- Sweep filter and/or spread over time

The manual specifically notes sync can sound very interesting at higher spread settings. This can produce animated, cutting lead timbres.

---

## Patch 5 — Dual-output melodic layering
**Goal:** one melody, two complementary timbres

- Sequencer → **1V/OCT**
- **SINE OUT** → VCA A
- **SAW OUT** → filter → VCA B
- Same envelope gates both VCAs
- Mix A and B together
- Add a little modulation to SPREAD

This gives a very complete melodic voice from a single oscillator module.

---

# Best modulation strategies for melodic music

## Good choices
- Small LFO to **SPREAD CV** for widening/narrowing
- Slow random to **CHAOS CV** for life
- Envelope to **FM** for transient pitch push
- Keyboard/mod wheel/pressure routed to spread or chaos for expressiveness

## Use carefully
- Large bipolar CV directly into SPREAD/CHAOS/BW without attenuation
- Fast random modulation if you want stable pitch perception
- Heavy FM for tonal melodies

---

# Tonal and compositional character

The E340 is ideal when you want melody to feel:

- **larger than one oscillator**
- **alive and moving**
- **dense without stacking many modules**
- **cinematic, dreamy, glossy, or swarming**

It is less ideal if you want:
- perfectly clinical single-oscillator purity
- explicit chord voicings from one pitch CV
- precise interval-based harmony between internal voices

Instead, it excels at **unison-based melodic richness**.

---

# Summary

The E340 Cloud Generator is a strong melodic oscillator because it combines:

- proper **1V/OCT pitch control**
- two simultaneous timbral outputs
- internal multi-oscillator unison
- animated detuning via **SPREAD**
- controlled instability via **CHAOS** and **CHAOS BW**
- timbral aggression via **SYNC**

## Best melodic applications
- supersaw-style leads
- ensemble sine melodies
- thick basses
- ambient unison lines
- sync leads with width
- layered mono voices using both outputs

## Most musical advice from the manual
Keep external CV moderated and use **small amounts of SPREAD and CHAOS first**. The E340 becomes most melodic when the central pitch stays clear and the cloud effect adds width rather than overwhelming note identity.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)