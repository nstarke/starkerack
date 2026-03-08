# Schlappi Engineering — Three Body

- [Manual PDF](../../manuals/three_body_manual_01302023a.pdf)

---

[Three Body Manual (Schlappi Engineering)](attachment)

# Using the Schlappi **Three Body** for melodic music

The **Three Body** is a 3-oscillator digital modulation complex oscillator focused on **phase modulation, linear FM, ratio relationships, and stereo motion**. For melodic use, its big strength is that the three oscillators can behave either as:

- **independent VCOs/LFOs**
- **ratio-locked harmonic oscillators**
- **cross-modulating carriers/modulators**
- **a stereo melodic voice with internal normalization**

That makes it especially good for:

- harmonic lead voices
- metallic but tunable FM tones
- animated basses
- chord / pseudo-paraphonic interval structures
- arpeggiated ratio melodies
- tempo-locked melodic modulation

---

## What the module fundamentally is

Three Body contains:

- **1 center oscillator**
- **2 outer oscillators**

Each oscillator can run in:

- **FREE mode**  
  Like a normal oscillator/LFO with pitch controlled by coarse/fine and V/oct.

- **RATIO mode**  
  The oscillator tracks another oscillator or external sync input at a **multiplied or divided ratio**.

Each oscillator also supports modulation:

- **phase modulation**
- **frequency modulation**
- **sync / tracking**

The center oscillator is special because it has:

- **sine + cosine**
- **saw + cosaw**
- dual phase inputs from the two outer oscillators
- especially strong stereo applications

---

# Why this module is musically useful for melody

For melodic work, the key manual points are:

1. **Outer oscillators can track the center oscillator in ratio mode** with no cable inserted into their sync jacks.
2. This creates stable **musical intervals and harmonic series relationships**.
3. The center oscillator can remain your pitch reference while the outer oscillators become:
   - harmonics
   - subharmonics
   - changing interval voices
   - FM operators
4. The module supports **1V/oct on the transpose and individual V/Oct/Ratio inputs**, so it can still play from sequencers and keyboards.
5. You can modulate the ratio CV inputs for **melodic interval animation**, not just timbre.

In practice, it can behave like:

- a **3-oscillator harmonic voice**
- a **DX-style operator cluster with analog patchability**
- a **subharmonic chord machine**
- a **stereo melodic oscillator**

---

# Most important melodic patching ideas from the manual

## 1. Harmonic interval voice

This is the most immediately musical use.

### Patch
- Set **center oscillator** to:
  - **FREE**
  - **HIGH**
- Patch your sequencer pitch CV to **TRANSPOSE**
- Set one or both **outer oscillators** to:
  - **RATIO**
- Listen to:
  - center sine/triangle
  - one or both outer sine outputs

### Result
The center oscillator plays the melody.  
The outer oscillators become interval voices related by integer multiply/divide settings.

### Musical use
You get:

- octaves
- fifths
- fourths
- more complex overtone relationships
- moving chord-like stacks from a single pitch line

### Good settings
With divide at 1 and multiplication changing:
- 1:1 unison
- 2:1 octave
- 3:2 fifth-ish relationships depending on settings
- harmonic series climbing

This is ideal for:

- bass + upper harmonic
- drone melodies
- simple two-note harmonization
- pseudo chords from one sequencer lane

---

## 2. Subharmonic melody generator

The manual makes clear that in ratio mode the oscillators can also **divide**.

### Patch
- Center oscillator = **FREE, HIGH**
- Outer oscillator(s) = **RATIO, DIV**
- Sequence the center from **TRANSPOSE**
- Take audio from outer oscillators

### Result
Instead of upper harmonics, you get **subdivided pitch relationships**. This can feel like:

- suboctaves
- undertone series
- organ-like interval structures
- Subharmonicon-style harmonic motion

### Musical use
Great for:

- dark bass lines
- medieval/drone harmony
- thick mono leads
- pseudo counterpoint from one CV source

---

## 3. Ratio-CV arpeggiation

One of the most interesting melodic functions in the manual: feed CV into the **V/OCT RATIO** input of an outer oscillator.

### Patch
- Center oscillator = melodic source in FREE mode
- Outer oscillator = RATIO mode
- Send a slow stepped CV, envelope, or sequencer row into **outer V/OCT RATIO**
- Attenuate carefully

### Result
The outer oscillator changes multiplier or divider values, creating **discrete interval jumps** relative to the center pitch.

### Musical effect
This creates:

- arpeggiation
- harmonic melody doubling
- interval sequencing
- pseudo chord inversions

If modulation is subtle, it can hop between a few ratio values and feel like a musically locked harmony line.

This is one of the strongest ways to get **melodic movement without repitching the root**.

---

## 4. Three-note harmonic stacks from one sequence

Because all oscillators can be heard independently, Three Body can produce three related musical lines.

### Patch
- Sequencer CV to **TRANSPOSE**
- Center oscillator = **FREE**
- Left oscillator = **RATIO**
- Right oscillator = **RATIO**
- Use different mult/div settings on left and right
- Take all three sine outputs into a mixer

