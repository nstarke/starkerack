# Fancyyyyy — K-Accumulator Digital Complex Oscillator

- [Manual PDF](../../manuals/K_ACCUMULATOR_Quickstart_v1.02.pdf)

---

[Manual PDF](https://fancysynthesis.net)

# K-ACCUMULATOR modulation ideas for distorted percussion, basslines, and haunted pads

K-ACCUMULATOR is unusually rich because it is not just “an oscillator with some FM.” It is a whole internal ecosystem:

- main OSC with multiple waveshaping domains
- Mod oscillator for PM/XPM behavior
- UFG as envelope/LFO/audio oscillator
- Δ–∑ pattern generator for stepped/smoothed modulation
- internal normalled routing to many CV inputs

That means the best sounds usually come from **stacking small modulations in several places at once**, not maxing one knob.

A useful mindset:

1. Start from **Centre**
2. Choose a **Morph mode**
3. Pick one internal mod source:
   - **UFG** for organic motion, envelopes, pulses
   - **Δ–∑** for stepped instability and evolving sequences
4. Add one external CV if desired
5. Use **Stretch** and **Damped/Pulsar** as “make it strange” controls

---

## First: the best general modulation strategies

## 1. Use the internal normalisations aggressively
On the OSC section, the CV inputs/attenuverters are internally normalled from either:

- **UFG** when the LED is unlit
- **Δ–∑** when the LED is lit

So even without patching cables, you can modulate:

- Shift
- Depth
- Shape
- Morph
- 1V/TZ

This is the fastest way to find complex timbres.

### Great default trick
- Set **one waveshaper attenuverter positive**
- Set **another slightly negative**
- Feed one from **UFG**
- Feed the other from **Δ–∑**

This creates counter-motion inside the oscillator, which often sounds much more alive than moving everything in the same direction.

---

## 2. Morph slowly, shape quickly
The Morph system is continuous, but the character of the controls changes depending on which path you’re on.

### Best approach
- Use **Morph** as a slow macro movement
- Use **Shift/Depth/Shape** as faster or performance controls

This works because:
- Morph changes the topology
- Shift/Depth/Shape exploit the current topology

For performance, try:
- slow Δ–∑ or UFG to Morph
- manual performance on Depth and Shape
- light modulation on Shift

---

## 3. Use small modulation depths first
This module seems designed so that **small amounts of modulation can produce large spectral changes**. Especially in:

- XPM / XPM2
- FBPM2
- high Damped/Pulsar settings
- high Stretch with active shaping

For punchy results:
- keep attenuverters around 9–10 o’clock or 2–3 o’clock first
- only push further once the base patch is good

---

# Best Morph modes by sound goal

## For distorted percussion
Best starting modes:

- **FBPM**: stable, clear, sine-to-saw distortion
- **2OP**: controlled mod-oscillator aggression
- **FBPM2**: chaotic and nasty
- **Asym**: brittle, granular, clicky, unusual

## For dubstep / DnB bass
Best starting modes:

- **XPM**: filthy but still playable
- **XPM2**: more separated controls, highly designable
- **2OP2**: good for “speaking” basses
- **FBPM** with Stretch: great for reese-adjacent spectral tearing

## For haunted pads
Best starting modes:

- **FMNT**: formant-like, vocal, airy
- **2OP**: smooth animated harmonic motion
- **Asym**: eerie and unstable if used gently
- **XPM** at low depth: slowly evolving spectral bloom

---

# Distorted percussive sounds

These patches lean on **UFG as envelope/pulse source** and **Damped/Pulsar** for internal sync/amplitude shaping.

## Patch idea 1: metallic distorted kick / tom
### Goal
A low fundamental with a sharp distorted transient and internal pitch snap.

### Setup
- Start from **Centre**
- Route **Root to OSC**
- Set OSC frequency low
- Set Morph to **FBPM** or **2OP**
- Turn up **Damped/Pulsar** to medium-high
- Set **UFG Time** to sub-audio, single-shot or looping slowly
- Use **raised cosine or exponential-ish UFG shape**
- Add a bit of **Depth**
- Add a little **Shape**
- Keep **Stretch** low at first

### Modulation ideas
- Send **UFG to 1V/TZ** with positive attenuverter for a pitch envelope
- Send **UFG to Depth** lightly for attack-only distortion bloom
- Send **Δ–∑ to Shape** very lightly for changing attack character each hit

### Why it works
- Damped/Pulsar gives sync plus AM, making the transient more percussive
- 1V/TZ from UFG gives the classic downward pitch strike
- FBPM/2OP gives controlled harmonic smear without losing impact

### Push it further
- In **2OP**, tune Mod to a non-octave harmonic
- Add slight **Detune**
- Increase **Shape**
- Add a touch of **Stretch** for weird overtone tearing while preserving low pitch

This can move from kick/tom into broken industrial drum territory.

---

## Patch idea 2: snare / clap / noise-burst style percussion
### Setup
- Morph to **Asym** or **FBPM2**
- Root/OSC in midrange
- UFG in triggered one-shot mode
- **Damped/Pulsar** high
- **Depth** medium
- **Shape** medium to high
- **Shift** low to medium

### Modulation ideas
- UFG to **Damped/Pulsar CV** if available externally, or just perform manually
- Δ–∑ to **Morph** lightly
- Δ–∑ to **Shift** or **Shape**
- Mod oscillator tuned to inharmonic interval with slight detune

### Result
You’ll get:
- noisy broadband crack
- unstable upper harmonics
- changing “snare wires” texture if Δ–∑ is moving Shape or Morph

### Performance move
Shorten UFG Time and increase Damped/Pulsar toward max:
- lower values = papery percussion
- higher values = hard synced tearing snap

---

## Patch idea 3: glitch hats and digital shards
### Setup
- High OSC frequency
- Morph in **Asym**, **XPM2**, or **FBPM2**
- UFG as high-speed trigger or audio-rate modulator
- Very little low end
- Shape and Shift active
- Stretch moderate

### Modulation ideas
- Δ–∑ to **1V/TZ** for stepped micro-pitch chatter
- UFG to **Depth**
- Morph lightly modulated
- Mod tracking OSC, harmonic above center, Order biased toward odd harmonics

### Why it works
At high frequencies, the PM/folding/stretch interactions create hat-like sidebands and digital splatter.

---

# Dubstep / drum & bass basslines

K-ACCUMULATOR seems excellent for bass because it can keep a strong root while heavily altering upper harmonics.

## Core bass design principle
For basses, start by protecting the fundamental:

- Keep the fundamental low and stable
- Use **Stretch** to move harmonics while keeping the root
- Use **Shift** for harmonic blending
- Use **Depth/Shape** for aggression
- Use **Morph** and Mod tuning for vowel/talking motion

---

## Patch idea 4: modern talking neuro bass
### Setup
- Start from Centre
- Route **Root to OSC**
- Quantize if you want a playable scale
- Morph to **XPM** or **XPM2**
- Tune main OSC low
- Set Mod to track **OSC**
- Harmonic above center, around 2nd–5th harmonic region
- Add slight **Detune**

### Sound design
- **Depth** = PM intensity
- **Shape** = extra fold or XPM index depending on mode
- **Shift** = harmonic emphasis / damping depending on mode
- **Stretch** = medium

### Modulation
- **Δ–∑ to Morph** lightly
- **UFG to Shift** or **Shape**
- **Δ–∑ to 1V/TZ** for sequenced pitch
- Use **Scale quantisation** for locked riffs
- Set **Q.Trig on** with Root tracking and scale active for auto-arpeggiated behavior

### Best movement recipe
- slow UFG to one timbre axis
- stepped Δ–∑ to another
- manual performance on Morph

This gives the classic “talking / yawing / barking” bass behavior.

---

## Patch idea 5: reese-ish tearing bass
### Setup
- Morph to **FBPM**, **2OP**, or **XPM**
- Low OSC frequency
- Mod tracks OSC
- Harmonic set close to fundamental or low harmonic
- **Detune** slightly off center
- **Depth** medium
- **Shape** low-medium
- **Stretch** medium-high

### Why this is strong here
Detune affects both:
- Mod oscillator relationship
- harmonic wavefolder animation

That means one control can create moving internal beating and tearing.

### Modulation ideas
- Slow UFG to **Detune** externally if possible
- Δ–∑ to **Stretch** or **Shape**
- UFG to **Depth**
- external slow LFO to Morph

### Character
- mild detune = thick reese
- more stretch = spectral ripping
- more depth = aggressive, metallic edge
- morph toward XPM = more vocal and unstable

---

## Patch idea 6: wobble bass that avoids sounding generic
Instead of only modulating filter cutoff externally, use the internal structure.

### Setup
- Morph in **2OP2** or **XPM2**
- Root to OSC
- Mod tracks OSC
- Set a useful harmonic relation
- Damped/Pulsar low to medium
- Stretch medium
- Shape medium

### Modulation routing
- UFG looping in tempo-synced LFO range
- UFG to **Depth**
- UFG or Δ–∑ to **Morph**
- opposite-polarity modulation to **Shift**
- Δ–∑ to **1V/TZ** for phrase movement

### Trick
Use **Skew** and **Shape** on the UFG to alter how the wobble feels:
- ramp = aggressive forward lurch
- triangle/linear = even sweep
- raised cosine = rounded breathing
- exponential = punchy “grab”

This makes the bass movement feel less like a standard LFO/filter wobble and more like spectral articulation.

---

## Patch idea 7: sub bass with violent top layer
### Setup
- Keep OSC tuned low
- Use moderate **Depth**
- Low-medium **Shape**
- Moderate-high **Stretch**
- Morph in **FBPM** or **2OP**
- Damped/Pulsar low

### Modulation
- Δ–∑ to **Shift**
- UFG to **Shape**
- very light Morph modulation
- quantized pitch via Root/Scale

### Why it works
Stretch can move harmonics while keeping the fundamental stable, which is perfect for bass music where the sub must stay anchored while the top end mutates.

---

# Haunted atmospheric pads

This module is stereo by design at the main sine/cosine outputs, so it should excel at spatial pads.

## Main pad strategy
For pads:
- use the stereo sine/cosine outs as a pair
- keep modulation slow
- use small modulation amounts
- let several parameters drift independently
- avoid too much Damped/Pulsar unless you want tremolo/pulsar texture

---

## Patch idea 8: ghost choir pad
### Setup
- Start at Centre
- Morph to **FMNT**
- Root to OSC and maybe UFG too
- Tune to low-mid register
- Depth low-medium
- Shift low
- Shape low-medium
- Stretch low

### Modulation
- UFG looping slowly
- UFG to **Depth**
- Δ–∑ smoothed and very light to **Morph**
- Δ–∑ or slow external CV to **Shift**
- Mod oscillator tuned to a consonant ratio or scale degree

### Why it works
FMNT uses raised-cosine AM and PM to create formant-like spectra, so small modulations create vocal/choir movement without needing filters.

### Extra haunting move
Use **Just Intonation** scales and scan scale choices around center/right side for less familiar harmonic spacing.

---

## Patch idea 9: drifting horror pad
### Setup
- Morph to **Asym** or low-depth **XPM**
- Main pitch fairly low
- Mod tracks Root or OSC
- Harmonic set to a strange interval
- Detune slightly off center
- Stretch low-medium
- Damped/Pulsar very low or off

### Modulation
- Δ–∑ clocked slowly by UFG
- Increase **Smooth** on Δ–∑ so it glides
- Route Δ–∑ to **Morph** and/or **1V/TZ** lightly
- Route UFG to **Shape** with shallow amount
- Use negative modulation on one parameter and positive on another

### Result
- unstable harmonic fog
- slight melodic drift
- quasi-organic spectral breathing
- eerie tonal asymmetry

---

## Patch idea 10: pulsar-cloud ambient wash
### Setup
- Morph to **FMNT** or **2OP**
- UFG in looping mode at slow to medium rate
- **Damped/Pulsar** medium-high
- OSC in mid register
- Shape low-medium
- Depth low-medium

### Modulation
- Use UFG as the pulsar window via Damped/Pulsar
- Slowly modulate **UFG Shape** and **Skew**
- Δ–∑ to **Morph** lightly
- Δ–∑ Smooth above halfway for flowing transitions
- Stretch a little to separate upper harmonics from the root

### Why it works
The manual explicitly describes UFG as:
- modulation source
- pulsar window generator
- clock for Δ–∑

When all three are linked, you get self-coherent motion that feels composed rather than random.

---

# Specific advanced tricks

## 1. Use Q.Trig for self-generating rhythmic bass/arps
If:
- Root is routed to OSC
- a scale is enabled
- Q.Trig is active

then a trigger is sent to UFG whenever oscillator frequency crosses a quantizer threshold.

### Try this
- Patch an LFO or Δ–∑ into **1V/TZ**
- Set **Damped/Pulsar** high
- Put UFG in non-looping mode

Now pitch movement can generate rhythmic triggers/envelopes internally. This is great for:
- bubbling bass sequences
- auto-arpeggiation
- semi-chaotic percussion

---

## 2. Use external audio into Ext. Sync/Track
The external input can do:
- sync
- pitch tracking

### Creative uses
- Feed a drum loop, voice, or another oscillator
- In **Track** mode, the OSC follows incoming pitch but keeps its own timbre system
- Then use Morph/Depth/Shape/Stretch on that tracked pitch

This can make:
- voice-following demonic drones
- bass that tracks external riffs but becomes alien
- percussion locked to another sound source’s motion

For haunted material, feed vocals or field recordings with pitch content.

---

## 3. Audio-rate UFG modulation
The UFG tracks into audio rate and has anti-aliased output.

### Try
- set UFG to audio rate
- route it internally to Shift, Depth, Shape, or 1V/TZ
- use small attenuation

This will add a more “synth-operator” quality than simple LFO motion:
- buzzy bass articulation
- metallic percussion
- animated formants in pads

---

## 4. Δ–∑ as both sequencer and timbre source
The Δ–∑ is more interesting than a normal random sequencer because:
- it derives from delta-sigma encoding of Mod
- has non-destructive mutation
- can be stepped or smoothed
- behaves differently at audio rates

### Good uses
- to **1V/TZ** for riffs
- to **Morph** for evolving timbral structure
- to **Shape** or **Shift** for note-by-note articulation changes

### Best trick
Lock a good sequence with **Chance at minimum**, then:
- raise Chance temporarily for mutations
- drop it back to restore the original

This is perfect for live basslines: controlled chaos with a reset point.

---

# Practical recipe sets

## Recipe A: distorted industrial kick
- Morph: FBPM
- OSC low
- UFG: one-shot, fast decay shape
- UFG → 1V/TZ positive
- UFG → Depth slight
- Damped/Pulsar: medium-high
- Shape: low-medium
- Stretch: low
- Optional Δ–∑ → Shape tiny amount

---

## Recipe B: snarling neuro bass
- Morph: XPM2
- Mod tracks OSC
- Harmonic: 2nd–4th region
- Detune: slight
- Depth: medium-high
- Shift: low-medium
- Shape: medium
- Stretch: medium
- Δ–∑ → Morph
- UFG → Depth or Shift
- Root scale quantized for riffs

---

## Recipe C: reese with spectral tear
- Morph: 2OP or FBPM
- Mod tracks OSC
- Harmonic near fundamental
- Detune slightly off center
- Depth medium
- Shape low
- Stretch medium-high
- slow UFG to Shape
- slow Δ–∑ to Shift
- external saturation after module if desired

---

## Recipe D: haunted choir
- Morph: FMNT
- stereo outs to reverb
- Depth low-medium
- Shape low
- Shift low
- slow UFG → Depth
- smoothed Δ–∑ → Morph tiny amount
- JI scale selected
- slight Detune

---

## Recipe E: broken alien hats
- Morph: Asym or FBPM2
- OSC high
- Damped/Pulsar high
- UFG triggered quickly
- Shape medium-high
- Shift medium
- Δ–∑ → 1V/TZ tiny
- Mod high harmonic with odd spread
- Stretch moderate

---

# Best control interactions to explore

## Shift + Stretch
This is one of the most unique pairings on the module.

- **Shift** introduces blended harmonic frequency shifting
- **Stretch** frequency-shifts generated harmonics while holding the fundamental

Use this for:
- basses with stable sub and moving top
- metallic percussion
- widening, detuned-feeling pads without destabilizing pitch

---

## Depth + Shape
Usually the most immediate “distortion pair.”

- **Depth** often introduces PM with damping
- **Shape** often introduces harmonic wavefolding

Use:
- more Depth for internal pressure/aggression
- more Shape for visible folds/edges

On percussion:
- modulate Depth with UFG envelope
- leave Shape more static

On bass:
- modulate Shape slowly
- play Depth manually

---

## Damped/Pulsar + UFG Time/Shape/Skew
This is your secret weapon for percussive and animated sound.

- Time = rate or envelope length
- Shape = contour character
- Skew = asymmetry/pulse geometry
- Damped/Pulsar = how much that contour invades the OSC

This can create:
- kicks
- plucks
- tremolo clouds
- hard-sync tearing
- pseudo-granular pulses

---

## Harmonic + Order + Detune on Mod
This cluster determines how “intelligent” the mod oscillator relationship feels.

### Suggestions
- **Order near center**: more blended harmonic behavior
- **Order toward odd/even**: more selective overtone families
- **Order max**: scale-locked or integer-ratio behavior
- **Detune slight**: movement and growl
- **Detune larger**: instability and tearing

Excellent for bass and evolving pads.

---

# If I were patching it for your three goals

## 1. Distorted percussion starter patch
- Morph: FBPM2
- OSC: low-mid
- UFG: triggered one-shot
- Damped/Pulsar: 2–4 o’clock
- UFG to 1V/TZ positive
- UFG to Depth slight
- Δ–∑ to Shape tiny
- Mod detuned inharmonically

## 2. Dubstep / DnB bass starter patch
- Morph: XPM2
- Root quantized
- Δ–∑ to 1V/TZ
- UFG looped in tempo
- UFG to Shift
- Δ–∑ to Morph
- Stretch up until the top starts talking
- Shape to taste
- Detune slightly off center

## 3. Haunted pad starter patch
- Morph: FMNT
- stereo outs hard left/right
- UFG slow looping
- UFG to Depth light
- smoothed Δ–∑ to Morph very light
- Shift barely on
- Shape barely on
- JI scale
- huge reverb after

---

# Final advice

K-ACCUMULATOR seems to reward this exact workflow:

1. Return to **Centre**
2. Pick a **Morph mode** for the general voice
3. Add **one** shaper
4. Add **one** modulation source
5. Add **Stretch**
6. Add **Damped/Pulsar**
7. Only then start moving Mod harmonic relationships

That order tends to preserve intention while still getting into wild territory.

If you want, I can also turn this into:
- a **cheat sheet by panel section**
- **10 exact knob-position patches**
- or a **performance-oriented patch guide** for techno / dubstep / ambient sets.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)