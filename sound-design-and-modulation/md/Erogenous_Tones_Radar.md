# Erogenous Tones — Radar

- [Manual PDF](../../manuals/radar-instructions.pdf)

---

[Manual PDF / Manufacturer Info](http://erogenous-tones.com)

# Erogenous Tones RADAR — modulation ideas for distorted percussion, basslines, and haunted pads

RADAR is much more than “8 envelopes.” The manual makes clear that it can act as:

- **8 independent AD/AR/repeating envelopes**
- **2 quad phase-related modulation clusters**
- **1 octal phase-related modulation cluster**
- a source of **composite/max envelopes**
- a bank of envelopes with **digital vs analog behavior**
- a bank of **shape-morphing function generators/LFOs**

That means the most interesting sounds come from using RADAR not just to open VCAs, but to **cross-modulate timbre, FM depth, filter behavior, wavefolder amount, distortion drive, and pitch movement**.

---

## What matters most sonically from the manual

A few features are especially useful for aggressive and expressive patching:

### 1. Digital vs Analog modelling
This is one of the biggest tone-shaping features.

- **Digital mode**
  - retriggers reset the envelope back to zero
  - creates discontinuities
  - repeating mode has more constant frequency
  - great for **hard, snappy, clicky, artificial, mechanical** modulation

- **Analog modelling**
  - retriggers do **not** always reset hard
  - attack can begin from the current level
  - in AR mode, short gates may not reach full peak before release
  - great for **rubbery, elastic, smeared, acid-like, organic** modulation

### 2. Shape control: LOG / LIN / EXP and CV
Shape is not just feel — it changes the sound dramatically when modulating:

- **EXP**: front-loaded, punchy, ideal for strikes and hard filter snaps
- **LOG**: slower start, often great for bloom, sucking attacks, and creepy motion
- **LIN**: useful center point and for neutral movement
- **Shape CV**: especially powerful if routed from another modulation source with attenuation

### 3. E/O mode
This changes whether decay/release follows the same curve or the opposite curve.

This matters a lot for punch:

- same-shape attack/release = more symmetrical motion
- opposite release = attack and decay feel more animated and asymmetrical

### 4. Repeating mode
This turns lanes into cycling envelopes/LFOs. Since shape and modelling change the waveform behavior, repeating mode is useful for:

- audio-ish modulation
- weird pseudo-oscillator shapes
- phase-offset modulation in QUAD/OCT modes
- timed rhythmic pumping and wobble

### 5. Composite outputs on lane 4 and lane 8
In Envelope Mode:

- **Lane 4 output switch** can output the **max of lanes 3 and 4**
- **Lane 8 output switch** can output the **max of lanes 6, 7, and 8**

This “max” behavior is extremely useful for creating:
- accented transient stacks
- semi-random contour mergers
- thicker modulation for distortion/filter drive
- pseudo-logic dynamics

---

# General patch strategy with RADAR

Instead of “one envelope to one VCA,” try splitting roles:

- **one lane for amplitude**
- **one lane for filter cutoff**
- **one lane for distortion or wavefolder drive**
- **one lane for oscillator FM amount**
- **one lane for pitch envelope**
- **one lane in repeating mode to wobble another destination**
- **lane 4 or 8 composite output to merge energy from multiple lanes**

That’s where RADAR becomes monstrous.

---

# 1. Distorted percussive sounds

For percussion, RADAR shines when you use **different envelope shapes for different parts of the same hit**.

## A. Industrial kick
Patch:
- Oscillator sine or triangle to VCA/audio path
- Lane 1: VCA amplitude envelope
- Lane 2: pitch envelope to oscillator 1V/oct or FM attenuated input
- Lane 3: filter cutoff envelope
- Lane 4 composite max out: distortion drive CV or wavefolder amount

Suggested setup:
- **Lane 1**: AD, **EXP attack/decay**, short attack, medium-short release
- **Lane 2**: AD, very short, **EXP**, stronger than lane 1
- **Lane 3**: AD, short-medium, maybe **LOG or opposite mode**
- **Lane 4**: another short AD or repeating burst, then use **lane 4 composite output**

Why it works:
- Lane 2 gives the kick its “thwack” by pitching down quickly
- Lane 1 gives body
- Lane 3 makes the filter smack open briefly
- Lane 4 max output can create a transient-heavy control shape for distortion drive, so the hit is dirtier at the start than at the tail

### Make it nastier
Use **digital modelling** for lanes 1–2 to get hard reset behavior. That gives a more artificial, clicky transient.

### Make it more “broken speaker”
Use **analog modelling** for the pitch envelope lane so retriggers start from current level and smear in a less predictable way.

---

## B. Metallic snare / broken clap
Patch:
- Noise + oscillator mixed
- Lane 1: VCA for noise burst
- Lane 2: VCA/filter for tonal body
- Lane 3: bandpass or highpass cutoff
- Lane 4: wavefolder, sample-rate reducer, or distortion amount

Suggested setup:
- Lane 1: very short AD, **EXP**
- Lane 2: short AD, slightly longer than lane 1
- Lane 3: short AD, **LOG** or opposite
- Lane 4: repeating mode at high speed or short AD envelope into timbral destruction

Interesting trick:
- Put **lane 4 in repeating mode** and use trigger resets.
- Every snare hit resets the cycle, so the distortion/wavefold amount starts in a repeatable but animated way.
- In **analog mode**, if the lane is in release when retriggered, it can restart from current level, making each hit feel less static.

This can create claps/snares that sound like:
- tearing foil
- overdriven tape bursts
- granular industrial splashes

---

## C. Neuro hi-hats / glitch percussion
Use short repeating envelopes almost like temporary oscillators or high-speed modulation sources.

Patch:
- Hat sound source through VCA/filter/wavefolder
- Lane 1: amplitude
- Lane 2: filter
- Lane 3: repeating envelope to FM amount or wavefolder symmetry
- Lane 4: composite max output to stereo VCA/panner or second timbre destination

Suggested setup:
- Lane 3 in **Repeating mode**
- Use very fast rise/fall times
- Try **digital mode** first for stable, rigid modulation frequency
- Sweep shape from LIN to EXP/LOG

What to listen for:
- high-frequency chatter
- zappy alias-like edge
- formant-like movement when modulating filter or fold amount

Because the manual notes repeating mode can run quite fast, this can push into audio-rate-ish or near-audio-rate behavior depending on settings.

---

## D. Stacked transient percussion using lane 4 / lane 8 max outputs
This is one of the coolest tricks in the manual.

Set up:
- lanes 3 and 4 with different AD times/shapes
- lane 4 output switch to composite/max
- send that composite envelope to:
  - distortion drive
  - VCA CV for accent
  - LPG CV
  - filter resonance/cutoff

Or:
- lanes 6, 7, 8 with different contours
- lane 8 composite/max to one destination

Why this is useful:
A max-envelope combination behaves differently than a summed envelope:
- it preserves peaks
- doesn’t overload CV as easily
- gives a more “selected transient” response
- can sound like a dynamic envelope follower crossed with logic

Use this for:
- flam-like transient shaping
- ghost notes merged into a main hit
- percussive accents that sound “designed,” not merely louder

---

# 2. Crazy basslines for dubstep / drum and bass

RADAR is ideal for bass because those sounds usually need **multiple moving contours at once**:
- amp contour
- filter contour
- FM/index contour
- distortion contour
- wobble/LFO
- pitch dip or attack transient

## A. Classic reese/neuro bass architecture
Patch:
- 2 detuned oscillators or a complex oscillator
- filter
- distortion/saturation
- VCA
- optional wavefolder/FM

Assign:
- **Lane 1**: amp envelope
- **Lane 2**: filter envelope
- **Lane 3**: distortion/folder drive envelope
- **Lane 4**: pitch drop at note onset
- **Lane 5**: repeating LFO to filter or wavetable position
- **Lane 6**: repeating LFO to FM amount
- **Lane 7**: shape CV target somewhere dynamic
- **Lane 8 composite**: merged accent modulation to “macro” destination

### Good starting settings
- Lane 1: AD or AR depending on note length
- Lane 2: AD, medium decay, **EXP**
- Lane 3: AD, slightly shorter than lane 2
- Lane 4: very short AD, strong negative pitch envelope
- Lane 5: repeating, medium tempo
- Lane 6: repeating, slower or faster than lane 5
- Lane 7: another envelope opening a second filter or VCA
- Lane 8 composite mode to merge lanes 6/7/8 behaviors

### Why this gets huge
Dubstep/DnB bass sounds often come from **different parameters peaking at different times**:
- filter opens first
- distortion blooms second
- FM grit appears later
- pitch settles after a short slam

RADAR gives enough channels to stage all of that.

---

## B. “Talking” bass with QUAD mode
QUAD mode is especially interesting for bass because the lanes are phase-related and offset by 90 degrees.

The manual says:
- only lane 1 or 5 sets time for the group
- the other lanes can act as CV controls:
  - **SPEED**
  - **GRAVITY**
  - **SDELTA**

This is excellent for vocal, morphing movement.

### Patch concept
Use QUAD mode on lanes 1–4.
Send:
- lane 1 to filter cutoff
- lane 2 to wavetable position or formant filter
- lane 3 to FM amount
- lane 4 to distortion drive or second filter

Now the 4 outputs are phase-offset relatives of each other.

### The magic parameters
#### SPEED
Modulates overall cycle speed for the whole quad.
Use this for:
- accelerating wobble
- irregular phrase motion
- “inhaling/exhaling” bass motion

#### GRAVITY
The manual describes it as how the phase-shifted waves are attracted/repelled in time relative to the 0° waveform.

That means:
- the relationship between the modulation lanes bends
- the 90/180/270 offsets stop feeling evenly spaced
- this can create vowel-like asymmetry and lurching motion

For bass, this is gold.
Modulate a formant filter with one lane and distortion amount with another, and changing GRAVITY creates moving “speech” relationships.

#### SDELTA
Shape delta offsets shape across the phased channels.

This can create:
- one lane more log
- another more linear
- another more exponential

That gives a coordinated but non-identical movement — very useful for “alive” basses.

### Dubstep trick
Clock/reset the QUAD cycle rhythmically from your sequencer.
Because QUAD mode resets all lanes together, you can force the bass movement to restart at phrase points.

This creates:
- repeatable hooks
- controllable wobble starts
- more “performed” rhythmic growls

---

## C. OCT mode for monster macro bass movement
OCT mode gives 8 lanes 45 degrees apart.

This is ideal if your patch has many CV destinations:
- main filter
- second filter
- distortion
- wavefolder
- FM amount
- sub VCA
- stereo panning/filter split
- reverb send amount

You can build one giant animated bass voice where every parameter is moving in related but offset ways.

### Great use case
Take one sustained bass note and route OCT outputs to:
1. cutoff
2. resonance
3. fold
4. distortion
5. phase modulation amount
6. VCA level for a parallel band
7. chorus depth
8. delay send

Now adjust:
- shape
- speed
- gravity-like lane functions depending on mode setup

The result can move from:
- classic wobble
- to tearing neuro
- to broken robotic vowel
- to spiraling modulated swarm

---

## D. AR mode for playable bass articulation
For basslines, **AR mode** is often more musical than AD because note length matters.

The manual notes:
- in analog modelling mode, if the gate is short, attack may not reach full level
- if held high past attack, it remains high until gate goes low

This is fantastic for expressive sequenced bass.

### Patch idea
- Lane 1 AR to VCA
- Lane 2 AR to filter
- Lane 3 AD to pitch transient
- Lane 4 AD to drive

Now note length changes:
- amplitude sustain
- filter sustain
- the relationship between body and transient

Short notes become gnarlier and less fully opened.
Long notes bloom and snarl.

This is how you get basslines that feel “played,” not just triggered.

---

## E. Retrigger abuse for tearing bass
Use **digital mode** and feed rapid trigger bursts into a lane controlling:
- distortion drive
- filter cutoff
- FM amount
- wavefolder symmetry

Because digital mode hard-resets to zero, burst retriggers create abrupt control discontinuities. That can sound like:
- tearing
- zippering
- machine-gun articulation
- aggressive “yoi” attacks

Then compare with **analog modelling**, where repeated triggers can charge from current level and produce more fluid, acid-like tearing.

---

# 3. Haunting atmospheric pads

RADAR can make pads interesting because it can create **many related but non-identical slow modulations**.

The key is to stop thinking “envelope” and think:
- phased contour generator
- slow shape-morphing modulation bank
- event-responsive pad animator

## A. Breathing pad in OCT mode
Use OCT mode for one sustained voice or layered voices.

Route the 8 outputs to:
1. main VCA
2. lowpass cutoff
3. bandpass center frequency
4. resonance or Q
5. wavetable position
6. FM index
7. reverb send
8. stereo panning or crossfade

Set long times and slow cycles.

What makes this special:
- each lane is 45 degrees apart
- modulation relationships are coherent
- the patch evolves continuously without random chaos

Result:
- spectral drift
- ghostly stereo movement
- tone opening before space blooms
- delayed emotional swells

### For more eerie motion
Use **LOG shapes** for some destinations and **opposite release** behavior.
That creates swells that arrive slowly and disappear differently than they appeared.

---

## B. Uneven breathing using analog AR
Patch a keyboard/sequencer gate to several lanes in Envelope mode.

Use:
- Lane 1 AR to amplitude
- Lane 2 AR to filter
- Lane 3 AR to oscillator shape
- Lane 4 composite with lane 3/4 to reverb send or shimmer amount

Set to **analog modelling mode**.

Because short gates may not fully reach peak before release, playing shorter and longer notes gives:
- incomplete blooms
- fragile swells
- dynamic spectral “underdevelopment”
- a haunted, human feel

This is especially good for:
- choir-like pads
- bowed textures
- dissonant drones
- Boards-of-Canada-meets-horror motion

---

## C. Composite max envelopes for ghost accents
The lane 4 and lane 8 max outputs are not only for percussion.

For pads:
- use lanes 6, 7, and 8 with different long repeating contours
- take lane 8 composite/max output
- route to delay feedback, shimmer amount, or secondary filter resonance

Because the output follows whichever source is currently highest, the modulation becomes:
- selective
- drifting
- less obviously periodic
- more “presence shifting”

This is excellent for making an effect send swell in a way that feels intentional yet elusive.

---

## D. QUAD mode for rotating spectral movement
Take a rich pad and split it into 4 parallel processing paths:
- lowpass voice
- bandpass voice
- distorted voice
- shimmer/reverb-heavy voice

Control each path’s VCA or filter with one lane of a QUAD set.

Since each lane is phase-related, the pad rotates through spectral identities.

Now modulate:
- **SPEED** for acceleration/deceleration
- **GRAVITY** for uneven temporal pull
- **SDELTA** for differences in shape between paths

This can create:
- spectral orbiting
- swelling that “leans”
- cursed choral breathing
- unstable dreamlike animation

---

# Best modulation destinations for RADAR

RADAR is strongest when patched to destinations with nonlinear sonic impact:

## Excellent destinations
- filter cutoff
- filter resonance
- wavefolder amount
- distortion drive
- FM index
- wavetable position
- VCA level
- LPG CV
- delay feedback
- reverb send
- stereo crossfade
- parallel distortion blend
- sub oscillator level

## Especially powerful combinations
- **amp + filter + drive**
- **pitch transient + amp + fold**
- **filter + FM amount + resonance**
- **reverb send + cutoff + stereo pan**
- **distortion drive + post-distortion filter cutoff**

---

# Practical recipes

## Recipe 1: Dubstep growl
- Envelope Mode
- Lane 1: AR to VCA
- Lane 2: AD to filter
- Lane 3: repeating to wavetable position
- Lane 4 composite: to distortion drive
- Lane 5: AD to pitch dip
- Lane 6: repeating slow to FM amount
- Lane 7: AD to resonance
- Lane 8 composite from 6/7/8 to macro VCA/filter

Use:
- digital for attack-heavy lanes
- analog for repeating and AR lanes
- shape around EXP for attack, LOG for evolving timbre

## Recipe 2: Neuro stab
- very short VCA envelope
- short strong pitch envelope
- medium filter envelope
- second envelope to folder amount
- repeating lane reset by each note to create animated onset

Use digital mode for hard restarts and harsh edges.

## Recipe 3: Haunted drone pad
- OCT mode
- very slow cycle
- route 8 outputs across tone and FX network
- use LOG/LIN leaning shapes
- slow modulation of SPEED from an external LFO

Reset occasionally from a gate sequencer so the whole atmosphere “inhales” again at phrase boundaries.

## Recipe 4: Broken percussion bus
Use several lanes triggered from one source due to normalized trigger behavior:
- one trigger into top lane
- each lane configured differently
- route outputs to multiple modulation targets on a drum voice

Then use lane 4/lane 8 composite outputs to create dynamic transient overlays.

---

# Performance tips

## 1. Use attenuation everywhere
The manual explicitly warns shape CV is offset by incoming CV and suggests external attenuation. This is true for most interesting RADAR modulation uses. Small modulation often sounds better than full-swing chaos.

## 2. Pair digital and analog behaviors intentionally
- **Digital** = impact, precision, aggression
- **Analog** = glide, smear, weight, elasticity

For a single sound, use one of each on different destinations.

## 3. Shape is a timbre control
When an envelope controls drive, FM, or fold depth, shape behaves like a macro-timbre parameter, not just contour.

## 4. Retriggering is part of the sound
Especially in digital mode, retriggers are audible as control discontinuities. Lean into that for:
- glitches
- tearing bass attacks
- machine-gun percussion

## 5. Composite outputs are secret weapons
The max outputs are not obvious, but they’re one of the most unique features on RADAR for designing sophisticated transient behavior.

---

# My favorite “weird” patch ideas from this manual

## 1. Distortion-first envelope stack
- lane 1 to VCA
- lane 2 to filter
- lane 3 and 4 combined via max output to distortion drive
- lane 5 repeating slowly to tone control

This gives transients that explode in dirt before the body settles.

## 2. Phase-spread bass organ
Use OCT mode and route all 8 lanes to:
- several oscillator levels
- filter offsets
- distortion amounts
- effects sends

You get a single bass note that mutates like a living machine.

## 3. AR underfilled pad
In analog AR mode, use intentionally short gates so attacks never fully complete. This makes every note feel like a failed bloom or a half-remembered swell — perfect for eerie pads.

## 4. Resettable wobble phrase design
Use QUAD/OCT repeating structures and reset them from your sequencer at phrase starts. This keeps modulations wild but musically aligned.

---

# Bottom line

RADAR excels when you treat it as a **multi-lane motion designer** rather than just an envelope bank.

For your target sounds:

- **Distorted percussion:** use short EXP envelopes, digital retriggering, and composite max outputs into drive/filter/pitch
- **Dubstep / DnB basslines:** combine AR for body, AD for transient pitch/filter/drive, and QUAD/OCT for coordinated moving timbre
- **Haunting pads:** use slow analog AR or OCT movement, LOG-heavy contours, and composite outputs into FX sends and spectral controls

The manual’s most creatively useful features are:
- **digital vs analog modelling**
- **shape and opposite-shape behavior**
- **repeating mode**
- **quad/oct phase offsets**
- **lane 4/lane 8 max composite outputs**

Those are the features that will get you from “envelopes” to genuinely unusual sound design.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)