### Result
A single melodic line becomes a 3-voice interval stack.

### Musical use
This gives:
- instant triad-ish structures
- open fifth drones
- stacked harmonics
- organ/register sounds

It won’t always map to equal-tempered harmony in a traditional way, because ratio relationships are just intonation/harmonic-based rather than fixed semitone transposition. But that’s often exactly why it sounds rich.

---

## 5. Stereo melodic voice

The center oscillator has special outputs:

- **SINE**
- **COSINE**
- **SAW**
- **COSAW**

The manual explains that these are phase-related outputs designed for wide stereo use, especially under phase modulation.

### Patch
- Use center **SINE** to left channel
- Use center **COSINE** to right channel
- Or use **SAW / COSAW**
- Bring up **PHASE INDEX 1** and **PHASE INDEX 2**
- Let outer oscillators modulate the center

### Result
A single melodic line becomes a **wide stereo voice** with internal timbral animation.

### Musical use
Excellent for:

- leads
- pads
- drones
- melodic ambient voices
- stereo bass textures

This is especially nice because you can keep the melody simple while the timbre blooms around it.

---

## 6. Tuned FM voice

The manual strongly supports **linear FM in ratio mode** for harmonic sounds.

### Patch
- Center oscillator = base pitch source
- Outer oscillators = **RATIO + LIN FM**
- Outer oscillators tuned above center with mult settings
- Listen to outer sine outputs
- Bring up their **FM INDEX**
- Optionally modulate FM index with envelopes

### Result
You get classic **tuned FM sidebands** with better harmonic stability when simple ratios are used.

### Musical use
This is ideal for:

- bells
- electric piano-ish tones
- glassy leads
- metallic basses
- plucked digital tones

The manual notes an important rule:

- for harmonic audio-rate modulation, use **simple ratios**

So melodic patches are strongest when carrier/modulator relationships are kept simple.

---

## 7. Animated timbre while pitch stays stable

A major musical advantage of **phase modulation** over FM, according to the manual, is that PM avoids some pitch drift and DC-offset pitch problems.

### Patch
- Center oscillator is your audible melodic output
- Outer oscillators modulate center via **PHASE 1** and **PHASE 2** normalization
- Sequence only the center with **TRANSPOSE**
- Use the outer oscillators either:
  - ratio-locked for harmonic PM
  - or free-running for more unstable colors

### Result
The melody remains more stable while timbre shifts dramatically.

### Musical use
This is ideal when you want:

- recognizably pitched melody
- evolving harmonics
- strong articulation without filter reliance

It’s a very effective way to create expressive melodic phrases that sound “complex oscillator” but remain playable.

---

# Internal normalizations that matter for melodic patching

The manual describes several normalizations that make melodic patching easy without many cables.

## Modulation normalization

- **Center oscillator PHASE inputs** are normalized from the two outer sine outputs
- **Outer oscillator FM inputs** are normalized from the center oscillator:
  - left gets center sine
  - right gets center cosine
- **Outer oscillator PHASE inputs** are normalized from the opposite outer sine

## Ratio normalization

- Outer oscillators in **RATIO mode** track the center oscillator if no cable is inserted in their sync inputs

### Why this matters
This means you can quickly get:

- a harmonic 3-oscillator voice
- stereo FM pair
- center-carried melody with outer interval tones
- cross-modulated harmonic stack

without much patching.

---

# Best melodic roles for each oscillator

## Center oscillator
Best as:
- root pitch
- main melodic oscillator
- stereo voice source
- PM target
- master for harmonic tracking

Use outputs:
- **sine/cosine** for cleaner stereo melody
- **saw/cosaw** for richer harmonic material
- **triangle** for a middle-ground tone

## Outer oscillators
Best as:
- harmony oscillators
- FM carriers
- PM modulators
- ratio-derived intervals
- subharmonic voices

Use outputs:
- **sine** for cleaner FM/melodic tones
- **saw/triangle/square** for more aggressive layered voicing

---

# Practical melodic patch recipes

## Patch 1: Simple harmonic lead
- Center: FREE / HIGH
- Left: RATIO / MULT
- Right: RATIO / MULT
- Sequencer to TRANSPOSE
- Mix center sine + left sine + right sine
- Set outer ratios to octave/fifth-ish relationships

**Sound:** harmonically rich mono/stereo lead from one sequence.

---

## Patch 2: Subharmonic bass melody
- Center: FREE / HIGH
- One outer oscillator: RATIO / DIV
- Sequence center pitch from TRANSPOSE
- Listen mainly to the divided outer oscillator plus some center sine

**Sound:** deep, organ-like bass with strong tonal center.

---

## Patch 3: Melodic stereo PM lead
- Center: FREE / HIGH
- Outer oscillators: RATIO
- Listen to center **SINE + COSINE**
- Raise **PHASE INDEX 1/2**
- Sequence center with TRANSPOSE

**Sound:** wide stereo melodic voice with animated timbral motion.

---

