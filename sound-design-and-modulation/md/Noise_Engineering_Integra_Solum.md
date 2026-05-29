# Noise Engineering — Integra Solum

- [Manual PDF](../../manuals/Integra Solum Manual - Noise Engineering Documentation.pdf)

---

[Manual / Source](https://manuals.noiseengineering.us/is/)

# Noise Engineering Integra Solum: modulation ideas for aggressive percussion, basslines, and dark atmospheres

Integra Solum is not a sound source by itself; it’s a **dual rotating clock divider / trigger generator**. That means its real power is in how it **animates other modules**: envelopes, LPGs, VCAs, switches, sequential switchers, filters, distortion, sample-and-holds, drum voices, and modulation sources.

The module gives you:

- **2 independent divider sections**
- **8 trigger outputs per side**
- **independent or shared clocking/reset**
- **Shift/Offset rotation** per side
- **3 main modes**
  - `/2N` = powers-of-two divisions
  - `N` = sequence of eight
  - `/2N+1` = odd divisions
- **Wack mode** for randomized trigger behavior

## Important behavior to exploit

From the manual:

- Clock responds to a rising edge around **3.3 V**
- One clock can **normal to both sides**
- Outputs update with about **70 µs latency**
- Reset can be used to **re-align patterns**
- Output triggers are about **0–5 V**, triggering around **3.4 V**
- **Shift** rotates which jack is considered first in the cycle
- **Wack mode** changes the mode behavior:
  - `/2N` becomes **probabilistic divide by two**
  - `N` becomes **one random trigger per step**
  - `/2N+1` makes **each output independently 50% likely** on each clock

That means this module excels at:
- stable rhythmic scaffolding
- rotating accents
- bursty probabilistic events
- clock-related modulation changes
- controlled chaos

---

# Core patching mindset

Think of Integra Solum as a **rhythm brain** for:
- **when a sound happens**
- **when a modulation changes**
- **when distortion amount jumps**
- **when a filter snaps open**
- **when a voice changes pitch**
- **when a delay or reverb gets hit**

For the styles you asked about, the magic is usually:

1. **Use one side for note or drum timing**
2. **Use the other side for modulation timing**
3. Rotate one or both sides with **Shift**
4. Periodically **Reset** for phrase structure
5. Use **Wack mode** selectively for controlled instability

---

# 1. Distorted percussive sounds

## A. Rotating industrial kick/snare pattern

### Patch
- Master clock into one **Clock** input so both sides run
- Side A in **N mode**
- Patch several outputs from Side A to:
  - kick trigger
  - snare trigger
  - envelope trigger for a VCA’d noise burst
  - envelope trigger for a click transient
- Side B in `/2N+1` or Wack `/2N+1`
- Use Side B outputs to trigger:
  - distortion CV changes
  - filter envelope retriggers
  - wavefolder strike or VCA pings
  - a sequential switch selecting different percussion sources

### Why it works
Side A gives a more structured pulse stream. Side B creates asymmetry and movement. If Side B controls timbre rather than note timing, your percussion sounds like it is being “re-synthesized” each hit.

### Best modulation targets
- **filter cutoff CV**
- **resonance CV** in tiny amounts
- **distortion amount**
- **wavefolder symmetry/fold**
- **sample rate / bit depth** on a crusher
- **decay time** of percussion envelopes
- **switches** that alternate between sine/noise/FM transients

### Trick
Take one output from Side B and send it to a **very fast decay envelope** controlling VCA level into a distortion. Some hits slam harder, creating uneven clipped transients. That produces very alive, broken-machine percussion.

---

## B. Broken DnB hats with probabilistic fill behavior

### Patch
- Fast clock, e.g. 1/16 or faster
- Side A in `/2N`
- Trigger closed hats from a faster division
- Trigger open hats from a slower division
- Put Side B in **Wack `/2N`** or **Wack `N`**
- Use Side B random triggers for:
  - extra hat accents
  - burst generator trigger
  - short noise stabs
  - panning modulation envelope

### Sound design tip
Send hats/noise through:
- HPF
- distortion
- very short room reverb
- compressor/saturator

Now use Integra Solum to trigger **different envelope shapes** for the same noise source. That creates metallic, tearing top-end.

### Trick
Patch two outputs to a **logic OR** or mixer before a hat trigger input. Then rotate **Shift**. You’ll get changing composite rhythms without repatching.

---

## C. Kick with unstable “speaker-rip” attack

### Patch
- Use a kick voice or sine oscillator with pitch envelope
- Side A triggers the kick
- Side B triggers:
  - an extra click envelope
  - a super-short FM envelope to the oscillator pitch or phase modulation input
  - distortion wet/dry or drive CV

### Best mode
- Side A: `/2N` or `N`
- Side B: Wack `N` or `/2N+1`

### Why it gets nasty
If the attack transient and distortion amount are triggered independently but clock-related, you get those **ripped-cone**, overdriven, neuro-style drum impacts.

---

# 2. Dubstep / drum & bass bassline generation

Integra Solum won’t generate pitch directly, but it can create the **event structure** for bass modulation. That’s often more important than the actual oscillator.

## A. Reece / neuro bass motion network

### Patch
Use one bass voice:
- 2 detuned oscillators or a supersaw/reese source
- lowpass or bandpass filter
- distortion/wavefolder
- VCA
- maybe phaser/flanger

### Timing architecture
- Side A triggers your **main amp envelope**
- Side B triggers changes to modulation destinations:
  - sample-and-hold for filter cutoff
  - sequential switch for different envelope depths
  - burst or extra envelope for FM spikes
  - logic module to combine triggers into growl phrases

### Suggested mode setup
- Side A in `N` for regular phrase stepping
- Side B in `/2N+1` for uneven modulation accents
- Occasionally use **Wack `N`** for random “which step gets movement”

### Great CV chains
Use Side B trigger outputs to trigger:
- **sample & hold** sampling random voltage for filter cutoff
- **track-and-hold** on wavetable position
- **sequential switch** choosing one of 4 modulation sources
- **envelope generator** with varying decay amounts
- **clocked slew** for stepped wobble contours

### Result
You get bass notes that remain rhythmically anchored while their tone mutates every few steps: classic **talking / snarling / neuro** movement.

---

## B. Half-time dubstep wobble with rotating accents

### Patch
- Slow host clock synced to tempo
- Side A in `/2N`
- Use one output for note gate / VCA envelope
- Use slower outputs for filter plucks and sub drops
- Side B in `N`
- Patch different Side B outputs to:
  - LFO reset
  - envelope retrigger for filter
  - accent VCA
  - distortion boost
  - delay send gate

### Shift strategy
Turn **Shift** on Side B during playback. This rotates which trigger output occurs first, so the phrase changes but remains grid-locked.

### Why this is especially good
Instead of modulating the bass continuously with one LFO, Integra Solum gives you **discrete rhythmic gestures**. That often sounds more modern and intentional in dubstep.

### Patch extension
Use one trigger to **reset the LFO phase** on certain steps only. That creates “wobble that restarts” on selected hits, which is a strong bass design trick.

---

## C. DnB rolling bass with ghost triggers

### Patch
- Fast clock from your sequencer or Pam’s-style source
- Side A in `/2N+1`
- Main bass envelope on one output
- Side B in **Wack `/2N`**
- Use Side B outputs for:
  - short muting envelopes to chop the bass
  - FM spikes
  - notch filter modulation hits
  - pitch envelope retriggers for zaps

### Sound design stack
- saw/reese source
- bandpass into distortion
- second filter after distortion
- sub sine layered underneath
- VCA controlled by Side A
- additional “interrupt” VCA controlled by Side B

### Why it sounds DnB
The “interrupt” VCA creates those machine-gun internal articulations and ghost syncopations inside a sustained bass phrase.

---

## D. Triggered modulation matrix for basses

This is one of the best uses of Integra Solum.

### Patch
Take 4–6 outputs and assign each to trigger one event:
- sample random cutoff
- switch distortion type
- retrigger transient envelope
- open parallel bandpass
- trigger short reverb send burst
- switch oscillator sync on/off via VCA or logic

Then:
- Side A = rhythm skeleton
- Side B = modulation decorations

The bass becomes **structurally repeatable but timbrally unstable**, which is exactly where a lot of advanced bass music lives.

---

# 3. Haunting atmospheric pad sounds

Pads benefit less from many triggers directly hitting the audio path, and more from Integra Solum creating **slow structural evolution**.

## A. Triggered pad animation

### Patch
Create a pad voice:
- 1–3 oscillators or a drone source
- long attack/release envelope or sustained gate
- lowpass/bandpass filter
- chorus/phaser/reverb/delay

### Integra Solum role
Use very slow clocking.

- Side A in `/2N`
- Trigger:
  - long envelope retriggers
  - filter contour pulses
  - VCA swells
  - reverb send accents
- Side B in `N` or Wack `N`
- Trigger:
  - sample-and-hold for subtle pitch drift
  - random panning changes
  - wavefolder amount changes
  - switching among modulation routings

### Why it works
Pads become eerie when their changes happen **discretely but infrequently**. Integra Solum can create those phrase-level shifts cleanly.

---

## B. “Breathing haunted choir” patch

### Patch
- Very slow master clock
- Side A in `N`
- Use one output every few clocks to retrigger a **long envelope**
- Use another output to briefly increase **filter resonance**
- Use another to send a burst to **reverb freeze / shimmer / feedback VCA**

- Side B in Wack `N`
- Each random trigger step controls:
  - slight FM amount burst
  - sample-and-hold on wavetable position
  - delayed sub-octave swell
  - noise layer into the pad

### Result
The pad seems to inhale, shift tone, and occasionally reveal ghost overtones.

---

## C. Dark evolving drone with reset phrasing

### Patch
- Clock Side A and Side B from the same slow clock
- Put one side in `/2N`, the other in `/2N+1`
- Patch outputs to:
  - two different envelope generators
  - one switch selecting filter modes
  - one strike to a resonator mixed beneath the pad
  - one trigger to reverse or clock a delay/reverb modulation source if available

Then periodically **Reset** both sides manually or from a sequencer phrase reset.

### Why reset matters
Without reset, the interaction slowly drifts into long evolving forms. With periodic reset, the atmosphere gets a recurring “haunting motif.”

---

# Best mode choices by goal

## For distorted percussion
- **`N`**: best for linear, stepped, rotating drum lines
- **`/2N+1`**: best for asymmetrical industrial rhythms
- **Wack `/2N+1`**: best for explosive glitch percussion and metallic chaos

## For basslines
- **`N`**: strong for phrase-locked modulation events
- **`/2N`**: good for halftime and predictable wobble scaffolding
- **Wack `N`**: great for inserting random motion while keeping one event per step
- **Wack `/2N`**: good for unstable accents and ghost modulation

## For pads
- **`/2N`** at slow clocks: best for broad structural breathing
- **`N`**: useful for orderly long-form rotation
- **Wack `N`**: subtle haunted unpredictability

---

# Shift/Offset performance techniques

The **Shift** control is one of the most musically important features.

Because it rotates the outputs, you can repurpose the same patch into many patterns without moving cables.

## Great uses of Shift
- Rotate which drum gets the downbeat
- Move accents around a bass phrase
- Change which modulation occurs first in a cycle
- Reframe a pad’s sequence of tonal changes

## Performance idea
Patch 4–8 outputs into a network of:
- triggers to drums
- modulation retriggers
- switch advances
- random sample clocks

Then perform with only:
- **mode switch**
- **Shift**
- **Reset**

This gives dramatic variation with low patch complexity.

---

# Wack mode: where the weirdness lives

Wack mode is especially useful for the genres you mentioned.

## Wack `/2N`
- Great for humanized or unstable accents
- Excellent for broken hats, ghost snares, crackle percussion
- Good for bass timbre changes that shouldn’t happen every cycle

## Wack `N`
- One random trigger each step
- Great for selecting one of many timbral events
- Very useful for “one thing changes each beat” bass animation
- Excellent for haunted pad articulation

## Wack `/2N+1`
- Wildest setting
- Dense trigger clouds
- Perfect for glitch percussion, FM burst clusters, reverb splashes, and chaotic control events
- Use with attenuated modulation or logic if it becomes too busy

---

# Advanced patch ideas

## 1. Distortion scene switching
Use Integra Solum to trigger a sequential switch that changes:
- clean path
- overdrive path
- wavefold path
- bitcrush path

Same sound source, different processing per trigger = massive rhythmic timbral variation.

## 2. Triggered FM spikes
Take one output to a very short decay envelope controlling FM amount on an oscillator.  
This is amazing for:
- punchy kicks
- tearing bass growls
- ghostly pad overtones

## 3. Parallel percussion architecture
Use different outputs to hit:
- body layer
- click layer
- noise layer
- resonator layer

Then mix them. As Shift rotates, the composite drum identity changes.

## 4. Bass articulation by selective muting
Instead of only triggering the bass on/off, use some Integra Solum outputs to trigger a second envelope that briefly **ducks** the bass with a VCA.  
This creates internal syncopation and stutter-groove.

## 5. Reverb and delay as instruments
Trigger short envelopes that open VCAs feeding effect sends:
- percussion trigger opens reverb send only on selected hits
- bass trigger opens delay send only on phrase endings
- pad trigger splashes shimmer reverb randomly

This gives a very cinematic, haunted space.

---

# Practical patch recipes

## Recipe 1: Neuro snare engine
- Side A `N`: trigger snare body
- Another Side A out: trigger noise burst
- Side B Wack `/2N`: trigger distortion boost
- Another Side B out: trigger bandpass envelope
- Rotate Shift until groove locks

Result: unstable tearing snare with changing transient aggression.

## Recipe 2: Dubstep bass growl
- Side A `/2N`: trigger amp envelope
- Side B `N`: trigger sample-and-hold for filter cutoff
- Another Side B out: trigger FM spike envelope
- Another Side B out: trigger delay-send accent
- Reset every 1 or 2 bars

Result: consistent groove with mutating growl character.

## Recipe 3: Rolling DnB reese
- Fast clock
- Side A `/2N+1`: trigger VCA chopper
- Side B Wack `N`: one random modulation event per step
- Modulation events:
  - notch sweep
  - distortion gain jump
  - phaser feedback rise
  - transient pitch jab

Result: rolling, complex, forward-moving bass texture.

## Recipe 4: Haunted pad
- Slow clock
- Side A `/2N`: long envelope retriggers
- Side B Wack `N`: random shimmer, filter swell, or pitch-drift resample
- Heavy reverb and stereo modulation
- Occasional manual Reset

Result: drifting, ghostly, semi-repeating ambient texture.

---

# Things to watch out for

- Integra Solum outputs are **triggers**, not continuous CV shapes.
  - For richer modulation, send triggers to:
    - envelopes
    - function generators
    - sample-and-holds
    - switches
    - logic
- If a patch gets too chaotic, reduce complexity by:
  - using only 2–4 outputs per side
  - slowing the clock
  - using reset every bar or phrase
  - moving randomization to timbre, not note timing
- If your target module needs hotter gates, check whether 5 V triggers are sufficient. Usually they are in Eurorack.

---

# Best companion modules for Integra Solum

It pairs especially well with:
- **envelope/function generators**
- **VCAs**
- **distortion/wavefolders**
- **sample & hold**
- **sequential switches**
- **logic modules**
- **clock multipliers/dividers**
- **filters with CV over resonance/cutoff**
- **burst generators**
- **effects with CV-able send or parameters**

If you want, I can also give you:

1. a **10-patch performance cheat sheet** for Integra Solum,  
2. a **genre-specific patch list** for dubstep vs DnB vs dark ambient, or  
3. a **“what to patch each of the 16 outputs to” template**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)