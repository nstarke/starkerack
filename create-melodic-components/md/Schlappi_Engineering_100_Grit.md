# Schlappi Engineering — 100 Grit

- [Manual PDF](../../manuals/100_GRIT_MANUAL_20190826.pdf)

---

[100 Grit Manual PDF](attachment)

# Using Schlappi Engineering 100 Grit for Melodic Music

The **Schlappi Engineering 100 Grit** is often described as a touch-controlled distortion/filter/performance instrument, but it can absolutely be used to create **melodic material**, not just noise and destruction. From the manual, the key melodic building blocks are:

- a **low pass transistor ladder filter**
- a **VCA**
- a **distortion stage**
- **filter FM inputs**
- **resonance behavior that can approach self-oscillation**
- **touch points** that act like resistive patch points into circuit nodes
- several **internal feedback normalizations** that can turn the module into a playable voice or animated processor

Because this manual only covers **one module**, the most useful way to answer your question is to explain how the **different sections of the 100 Grit work together** to produce melodic components such as:

- tuned filter pings
- basslines
- distorted leads
- FM-like tones
- self-oscillating sine-ish melodic voices
- animated harmonics that follow pitch CV

---

## What in 100 Grit is useful for melody?

## 1. Filter as the pitch-bearing core
The manual says:

- **FM1 and FM2 sum together and control the cutoff frequency**
- **FM2** can be used for **V/OCT CV to roughly track along with incoming signal**
- the filter can be trimmed so resonance **just starts to self-oscillate**

This means the filter is not just a tone shaper — it can become a **quasi-oscillator** or at least a **pitch-emphasizing resonant core**.

### Melodic implications
- Send **1V/oct or sequencer pitch CV** into **FM2**
- Raise **RES**
- Tune **FREQUENCY** to the desired range
- Use **OUT** for cleaner melodic material or **DIST** for a more aggressive voice

This likely won’t behave like a precision oscillator, but it can produce:
- rough melodic tracking
- tuned resonant notes
- acid-like lines
- screaming leads with recognizable pitch centers

---

## 2. VCA lets envelopes articulate notes
The manual is clear that:

- **GAIN controls the gain of the VCA**
- **No sound will come out of either output without some initial gain**
- **5V at GAIN CV gives unity gain**
- you can use **GAIN CV** as a normal VCA control input

### Melodic implications
A VCA is one of the main things needed to turn a continuous tone into a **note phrase**.

Use:
- envelope to **GAIN CV**
- pitch CV to **FM2**
- gate/trigger to your envelope generator
- output from **OUT** or **DIST**

This gives you a standard melodic voice structure:
**pitch CV → FM2**  
**envelope → GAIN CV**  
**audio source or self-oscillation → audio path**

So even though 100 Grit is wild, it can still function as a classic **articulated mono synth voice**.

---

## 3. Resonance can make tones sing or self-oscillate
The resonance section is especially important melodically.

From the manual:
- **RES controls resonance**
- **RES CV** can modulate resonance
- internal resonance trim can be set so the filter **just starts to self-oscillate**
- removing the **Input to Resonance header (J9)** changes the character and allows self-oscillation to overtake the input signal more strongly

### Melodic implications
This enables at least three melodic uses:

#### A. Resonant filtering of an existing oscillator
Patch an oscillator into **IN1** and use:
- **FM2** for pitch-related movement if desired
- **RES** to emphasize harmonics
- **GAIN CV** for note articulation

This yields strong melodic bass/lead processing.

#### B. Filter ping voice
With high resonance and short envelopes into frequency or gain, the module can behave like a **pinged resonant filter**, producing percussive but pitched notes.

#### C. Self-oscillating voice
If trimmed appropriately and set for strong resonance, the filter can become a **standalone tone source**. Then:
- sequence **FM2**
- envelope **GAIN CV**
- monitor **OUT**

This is one of the clearest ways to get melody directly from the 100 Grit without another oscillator.

