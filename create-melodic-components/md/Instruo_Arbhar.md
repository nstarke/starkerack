# Instruo — Arbhar

- [Manual PDF](../../manuals/Arbhar-Manual-Firmware-2.0-A5.pdf)

---

[arbhar Granular Audio Processor User Manual (Firmware 2.0)](https://www.instruomodular.com/wp-content/uploads/2023/09/arbhar-Manual-Firmware-v2.0.pdf)

# Using Instruō arbhar to Create Melodic Components in Music

The **Instruō arbhar** is primarily a **granular sampler/processor**, but the manual makes it clear that it can also function as a very capable **melodic voice, phrase manipulator, pitch texture generator, and wavetable oscillator**. If you treat it less like a “special effect” and more like a playable instrument, it can contribute **lead lines, chord clouds, tuned textures, rhythmic motifs, and loop-based melodic fragments**.

## What makes arbhar melodic?

From the manual, these features matter most for melody:

- **1V/Oct pitch tracking**
- **Pitch knob + external pitch CV**
- **Per-grain pitch application**, allowing polyphonic overlaps
- **Quantized random pitch deviation**
- **Six layers of recorded/imported audio**
- **Scan and Follow playback modes**
- **Wavetable mode**
- **Strike input/button for articulated note events**
- **Up to 88 grains across two engines**

That means arbhar can work as:

- a **pitched sample voice**
- a **granular oscillator**
- a **phrase looper with transposition**
- a **probabilistic harmonizer**
- a **wavetable synth voice**
- a **melodic texture source**

---

## 1. Basic melodic use: play arbhar as a pitched voice

The simplest melodic patch is:

- Record or load a **pitched sound** into a layer
- Patch a sequencer into **1V/Oct**
- Use **Pitch** knob as transpose
- Use **Strike input** for note articulation
- Tune **Length**, **Intensity**, **Scan**, and **Spray** for clarity

### Why this works
The manual states that pitch is applied **at the beginning of each grain**. This gives arbhar a distinctly polyphonic-feeling playback behavior when grains overlap. Shorter grain lengths make pitch changes feel more immediate and tighter; longer grains smear pitch into lush harmonic motion.

### Good source material for melody
Record or import:

- single sine/triangle tones
- plucked strings
- vocal vowels
- piano notes
- mallet hits
- short synth stabs
- harmonic field recordings

These give the granular engine stable spectral material to transpose musically.

### Best settings for cleaner melodies
For focused pitch playback:

- **Spray** low
- **Length** medium-short
- **Intensity** moderate
- **Grain Window** near Gaussian for smoothness or square-ish for more attack
- **Grain Direction** mostly forward
- **Scan** set to a stable, harmonically rich point in the sample

This yields a playable granular lead or pad.

---

## 2. Use the Strike engine as a melodic note trigger

arbhar has two engines:

- **Continuous granular engine**
- **Strike granular engine**

The **Strike engine** is very useful melodically because each trigger creates a grain event like a note articulation. The manual also notes these grains are **15% louder**, which helps them read like accents or notes in a phrase.

### Patch concept
- Sequencer pitch CV → **1V/Oct**
- Trigger sequencer / gate sequencer → **Strike input**
- Set **Intensity** to an extreme to disable continuous grains
- Now arbhar behaves more like a playable sampled/granular voice

This is one of the most direct ways to extract melody from arbhar.

### Results
You get:

- plucked granular notes
- tuned vocal hits
- transposed snippets
- pseudo-sampler lines
- percussive melodic fragments

For best note definition:

- shorten **Length**
- reduce **Spray**
- use **square** or **saw-like** grain windows for attack
- use a controlled **Scan** position

---

## 3. Build melodies from different layers

arbhar has **6 layers**, each with up to **10 seconds** of audio. This is huge for melodic composition.

You can store:

- different notes
- different timbres
- different chord tones
- different multisamples
- different articulations of the same sound

### Musical strategies

#### A. One note per layer
Load six tuned notes, for example:
- alpha = C
- beta = D
- gamma = E
- delta = G
- epsilon = A
- zeta = C

Then modulate **Layer CV** or turn the layer knob with a sequence. Combined with **1V/Oct**, this becomes very expressive—layer choice changes timbre and register relationships.

#### B. One chord tone per layer
Store:
- root
- third
- fifth
- seventh
- ninth
- suspended tone

Then sequence the layer selection to generate harmonic melodies and arpeggios.

#### C. One articulation per layer
Put the same note in six forms:
- pluck
- bowed
- breathy
- noisy
- reversed
- percussive

Now the melodic line stays harmonically coherent while timbre evolves.

### Omega mode for melodic scanning
The manual notes that with the layer knob fully clockwise, **omega** links all layers consecutively and makes them available via **Scan**. This means you can effectively create a **longer composite phrase/sample map** across all six layers.

That opens up:

- melodic phrase scanning
- wavesequencing-style movement
- long evolving multisample playback
- CV-addressed phrase composition

---

## 4. Use Scan as a melodic selector

The **Scan** knob sets grain position in the layer. This is one of arbhar’s strongest melodic tools because different parts of a recorded sound often contain different pitch and harmonic density.

### Example uses

#### A. Scan a vocal sample
Different vowel regions produce different perceived pitches/formants. Sequencing or slowly modulating Scan creates singing melodic material.

#### B. Scan a recorded instrument note
The attack, sustain, and decay portions all behave differently when granulated:
- attack = bright/percussive
- sustain = stable pitch
- decay = airy/fragile

That means Scan can act almost like a **timbre address** for melodic notes.

#### C. Scan across a recorded phrase
If you record or import a melody, then use Scan to freeze and re-articulate particular moments, you can create:
- melodic rearrangements
- glitch arpeggios
- harmonized fragments
- pseudo time-stretched hooks

### Melodic advice
For more intelligible melody:
- keep **Spray** low to medium
- use **Scan CV** from a sequencer, envelope, or stepped random
- use **Track and Hold mode** if you want changes to happen only on release for precise staging

---

## 5. Follow Mode turns arbhar into a pitchable phrase player

The manual’s **Follow Mode** is especially important for melodic work.

In **Scan Mode**, you freeze/select positions.
In **Follow Mode**, playback progresses internally and **Scan becomes speed control**.

This means arbhar can separate:
- **playback speed**
- **pitch transposition**

That is a major melodic advantage.

### Why it matters
Normally, sampling-style playback ties speed and pitch together. arbhar can decouple them, so you can:

- keep phrase contour while transposing
- slow down or speed up a loop without conventional pitch shift behavior
- create melody from recorded phrases while retaining gesture

### Melodic patch ideas

#### A. Recorded phrase transposer
- Record a melodic riff
- Switch to **Follow Mode**
- Trigger playback with **Strike** or **Capture**
- Sequence **1V/Oct**
- Use **Scan** to alter phrase speed/direction

This creates pitch-shifted phrase melodies that can stay musically locked to a track while being rhythmically fluid.

#### B. One-shot granular lead
Disable Follow looping in preset configuration if desired, then trigger short one-shot phrase playback and transpose each trigger.

#### C. Loop-window melody
The manual says **Hold** can set loop length in Follow Mode. Use short loop lengths on tonal material and sequence pitch CV for wavetable-like or microsample-like melodies.

---

## 6. Wavetable Mode makes arbhar a true melodic oscillator

One of the clearest melodic uses in the manual is **Wavetable Mode**.

Turning **Length fully anticlockwise** crossfades into Wavetable Mode, where arbhar derives a single-cycle waveform from recorded content. This is no longer just granular playback in the usual sense—it becomes an oscillator voice sourced from your sample material.

### Why this is powerful
You can:
- record any acoustic or synthetic sound
- extract single-cycle behavior from it
- play it melodically with **1V/Oct**
- move through timbres via **Scan** and **Spray**

The manual notes:
- center pitch is calibrated to **C** with Pitch at center
- **Pitch Deviation** still works
- **Scan/Spray** choose where in the layer the wavetable is derived
- **Grain Direction** influences interpolation speed between wavetables
- **Strike** can trigger accented notes when continuous oscillation is disabled

### Musical applications

#### A. Custom wavetable lead
Record a vocal, bell, or synth chord.
Enter Wavetable Mode.
Sequence 1V/Oct.
Use Scan for timbre animation.

#### B. Bass voice
Use a lower wavetable center frequency preset or keep default and transpose down.
Reduce modulation and Spray for stability.

#### C. Morphing pad melody
Keep continuous oscillation on.
Modulate Scan slowly.
Sequence pitch CV.
Result: a harmonically alive drone or lead.

This may be the most conventionally “melodic synth voice” role arbhar can play.

---

## 7. Quantized Pitch Deviation can generate harmonies and melodic variation

The **Pitch Deviation** control is especially useful for making melody less static.

According to the manual:

- center = no deviation
- anticlockwise = unquantized random pitch deviation
- clockwise = **quantized random pitch deviation**
- deviation is chosen per grain

This means arbhar can generate harmonized or aleatoric melodies around a central note.

### Useful melodic applications

#### A. Trills and ornamentation
With modest clockwise pitch deviation and shorter grains, each triggered event may branch into intervallic motion around the base pitch.

#### B. Chord-cloud melody
Feed a melodic sequence into **1V/Oct**, then add quantized pitch deviation. Each grain may choose intervals around the played note, creating:
- harmonized leads
- clustered chords
- shimmering triadic textures
- generative arpeggios

#### C. Scale-like probabilistic melodies
The default tables are interval-based, but the manual says the quantized table can be customized in `preset.txt`. That means you can define interval sets that behave more like:
- octaves
- triads
- modal degrees
- symmetric scales

So arbhar can become a **probability harmony engine**.

---

## 8. The Intensity control changes melodic density

For melody, **Intensity** is not just “more grains.” It determines how dense and legible the note material is.

### Lower intensity
- clearer individual grains
- more rhythmic articulation
- useful for plucks and pointillistic melody

### Center/high density
- thicker sustained notes
- clustered harmony
- choir/string-like melodic clouds

### Extreme positions
The continuous engine disables, letting you use only **Strike** for more note-like performance.

This is often ideal when you want arbhar to sit in a track as an actual melodic line instead of a texture wash.

---

## 9. Grain window shapes change note articulation

The **Grain Window** knob shapes how notes feel.

From the manual:
- center = **Gaussian**
- anticlockwise = **square**
- clockwise = **descending sawtooth**

### Melodic implications

#### Gaussian
Best for:
- pads
- legato leads
- sustained drones
- smooth melodic overlays

#### Square
Best for:
- loop-like tones
- chopped phrases
- more abrupt note edges
- rhythmic melodic cells

#### Descending saw
Best for:
- plucks
- percussive notes
- pseudo-envelope articulation
- sequenced melodic hits

If you want arbhar to play “notes,” grain window choice matters as much as pitch.

---

## 10. Grain direction can create melodic call-and-response

The **Grain Direction** probability determines whether grains play forward or reverse.

This is not just a textural parameter. On melodic material, it changes articulation and contour.

### Uses
- Mostly forward for clear melody
- Mixed forward/reverse for ornamented phrases
- Mostly reverse for swelling, uncanny lead lines

If your source audio includes a melodic phrase or a transient-rich note, reversing grains creates ghost notes and inhale-like attacks—great for ambient melodies.

---

## 11. Onset detection can harvest melodic material automatically

arbhar’s **Onset Input** and onset detection can trigger recording based on attacks in incoming audio.

This is very useful for building melodic systems from external instruments:
- piano
- guitar
- voice
- plucked strings
- percussion with pitch

### Patch idea: live melodic granulator
- Feed a melodic instrument into arbhar
- Set onset mode to trigger recording automatically
- Let arbhar capture each new event
- Sequence 1V/Oct or strike grains from captured material

Now your played instrument becomes the sound source for a new granular melodic voice.

### Another technique
Use **Pulse Out** derived from onset or grain generation to trigger other melodic modules in sync. Even though the user asked about these modules together, with just arbhar plus its expansion, you can still create a self-derived clocking relationship:
- arbhar detects note attacks
- outputs triggers
- those triggers can retrigger arbhar’s own capture or external sequencers/quantizers

That makes it possible to build reactive melodic ecosystems around incoming audio.

---

## 12. Accumulative capture is great for melodic collaging

The manual’s **Accumulative Capture Mode** is extremely musical.

Instead of replacing the layer from the start every time, you can keep filling different parts of a layer with successive recordings.

### Melodic uses
Record:
- note 1 into one spot
- note 2 into another
- note 3 into another

Then scan through the curated layer to access a hand-built melodic sample map.

This is excellent for:
- building phrases from separate notes
- vocal syllable melodies
- custom multisampling
- assembling tuned loop points

If you then use **Scan CV** or **Follow Mode**, the layer becomes a custom melodic timeline.

---

## 13. Use imported audio to create tuned melodic banks

The USB functions let you load layers or full scenes from `_arbhar_library` and `_arbhar_scenes`.

This matters melodically because you can prepare:
- multisampled notes
- tuned chord sets
- phrase fragments
- scale-degree recordings
- song-specific timbres

### Smart preparation ideas

#### A. 6-note scale bank
One note per layer from a scale.

#### B. 6 chord bank
Each layer contains a different chord stab.

#### C. 6 phrase bank
Each layer contains a different melodic motif.

#### D. 6 wavetable-source bank
Each layer contains a timbrally rich steady-state sound ideal for Wavetable Mode.

Then during performance:
- choose layers manually
- sequence Layer CV
- switch to omega to sweep the whole set

This gives arbhar a role similar to a melodic phrase module or sample-based oscillator bank.

---

## 14. Stereo input can preserve harmonic information

The manual notes **Stereo Input Mode** uses:
- Input = left
- Onset Input = right

For melodic sampling, this matters when recording:
- stereo synth patches
- piano
- field recordings with tonal width
- chorus-heavy sources

Because arbhar can also perform stereo granular output behavior, stereo source material can make melodic layers feel wider and more harmonically immersive.

For conventional melodic use:
- use **phase-corrected** output mode when working stereo
- consider reverb/delay Mod CV modes for spacious melodic results

---

## 15. Mod CV modes support melody through spatial and temporal shaping

The **Mod CV input** can target:
- panning
- hold
- reverb
- feedback/delay

These are not directly pitch controls, but they strongly affect melodic presentation.

### Reverb mode
Excellent for:
- sustained lead bloom
- frozen harmonic pads
- melodic ambience

### Delay mode
Excellent for:
- echoing arpeggios
- Karplus-like pitched shimmer
- rhythmic melodic feedback

### Hold mode
In Follow Mode, this affects loop length. That means it becomes a **melodic phrase-length control**.

### Panning mode
Useful for stereo melodic animation, especially with dense grain clouds.

---

## 16. Practical melodic patch recipes

## Patch 1: Granular lead voice
**Goal:** playable melodic line

- Record a stable pitched tone into one layer
- Set **Spray** low
- Set **Length** short-medium
- Set **Intensity** to an extreme so only Strike engine is used
- Sequencer CV → **1V/Oct**
- Trigger sequencer → **Strike**
- Grain Window → slightly clockwise for plucky articulation
- Dry/Wet fully wet

**Result:** articulate granular notes from sampled material

---

## Patch 2: Harmonized melody cloud
**Goal:** melody plus chord shimmer

- Record a vocal or synth tone
- Sequencer → **1V/Oct**
- Moderate **Intensity**
- Medium-long **Length**
- **Pitch Deviation** clockwise for quantized intervals
- Gaussian window
- Low-medium Spray

**Result:** each note blooms into harmonized grains around the played pitch

---

## Patch 3: Phrase-based arpeggiator
**Goal:** melodic rearrangement from recorded material

- Record a melodic phrase
- Use **Scan Mode**
- Clocked stepped CV into **Scan CV**
- Trigger **Strike** from rhythm source
- Set **Length** short
- Set **Spray** low
- Add pitch CV to transpose globally

**Result:** different slices of the phrase become a resequenced melody

---

## Patch 4: Follow Mode tape-melody engine
**Goal:** independent pitch and phrase speed

- Record a riff
- Enter **Follow Mode**
- Trigger playback with **Strike**
- Sequencer → **1V/Oct**
- Use **Scan** as speed/direction
- Use **Hold** to define loop length
- Optional Mod CV = Hold for animated loop size

**Result:** transposable phrase playback with unusual temporal elasticity

---

## Patch 5: Wavetable synth line
**Goal:** use arbhar as oscillator

- Record/import harmonically rich audio
- Turn **Length** fully anticlockwise into **Wavetable Mode**
- Sequencer → **1V/Oct**
- Set **Intensity** for continuous tone or disable for triggered notes
- Modulate **Scan** slowly
- Use **Pitch Deviation** for interval variation if desired

**Result:** custom wavetable lead or bass voice

---

## Patch 6: Melodic collage instrument
**Goal:** hand-built phrase bank

- Enable **Accumulative Capture Mode**
- Record separate notes/syllables into different positions in one layer
- Use **Scan** or **Scan CV** to address these zones
- Trigger with Strike
- Transpose with 1V/Oct

**Result:** a custom granular keyboard made from your own note fragments

---

## 17. Best source types for different melodic roles

### For clear leads
- flute
- sine or triangle waves
- whistling
- single vocal vowel
- filtered saw

### For pads/chords
- choir
- bowed strings
- sustained synth chords
- organ
- field recordings with tonal content

### For plucks and pointillistic melody
- kalimba
- piano attacks
- guitar plucks
- muted strings
- mallets

### For wavetable mode
- harmonically rich steady tones
- vocal sustains
- synth chords
- resonant percussion tails

---

## 18. Performance advice as a Eurorack musician

From a musical standpoint, arbhar works best melodically when you decide which of these three roles it is playing:

### 1. Note voice
Use Strike, low Spray, shorter Length, stable Scan, 1V/Oct.

### 2. Phrase voice
Use Scan or Follow Mode, longer recordings, transposition, rhythmic triggering.

### 3. Harmonic texture voice
Use continuous grains, moderate intensity, quantized pitch deviation, reverb/delay.

Trying to do all three at once can sound beautiful, but if you want the melody to read clearly in a mix, choose one role first.

---

## 19. Most powerful melodic features in arbhar

If I were using arbhar specifically for melodic composition, the most important features from this manual would be:

1. **1V/Oct control**
2. **Strike-triggered grains**
3. **Quantized Pitch Deviation**
4. **Layer-based sample organization**
5. **Omega scanning across all layers**
6. **Follow Mode with independent speed behavior**
7. **Wavetable Mode**
8. **Accumulative Capture Mode for hand-built phrase maps**

Together, those make arbhar much more than a texture processor—it can genuinely become a **melodic voice and compositional instrument**.

## Conclusion

The arbhar is best understood melodically as a hybrid of:

- sampler
- granular synth
- wavetable oscillator
- phrase looper
- harmonic randomizer

It can create melodic material in several distinct ways:

- **play notes from captured audio**
- **transpose and articulate grains via Strike and 1V/Oct**
- **scan through recorded melodic fragments**
- **create harmonized lines using quantized pitch deviation**
- **play time-flexible phrases in Follow Mode**
- **become a custom wavetable synth in Wavetable Mode**
- **assemble melodic collages with accumulative recording and layers**

If you patch it with a sequencer, pitch CV source, and triggers, arbhar can function as a surprisingly expressive **melodic instrument**, not just a sound mangler.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)