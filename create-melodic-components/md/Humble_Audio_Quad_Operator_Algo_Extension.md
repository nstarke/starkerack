# Humble Audio — Quad Operator Algo Extension

- [Manual PDF](../../manuals/Quad Operator Manual.pdf)

---

[Quad Operator Manual PDF](https://www.dropbox.com/paper/doc/print/JsIQoU7GbeAboEJku9ZgE?print=true)

# Humble Audio Quad Operator (+ Algo) for melodic patching

The **Quad Operator** is a 4-operator digital FM voice for Eurorack, with:

- 4 independently available operators
- lock/free modes per operator
- variable waveshapes per operator: **sine → triangle → square → saw**
- a full **modulation matrix**
- per-operator gain acting like a built-in modulation VCA
- external **AR FM** input for bringing another oscillator/audio source into the FM network
- optional **Algo expander** for storing and morphing FM matrices

From a melodic musician’s perspective, this is not just an FM drum/noise machine. It can be a:

- classic FM voice
- chord/harmony generator
- 4-oscillator melodic bank
- animated bass/lead source
- complex phase-locked modulation source
- algorithm-morphing timbre voice

---

# What matters most for melodic use

## 1. Lock mode is the melodic sweet spot
In **lock state**, each operator tracks the master pitch in **integer ratios** relative to the global Coarse/Fine tuning. This is the most important mode for tonal FM because:

- harmonic relationships are preserved
- pitch stays musically stable
- classic FM sidebands are easier to control
- operators can act as harmonically related carriers/modulators

If your goal is **basslines, leads, bells, keys, plucks, pads, or chord-like tones**, start here.

### Best starting point for melodic FM
The manual itself strongly suggests this kind of setup:

- **VCO mode**
- all operators in **lock**
- all **Detune** knobs at 12 o’clock
- all **Shape** knobs fully CCW for **sine**
- all **Mod sends** fully CCW to begin

That gives you a clean, harmonically sensible baseline. Then add FM gradually.

---

## 2. Free mode turns it into a 4-oscillator melodic bank
In **free state**, an operator becomes an independent oscillator:

- the **Ratio knob** becomes coarse tuning
- **Ratio CV** becomes **1V/oct** for that operator
- each output can be patched as its own voice or layer

This is very useful melodically if you want:

- 4 tuned drones
- intervals/chords from separate operators
- paraphonic textures
- layered detuned melody lines
- one operator as audible pitch, others as tuned modulators

This means the Quad Operator can behave like either:

- **one complex FM voice**, or
- **four related oscillators**

That flexibility is the key to melodic composition with it.

---

# Core melodic patching strategies

## Strategy A: Classic 2-op or 4-op FM voice
Use one operator as the main audible output and the others as modulators.

### Patch idea
- Put all operators in **lock**
- Send your sequencer to **1V/Oct**
- Listen primarily to **Op 1 out**
- Turn up modulation sends from Op 2 and/or Op 3 into Op 1
- Use **Gain CV** on the modulating operators with envelopes to animate timbre

### Why this works
Because operator gain controls both:

- the output level of that operator
- how strongly it modulates other operators through its sends

So if an envelope opens/closes the gain of a modulator, you get **dynamic FM index**—the classic recipe for:

- plucks
- electric piano tones
- struck metal
- evolving bass
- vowel-like movement

### Melodic results
- **Low FM amount**: warm, stable leads and basses
- **Envelope-shaped FM**: punchy attack transient with mellow sustain
- **Multiple modulators**: richer harmonic motion across the melody

---

## Strategy B: Chord voice from multiple outputs
Since each operator has its own output, you can use the Quad Operator as a harmonic cluster generator.

### Patch idea
- Put all operators in **free** mode
- Send different pitch CVs to each **Ratio CV** input
- Patch all four outputs to a mixer
- Tune operators as chord tones:
  - Op 1 = root
  - Op 2 = third
  - Op 3 = fifth
  - Op 4 = seventh or octave
- Optionally send one common envelope/VCA downstream

### Why this works
In free mode, each operator is a separate oscillator. You can make:

- triads
- jazz chords
- stacked octaves
- contrapuntal lines if each goes to a separate VCA/filter

### Extra musical trick
Keep one or two operators in free mode and others in lock mode for a hybrid patch:
- locked operators provide harmonic FM structure
- free operators add independently tuned chord tones or dissonant color

---

## Strategy C: One melodic carrier, self-FM and cross-FM for expression
The matrix allows each operator to modulate:

- other operators
- **itself**

That means you can use subtle self-modulation for extra brightness and edge.

### Patch idea
- All ops in **lock**
- Use **Op 1** as the main audible voice
- Turn up:
  - Op 2 → Op 1 slightly
  - Op 3 → Op 1 slightly
  - Op 1 → Op 1 very subtly
- Envelope the gain of Op 2 or Op 3

### Result
You get a very playable melodic timbre that can move between:

- sine-like purity
- reed-like brightness
- metallic bite
- buzzy harmonic saturation

This is especially good for **melodic techno**, **IDM leads**, and **FM bass**.

---

## Strategy D: Use shapes beyond sine for more melodic density
Each operator can morph continuously:

**sine → triangle → square → saw**

For melodic work, this is huge. Classic FM often starts with sine waves, but the Quad Operator lets you begin with already-rich spectra.

### Practical use
- Start with **sine** for clean, stable pitch perception
- Move a modulator toward **triangle** or **square** for stronger harmonic complexity
- Move the carrier toward **saw** if you want brighter, more present melodic lines

### Caution
The manual notes that overtones plus modulation can quickly create:

- aliasing
- noise
- harsher spectra

Musically, that means:
- use richer shapes sparingly for melody
- try brighter modulators but keep the carrier simpler
- reserve full saw/square FM for accents, choruses, or aggressive passages

---

# Best melodic roles for each control

## Coarse + Fine
These are global master tuning controls for locked operators.

Use them for:
- setting the overall register
- transposing the patch
- making the voice sit as bass, alto, or lead

## 1V/Oct
This controls all operators in lock state together.

Use it from:
- pitch sequencer
- keyboard controller
- quantized random source

This is the main melodic entrance point for conventional pitched use.

## LF FM
This is ±6 semitones and best for slow pitch movement.

Excellent for:
- vibrato
- pitch envelopes
- portamento-like bends
- expressive melodic instability

Use a slow LFO or envelope here for phrasing.

## Reset
This resets phase of all operators.

For melodic use, this matters because phase reset can make attacks more repeatable, giving:
- more consistent transients
- tighter plucks
- more percussive note starts
- repeatable modulation shapes when using LFO mode

Good for sequenced melodies where each note should articulate similarly.

---

# The hidden melodic superpower: Gain CV per operator

The manual makes a critical point: **Gain CV affects both output level and modulation intensity**.

That means one envelope can simultaneously control:

- how loud an operator is
- how much it modulates others

This is extremely powerful for melodic FM because it creates natural timbral articulation.

## Musical applications

### FM pluck
- Op 1 audible
- Op 2 modulates Op 1
- Envelope into **Gain CV 2**

Result:
- bright attack
- mellow decay
- very playable plucked tone

### Dynamic harmonic bloom
- Op 2 and Op 3 both modulate Op 1
- give each a different envelope or LFO
- one fast decay, one slow decay

Result:
- attack sparkle followed by sustained body
- useful for keys, mallets, bells, and evolving leads

### Carrier/modulator balance as composition
Because gain also controls output, you can mix audible operators and hidden modulators in fluid ways:
- start with modulator unheard but active
- fade it into audibility for a duet/chord feel
- blur the line between timbre generator and melodic voice

This is one of the most musical aspects of the module.

---

# Using the Algo expander for melodies

The **Algo** expander stores and morphs the modulation matrix states. It does not store every panel setting—specifically it stores the **Mod x knob positions** for all four operators plus AR FM.

Think of this as storing FM routing/intensity presets.

## Why this is musically useful
For melody, changing algorithm is often more dramatic than changing pitch. With Algo you can:

- store a mellow FM structure in slot A
- store a bright, stacked, feedback-heavy structure in slot B
- crossfade between them during a phrase

That gives you **timbre progression** over a melody line.

## Great melodic uses

### Verse / chorus timbre states
- **A** = soft, simple 2-op voice
- **B** = brighter, denser 4-op voice
- crossfade between them over a pattern

### Performance morphing
- assign CV to crossfade
- slowly move from one algorithm to another over several bars

### Call and response
- use one sequenced melody
- alternate between two algorithm states for contrast

Because the modulation matrix is the heart of the sound, Algo effectively gives you **macro-form timbral composition**.

---

# Using AR FM with the Quad Operator melodically

The **AR FM** input lets you bring in an external audio-rate source and route it to any operator with its own modulation sends and gain control.

## Melodic applications

### External oscillator as master color source
Feed another VCO into AR FM and use it to modulate one or more operators. This can produce:

- more organic FM tones
- richer attacks
- layered harmonic motion

If the external oscillator tracks the same pitch sequence, you get a tightly related but more complex melodic tone.

### Feedback-ish melodic textures
The manual specifically suggests trying a phase-locked operator, processing it externally, and feeding it back in.

That can create:
- vocal-like resonances
- metallic but pitch-stable leads
- aggressive basses with a coherent note center

### Audio-rate ornamentation
Patch a fast oscillator, wavetable source, or filtered noise burst into AR FM for:
- note attack articulation
- transient brightening
- unstable shimmer on top of a melodic line

Watch the **clipping LED**, and use the AR FM gain knob to avoid overdriving unless distortion is desired.

---

# Patch recipes for melodic music

## 1. FM bass
**Goal:** solid, punchy, harmonic bassline

- VCO mode
- all operators in **lock**
- all shapes on **sine**
- all detune centered
- sequence into **1V/Oct**
- listen to **Op 1**
- Op 2 modulates Op 1 moderately
- envelope to **Gain CV 2**
- slight envelope or LFO to **LF FM** for subtle pitch movement if desired

### Result
Clean low-end pitch center with a bright attack and rounded sustain.

---

## 2. Electric piano / mallet voice
**Goal:** percussive melodic keys

- all operators in **lock**
- Op 1 = carrier out
- Op 2 and Op 3 modulate Op 1
- keep ratios simple/integer
- sine or triangle shapes
- fast-decay envelope to Gain CV of modulators
- optional slight self-mod on Op 1

### Result
A struck, harmonic timbre with evolving overtone decay.

---

## 3. Bell lead
**Goal:** metallic but still playable melody

- all operators in **lock**
- use nontrivial integer ratios
- add a little detune to one operator if desired
- use sine carrier, triangle/square modulator
- moderate to high modulation depth
- long decay envelope on modulator gain

### Result
Shimmering melodic tones with bell-like sidebands.

---

## 4. Chord stack oscillator
**Goal:** one module producing harmonic accompaniment

- all operators in **free**
- send pitch CV individually to ratio inputs
- tune root/third/fifth/seventh
- mix Op 1–4 outputs
- optionally modulate shape separately per operator

### Result
A compact 4-oscillator chord source. Great into a shared filter/VCA for pads or stabs.

---

## 5. Morphing lead with Algo
**Goal:** one melody, evolving algorithms

- create two FM matrices:
  - **A**: gentle/simple
  - **B**: dense/aggressive
- save each on Algo
- sequence pitch normally
- crossfade manually or with CV over phrase length

### Result
A lead that grows from pure to complex without repatching.

---

## 6. Counterpoint patch
**Goal:** several melodic layers from one module

- put some operators in **free** and others in **lock**
- locked ops create the main FM voice
- free op becomes a separate drone/countermelody
- route outputs to separate VCAs/channels
- sequence or modulate independently

### Result
One module can handle foreground melody plus harmonic accompaniment.

---

# Tips for keeping melodies musical

## Stay simple first
FM can become dissonant quickly. For tonal writing:

- start with **sine**
- start with **one modulator**
- keep **detune centered**
- use **lock mode**
- add modulation slowly

## Use integer ratios for stable tonality
The manual emphasizes that lock mode is essential for harmonic overtone relationships. If you want notes to read clearly as pitches, stay there.

## Use gain envelopes instead of cranking static modulation
This creates notes that speak with articulation, rather than sounding constantly over-complex.

## Shape is a big compositional control
Changing shape may be more musically effective than adding more FM.

## Use Reset for repeatable attacks
Especially useful for sequenced melodic lines and plucks.

---

# Limitations to keep in mind

The manual suggests a few rough edges:

- some sections are incomplete, such as firmware notes and algorithm translation guidance
- the Algo stores modulation matrix states, not the entire voice
- complex shape + heavy FM can get noisy/aliased quickly
- free mode is less naturally harmonic unless intentionally tuned

None of these are dealbreakers, but they shape how melodic patches are best approached.

---

# Bottom line

The **Quad Operator** is especially strong for melodic music because it combines:

- stable locked-ratio FM for tonal playing
- four available outputs for layering and chords
- dynamic modulation index via Gain CV
- external audio-rate FM integration
- morphable FM matrix states with the Algo expander

In practice, the most musically useful workflows are:

1. **Locked 2-op/4-op FM voice** for bass, leads, keys, bells  
2. **Free-mode oscillator bank** for chords and layered harmony  
3. **Algo morphing** for phrase-level timbral development  
4. **Gain-CV animated modulators** for expressive note articulation  

If you want, I can also turn this manual into:
- a **“best melodic patch recipes” cheat sheet**
- a **signal-flow diagram**
- or a **beginner-friendly explanation of how to program DX-style algorithms on the Quad Operator**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)