---

## 4. Distortion can preserve melody while adding harmonics
The distortion path is not just chaos. The manual states:
- **DIST** is the output of the distortion circuit following the VCA
- **GAIN** controls how hard distortion is pushed
- the **x100** switch gives extreme distortion

### Melodic implications
For melodic work, distortion helps in two ways:

#### A. Make simple melodic lines more present
A basic sine/triangle/saw into 100 Grit can become:
- thicker bass
- screaming lead
- harmonically rich sequence

#### B. Create pitch-rich resonant tones
When resonance is already near oscillation, the distortion can turn a plain resonant tone into:
- acid basslines
- industrial melodies
- unstable but still trackable solos

For melody, it is often best to start with:
- **x100 off**
- moderate **GAIN**
- moderate **IN1**
- use **OUT** and **DIST** alternately to hear where pitch remains clearest

Then engage **x100** once the line is established.

---

## Internal interactions that matter for melodic patching

## 5. Normalizations can animate a melodic voice
One of the most interesting features in the manual is that **unused inputs have internal feedback normalizations**. These can make a melodic patch much more alive.

Key normalizations:

- **IN1 normalled to DIST2**
- **IN2 normalled to DIST**
- **FM1 normalled to DIST**
- **GAIN CV normalled to POLE 2**
- **RES CV normalled to DIST**

These are active only when the input is **unpatched**, and the associated control must be turned down if you do not want its effect.

### Melodic use of each normalization

#### IN2 ← DIST
The manual says this acts as a **distorted resonance path in opposition to RES**.

Use this for:
- more vocal melodic tones
- unstable harmonic emphasis on basslines
- snarling leads

With a pitched input, this can add motion without losing the basic note.

#### FM1 ← DIST
The manual says this applies the distortion output as dynamic frequency modulation.

Use this carefully for:
- metallic melodic lines
- laser-bass sequences
- aggressive pitch shimmer

For melody, keep FM1 amount low. Too much will smear pitch.

#### GAIN CV ← POLE 2
The manual calls this a relatively subtle form of distortion, shifting harmonic content.

This is one of the most useful melodic features because it creates:
- internal animation tied to the filter
- harmonic movement that follows the note
- a more “alive” tone without fully destroying pitch

Great for:
- basslines
- drones with melodic contour
- sustained leads

#### RES CV ← DIST
This introduces audio-rate modulation of resonance and can make laser sounds and screeches.

For melodic use:
- keep low
- use as accent coloration
- add only on select notes or phrases

This can be very expressive but becomes chaotic quickly.

---

## Touch points as melodic performance controls

The touch points are not only for noise. They expose:
- **DIST 2 OUT**
- **GAIN CV**
- **DIST 2 AMP PIN**
- **RES CV**
- **DIST 1 AMP PIN**
- **FREQ CV**
- **DIST OUT**
- another **GAIN CV**

The manual describes them as **direct resistive connections** to circuit points. You can bridge them with:
- fingers
- patch cable tips
- alligator clips
- conductive materials

### Melodic uses of touch points

## 6. Manual expressive pitch bending
Touching or injecting signal at **FREQ CV** can create:
- vibrato
- bends
- squeals
- expressive pitch movement

This makes 100 Grit act like a playable lead instrument.

## 7. Dynamic timbral articulation
Using:
- **DIST OUT → GAIN CV**
- **DIST 2 OUT → RES CV**
- or finger-bridging adjacent output/input points

you can add phrase-specific changes during a melodic performance.

This is useful for:
- turning sustained notes into expressive gestures
- adding grit at phrase endings
- making repeated notes vary naturally

## 8. Audio-rate modulation for pitched sidebands
The manual notes audio into **FREQ CV**, **GAIN CV**, or **RES CV** can create distortion and AM/FM-like effects.

If the source is pitched and somewhat related to the note being played, you can get:
- clangorous intervals
- quasi-FM melodies
- harmonic enrichment

