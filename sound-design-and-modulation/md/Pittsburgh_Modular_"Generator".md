# Pittsburgh Modular — "Generator"

- [Manual PDF](../../manuals/Generator - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF / source](https://pittsburghmodular.com/generator)

# Pittsburgh Modular Generator: modulation ideas and patch strategies

The **Pittsburgh Modular Generator** is basically a compact **2-oscillator FM voice** built for unstable, aggressive, non-1V/oct, wide-range sound design. From the manual:

- **Two triangle-core oscillators**
- **Generator 2 is internally FM’d by Generator 1’s Index Out**
- **External FM input** can be routed to modulate either **Gen 1 or Gen 2**
- **Shape knob** morphs both oscillators in opposite directions:
  - Gen 1: square → triangle
  - Gen 2: triangle → square
- **Index section** is a VCA on **Generator 1 output**, and that VCA output is also the internal FM source for Gen 2
- **Index pot behavior is inverted**:
  - full left = 100% gain
  - full right = 0% gain
- External FM attenuverter:
  - full left = inverted FM
  - noon = 0
  - full right = positive FM

This means the module shines when you think of it less like a “precise dual VCO” and more like a **chaotic FM percussion/bass laboratory**.

---

## Important behavior to exploit

## 1. Internal FM is tied to the Index section
Because **Gen 1’s Index Out** is internally routed to FM **Gen 2**, the **Index pot** and **Index CV input** are major performance controls.

Practical result:

- If you modulate **Index CV**, you are dynamically changing:
  - the audible level at **Index Out**
  - the amount of **internal FM sent from Gen 1 to Gen 2**

That is the main source of movement for:
- metallic percussion
- tearing bass attacks
- animated drones/pads

---

## 2. External FM routing makes the module semi-feedback friendly
The **External input** can be routed to modulate:
- **Gen 1** when switch is up
- **Gen 2** when switch is down

This allows:
- Gen 2 → FM Gen 1
- another module → FM either oscillator
- self-patching from one output into the FM input
- pseudo-feedback patches using mixers/VCAs/filters

This is where the most extreme sounds live.

---

## 3. The Shape knob is a hidden timbre macro
Because the waveforms of the two oscillators move in opposite directions, the **Shape knob** changes both:
- harmonic content
- FM character
- how sharply the oscillators “bite” each other

Use it like a **macro timbre control** rather than just a waveform selector.

---

# General modulation techniques that work especially well

## A. Envelope to Index CV
This is the first thing to patch for impact.

Why:
- it creates a **dynamic FM amount**
- it shapes attack brightness and aggression
- it can make sounds start noisy/metallic and settle into pitch

Try:
- short decay for kicks, snares, zaps
- medium decay for bass growl
- long attack/release for evolving pads

---

## B. Audio-rate cross modulation
Patch one oscillator output into the **External input** and route it to the other oscillator.

Examples:
- **2 → External In**, route to **Gen 1**
- **1 or Index Out → external processor/VCA → External In**, route to **Gen 2**

This creates:
- clangorous percussion
- distorted bass textures
- unstable digital-sounding sidebands
- “ripping zipper” tones mentioned in the manual

---

## C. Slow CV to Shape
Even though there’s no dedicated Shape CV in the manual, you can still perform it manually or use adjacent system tools to animate the output after the module. But if you’re playing live, the **Shape knob** is one of the best movement controls.

Good uses:
- square-heavy settings for more edge and impact
- triangle-heavy settings for softer, hollow, pad-like tones
- subtle movement around the center for evolving timbre

---

## D. Inverted FM with the attenuverter
The external FM attenuverter is extremely useful.

Try both:
- positive FM
- negative/inverted FM

Inverted modulation often gives:
- different attack behavior
- asymmetrical bass motion
- “inside-out” sounding timbres
- more complex percussion transients

---

## E. Use the range switches as a compositional tool
Each oscillator has:
- Low
- Mid
- High

Interesting combinations:
- **Gen 1 low / Gen 2 mid** = percussion, kicks, snapping bass
- **Gen 1 low / Gen 2 high** = broken digital artifacts, neuro bass textures
- **Gen 1 mid / Gen 2 low** = wobbling unstable sub with noisy overtone movement
- **Both high** = metallic, alias-like, insect, scream, lead tones
- **Both low** = chugging LFO/audio-borderline chaos, horror drones

---

# Distorted percussive sound design

The Generator is naturally excellent at **FM percussion**, especially because the internal FM depth can be hit by an envelope.

## 1. FM kick drum
Patch:
- Listen to **Index Out**
- Set **Gen 1 range = low**
- Set **Gen 2 range = low or mid**
- Patch **envelope → Index CV**
- Keep **Index pot** toward the side that gives strong gain (full left = max)
- Tune Gen 1 lower for body
- Tune Gen 2 slightly higher for attack click/knock
- Use Shape toward more triangle for rounder body, more square for harder punch

What happens:
- envelope opens Gen 1 VCA and increases FM into Gen 2
- attack gets brighter and more distorted
- decay settles into a lower thump

For more distortion:
- patch **Gen 2 out → External input**
- route external FM to **Gen 1**
- raise external FM amount carefully

Result:
- gabber-style kicks
- industrial thumps
- broken-machine toms

---

## 2. Snare / metallic hit
Patch:
- **Gen 1 range = low or mid**
- **Gen 2 range = high**
- **Envelope → Index CV**
- **Gen 2 output → External input**
- Route external FM to **Gen 1**
- Turn FM attenuverter to a moderate positive or negative amount
- Listen to **2** or **Index Out**

Tuning:
- Gen 1 provides body
- Gen 2 in high range provides noisy metallic shell

For sharper results:
- use more square content with Shape
- use very short envelope decay

This can produce:
- electro snares
- laser toms
- metallic knocks
- broken arcade percussion

---

## 3. Zap / laser percussion
Patch:
- Both oscillators in **mid or high**
- Patch a fast envelope to **Index CV**
- Route **Gen 2 → External input → Gen 1**
- Sweep one frequency knob while triggering

Best trick:
- start with low external FM, then increase until pitch starts smearing

This gives:
- old-school sci-fi zaps
- drum’n’bass fill hits
- “Nintendo zipper” sounds the manual hints at

---

## 4. Dirty FM hi-hats / ticks
Patch:
- Both oscillators **high**
- Shape toward square-heavy tones
- Short envelope to Index CV
- Listen to **2** or **Index Out**
- Optionally patch **Gen 1 output → external VCA/filter** for additional shaping

Try tuning the oscillators non-harmonically:
- not octave-related
- not fifth-related
- awkward intervals give more noisy metallic splatter

This yields:
- brittle hats
- glitch ticks
- harsh industrial tops

---

# Crazy basslines for dubstep / drum and bass

This module is not intended as a perfect tracking bass oscillator, but it is fantastic for **resampled, dirty, animated bass design**.

## Core bass principle
Use:
- one oscillator as the low fundamental
- the other as a moving FM aggressor
- Index CV for timed bursts of timbral violence

---

## 1. Reese-adjacent FM bass
Patch:
- **Gen 1 range = low**
- **Gen 2 range = mid**
- Listen to **2** for the more FM-affected voice
- Patch **slow/moderate envelope or LFO → Index CV**
- Patch **Gen 2 → External input**, route to **Gen 1**
- Use small to medium external FM amount
- Tune Gen 2 slightly detuned from a harmonic ratio

Why it works:
- internal FM from Gen 1 to Gen 2 creates movement
- external cross-modulation back into Gen 1 adds instability
- slight tuning offsets generate animated growl

For more dubstep:
- run output into a lowpass or bandpass filter with additional modulation
- automate Shape by hand while recording
- resample several passes

---

## 2. Neuro / talking bass source
Patch:
- **Gen 1 low**
- **Gen 2 high or mid**
- Listen to **2**
- Strong **envelope to Index CV**
- **Gen 2 output → External input**
- Route external FM to **Gen 1**
- Turn attenuverter negative, then compare with positive
- Set Shape near center and wiggle it manually

This creates:
- vowel-like FM shifts
- tearing attacks
- phasey vocal overtones

To push further:
- mult output to waveshaper, filter, phaser, or comb filter
- automate post-processing with synced LFOs

The Generator itself supplies the raw complex motion; your downstream modules turn it into full-on neuro funk.

---

## 3. Sub + tear bass
Patch:
- Use **Gen 1** as the sub-ish source
- Set **Gen 1 low**, shape closer to triangle
- Set **Gen 2 mid/high**
- Keep internal FM moderate with Index settings
- Use **Envelope → Index CV** for attack only
- Listen to:
  - **1** for cleaner source
  - **2** for more shredded version
  - **Index Out** for dynamic aggressive contour

Best workflow:
- split outputs and layer them externally:
  - **1** = sub/body
  - **2 or Index Out** = growl layer

This is especially good for:
- drum and bass stabs
- modulated one-shot basses
- fill transitions

---

## 4. Machine-gun bass sequence
Patch:
- Sequence pitch loosely through **EXP input**, but don’t expect precise melodic tracking
- Use short-decay envelope to **Index CV**
- Set **Gen 1 low**, **Gen 2 mid**
- Add **Gen 2 → External FM → Gen 1**
- Tune by ear per pattern, not by keyboard intervals

Important note:
Because the manual states it **does not track 1V/oct and is not temp compensated**, this works best for:
- short riffs
- one-note bass patterns
- manually tuned sequences
- hostile techno/dnb phrasing

This can sound huge if clocked tightly and fed into:
- VCA
- envelope
- lowpass filter
- saturation/compression

---

## 5. Wobble bass with FM grit
Patch:
- Build your bass tone on **2**
- Moderate internal FM using Index
- Put output through a filter
- Modulate the filter with an LFO
- At the same time, modulate **Index CV** with a second slower envelope/LFO

Why:
- filter movement gives the expected wobble
- FM-index movement adds internal animation
- the result is less static than a normal subtractive wobble patch

Try:
- lowpass wobble + subtle Index modulation = modern dubstep
- bandpass wobble + stronger Index modulation = screaming DnB lead bass

---

# Haunting atmospheric pads and drones

Generator can do pads, but not in a classic “stable polysynth oscillator” way. Think:
- unstable haunted organ
- metallic fog
- cold sci-fi choir
- detuned dread ambience

The magic is **slow movement** and **gentle FM**, not maximum brutality.

## 1. Hollow drifting drone
Patch:
- Set both oscillators to **low or mid**
- Keep frequencies close but not identical
- Use minimal internal FM at first
- Listen to **1** and **2** separately, or mix externally
- Set Shape toward more triangle content
- Slowly increase Index until overtones begin to bloom

What to modulate:
- slow LFO to **Index CV**
- manually sweep frequency knobs a tiny amount
- occasional external FM from another slow oscillator

Result:
- shifting organ-like drone
- eerie chorusing through non-precise tuning
- unstable spectral bloom

---

## 2. Ghost pad with slow FM breathing
Patch:
- **Gen 1 low**
- **Gen 2 mid**
- Long attack/long release envelope to **Index CV**
- Listen to **Index Out** and/or **2**
- Keep external FM low
- Shape near center or triangle-leaning

Behavior:
- sound opens gradually into complexity
- sidebands bloom during attack
- release falls back into a hollow core tone

Best with:
- reverb
- delay
- lowpass gate or VCA after the module

This makes beautiful:
- dark ambient beds
- soundtrack tension drones
- haunted intro pads

---

## 3. Dissonant metallic cloud
Patch:
- Both oscillators in **mid**
- Tune to a dissonant interval
- Use **Gen 2 → External input**
- Route to **Gen 1**
- Keep both internal and external FM modest
- Slowly move Shape during performance

Tip:
The sweet spot is just before the sound turns fully abrasive.

This produces:
- bell-like haze
- rusted choir tones
- frozen-air metallic ambience

Add:
- shimmer reverb
- granular delay
- stereo filtering

---

## 4. Pulsing cinematic atmosphere
Patch:
- Long cycling envelope or slow LFO to **Index CV**
- Another slow CV source to an external VCA/filter after the module
- Set **Gen 1 low**, **Gen 2 low or mid**
- Use **1** for a more stable component, **2** for unstable harmonics
- Mix both externally

This layered approach works very well:
- **1** = body
- **2** = moving spectral layer
- **Index Out** = animated transient/wash layer

Blend to taste and drown in reverb.

---

# Best self-patching ideas

## 1. Gen 2 into external FM for Gen 1
This is the most immediate “go crazy” patch.

Patch:
- **2 → External input**
- Route switch **up** to Gen 1
- Use attenuverter to set amount/polarity

Sound:
- violent cross-FM
- sharp percussion
- growling bass
- unstable drones

---

## 2. Use Index Out as the main audio output
A lot of the personality lives here.

Because Index Out is post-VCA and tied to internal FM behavior, it often feels more alive than the plain oscillator outputs.

Use when you want:
- dynamic percussion
- animated bass attacks
- envelope-shaped timbre shifts

---

## 3. Layer 1 and 2 externally
Take:
- **1** = cleaner/rawer Generator 1 before index VCA
- **2** = Generator 2, already influenced by internal FM
- **Index Out** = dynamic processed Gen 1

Mixing these externally gives a much bigger sound than using only one output.

Great for:
- bass layering
- drone stacks
- parallel distortion/filtering

---

# Sweet spots by genre

## For distorted percussion
- Gen 1: low
- Gen 2: mid/high
- Envelope to Index CV
- Gen 2 into External FM to Gen 1
- Shape toward square-ish
- Listen to Index Out or 2

## For dubstep / DnB bass
- Gen 1: low
- Gen 2: mid
- Moderate to strong Index modulation
- Cross-FM via External input
- Post-process with filter and saturation
- Layer 1 and 2 for sub + aggression

## For haunting pads
- Both low/mid
- Triangle-leaning Shape
- Low to moderate FM
- Slow Index CV modulation
- Subtle detuning
- Heavy reverb/delay afterward

---

# A few concrete patch recipes

## Patch 1: Industrial kick
- Gen 1 low
- Gen 2 mid
- Envelope to Index CV
- Listen to Index Out
- 2 → External input, route to Gen 1
- FM attenuverter around 1–2 o’clock
- Shape slightly toward square

## Patch 2: Neuro bass one-shot
- Gen 1 low
- Gen 2 high
- Strong envelope to Index CV
- Listen to 2
- 2 → External input, route to Gen 1
- Try negative FM first
- Record several knob movements of Shape and Gen 2 tuning

## Patch 3: Haunted drone
- Gen 1 low
- Gen 2 low
- Listen to 1 and 2 mixed
- Slow LFO to Index CV
- Minimal external FM
- Shape toward triangle
- Add long reverb

## Patch 4: Metallic snare burst
- Gen 1 mid
- Gen 2 high
- Short envelope to Index CV
- Listen to 2
- Add cross-FM from 2 to Gen 1
- Tune non-harmonically

---

# Final advice

The Generator rewards:
- **envelopes into Index CV**
- **self-patching with External FM**
- **non-harmonic tuning**
- **manual performance on Shape and frequency**
- **layering multiple outputs**

It is less about precise tonal FM and more about **alive, unstable, aggressive motion**. For your goals:

- **distorted percussion:** use short envelopes and hard cross-FM
- **dubstep / DnB bass:** use Gen 1 as low body, Gen 2 as tearing modulator, and animate Index
- **haunting pads:** back off FM, use slow Index movement, detune slightly, and lean on triangle shapes and effects

If you want, I can also turn this into:
1. a **quick-start cheat sheet**,  
2. a **set of 10 named patches**, or  
3. a **rack-aware patch plan** if you tell me what other modules you have.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)