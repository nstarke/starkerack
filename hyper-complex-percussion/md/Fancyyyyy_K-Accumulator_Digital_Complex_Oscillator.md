# Fancyyyyy — K-Accumulator Digital Complex Oscillator

- [Manual PDF](../../manuals/K_ACCUMULATOR_Quickstart_v1.02.pdf)

---

[Manual PDF](https://fancysynthesis.net)

# Using K-ACCUMULATOR for dense rhythmic / hyper-complex percussion

K-ACCUMULATOR is unusually good for percussion because it is not just an oscillator. From the quick-start, it combines:

- a main oscillator with deep internal waveshaping
- a Mod oscillator for PM/XPM relationships
- a UFG function generator that can run sub-audio to audio
- a Δ–∑ pattern generator clocked by the UFG
- a Root/scale system tying pitch relationships together

That means one module can act like:

- sound source
- envelope/pulsar engine
- internal clock
- pattern sequencer
- modulation generator
- pseudo-random variation source

If your goal is **densely rhythmic, polyrhythmic, asymmetrical percussion**, this module wants to be patched as a **self-contained percussion ecosystem** and then externally mixed/processed.

---

## Core idea

For percussion on K-ACCUMULATOR, the most important controls are:

- **Damped/Pulsar**: gives you sync + amplitude modulation from the UFG into the OSC
- **UFG Time / Loop / Trigger modes**: defines rhythmic pulse behavior
- **Δ–∑**: creates stepped or slewed evolving patterns
- **1V/TZ attenuverter on OSC**: lets Δ–∑ become pitch/percussion contour
- **Morph / Shift / Depth / Shape / Stretch**: turns basic hits into metallic, snappy, woody, noisy, tearing, or formant percussion
- **Mod Harmonic / Order / Detune**: controls overtone relations and “struck object” character

The fastest route to percussive complexity is:

1. Put **UFG in sub-audio**
2. Raise **Damped/Pulsar**
3. Use **Δ–∑** to animate oscillator pitch or timbre
4. Use **Morph modes** with PM/XPM for metallic/transient-rich attacks
5. Exploit **different rates and pattern lengths** for internal polyrhythm

---

# 1. Start with a percussion voice

## Basic struck/percussive patch

Start near Centre, then:

- Main sine/cosine outs to stereo mixer
- Set **Stretch, Shift, Depth, Shape low**
- Set **UFG Time** to sub-audio
- Turn up **Damped/Pulsar**
- Put **UFG in Loop** mode

What happens:

- The UFG becomes a repeating pulse/window source
- OSC gets synced and amplitude-modulated by the UFG
- At higher Damped/Pulsar settings, it moves from subtle motion to hard rhythmic gating/sync
- This creates the basis for kick/tom/woodblock/metal hit behavior

### Good starting sound zones
- **FMNT / FBPM**: cleaner struck tones, drum body, toms, claves
- **2OP / XPM**: brighter metallic percussion, zaps, aggro hats
- **Asym**: granular, crispy, pulse-train percussion, great for hats and digital hand percussion
- **FBPM2 / XPM2**: unstable, chaotic, broken-machine percussion

---

# 2. Make the UFG your master rhythm engine

The manual says the UFG is simultaneously:

- main modulation source for OSC
- pulsar window generator
- clock source for Δ–∑

So the first advanced trick is: **think of UFG as your drummer’s hands**.

## Rhythmic functions of UFG

### A. Looping sub-audio pulses
Set:
- **Loop on**
- **Time** in sub-audio
- **Skew** off-center
- **Shape** somewhere between linear and raised cosine

This creates repeating envelopes or pulse trains.

Use:
- **Raised cosine-ish shapes** for rounded hand-drum envelopes
- **Exponential-ish shapes** for sharper attacks
- **Extreme Skew** for asymmetrical attack/decay timing

That asymmetry is important because it creates rhythmic “lean” even before sequencing.

### B. Use trigger response modes for rhythmic behavior
The UFG’s trigger Type cycles through:
- hard sync with subharmonic locking
- sync reversal
- sustain + hard sync
- sustain + sync reversal

These are extremely useful for complex rhythms if you feed the UFG an external clock or trigger stream.

#### Practical uses:
- **Hard sync with subharmonic locking**: stable but strange rhythmic subdivisions
- **Sync reversal**: creates back-spinning envelope motion, ideal for irregular accents
- **Sustain modes**: turn gates into variable-length percussive windows

If you have an external clock source, send it to **UFG Trig** and let the UFG generate a differently-shaped rhythm than the incoming clock.

This is how you get **one pulse stream implying another meter**.

---

# 3. Use Δ–∑ for evolving percussion patterns

The Δ–∑ is the secret weapon for complex rhythm.

Per the manual, it is:

- internally clocked by the UFG
- a stepped/smoothed pattern generator
- non-destructive
- variable in chance, length, and smoothness

This means you can make a loop, destabilize it, then return to it.

## Best percussion use cases for Δ–∑

### A. Pitch sequence into OSC 1V/TZ
Turn up the OSC **1V/TZ attenuverter** so Δ–∑ modulates pitch.

This yields:
- tuned kick/tom sequences
- pseudo-melodic drum lines
- stepped attack transients
- broken electro percussion

If Scale quantization is on, you can get tuned percussion. If not, it gets more raw and drum-machine-like.

### B. Timbre sequence via internal normals
The OSC section says its CV inputs/attenuverters are normalled from either **UFG or Δ–∑**, selectable by the button beside each CV jack.

This is huge.

For each OSC modulation destination:
- **Shift**
- **Depth**
- **Shape**
- **Morph**

you can choose whether the normalled source is:
- **UFG** or
- **Δ–∑**

So you can assign:

- Δ–∑ to **Shape** for changing fold amount step-by-step
- UFG to **Depth** for cyclic transient motion
- Δ–∑ to **Morph** for algorithmic timbre switching
- UFG to **Shift** for repeated harmonic sweep per hit

That means each hit can have:
- its own pitch
- its own timbre
- its own transient profile

without external modulation.

---

# 4. Building polyrhythm from internal mismatches

K-ACCUMULATOR doesn’t advertise “polyrhythm mode” explicitly, but it absolutely supports polyrhythmic thinking because different sections can imply different periodicities.

## Method 1: UFG period vs Δ–∑ pattern length

Since Δ–∑ is clocked by UFG, the simplest route is to change **Δ–∑ Length** while keeping UFG steady.

For example:
- UFG pulse cycle = steady quarter-note-ish clock
- Δ–∑ Length = 5 steps

Now your pitch/timbre pattern cycles every 5 pulses while the pulse engine cycles every 4, 8, or whatever your phrase implies.

This gives:
- 5 over 4
- 5 over 8
- asymmetrical repeating percussion phrases

### Suggested Length settings
- **3 steps** for tresillo-like implied patterning
- **5 steps** for classic rotating asymmetry
- **7 steps** for long “never quite repeating” cycles
- **15 or 16 steps** for larger phrase structures

Because Length zooms into a section of the pattern based on current step, changing it live can create rotating metric illusions.

## Method 2: Mod oscillator harmonic ratios

Set Mod oscillator to track:
- OSC
- UFG
- or Root

Then use **Harmonic** and **Order** to get integer or near-integer relationships.

Examples:
- Mod at 3x or 5x harmonic relation can create spectra that imply different rhythmic densities when used in PM/XPM modes
- Slight detune creates beating that acts like micro-rhythm
- Even/odd harmonic spread changes the “grid feel” of transients

For metallic percussion, these spectral relationships can feel like nested tuplets.

## Method 3: Q.Trig for threshold-derived rhythmic events

The OSC has **Q.Trig**:
> sends a trigger to the UFG each time oscillator frequency crosses a quantizer threshold

This is weird and powerful.

If:
- OSC tracks Root
- a scale is enabled
- pitch is being modulated by Δ–∑ or external CV

then the oscillator crossing scale thresholds can re-trigger UFG activity.

This effectively converts melodic/pitch movement into rhythm.

That means:
- more pitch movement = more trigger density
- scale choice changes where triggers occur
- nonuniform quantized intervals create irregular trigger spacing

This is fantastic for **algorithmic percussion bursts** and **rhythms derived from tuning structure rather than clock divisions**.

---

# 5. Complex time signatures and asymmetrical phrase design

For complex meter, think in layers:

- **UFG** = beat pulse or sub-beat engine
- **Δ–∑ Length** = phrase length
- **Chance** = controlled mutation
- **Pattern edit switch** = manual insertion of accents
- **Morph modulation** = orchestrational variation
- **Scale / Root** = tuned drum framework

## Example: 7/8-ish percussion system

Patch:
- UFG looping in sub-audio as the hit engine
- Damped/Pulsar fairly high
- Δ–∑ to OSC 1V/TZ
- Δ–∑ Length set to **7**
- Smooth low
- Chance near minimum

Result:
- 7-step recurring percussion phrase

Then:
- assign Δ–∑ to **Shape**
- assign UFG to **Depth**
- put Morph around **2OP or XPM**

Now each of the 7 steps has:
- distinct pitch
- distinct fold
- cyclic PM transient behavior

That gets you asymmetrical meter with complex per-step articulation.

## Example: 5 against 4
Use an external 4-pulse bar clock to trigger or sync UFG, but keep Δ–∑ at **Length 5**.

Result:
- hit engine anchored to 4
- internal pitch/timbre cycle rotates every 5

This is a classic polyrhythmic setup.

## Example: 11-step machine groove
- UFG as constant pulse source
- Δ–∑ Length = 11
- Chance low but not zero
- Smooth medium
- Morph CV from Δ–∑ slightly positive
- Shift CV from UFG slightly negative/positive depending taste

You get an 11-hit phrase where:
- pitch steps recur every 11
- timbre slowly transforms
- glides create smeared transitions and flams

---

# 6. Use Chance non-destructively for “controlled breakbeats”

The manual’s Δ–∑ Chance behavior is ideal for evolving percussion:

- at minimum = locked loop
- increasing Chance = progressively injects new values
- returning to minimum restores original pattern

This is gold for live rhythmic mutation.

## Performance strategy
1. Build a tight core groove with Chance at minimum
2. Raise Chance during transitions or fills
3. Lower back to minimum to “snap home” to the original groove

This gives the feeling of:
- fills
- improvisation
- controlled breakage
- return to meter

without losing the underlying pattern.

For hyper-complex percussion, use this as your **fill generator** instead of programming separate fill patterns.

---

# 7. Smooth as glide, filter, and drum smear

Δ–∑ Smooth behaves differently depending on rate:

- sub-audio: glide between steps
- audio-rate: filtering / limiting of value changes

For percussion, this is useful in several ways.

## Low Smooth
- crisp stepped drum pitches
- strong attack identity
- machine-like sequencing

## Medium Smooth
- bends between hits
- talking drum / electro tom feel
- slurred percussion lines
- pseudo-flams when driving PM-related parameters

## High Smooth
- less distinct step changes
- more continuous modulation
- useful when driving Morph/Shape for swarming percussion textures

At audio-ish modulation rates, Smooth can produce filtered-control behavior that makes fast patterns less clicky and more liquid.

---

# 8. Best Morph modes for percussion

## FMNT
Good for:
- formant toms
- vocal-ish congas
- tuned hand percussion
- soft but articulate attacks

Use:
- Depth for bandwidth/body
- Shape for damping feel
- Shift for harmonic emphasis

## FBPM
Good for:
- kicks
- toms
- woodblock-ish attacks
- sine-to-saw drum tone sweeps

Use:
- Depth for body distortion
- Shape for extra fold edge
- Stretch for harmonic separation

## 2OP
Good for:
- metallic percussion
- digital claves
- bells
- struck membrane + overtone interaction

## XPM
Good for:
- aggressive industrial hits
- clangs
- high-density metallic patterns
- unstable upper transients

## Asym
Good for:
- hats
- ticks
- crisp digital percussion
- grainy attacks
- sparse pulse-train clusters

## FBPM2 / 2OP2 / XPM2
Good for:
- broken machine patterns
- chaotic fills
- unstable subharmonic percussion
- very animated transient structures

If you want “hyper complex percussion,” spend a lot of time in:
- **Asym**
- **XPM**
- **XPM2**
- **FBPM2**

---

# 9. Patches for specific rhythmic goals

## Patch 1: Rotating metallic 5-over-4 percussion

**Goal:** polyrhythmic metallic line

- UFG in Loop, sub-audio
- Damped/Pulsar at 60–80%
- Morph at **2OP** or **XPM**
- OSC 1V/TZ attenuverter up, using Δ–∑ normal
- Δ–∑ Length = 5
- Chance very low
- Smooth low
- Mod tracks OSC
- Harmonic above center, Order near quantized/harmonic behavior
- Small Detune offset

Why it works:
- 5-step pitch cycle rotates against the pulse frame
- PM gives metallic attack
- slight detune creates moving overtone rhythm

## Patch 2: 7-step asym hat engine

**Goal:** asymmetrical hi-hat / digital shaker pattern

- Morph to **Asym**
- UFG fast sub-audio
- Damped/Pulsar high
- Δ–∑ Length = 7
- Δ–∑ normalled to Shape or Morph attenuverter
- Smooth low to medium
- Shift moderate
- Depth moderate
- Shape moderate-high
- Mod tracks UFG, harmonic at a high ratio

Why it works:
- Asym already favors pulse-train-like spectra
- 7-step timbre cycle produces non-square-bar hat phrasing
- tracking Mod to UFG ties timbre density to rhythm engine

## Patch 3: Chaotic fill generator

**Goal:** fill bursts that return to a stable groove

- Build a stable pattern first in FBPM or XPM
- Δ–∑ Chance at minimum
- Length = 8 or 16
- During fill, raise Chance to 50–90%
- Increase Morph CV amount from Δ–∑
- Switch to **FBPM2** or **XPM2**
- Optionally raise Smooth a bit

Then return:
- Lower Chance back to minimum
- Double-press Morph encoder to snap to nearest morph position if needed
- Reduce Morph modulation

Why it works:
- non-destructive Chance means chaos is temporary
- right-hand morph path adds unstable modulation structures
- returning Chance to minimum recalls the original loop

## Patch 4: Quantizer-threshold trigger percussion

**Goal:** rhythm generated by pitch movement

- Route Root to OSC
- Enable a scale
- Turn on **Q.Trig**
- Feed stepped/sliding sequence to OSC 1V/TZ, ideally from Δ–∑ or external CV
- UFG not looping, or configured to respond clearly to triggers
- Damped/Pulsar high enough for obvious envelope/gating effect

Now UFG events occur when oscillator pitch crosses quantizer thresholds.

Why it works:
- rhythm depends on interval crossing, not fixed step grid
- unusual scales create unusual rhythmic density
- glides and stepped values create different trigger behavior

This is excellent for nonstandard meters and “intelligent chaos.”

---

# 10. How to imply multiple simultaneous rhythms from one voice

Since this is one module, you often won’t have separate drum voices internally. So create **perceived layers** instead.

## Layering strategies

### Stereo split
The main outputs are sine/cosine stereo pair. Use them as:
- left = body / drum shell
- right = transient / overtone image

Then process externally:
- one side through saturation/compression
- other side through HPF or reverb

This can feel like two related percussion voices.

### Alternating timbral accents
Use Δ–∑ on:
- pitch and Shape
or
- Morph and Depth

Some hits become:
- low / round
others:
- sharp / metallic

That creates the impression of kick-snare-hat interplay from one oscillator line.

### Mod detune as microtiming feel
Slight Mod detune in PM modes creates shifting beating and transient instability. This reads like internal swing or tuplet texture even if the trigger grid is steady.

---

# 11. External patching ideas for even more complexity

The manual suggests plenty internally, but for serious percussion systems, combine K-ACCUMULATOR with outside tools.

## Best pairings

### Clock divider / multiplier
Feed UFG Trig or Δ–∑ Clock externally with odd divisions:
- /3
- /5
- /7
- x3
- x5

Now K-ACCUMULATOR’s internal pattern logic sits on top of external odd meters.

### Sequential switch
Use the sine/cosine outputs and switch processing chains every few beats.

### Logic module
Take an external rhythm and use it to trigger UFG in one of the sync/reversal modes. Logic-combined clocks are great here.

### VCA / LPG
Especially for TZFM into UFG or external amplitude sculpting. The manual specifically notes external VCA before UFG TZFM for wavefolder-like patches.

### Filter / resonator
K-ACCUMULATOR can make raw drum matter; a resonant filter or resonator can help separate kick/snare/hat zones.

---

# 12. A practical workflow for writing complex percussion with it

## Workflow A: Compose the meter first
1. Set UFG pulse rate to your desired subdivision
2. Set Δ–∑ Length to odd values: 5, 7, 11
3. Lock Chance at minimum
4. Edit pattern with Pattern switch
5. Only then add Morph modulation and PM complexity

This gives deliberate odd-meter structure.

## Workflow B: Compose the texture first
1. Find a killer percussion timbre in XPM / Asym / FBPM2
2. Set Damped/Pulsar until it grooves
3. Use Δ–∑ for pitch and Morph modulation
4. Tune Length and Chance until a rhythmic cycle emerges

This gives more experimental/IDM outcomes.

## Workflow C: Performance mutation
1. Keep one stable base patch
2. Use only these for performance:
   - Chance
   - Length
   - Morph position
   - Damped/Pulsar
   - Smooth
3. Return to locked states frequently

This is best for live hyper-rhythmic improvisation.

---

# 13. Recommended parameter habits for “hyper-complex percussion”

If that specific aesthetic is the target, here are the habits I’d emphasize:

## Use odd lengths constantly
- 5, 7, 11, 13
- combine with stable UFG pulse base

## Keep Chance just above zero often
Not total randomness—just enough mutation to prevent exact repetition.

## Use right-hand morph path for fills
- FBPM2
- 2OP2
- XPM2

## Use Asym for hat families
Especially when you want pointillistic upper percussion.

## Use moderate Smooth, not always zero
A little slew makes lines feel alive and less step-grid-rigid.

## Detune the Mod subtly
Tiny offsets can create huge movement in PM percussion.

## Exploit Root/Scale selectively
Quantized tuned percussion can make chaotic rhythms still sound musically anchored.

---

# 14. A few “recipe” settings

## Broken electro kick
- Morph: FBPM
- Damped/Pulsar: high
- UFG Time: slow/sub-audio
- Depth: medium-high
- Shape: low-medium
- Stretch: low
- Δ–∑ to 1V/TZ lightly
- Smooth: low

## Metallic snare cluster
- Morph: XPM
- Mod tracks OSC
- Harmonic: above center
- Order: near harmonic/quantized region
- Detune: slight
- Damped/Pulsar: medium-high
- Δ–∑ to Shape or Depth
- Length: 5 or 7

## Digital hat spray
- Morph: Asym
- UFG fast sub-audio
- Damped/Pulsar: high
- Shape: medium-high
- Shift: medium
- Δ–∑ Length: 7
- Chance: low-medium
- Smooth: low

## Machine fill / broken memory
- Morph: XPM2
- Chance: high temporarily
- Length: modulate between 5 and 8
- Smooth: medium
- Detune: slight
- Return Chance to minimum to recover groove

---

# 15. Best conceptual takeaway

To get **densely rhythmic hyper-complex percussion** out of K-ACCUMULATOR, don’t treat it like a normal oscillator with occasional modulation.

Treat it as:

- **UFG = pulse engine**
- **Δ–∑ = phrase mutation and odd-length sequencer**
- **OSC = drum body/transient generator**
- **Mod = overtone/metallic structure**
- **Morph = percussion topology selector**
- **Damped/Pulsar = the “drum articulation” control**

If you build around that mindset, this module can generate:

- rotating odd-meter drum cycles
- self-mutating percussion phrases
- metallic PM polyrhythms
- unstable fills that snap back to the groove
- complex rhythmic illusions from threshold triggers, pattern length, and harmonic detune

If you want, I can also make you:
1. a **set of 10 concrete patch recipes** for IDM/glitch percussion,
2. a **techno-focused patch sheet**,
3. or a **“one-module polyrhythm performance workflow”** for K-ACCUMULATOR.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)