This works especially well if another oscillator is patched to a touch point while pitch CV sequences the filter.

---

# Practical melodic patch ideas

## Patch 1: Distorted bass voice
This is the most straightforward melodic use.

### Patch
- Oscillator saw/square → **IN1**
- Sequencer pitch CV → oscillator 1V/oct
- Same pitch CV or related CV → **FM2**
- Envelope → **GAIN CV**
- Listen to **OUT** first, then **DIST**

### Settings
- **IN1** around 50–75%
- **FREQUENCY** low to mid
- **RES** around 20–40%
- **GAIN** around 50–75%
- **x100** off initially

### Result
- solid bass articulation
- resonant vowel/growl tone
- controlled harmonic aggression
- notes remain defined

### Why it works
The oscillator provides stable pitch, while 100 Grit adds:
- filtering
- envelope shaping
- saturation
- internal harmonic animation

---

## Patch 2: Self-oscillating lead voice
Use the filter itself as the sound source.

### Patch
- No audio input, or very low audio input
- Pitch CV/sequencer → **FM2**
- Envelope → **GAIN CV**
- Listen to **OUT**
- Raise **RES** until near or at oscillation

### Optional
- use **J9** resonance header behavior if you want more self-oscillation dominance
- add slight **FM1** amount unpatched for internal distortion feedback FM

### Result
- unstable but playable lead tones
- sine-ish to tearing resonant voice
- great for acid, industrial lead lines, eerie melodies

### Notes
The manual only says **roughly track**, so expect:
- character over precision
- best results in narrower melodic ranges
- excellent expressive imperfections

---

## Patch 3: Pinged melodic percussion
This creates tuned percussive notes that can still form melodies.

### Patch
- No sustained input required, or use a very short transient input
- Triggered envelope → **GAIN CV**
- Pitch CV → **FM2**
- High **RES**
- Listen to **OUT**

### Result
- tuned blips
- tom-like notes
- wooden/plucky resonant sounds
- melodic percussion lines

### Enhancement
Use a little **DIST** output to add edge, but not so much that pitch disappears.

---

## Patch 4: Acid-style sequenced line
100 Grit looks especially suited for this.

### Patch
- VCO saw → **IN1**
- Sequencer pitch → VCO
- Envelope or accent CV → **GAIN CV**
- Pitch CV or envelope modulation → **FM2**
- Listen to **DIST** or **OUT**

### Settings
- **RES** medium-high
- **FREQUENCY** fairly open
- **GAIN** high enough to saturate
- **x100** off or momentary on for accents

### Result
- squelchy, aggressive, unstable acid lines
- strong melodic contour
- expressive accents through gain and resonance interaction

### Extra trick
Leave **FM1** unpatched and bring it up slightly so the **DIST-normalled modulation** adds bite and movement.

---

## Patch 5: Harmonic melody shaper for an external oscillator
Instead of making a voice from scratch, use 100 Grit to turn a plain melody into something animated.

### Patch
- Clean VCO/submix → **IN1**
- Melody from sequencer controls oscillator pitch
- Envelope → **GAIN CV**
- Leave **GAIN CV** normalization partially active if useful
- Listen to **OUT** and/or **DIST**

### Result
- melodic line stays recognizable
- harmonics move internally
- can go from warm to brutal without losing sequence identity

This is especially effective if your source oscillator is simple, because 100 Grit can supply much of the personality.

---

## Patch 6: Manual touch-played melodic solo
Use the touch points as performance controls over a sequenced note stream.

### Patch
- Oscillator → **IN1**
- Pitch CV → oscillator and optionally **FM2**
- Envelope → **GAIN CV**
- Listen to **DIST**
- During playback, touch:
  - **DIST OUT** with **FREQ CV**
  - **DIST 2 OUT** with **RES CV**
  - adjacent output/input pairs

### Result
- expressive bends
- phrase-ending shrieks
- manually injected timbral accents
- a playable solo voice rather than static sequence