## Patch 4: FM pluck / bell
- Center: lowish pitch
- Outer oscillators: RATIO + LIN
- Divide fully down, multiply above noon
- Listen to outer sine outputs
- Envelope into **FM INDEX**
- Sequence pitch with TRANSPOSE

**Sound:** tuned digital percussion, mallets, bells, sharp plucks.

---

## Patch 5: Arpeggiated interval companion
- Center sequenced melodically
- Right oscillator in RATIO
- Stepped CV into right **V/OCT RATIO**
- Heavily attenuate
- Mix center + right outputs

**Sound:** one melody plus automatically shifting interval accompaniment.

---

## Patch 6: Pseudo chord machine
- Center sequenced
- Left in ratio-div
- Right in ratio-mult
- Tune by ear to consonant relationships
- Mix all three outputs

**Sound:** evolving 3-note harmonic structures from one CV line.

---

# Melodic strategy: when to use FREE vs RATIO

## Use FREE mode when you want:
- traditional VCO behavior
- exact sequencer tracking
- independent pitch lines
- LFO duties
- looser, less locked harmonic behavior

## Use RATIO mode when you want:
- consonant interval relationships
- harmonic series control
- subharmonic structures
- stable audio-rate modulation
- one oscillator to derive melody-related voices from another

For melodic composition, **RATIO mode is the secret weapon**.

---

# How to keep it musical

The manual gives several strong hints.

## 1. Use simple ratios
For harmonic results:
- 1:1
- 2:1
- 3:2
- 4:3
- 5:4
- 6:5

These make FM/PM spectra feel pitched rather than chaotic.

## 2. Keep cross modulation moderate
Too much cross phase modulation can become:
- noisy
- shrieking
- unstable

A little adds life; too much destroys note identity.

## 3. Linear FM is strong
The manual says linear FM is amplified strongly internally. Small knob movements can have a big effect.

For melodic use:
- start low
- increase slowly
- use envelopes on index rather than constant high depth

## 4. Phase modulation is better for stable pitch color
If you want the note center to remain more obvious while adding harmonics, use PM rather than deep FM.

## 5. Use sine outputs first
For tuning and harmonic listening:
- start with sine outputs
- move to saw/cosaw later if you want more bite

---

# External tracking for melodic systems

The manual also notes that in **RATIO mode**, inserting an external signal into **SYNC** lets an oscillator track that external source.

### Musical uses
You can use this to:
- harmonize another oscillator in your system
- derive intervals from an external VCO
- create tempo-locked LFO divisions/multiplications
- build harmonic layers around another module’s voice

### Important caveat
Tracking is best with:
- simple waveforms
- monophonic sources
- steady signals

For audio harmonization, period tracking is preferred over PLL.

---

# Good compositional uses in a eurorack patch

## As a lead voice
Use center sine/cosine stereo pair, outer oscillators as ratio PM sources.

## As a bass voice
Use center as root, outer in divide mode for subharmonics, maybe add a little PM for growl.

## As a chord source
Use all three oscillators mixed together with different ratios.

## As an FM melody generator
Use outer oscillators as linear FM carriers and center as common modulator.

## As an accompaniment generator
Use one sequencer lane into transpose, then animate outer ratio CV inputs for shifting harmonies.

## As a drone/melodic hybrid
Sequence the center slowly, let outers track at ratios, cross-modulate lightly.

---

# Limitations to be aware of

Based on the manual:

- It is **not** a conventional equal-tempered chord oscillator.
- Ratio relationships are often **just-intonation / harmonic** rather than semitone-quantized.
- Deep FM or cross modulation can easily become:
  - noisy
  - unstable
  - inharmonic
- Audio-rate FM wants the modulator lower than the carrier for expected behavior.
- Heavy PM can become wavefold-like and noisy.

These are not flaws—they are the character of the module.

---

# Best overall melodic workflows

## Workflow 1: One-sequence harmonic voice
1. Sequence TRANSPOSE
2. Center in FREE
3. Outer oscillators in RATIO
4. Mix three outputs
5. Adjust mult/div for harmonic intervals

This is the most straightforward melodic use.

## Workflow 2: Stereo melodic timbre voice
1. Sequence center oscillator
2. Listen to center sine/cosine
3. Outer oscillators modulate center phase
4. Keep ratios simple
5. Use envelopes on indexes

This gives an animated modern melodic sound.

## Workflow 3: FM operator cluster
1. Center as modulator
2. Outer oscillators as ratio-locked carriers
3. Listen to outer sines
4. Envelope FM index
5. Tune ratios musically

This is the most “digital synth” style use.

---

# Bottom line

The **Schlappi Three Body** is extremely strong for melodic composition if you think of it as a **harmonic relationship generator**, not just a weird modulation oscillator.

Its most musical strengths are:

- **ratio-locked harmony**
- **subharmonic and overtone interval creation**
- **stereo phase-modulated melodic voices**
- **tunable FM tones**
- **one-sequence-to-many-related-pitches patching**

If you want, I can also turn this into:

1. a **“best melodic patches” cheat sheet**,  
2. a **signal-flow diagram**, or  
3. a **genre-oriented guide** like *techno / ambient / electro / soundtrack* uses for Three Body.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)