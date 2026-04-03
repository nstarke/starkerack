# 2hp — Tape

- [Manual PDF](../../manuals/2hp_Tape_Stop.pdf)

---

[Manual PDF](https://www.twohp.com/modules/tape-stop)

# 2hp Tape Stop — modulation ideas for wild sound design

The **2hp Tape Stop** is a compact, clock-syncable tape slow-down effect. On paper it looks simple, but in a modular patch it can become a **rhythmic pitch-drop generator**, **transient mangler**, **pseudo-glitch sequencer**, and **atmospheric smear tool**.

## What the module does well

From the manual:

- **Audio in / out** for up to **10Vpp**
- **Trig button + trig gate input** starts the tape stop
- **Momentary or latching** trig behavior
- **Lag knob** sets stop time:
  - free mode: **instant to 4 seconds**
  - clocked mode: **instant, 32nd, 16th, 8th, 4th, half, whole, 2 bars, 4 bars, 8 bars, 16 bars**
- **Clock input** syncs stop length to external clock
- **Lag CV input**: **-5V to +5V**
- **50/50 mode** at boot: hold **Trig** while powering on for a dry/wet mix of 50%, so the dry signal remains audible during the stop

This means the core modulation targets are:

1. **Trig timing**
2. **Lag amount**
3. **Clock relationship**
4. **Momentary vs latching behavior**
5. **Dry/wet strategy via normal mode vs 50/50 boot mode**
6. **Patch placement** before or after other modules

---

# How to think about modulating Tape Stop

Tape Stop is not just an effect; it is basically a **temporary, nonlinear pitch and time collapse**. Every trigger creates a falling-speed event. The sound you get depends on:

- **what audio you feed it**
- **when it’s triggered**
- **how long the slowdown lasts**
- **whether the slowdown is rhythmic or free**
- **whether you hear only wet or dry+wet together**

## Main modulation approaches

### 1. Trigger it rhythmically
Send clocks, gates, Euclidean patterns, ratchets, burst generators, or probabilistic triggers into **TRIG IN**.

Result:
- repeated tape drags
- pitched-down attacks
- rhythmic stutters
- stop-start motion synced to groove

### 2. Modulate Lag with CV
The **Lag CV input** is the real secret. Modulating it with:
- stepped random
- envelopes
- synced LFOs
- sequencers
- burst CV
- sample and hold

lets every tape stop have a different duration and character.

Result:
- unpredictable fills
- bass phrases that “bend” differently on every note
- pads that feel unstable and ghostly

### 3. Clock it
Patch a master clock to **CLOCK** so the Lag positions become musically related note values.

Result:
- cleaner rhythmic performance
- repeatable drops
- tempo-locked tape movement for dubstep/drum and bass grooves

### 4. Abuse placement in the chain
Try Tape Stop:
- **after distortion**
- **before distortion**
- **before a filter**
- **after a VCA**
- **inside a feedback loop**
- **on a send/return**
- **parallel with dry signal**

This changes whether the pitch-drop feels:
- smooth
- violent
- metallic
- smeared
- broken
- huge

---

# General patch tips before the genre-specific ideas

## 50/50 mode is extremely useful
Booting into **50/50 mode** makes Tape Stop much more flexible for:
- layered basses
- pads
- punchy drums that still keep their attack
- pseudo-flanging/comb-like interactions between dry and slowing signal

For sound design, I’d strongly recommend trying this first.

## Best modulation sources
For the most interesting results, feed **Lag CV** from:

- **Stepped random** for glitch unpredictability
- **Envelope** for “longer stop on harder hit” behavior
- **Sequencer row** for repeatable musical variation
- **Audio-rate or near-audio-rate CV** for experimental artifacts
- **Slow triangle/S&H** for evolving pad movement

## Best companion modules/functions
Even if not specifically from 2hp, Tape Stop loves:
- **distortion / wavefolder / bitcrusher**
- **filter with resonance**
- **VCA**
- **envelope follower**
- **clock divider / multiplier**
- **sequential switch**
- **delay / reverb**
- **sampler / looper**
- **parallel mixer**

---

# 1. Distorted percussive sounds

Tape Stop can turn percussion into crushed, dragging, broken impacts. The trick is to use it not just as a full stop, but as a **micro-pitch-envelope destroyer**.

## Patch idea: broken kick drums

### Basic patch
- Kick or percussion voice → **distortion** → **Tape Stop IN**
- Gate pattern to kick as usual
- Send selected triggers or ghost notes to **Tape Stop TRIG**
- Master clock to **CLOCK**
- Use **Lag** around **32nd, 16th, or 8th**

### What happens
Each trigger makes the drum pitch and tail sag downward, like:
- tape machine braking
- overdriven speaker collapse
- digital buffer malfunction

### Make it nastier
- Put **Tape Stop before distortion** for tearing, folding tails
- Put **Tape Stop after distortion** for heavier “dragging concrete” sound
- Modulate **Lag CV** with stepped random per hit
- Trigger Tape Stop only on every 4th or 8th hit for fills

### Best settings
- Short synced lag values = punchy drag
- Medium free lag = grotesque downward smear
- 50/50 mode = preserves transient while tail melts

## Patch idea: snare flam collapse

### Patch
- Snare or noise burst → filter → VCA → Tape Stop
- Fast trigger sequence or ratchet to snare
- A second offset trigger stream to **Tape Stop TRIG**
- Lag set short, clock synced

### Result
Instead of a normal flam, the second transient gets “reeled down” in pitch/time, producing:
- metallic crunches
- falling snare tails
- broken vinyl-stop fills

### Extra trick
Run a **resonant bandpass filter after Tape Stop** and sweep it slightly. This emphasizes different parts of the slowed noise and can sound like:
- industrial hits
- tortured cymbal bends
- biomechanical percussion

## Patch idea: hi-hat suction effect

### Patch
- Closed hats or filtered noise into Tape Stop
- Trigger Tape Stop occasionally rather than every hit
- Lag around **32nd or 16th**
- Add distortion after Tape Stop

### Result
You get hats that seem to:
- inhale
- buckle
- pitch dive
- smear into gritty reverse-like wisps

This is excellent for:
- neurofunk tops
- broken beat textures
- post-drop fills

## Patch idea: percussion bus abuse
Instead of processing individual drums, route:
- kick + snare + hats submix → Tape Stop

Then trigger Tape Stop from:
- a sparse trigger pattern
- a burst generator at transition points
- manual button presses during performance

### Result
Whole drum loops buckle together, which sounds more like:
- DJ brake
- broken reel-to-reel
- brutal transition fill

### Performance move
Use **latching mode** so one press starts the stop and another releases it. Great for live “oh no the mix is dying” moments.

---

# 2. Crazy basslines for dubstep / drum and bass

This is where Tape Stop gets especially good. Because it imposes a downward pitch-time effect on already aggressive material, it can create bass movement that sounds impossible to get from oscillators alone.

## Core principle for bass
Feed Tape Stop with harmonically rich material:
- wavetable bass
- FM bass
- reese bass
- distorted sine/saw
- sample playback
- filtered noise layer mixed with bass

Then use **short, rhythmic triggers** and **modulated Lag**.

---

## Patch idea: stop-start wobble bass

### Patch
- Oscillator(s) → filter → distortion → VCA → Tape Stop
- Bass sequence drives oscillator pitch/VCA
- Clock to Tape Stop
- Sync’d trigger pattern into Tape Stop TRIG on offbeats or selected steps
- Lag around **16th, 8th, or quarter**

### Result
Instead of classic filter wobble, the bass line gets:
- sudden downward dips
- braked note endings
- staggered “falling speaker cone” movement

This gives a very modern:
- dubstep stutter-drop
- halftime bass choke
- drum and bass phrase punctuation

### Improve it
Modulate **Lag CV** from a sequencer row so each note has a different brake length.

For example:
- step 1 = instant
- step 2 = 32nd
- step 3 = 8th
- step 4 = quarter

That gives bass phrasing that feels animated and vocal.

---

## Patch idea: reese bass degradation

### Patch
- Two detuned saws or a reese source → saturation → lowpass filter → Tape Stop
- Clock to Tape Stop
- Sparse triggers to TRIG, maybe once every bar or on syncopated steps
- Slow modulation to Lag CV

### Result
The reese suddenly droops and tears downward in pitch, causing moving phase relationships to collapse in an ugly, beautiful way.

This can create:
- neurofunk-like tearing
- huge drop transitions
- sick “engine braking” bass gestures

### Advanced version
Put **chorus/phaser before Tape Stop**, then distortion after Tape Stop.  
The modulation gets frozen and bent during the slowdown, making the reese feel alive and unstable.

---

## Patch idea: one-note monster bass with changing tape envelopes

### Patch
- Single low sine/triangle + distorted mid layer mixed together
- Into Tape Stop
- Repeating trigger pattern to TRIG every note
- Sequencer or sample & hold to Lag CV
- Optional clock sync

### Why it works
Even if pitch stays mostly constant at the oscillator, each Tape Stop event creates a different downward contour. So the bassline feels sequenced even when the note content is simple.

### Great for
- minimal dubstep
- rollers
- halftime
- warehouse bass motifs

---

## Patch idea: bass growl choking through 50/50 mode

### Patch
- Boot Tape Stop in **50/50 mode**
- Bass source → Tape Stop
- Trigger on certain notes only
- Distortion and filter after Tape Stop

### Result
Because dry and wet overlap, the slowing signal rubs against the unchanged original, creating:
- phasey grind
- comb-like tearing
- dual-pitch growl
- spectral choking

This is one of the best tricks in the whole module for bass design.

### Make it bigger
Mult the source:
- one copy dry to mixer
- one copy through Tape Stop
- pan or EQ them differently

Then automate Tape Stop only on the wet chain.

---

## Patch idea: drum and bass fill generator

### Patch
- Fast bass sequence into Tape Stop
- Clock from the same master tempo
- Send a trigger burst to Tape Stop near the end of a phrase
- Lag CV from random or pressure/velocity source

### Result
The bass repeatedly brakes and re-grabs, creating frantic:
- machine-gun tape dives
- collapsing phrase endings
- DJ-stop fills
- glitch stammers

Very effective before returning to a straight groove.

---

## Patch idea: post-filter tape stop vs pre-filter tape stop

### Version A: filter before Tape Stop
Bass → filter → Tape Stop

- More recognizable pitch dive
- cleaner note identity
- more “musical” bass drag

### Version B: Tape Stop before filter
Bass → Tape Stop → filter

- more unusual
- filter tracks the changing harmonic density after slowdown
- better for alien/creature basses

### Version C: distortion after Tape Stop
Bass → Tape Stop → distortion

- harsher
- more aggressive top-end breakup
- perfect for “speaker shredding” bass

---

# 3. Haunting atmospheric pad sounds

Tape Stop is also excellent for ambient and cinematic work. If you stop thinking of it as a special effect and start thinking of it as a **time-bending modulation layer**, it becomes a pad haunting machine.

## Patch idea: collapsing drone cloud

### Patch
- Rich drone or chord source → Tape Stop → long reverb
- Slow clock or no clock
- Trigger Tape Stop manually or with sparse random gates
- Lag set medium to long
- Lag CV from a slow random or very slow LFO

### Result
Your drone blooms, then slumps downward into spectral shadow. The reverb catches the slowing harmonics and turns them into:
- ghost tails
- sinking choirs
- decayed tape memory
- haunted cassette ambience

### Best practice
Tape Stop before reverb usually sounds more atmospheric than after.

---

## Patch idea: pad with unstable memory effect

### Patch
- Polyphonic/chordal source or stacked oscillators → Tape Stop
- Boot in **50/50 mode**
- Add chorus and reverb after
- Trigger Tape Stop rarely, with long lag times
- Slow CV into Lag input

### Result
The dry pad stays stable while the wet layer drags and sags underneath it, creating:
- detuned shadows
- melancholic pitch droop
- blurred memory effect
- “the tape is dying” texture

This is incredibly effective for dark ambient and cinematic intros.

---

## Patch idea: clocked ambient pulses

### Patch
- Soft pad or filtered noise chord → Tape Stop
- Master clock into CLOCK
- Trigger at long intervals, maybe every 2 or 4 bars
- Lag set to **whole note / 2 bars / 4 bars**
- Delay and reverb after

### Result
Huge synchronized sinking motions that feel like the whole harmonic bed is slowly falling away. Great for:
- intro sections
- breakdowns
- dark liquid DnB transitions
- soundtrack atmospheres

---

## Patch idea: granular-like ghosting from short triggers

### Patch
- Sustained pad → Tape Stop
- Rapid but irregular short triggers to TRIG
- Short lag values
- 50/50 mode on
- Reverb after

### Result
Instead of one obvious stop, you get lots of tiny temporal pitch dips that smear into a granular-feeling texture:
- fluttering shadows
- degraded tape chorus
- spectral shiver

### Better with
- slight filter modulation before Tape Stop
- subtle wow/flutter source upstream
- noise mixed into pad

---

## Patch idea: feedback haze

### Patch
- Pad/drone → Tape Stop → delay/reverb → mixer
- Send some wet signal back, carefully, into the source chain or a feedback path
- Trigger Tape Stop occasionally with long lag

### Result
The slowed material accumulates in the effects tail and feedback path, causing:
- sinking harmonic residue
- frozen-like decays
- eerie unstable resonances

Use caution with feedback, but this can produce very unique haunted environments.

---

# Best modulation sources for each sound category

## For distorted percussion
Use:
- trigger sequencer
- burst generator
- clock divider
- stepped random to Lag CV
- accent envelope to Lag CV

### Why
You want short, rhythmic, sharply contrasting stop times.

---

## For dubstep / DnB bass
Use:
- sequencer row to Lag CV
- offbeat gate pattern to Trig
- clock multiplier/divider at CLOCK
- manual button for fills
- velocity/accent CV into Lag CV

### Why
You want repeatable but animated pitch-drop phrases.

---

## For haunting pads
Use:
- slow random voltages
- long LFOs
- sparse probabilistic triggers
- very slow external clock divisions
- manual latching mode

### Why
You want irregular, evolving temporal collapse rather than obvious rhythmic effect.

---

# Creative techniques that go beyond the manual

## 1. Audio-rate or fast CV into Lag
The manual specifies **-5V to +5V** for Lag CV. If your system allows it, try feeding:
- oscillator
- fast LFO
- chaotic CV

into Lag CV.

You may get unusual, unstable behavior depending on the internal response of the module. It may not track “cleanly,” but that’s often the point.

Potential result:
- sputtering tape lengths
- unstable glitch edges
- bizarre transient warping

## 2. Trigger from derived envelopes
Use an envelope follower or comparator on incoming audio to trigger Tape Stop only when the source exceeds a threshold.

This makes Tape Stop react dynamically to:
- loud drum hits
- bass accents
- performance intensity

Result:
- responsive, semi-self-playing destruction

## 3. Sequential switch between trigger patterns
Feed multiple different trigger sources into a switch, then route the selected one to Tape Stop TRIG.

Example sources:
- straight 8ths
- ratchets
- random gates
- manual gate button

Result:
- evolving rhythmic braking styles without changing your main patch

## 4. Use latching mode as a tension generator
In **latching mode**, one trigger starts the tape stop and another ends it.

Try:
- starting a long stop right before a drop
- letting the signal sink into near-failure
- releasing it exactly on the 1

This is especially effective on:
- drum buses
- reese basses
- pad swells
- transitions

## 5. Put Tape Stop on parallel sends
Instead of inserting it inline:
- mult source
- dry path to mixer
- wet path through Tape Stop
- optionally through extra distortion/filter/reverb

Then blend manually or with VCAs.

This gives much more control and often sounds bigger than the insert approach.

---

# Specific patch recipes

## Recipe 1: distorted industrial kick
- Kick voice → wavefolder/distortion → Tape Stop → VCA
- Clock to Tape Stop
- Trigger kick every quarter note
- Trigger Tape Stop on every 4th kick only
- Lag at 16th or 8th
- Random CV to Lag

**Sound:** collapsing, tearing kick tail with brutal texture.

---

## Recipe 2: dubstep bass choke
- Wavetable oscillator + sub → filter → distortion → Tape Stop
- Trigger bass notes from sequencer
- Trigger Tape Stop on selected syncopated notes
- Clock sync on
- Sequenced CV to Lag
- 50/50 mode enabled

**Sound:** vocal, choking, dual-pitch bass phrases.

---

## Recipe 3: neuro reese brake
- Dual detuned saws → chorus → saturation → Tape Stop → notch filter → distortion
- Sparse triggers to Tape Stop
- Long-ish lag values
- Manual extra triggers for fills

**Sound:** tearing reese with sudden engine-brake dive.

---

## Recipe 4: haunted cassette pad
- Chord source → subtle saturation → Tape Stop → chorus → huge reverb
- 50/50 mode enabled
- Slow random CV to Lag
- Very sparse trigger pattern

**Sound:** fading memory, unstable harmonic shadow, ghostly ambience.

---

## Recipe 5: broken drum bus transition
- Drum submix → Tape Stop → compressor/clipping
- Latching mode
- Clock sync enabled
- Start stop one beat before transition
- Release on downbeat

**Sound:** whole groove buckles and snaps back dramatically.

---

# Practical performance advice

## Use the Trig button live
The front panel **Trig button** is a real performance weapon:
- tap it for sudden DJ-stop gestures
- hold it in momentary mode for manual “slow and release”
- use latching mode for big transitions

## Keep one hand on Lag
The Lag knob defines whether the effect is:
- a tiny pitch dip
- a rhythmic brake
- a dramatic collapse
- a long ambient sink

Sweeping this in performance is often more musical than static settings.

## Don’t overuse it
Tape Stop is very characterful. A few strategically placed events often sound better than constant triggering, especially in bass music.

---

# Best use cases by style

## For distorted percussion
Best settings:
- clocked
- short lag
- random or accent-based lag CV
- distortion before and/or after

## For dubstep / DnB bass
Best settings:
- clocked
- sequenced lag CV
- syncopated trig pattern
- 50/50 mode
- rich harmonic bass input

## For haunting pads
Best settings:
- long lag
- sparse triggers
- slow random lag CV
- reverb after Tape Stop
- 50/50 mode or parallel mixing

---

# Final take

The **2hp Tape Stop** is most interesting when you stop treating it like a one-shot novelty and start using it as a **rhythmic pitch-collapse modulator**.

If you want:
- **distorted percussion**, use short clocked stops on transient-heavy material and vary Lag per hit
- **dubstep/DnB basslines**, sequence the Lag CV and trigger the module selectively for choked, falling bass phrases
- **haunting pads**, use long sparse triggers with 50/50 mode and huge reverb after the module

The big unlock is this:

> **Trig creates the event, Lag defines the contour, Clock makes it musical, and signal-chain placement determines whether it sounds smooth, violent, or spectral.**

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)