This is one of the most unique melodic uses of the module.

---

# Which output is better for melody: OUT or DIST?

## OUT
Better for:
- clearer pitch
- filter-based melodic work
- self-oscillation patches
- basslines where note definition matters

## DIST
Better for:
- aggressive leads
- industrial bass
- harmonically dense melodic phrases
- expressive destruction after the note is established

A good strategy is:
1. build the melody on **OUT**
2. switch to **DIST**
3. add x100 or feedback slowly

---

# Headers and their role in melodic behavior

## J9: Input to Resonance
Default is **ON**.

Manual says this:
- maintains bass frequencies
- prevents some classic resonance-related volume loss
- removing it allows more whistling sounds and lets self-oscillation overtake the input

### Melodic use
- **ON**: better for basslines and fuller melodic material
- **OFF**: better for whistling resonant leads and self-oscillating melodic patches

## J10: Output Source
Default is **VCA**

If moved, **OUT** can come directly from the filter rather than post-VCA.

### Melodic use
- **VCA position**: best for articulated notes with envelopes
- **Filter output position**: best if you want continuous filter tone independent of GAIN, or want to use DIST and OUT as two different melodic/timbral taps

---

# Best strategies for making 100 Grit musical instead of random

## 1. Start with stable pitch elsewhere
The easiest way to make 100 Grit melodic is to feed it:
- a tuned VCO
- quantized sequence
- bass drone with pitch center

Then use 100 Grit for articulation and color.

## 2. Add chaos gradually
Because many controls are normalized to feedback sources, it is easy to lose pitch definition. For musical use:
- begin with all secondary controls fully CCW
- add one modulation path at a time
- monitor whether the note center remains audible

## 3. Use FM2 for pitch, FM1 for character
Based on the manual, **FM2** is the better destination for external pitch tracking, while **FM1** is often useful as a character modulation lane due to its distortion normalization.

## 4. Keep distortion after pitch is established
If the melody is disappearing:
- lower **GAIN**
- reduce **IN1**
- use **OUT** instead of **DIST**
- reduce **FM1**
- reduce **RES CV**

## 5. Treat touch points like expressive macros
Rather than using them constantly, use them for:
- fills
- transitions
- accents
- note bends at phrase ends

That keeps the melodic line intelligible.

---

# Best melodic roles for 100 Grit in a system

The manual suggests a module that excels at these melodic jobs:

## Bass voice processor
Probably one of its strongest roles:
- input oscillator
- sequence pitch externally
- use resonance and gain for weight and aggression

## Dirty lead synth
Especially with:
- resonant filter
- rough tracking via FM2
- touch point performance

## Resonant auxiliary voice
Self-oscillation or filter ping patches can act as:
- second melody line
- countermelody
- tuned percussion

## Performance sound design layer
Even if another module provides pitch, 100 Grit can provide:
- expressive harmonic movement
- phrase-level distortion
- live tactile interaction

---

# Summary

The **Schlappi 100 Grit** can create melodic components by combining its sections in a few core ways:

1. **Filter + FM2 + resonance** can act as a rough pitch-bearing voice
2. **GAIN CV** gives note articulation, making it usable like a synth voice
3. **OUT** preserves note clarity; **DIST** adds aggressive harmonic content
4. **Self-oscillation** and **filter pinging** make it capable of generating melody on its own
5. **Feedback normalizations** add animated harmonics and movement that can follow a sequence
6. **Touch points** provide highly expressive manual performance control for bends, modulation, and accents

In practice, the most musical uses are:
- **distorted basslines**
- **acid leads**
- **resonant self-oscillating melodies**
- **pinged tuned percussion**
- **externally pitched melodies made more alive through internal feedback and touch control**

So while 100 Grit is famous for destruction, the manual makes it clear that it is also a very strong **melodic performance processor and semi-voice**, especially when used with pitch CV, envelopes, and careful control of its internal feedback paths.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)