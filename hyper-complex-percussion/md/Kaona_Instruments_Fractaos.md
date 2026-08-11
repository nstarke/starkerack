# Kaona Instruments — Fractaos

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Fractaos User Manual v1.5 (PDF)](https://kaona.fr/wp-content/uploads/2025/08/Fractaos_Manual_1.5.pdf)

# Using Fractaos for densely rhythmic, hyper-complex percussion

Fractaos is unusually good for this because it is not just a “pretty poly oscillator” — it has:

- **4 voices**
- **4 trig inputs**
- **4 separate 1V/oct inputs**
- **5 dedicated drum fractals**
- **per-voice envelopes**
- **multitimbral mode**
- **driver/follower oscillator interactions**
- **LFO/one-shot primitive modulation**
- **texture/filter behavior**
- **drone and chord-spread behaviors for layered clusters**

That means you can treat it like a **4-part percussion synth**, a **polyrhythmic drum ensemble**, or a **hybrid drum+pitched fracture machine**.

---

## Best overall mindset

For hyper-complex percussion, think of Fractaos as:

- **Voice 1:** kick / low thud / sub impact
- **Voice 2:** snare / rim / metallic body
- **Voice 3:** hat / shaker / granular tick stream
- **Voice 4:** cymbal / tom / glitch accent / tonal stab

Then drive those four voices from:

- separate triggers with **different loop lengths**
- different clock divisions/multiplications
- separate pitch CV lanes
- different MIDI channels in **MULTI** mode
- or combinations of CV trig + MIDI note streams

This is where the complexity comes from: **independent voice timing + different timbres + different pitch behavior + different envelopes**.

---

# Core strategies

## 1. Use the 5 Drum fractals as your starting percussion engine

The manual gives you these drum models:

- **Kick**
- **Tom**
- **Snare**
- **HiHat**
- **Cymbal**

These are not samples. They are modeled one-shots with:

- excitation
- resonances
- filtered noise
- micro-variation

That means they respond musically to parameter motion, rather than just replaying fixed samples.

### Why this matters for complex rhythm
When you run dense irregular patterns, repeated hits can get boring fast. Fractaos avoids that because:

- **Chaos** changes hit variation, instability, roughness, internal detuning
- **Depth** changes decay/open-ness/tail
- **Morph** can blend the drum with a geometric fractal
- **Texture** can reshape resonance/formant behavior
- **Pitch CV / MIDI note** still affects drum color

So even a repeating trigger pattern can become **constantly shifting percussion**.

---

## 2. Make each voice a different rhythmic identity

Because Fractaos has **4 trig inputs and 4 pitch inputs**, use four separate sequencer lanes.

Example setup:

### Voice allocation
- **Voice 1:** Kick — sequence in 11 steps
- **Voice 2:** Snare — sequence in 7 steps
- **Voice 3:** HiHat — sequence in 13 steps
- **Voice 4:** Cymbal/Tom — sequence in 5 steps

This instantly creates a **long non-repeating composite cycle**.

### Good clock/pattern ideas
- Kick on a sparse Euclidean lane
- Snare with occasional ratchets
- HiHat on a fast clock with probability/skips
- Tom or Cymbal on odd accents every 5 or 9 pulses

If your modular has:
- clock dividers
- burst generators
- Euclidean sequencers
- logic modules
- probability triggers
- sequential switches

…Fractaos will reward all of them.

---

## 3. Use MULTI mode as a percussion kit

Fractaos’s **MULTI mode** is one of the best features for this use.

In MULTI:

- each voice can load a **different preset**
- each voice can listen on a **different MIDI channel**
- LIVE voices can remain hands-on
- preset voices keep their own stored settings

So you can build a **4-piece percussion kit**, where each voice is a distinct instrument patch.

### Example percussion kit in MULTI
- **Voice 1 preset:** short Kick, low pitch, low morph, medium chaos
- **Voice 2 preset:** noisy Snare blended with Cantor or Rule30
- **Voice 3 preset:** sharp HiHat with short depth and high texture
- **Voice 4 preset:** Cymbal blended with Hilbert for metallic upper noise

Then sequence them separately by MIDI channel or trig/CV logic.

### Why MULTI is powerful here
It lets you maintain:
- distinct tone per voice
- distinct volume per voice
- stable roles in a composition
- independent sequencing behavior

This is ideal for **polymetric percussion architecture**.

---

# Make Fractaos sound punchy and percussive

## 4. Use short ADSR settings globally for impact

Fractaos shares ADSR settings across voices, so dial them with percussion in mind.

### Percussive envelope starting point
- **Attack:** as low as possible
- **Decay:** short to medium
- **Sustain:** 0 or near 0
- **Release:** short, but not always zero
- **Curve:** exponential or logarithmic depending on desired snap

### Important manual note
Even with **Sustain = 0**, Release still matters if the note is released before decay finishes.

So for CV/gate percussion you can get useful expressive differences from gate length.

### For punch
Use:
- very fast attack
- short decay
- low sustain
- short release
- curve toward exponential feel

This gives tighter transient emphasis.

---

## 5. Use Depth as your “drum open/close/length” macro

On drum fractals:

- **Depth** mainly controls **duration**
- on **HiHat**, it controls opening/closing
- on **Kick/Tom/Cymbal**, it changes tail length and resonance decay

### Rhythmic application
Modulate or manually vary Depth between pattern sections:
- short hats in busy fills
- longer cymbals for phrase endings
- tighter kick for dense passages
- longer toms for sparse accents

If your patch can’t CV Depth directly, save several presets with different depth states and use them in MULTI or preset changes.

---

## 6. Use Chaos for humanized instability and aggression

On drum fractals, **Chaos** affects:

- variation between hits
- roughness
- instability
- detuning
- explosiveness

This is one of the best controls for “alive” percussion.

### How to use it musically
- **Low chaos:** clean electro hits
- **Medium chaos:** lively modular drums
- **High chaos:** broken, unstable, splattering percussion

### Great trick
Patch a stepped random CV or a slow modulation into:
- **F-Chaos**
- **P-Chaos**

Use attenuation carefully. Small amounts go far.

That gives you:
- slight hit-to-hit change
- timbral drift over bar cycles
- asymmetry across repeated figures

For hyper-complex patterns, this prevents static machine-gun repetition.

---

## 7. Morph drums into pitched or metallic hybrids

This is where Fractaos gets special.

Per the manual:
- Drum curves can’t be FM’d
- but **Morph** can blend a drum with the second geometric fractal

So you can create:
- percussive attack + tonal tail
- snare transient + pitched body
- cymbal hit + harmonic cloud
- kick impact + distorted oscillator bloom

### Excellent pairings
- **Kick + Sierpinski/Koch** = tight body with harmonic tone
- **Snare + Rule30** = noisy fractured snare
- **HiHat + Hilbert** = stepped metallic clockwork hat
- **Cymbal + Dragon/Rössler** = unstable shimmering metal
- **Tom + Fibonacci** = tunable melodic drum

### For punch
Keep Morph low to medium:
- enough to add body
- not so much that you lose attack

### For weird fills
Push Morph higher on selected voices or sections so percussion becomes part-note, part-impact.

This is perfect in complex meters where you want the drums to blur into melodic rhythm.

---

# Advanced rhythmic modulation techniques

## 8. Use primitive LFO as a one-shot contour generator

The switches **Loop** and **Trig** are critical.

From the manual:

- **Loop OFF + Trig ON** = one-shot modulation restarted on each note
- **Loop ON + Trig ON** = loops while note is held
- **Loop ON + Trig OFF** = free-running
- **Loop OFF + Trig OFF** = inactive except special modes like FM

For percussion, the killer move is:

### Use one-shot primitive modulation
Set:
- **Loop OFF**
- **Trig ON**

Now every hit retriggers the primitive-derived motion.

Use switch targets:
- **Morph**
- **Spread**
- **Chaos**

This turns each hit into a micro-event with internal motion.

### Example uses
- **Morph ON:** each hit shifts from attack to tonal tail
- **Chaos ON:** each hit blooms into instability
- **Spread ON:** each hit detunes internally like flams or metallic wobble

This is extremely useful for making percussion feel animated and “composed” rather than static.

---

## 9. Use Speed + Amount to make different rhythmic densities

The primitive modulation has:
- **Speed** = rate
- **Amount** = depth/intensity

Since Speed goes very slow up to 12 Hz, you can use it two ways:

### Slow modulation
For long-cycle form:
- very slow Speed
- medium Amount

This makes the drum timbre evolve over many bars while your trigger patterns stay dense.

### Fast modulation
For micro-rhythm:
- higher Speed
- modest Amount

This creates:
- buzzing hats
- tearing snares
- unstable metallic ticks
- trembling kick harmonics

With one-shot trig behavior, Speed becomes almost like the **internal shape speed of each transient**.

---

## 10. Use Spread as metallic detune or per-voice interval offset

Outside Drone mode, **Spread** introduces detune between driver and follower.

For percussion this is excellent for:

- metallic broadening
- pseudo-flams
- pitch smear
- resonant shell complexity

### Best applications
- **Kick:** tiny Spread for thicker low-end
- **Snare:** medium Spread for shell/noise separation
- **HiHat/Cymbal:** larger Spread for metal shimmer
- **Tom:** tuned detune for dual-head-like motion

If you modulate Spread with the primitive, it can create **oscillating detune** that feels like animated resonances.

That’s useful for:
- industrial hats
- broken cymbals
- tuned percussion swarms

---

## 11. Texture is your “resonant articulation” control

Texture is not just a filter amount. It affects:

- fractal filter resonance
- formant detection/application
- organic micro-detuning
- filter intensity

This is huge for percussion.

### Low Texture
- tighter
- drier
- more direct
- better for kick/transient definition

### Medium Texture
- more body
- more resonant identity
- snappier spectral articulation

### High Texture
- ringing
- formant-y
- unstable
- can become self-oscillatory on some materials

### Suggested use
- Kick: low to medium
- Snare: medium
- HiHat: medium-high
- Cymbal: medium-high to high
- Experimental percussion: high with chaos modulation

Texture is one of your main tools for moving from **drum machine** to **alien percussion organism**.

---

# Best fractals for non-drum percussive synthesis

You do not have to stick to the drum algorithms.

## 12. Use geometric fractals as percussion voices

Some geometric fractals are very percussion-friendly.

### Strong candidates

#### Rule30
Manual says:
- pseudo-random cellular automaton
- dense granular spectrum
- perfect for percussive sounds, basses, etc.

Use it for:
- glitch hats
- digital snares
- granular ticks
- noisy tom transients

#### Collatz
- stepped, jerky profile
- ideal for rhythmic textures

Use it for:
- click sequences
- clave-like pulses
- mechanical percussion

#### Hilbert
- evolving rectangles
- stable plateaus with abrupt changes

Use it for:
- robotic percussion
- hard-edged zaps
- square-ish impact tones

#### Dragon
- internal beating
- expressive under chaos modulation

Use it for:
- resonant metallic strikes
- unstable mid percussion

#### Lorenz / Hénon / Logistic
These can become unstable and irregular. Great for:
- ghost percussion
- broken fills
- non-repeating accent voices

---

## 13. Build synthetic percussion from non-drum fractals

Try this recipe:

- Fractal Type: Rule30 or Collatz
- Primitive: Hilbert or Koch
- Attack: very short
- Decay: short
- Sustain: 0
- Release: short
- Morph: low-medium
- Texture: medium-high
- Spread: medium
- Chaos: medium

This often yields:
- clicks
- zaps
- metallic taps
- pseudo-snare textures
- articulate glitch percussion

It’s great when you want percussive sounds that don’t read as conventional drums.

---

# Polyrhythm and odd meter patch ideas

## 14. Four-lane polymeter patch

Patch:
- 4 independent trigger streams into the 4 trig inputs
- 4 independent pitch CV lanes into the 4 pitch inputs

Pattern lengths:
- Voice 1: 8
- Voice 2: 5
- Voice 3: 7
- Voice 4: 11

Voice roles:
- V1 Kick
- V2 Snare
- V3 HiHat
- V4 Tom/Cymbal hybrid

Result:
- long evolving composite rhythm
- repeating only after large cycle length
- excellent for techno, IDM, ritual polyrhythm, broken beat

### Extra move
Slightly modulate Chaos or Texture globally so each cycle mutates.

---

## 15. Complex time-signature percussion ensemble

Use Fractaos voices as subgroups in different meters:

- Voice 1 accents 4/4 anchor
- Voice 2 runs 3 over 4
- Voice 3 runs 5-step hat phrase
- Voice 4 runs 7-step metallic fill

Because Fractaos has distinct voices, this works much better than forcing one mono drum voice to do everything.

### Good sound assignments
- Anchor meter = Kick
- 3-beat overlay = Snare/Tom
- 5-beat overlay = HiHat
- 7-beat overlay = Rule30/Cymbal glitch

This gives the sensation of **interlocking percussive logic**.

---

## 16. Ratchet and burst patch

Use an external burst generator or ratcheting trigger sequencer.

Assign:
- Cymbal or HiHat drum fractal
- short Depth
- medium Chaos
- high Texture
- primitive one-shot on Chaos or Morph

Now bursts become:
- sizzling rolls
- fractured hat swarms
- metallic stutters

With pitch CV changing during bursts, you can create **spectral rolls**, not just repeated hits.

---

## 17. Ghost-note architecture

Use two voices for “main drums” and two for ghost layers.

Example:
- Voice 1: Kick
- Voice 2: Snare
- Voice 3: low-level Rule30 or Snare ghost notes
- Voice 4: subtle metallic hat/texture accents

Lower the volume of ghost voices in MULTI.

Then sequence them with:
- denser patterns
- lower velocities if using MIDI velocity
- more randomness
- shorter envelopes

This creates dense internal motion without cluttering the front layer.

---

# MIDI-based complexity ideas

## 18. Use MIDI channels in MULTI for separate sequencer tracks

In **multitimbral mode**, each voice can listen on its own MIDI channel.

So from a DAW, tracker, or advanced hardware sequencer:
- CH1 = kick lane
- CH2 = snare lane
- CH3 = hat lane
- CH4 = cymbal/glitch lane

This is ideal if you want:
- tuplets against tuplets
- deliberately irrational-feeling timing
- alternating accents
- probability automation
- per-lane velocity programming

Since Fractaos supports **MIDI velocity** and **aftertouch**, you can add performance variation from the sequencer too.

### Velocity use
If enabled, use velocity to emphasize:
- downbeats
- ghost notes
- burst tails
- phrase accents

### Aftertouch use
Manual says aftertouch affects internal movement rather than pitch. Great for:
- swelling cymbal complexity
- live pressure-driven turbulence
- expressive transitions in dense sequences

---

# Sound design recipes

## 19. Punchy modular kick
- Drum: **Kick**
- Depth: low-medium
- Chaos: low-medium
- Morph: very low
- Spread: tiny amount
- Texture: low-medium
- ADSR: fastest attack, short decay, sustain 0, short release

Optional:
- add slight pitch CV accents
- occasional chaos CV for dirtier strikes

Result: tight but alive low-end.

---

## 20. Fractured IDM snare
- Drum: **Snare**
- Primitive: **Rule30** or **Hilbert**
- Morph: medium
- Chaos: medium-high
- Primitive Chaos: medium
- Texture: medium-high
- Switches: **Trig ON**, **Loop OFF**, **Morph ON** or **Chaos ON**
- Speed: medium-fast
- Amount: moderate

Result: snare hits with internal tearing motion and metallic fragmentation.

---

## 21. Metallic hat swarm
- Drum: **HiHat**
- Depth: short
- Chaos: medium-high
- Spread: medium-high
- Texture: high
- Primitive: **Koch** or **Dragon**
- Trig one-shot modulation on Spread or Chaos

Drive with:
- fast clock
- skip/probability
- bursts

Result: hyper-detailed animated hats.

---

## 22. Tuned tom matrix
- Drum: **Tom**
- Pitch CV sequence on odd pattern length
- Morph: low-medium with **Fibonacci** or **Sierpinski**
- Spread: low-medium
- Texture: medium
- Chaos: low-medium

Result: melodic percussive line that can lock into odd meters.

---

## 23. Cymbal cloud accent voice
- Drum: **Cymbal**
- Depth: medium-high
- Chaos: medium
- Texture: high
- Morph: medium with **Dragon** or **Rössler**
- Speed: slow-medium
- Amount: moderate

Use sparsely on a 5-, 7-, or 9-step cycle.

Result: evolving metallic punctuation that feels larger than a normal cymbal hit.

---

# Performance methods

## 24. Save multiple percussion presets and rotate roles

Because Fractaos supports SD-card presets, build a percussion library:
- short kick
- long kick
- tight snare
- noise snare
- closed hat
- open hat
- metallic burst
- tuned tom
- glitch accent

In MULTI, assign these per voice for different sections.

This is especially useful in live sets where you want:
- verse/chorus rhythm kit changes
- denser breakdown kits
- sparse intro drones that become percussion
- reloadable structured complexity

---

## 25. Exploit LIVE voices inside MULTI

Manual says LIVE voices in MULTI behave exactly like outside MULTI: panel controls still affect them.

This is excellent live.

### Practical setup
- Voices 1–2 = preset percussion anchors
- Voices 3–4 = LIVE experimental percussion

Then during performance:
- twist Chaos
- sweep Morph
- animate Texture
- push Spread
- alter primitive behavior

This gives you stable structure plus performable instability.

---

## 26. Use Drone mode for layered percussive clusters

Drone mode may not sound obviously “percussion-oriented,” but it can be very useful.

In Drone mode:
- all 8 oscillators play continuously
- Spread can move through unison, octave spread, or predefined chords/microtunings

### Percussive application
Patch external VCAs or gates after Fractaos and rhythmically chop the drone output.

Then Fractaos becomes a **continuously evolving cluster source** for:
- struck chord-noise bursts
- metallic stabs
- tuned industrial hits
- complex harmonic percussion swells

Especially effective with:
- Cluster / Ensemble / Aliasing / Cymbal-like sources
- chord Spread zone
- odd trigger chopping patterns

This is a different but powerful route to dense rhythm.

---

# Best external module pairings

## 27. Modules that make Fractaos shine for hyper-complex percussion

Pair it with:

- **Euclidean trigger sequencers**
- **polymeter step sequencers**
- **logic modules** (AND, XOR, OR)
- **clock dividers/multipliers**
- **burst generators**
- **probability/skipping trigger tools**
- **sequential switches**
- **CV-addressed routers**
- **VCAs and LPGs after the outputs**
- **transient shapers / compressors**
- **wavefolders / distortion after output**
- **multiband or resonant filters downstream**

### Why downstream shaping helps
Fractaos already generates intricate spectra, but external processing can make it more mix-ready:
- VCA envelope for extra snap
- LPG for woody articulation
- distortion for transient edge
- compression for punch
- EQ for kick/snare separation

---

# Important limitations to remember

## 28. Things to keep in mind

- **Depth is stepped and cannot be CV modulated**
- **ADSR settings are shared across voices**
- **FM has no effect on Drum curves**
- **Texture and drum models may use more computation**
- **Primitive cannot be a texture or drum model**
- in LOAD mode, pots/CVs do not control until returning to LIVE

So for percussion architecture:
- use **MULTI presets** for distinct drum voices
- use triggers, pitch CV, Chaos CV, Morph CV, Spread CV, Texture CV for live variation
- rely on external sequencing complexity more than expecting full internal modulation of every parameter

---

# Best practical recipe for your goal

If your goal is **densely rhythmic, hyper-complex percussion**, I would use Fractaos like this:

## Recommended master patch
1. Enter **MULTI mode**
2. Load:
   - V1 Kick preset
   - V2 Snare preset
   - V3 HiHat preset
   - V4 Cymbal/Rule30 hybrid preset
3. Feed each voice:
   - unique trigger stream
   - unique pitch CV or MIDI lane
4. Set global ADSR for short, punchy percussion
5. Use primitive modulation as **one-shot per-hit movement**
6. Add mild CV to Chaos and Morph
7. Use odd pattern lengths across voices
8. Mix external accent logic and ratchets
9. Process outputs with compression/distortion/filtering
10. Perform with LIVE voices or reload alternate kits

That will get you into:
- polyrhythm
- polymeter
- glitch percussion
- metallic drum complexity
- animated hits
- non-repeating structures

---

# Short patch examples

## Patch A: Broken polyrhythmic techno
- V1 Kick on 4-step / 16th accents
- V2 Snare on 7-step lane
- V3 HiHat on 11-step lane with skips
- V4 Rule30/Cymbal on 5-step sparse accents
- Chaos CV from slow random
- one-shot Morph modulation on snare and cymbal

## Patch B: IDM drum lattice
- all 4 voices in MULTI
- drum/geometric hybrids
- ratchets on hats
- pitch sequencing on tom/snare voices
- odd bar lengths: 13, 9, 15, 8
- high Texture on upper voices
- medium Spread on metallic voices

## Patch C: Ritual/tribal alien ensemble
- Kick, Tom, Tom, Cymbal
- long composite polymeter
- lower chaos on low voices
- higher chaos on cymbal voice
- occasional morph into Fibonacci/Dragon
- external reverb only on top voices

---

# Final take

Fractaos is not just capable of percussion — it’s especially strong for **percussion with internal motion**, **timbral instability**, and **hybrid drum/oscillator identities**. For complicated rhythmic music, its strength is the combination of:

- **4 independently triggerable voices**
- **MULTI kit behavior**
- **drum fractals**
- **geometric fractals for synthetic percussion**
- **per-hit one-shot modulation**
- **chaos-driven micro-variation**
- **morphing between impact and pitched body**

If you want, I can also give you:

1. a **4-voice Fractaos patch sheet** for IDM/glitch percussion  
2. a **kick/snare/hat/cymbal preset design guide**  
3. a **modular system pairing guide** showing what kinds of sequencers and utilities work best with Fractaos

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)