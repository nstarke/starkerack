# Making Sound Machines — DivSkip

- [Manual PDF](../../manuals/SKORPION_Manual.pdf)

---

[WMD Skorpion Manual (PDF)](https://wmdevices.com/cdn/shop/files/Skorpion_Manual_Rev1.00.pdf)

# WMD Skorpion modulation ideas for distorted percussion, monstrous basslines, and haunted pads

Skorpion is not just a wavefolder. It’s really a **comparator-driven waveform animation system** with a **vector core**, **per-threshold behavior**, **target sequencing**, **feedback-based slope shaping**, and **stereo widening/delay**. That means it rewards modulation much more than static knob settings.

Below I’ll focus on ways to modulate it for:
- **distorted percussion**
- **dubstep / DnB basslines**
- **haunting atmospheric pads**

I’ll also point out the most powerful modulation points and self-patching tricks from the manual.

---

# First: what matters most for sound design on Skorpion

These are the parameters that seem to matter most when patching for movement:

## 1. FOLD
Controls how hard the input is amplified against the threshold stack.  
This is the most immediate “more chaos / more aggression” control.

**Best modulation use:**
- envelopes for transient punch
- stepped CV for rhythmic changes
- audio-rate modulation for harshness

---

## 2. SLOPE
Controls how fast the vector core moves. Higher slope = more harmonic content.

**Best modulation use:**
- pitch tracking via **1V/OCT** for consistent timbre
- envelopes to make attack brighter than sustain
- LFOs for evolving harmonic motion

This is one of the biggest tone controls on the module.

---

## 3. SHIFT
Offsets the input against thresholds and creates asymmetry.  
The manual notes that **slow modulation here can create a frequency shift effect**.

**Best modulation use:**
- slow triangle/sine for movement
- envelopes for transient asymmetry
- audio-rate modulation for unstable, tearing sounds

This is especially useful for bass and pads.

---

## 4. TARGET
Determines where the vector core is trying to go:
- **5V** = more square-like
- **CLIP** = overlay with input waveform
- **SLIDERs/TRGTs** = threshold-crossing sequenced voltage destinations

**Best modulation use:**
- animated transitions between square-ish, clipping, and sequenced destinations
- external CV into **TRGT MOD**
- using **TRGTs** as a pseudo wavetable / contour source

This is one of Skorpion’s most unique sound design dimensions.

---

## 5. SHAPE + SHAPE SOURCE
SHAPE modulates SLOPE using feedback and internal signals:
- **IN**
- **OUT**
- **DELAY**
- **COUNT**
- **DIFF**
- **TRGTs**
- **DAC**
- **DIR**

This is probably the deepest sound-design section of the module.

**Best sources by vibe:**
- **OUT**: log/exp-style nonlinear feedback, great for growl
- **DIFF**: spiky, harsh, very aggressive
- **COUNT**: staircase modulation linked to threshold crossings
- **TRGTs**: per-segment waveform shaping
- **DIR**: skew and directional asymmetry
- **DELAY**: animated stereo and unstable movement

---

## 6. THLD sliders / threshold modulation
The thresholds decide where folds happen. This is huge.

You can:
- set them manually
- equalize them for more “classic wavefolder” behavior
- modulate all thresholds via **THLDs/**
- modulate threshold 1 directly via **THLD1**
- add internal threshold LFOs with Macro Setup

This is how you move from normal wavefolding into animated, comparator-chaos territory.

---

## 7. OUTPUT / WIDE / FILTERS / DELAY
The upper half of OUTPUT introduces widening and delay behavior.  
With FILTERS on, lows remain centered and highs spread, which is excellent for bass and pads.

**Use this for:**
- wide metallic percussion
- basses with mono low-end and wide top
- drifting stereo atmospheres

---

# Most powerful modulation concepts on Skorpion

Before the genre patches, here are the most important general techniques.

## A. Use envelopes on FOLD and SLOPE together
This creates a very “acoustic-mechanical” motion:
- more fold at attack
- more slope at attack
- then both decay differently

Result:
- snappy percussion
- basses with a bark on the transient
- pads that bloom and then soften

---

## B. Modulate SHIFT slowly for unstable spectral drift
Because SHIFT offsets the input against thresholds, it changes which folds happen and when.

Result:
- evolving timbre without sounding like a generic filter sweep
- very good for haunted drones and living basslines

---

## C. Use SHAPE source switching as a performance move
Even if the SHAPE amount stays similar, changing the source from:
- **OUT** to **DIFF**
- **COUNT** to **TRGTs**
- **DIR** to **DELAY**

can completely recharacterize the sound.

This is one of the best ways to get “multiple personalities” out of one patch.

---

## D. Self-patch the auxiliary outputs
Skorpion gives you:
- **ABS(IN)**
- **G(IN>0)**
- **TRGTs**
- **DIFF**
- **±G(DIR)**
- **COUNT/**
- **DAC**
- **DELAY**

These are perfect self-mod sources.

Especially useful:
- **DIFF → SHAPE CV**
- **COUNT/ or DAC → FOLD CV**
- **TRGTs → SHIFT CV**
- **DELAY → SHAPE or TARGET modulation**
- **±G(DIR) → something external**, or into utilities for rhythmic switching

---

## E. Use TRGTs like a hidden sequencer
The manual explicitly says the 8 targets form an 8-step voltage-controlled sequencer.

That means you can:
- shape the folded waveform in segments
- output TRGTs to modulate external modules
- modulate all targets together with the **TRGTs input**
- choose target order:
  - **SEQ** = by count of active thresholds
  - **TIED** = by most recently crossed threshold

This is extremely good for bass growls and animated pads.

---

## F. Use HALT strategically
- **HALT jack** stops the vector core at its current voltage
- **HALT IF TARG=0** lets target segments freeze when their target is 0

This can create:
- square-like segments
- abrupt rhythmic stutters
- frozen spectral moments
- gated, robotic bass articulation

Very powerful for aggressive sounds.

---

# Patch ideas for distorted percussion

---

## 1. Broken industrial kick / tom
**Goal:** a punchy, crushed, metallic kick or tom with folding grit.

### Patch
- Sine or triangle oscillator into **IN**
- Pitch envelope on oscillator if desired
- Envelope to **FOLD CV**
- Short decay envelope to **SLOPE CV**
- Set **TARGET** somewhere between **5V** and **CLIP**
- **SHAPE source = DIFF** or **OUT**
- OUTPUT around wet, not yet too wide

### Modulation idea
- Make **FOLD envelope** slightly longer than **SLOPE envelope**
- Use **SHIFT** slightly off noon for asymmetry
- Turn on **SYNC = HARD** for consistent attack/reset behavior
- Try **HALT IF TARG=0** with one or two targets at zero if using SLIDER target mode

### Why it works
The attack gets fast, bright, and nonlinear, then relaxes into a lower harmonic sustain. DIFF-based shape makes the transient nasty and sharp.

### Make it nastier
- Send **DIFF output** back into **SHAPE CV**
- Modulate **TRGT MOD** with a click, noise burst, or another percussion voice
- Use **CLIP jack** with a different source than the input

Using another sound in CLIP is especially good for weird percussion because the output overlays against that foreign contour.

---

## 2. Snare / clap annihilator
**Goal:** noise-heavy, crispy, tearing snare layers.

### Patch
- Noise or noise+oscillator mix into **IN**
- **FOLD** high
- **SLOPE** medium-high
- **SHIFT** slightly positive or negative
- **TARGET = CLIP**
- Feed a separate sharp source to **CLIP**, like:
  - short square click
  - rimshot signal
  - another oscillator
- **SHAPE source = COUNT** or **DIFF**
- OUTPUT into **WIDE**, FILTERS on

### Modulation
- Envelope to **FOLD**
- Fast random or stepped modulation to **SHIFT**
- Threshold LFO amount via Macro Setup at subtle depth
- Slow modulation of **OUTPUT** between WET and WIDE

### Result
The threshold-crossing behavior turns noise into ripped layers of transient detail, while stereoized highs make the snare sound wider without losing low-end center.

---

## 3. Hi-hats / cymbal shatter patch
**Goal:** glitchy, metallic, animated hats.

### Patch
- Bright noise, FM metallic source, or high triangle into **IN**
- **EQUALIZE THLDs = ON** for more classic evenly-spaced folding
- High **SLOPE**
- **SHAPE source = COUNT** or **DAC**
- OUTPUT above noon into WIDE
- FILTERS on

### Modulation
- Very short envelope to **FOLD**
- Fast LFO to **SHIFT**
- Slow LFO to **SHAPE**
- Internal threshold LFOs enabled in Macro Setup
- Optional: **G(IN>0)** or **±G(DIR)** to clock something external that modulates Skorpion back

### Result
COUNT and DAC create stepped modulation tied to active thresholds, giving a metallic digital-meets-analog chatter that is excellent for hats.

---

## 4. Glitch percussion with HALT
**Goal:** stop-start robotic percussion and fractured impacts.

### Patch
- Percussive source into **IN**
- Patch gates or audio-rate square wave into **HALT**
- Set **TARGET = SLIDERs**
- Put some **TRGT sliders** at zero
- Enable **HALT IF TARG=0**
- SHAPE source = **TRGTs** or **DIR**

### Modulation
- Modulate **TARGET pot**
- Modulate **THLDs/** with a rhythmic CV
- Switch **TARGET ORDER** between **SEQ** and **TIED**

### Result
The vector core freezes on certain segments, creating abrupt flat spots, gated edges, and machine-gun contour distortions.

This is excellent for IDM-ish percussion or neurofunk drum mangling.

---

# Patch ideas for dubstep / drum & bass basslines

---

## 1. Classic growl bass, but stranger
**Goal:** a bass that snarls and changes internal shape beyond ordinary filter/FM growls.

### Patch
- Saw, square, or complex oscillator into **IN**
- Patch pitch CV to oscillator and to **1V/OCT** on Skorpion
- **FOLD** medium-high
- **SLOPE** medium
- **SHIFT** near noon
- **TARGET** between **SLIDERs** and **CLIP**
- **SHAPE source = OUT**
- OUTPUT around wet or slightly into wide with FILTERS on

### Modulation
- LFO or envelope to **SHIFT**
- Envelope to **FOLD**
- Different envelope to **SLOPE**
- Slow CV to **TARGET**
- Use Macro LFO on **SHAPE** or **SLOPE**

### Why it works
1V/OCT keeps the slope behavior musically consistent across notes. OUT-based shape gives organic nonlinear feedback, which is great for talking/growling basses.

---

## 2. Neuro bass / tearing reese mutation
**Goal:** moving bass with vocal tearing, internal segment changes, and asymmetry.

### Patch
- Detuned saw pair or Reese source into **IN**
- **TARGET = SLIDERs**
- Set 8 TRGT sliders to alternating positive/low/zero-ish contour shapes
- **TARGET ORDER = TIED** for more chaotic selection
- **SHAPE source = TRGTs**
- **SHIFT** slightly offset from noon
- OUTPUT in FILTERS mode, slightly wide

### Modulation
- Slow LFO to **SHIFT**
- Envelope follower or synced LFO to **THLDs/**
- **TRGT MOD** with an LFO, envelope, or external audio source
- **DIFF output → SHAPE CV**
- Optional: **DELAY output → TRGT MOD** or **SHAPE CV**

### Result
Each threshold-crossing can push the vector core toward a different destination, while SHAPE sourced from TRGTs changes the slope segment-by-segment. This gives highly articulated, speech-like growls.

---

## 3. Talking wobble bass without a filter
**Goal:** vowel-like movement using threshold and target animation rather than standard filter sweeps.

### Patch
- Rich oscillator into **IN**
- **TARGET = SLIDERs**
- Create a non-linear TRGT pattern with valleys and peaks
- **SHAPE source = COUNT** or **DAC**
- **EQUALIZE THLDs = XOR** so CV can dynamically switch equalized/non-equalized threshold behavior
- OUTPUT with FILTERS on

### Modulation
- Sync’d LFO to **THLDs/**
- Another LFO to **SHIFT**
- Envelope to **FOLD**
- Sequencer row or stepped random to **TRGTs input**
- Gate pattern into **EQ THLDs jack** to alternate classic wavefolder vs irregular threshold map

### Result
The bass articulates in a vocal-ish way because threshold activation patterns change, not just brightness. Toggling equalized thresholds can sound like switching between different “mouth shapes.”

---

## 4. Over-the-top DnB bass stab
**Goal:** hard transient, aggressive midrange, wide top, mono low end.

### Patch
- Oscillator or bass chord source into **IN**
- Pitch to oscillator and **1V/OCT**
- **SYNC = HARD**
- **TARGET = 5V** or near 5V
- **SHAPE source = DIFF**
- **FOLD** high
- **SLOPE** high
- OUTPUT into upper half, **FILTERS** engaged

### Modulation
- Fast decay envelope to **SLOPE**
- Medium decay envelope to **FOLD**
- Short accent envelope to **SHIFT**
- Use **COUNT/** or **DAC** out to modulate an external VCA/filter in parallel
- Slow LFO on OUTPUT amount for evolving width

### Result
Very strong square-ish, ripping attack with stable low fundamentals and stereo spread in the upper band.

---

## 5. Audio-rate FM-style brutality
**Goal:** harsh, screeching, modern bass destruction.

### Patch
- Oscillator into **IN**
- Another oscillator or bright audio source into:
  - **TRGT MOD**
  - or **SHIFT CV**
  - or **THLDs/**
- **SHAPE source = DIFF** or **OUT**
- **TARGET = CLIP** or between CLIP and SLIDERs

### Modulation
- Audio-rate modulation to **SHIFT** is especially wild
- Audio-rate into **THLDs/** changes threshold map at audio speeds
- Audio-rate signal into **CLIP** replaces the clipping reference with another waveform

### Result
Skorpion becomes a bizarre comparator/FM/wavefold hybrid. This is ideal for screaming fills, transitions, or extreme basses.

---

# Patch ideas for haunting atmospheric pads

---

## 1. Evolving ghost pad
**Goal:** soft but uncanny harmonic movement, slowly shifting asymmetry, wide stereo top.

### Patch
- Slow chord, drone, or detuned oscillator stack into **IN**
- **DRY IF NO THLDs = ON**
- Moderate **FOLD**
- Lower **SLOPE**
- **SHIFT** at or near noon
- **TARGET** between **CLIP** and **SLIDERs**
- **SHAPE source = OUT** or **DELAY**
- OUTPUT in upper half, FILTERS on

### Modulation
- Very slow LFO to **SHIFT**
- Very slow LFO to **SHAPE**
- Very slow modulation to **TARGET**
- Internal Macro envelope controlling threshold LFOs with long attack/release
- Use Macro Setup to create extremely slow movement over minutes

### Why DRY IF NO THLDs matters
When heavily modulating FOLD or threshold conditions, it ensures you still get signal and can create gentle transitions between dry-following and folded states. That’s very useful for atmospheric work.

---

## 2. Haunted shimmer cloud
**Goal:** unstable stereo bloom with delayed spectral feedback.

### Patch
- Harmonic source into **IN**
- **OUTPUT** above noon into WIDE
- **FILTERS** on
- **SHAPE source = DELAY**
- **TARGET = CLIP**
- Use a soft source, like triangle/pulse blend or processed field recording oscillator texture

### Modulation
- Very slow triangle to **SHIFT**
- Slow CV to **OUTPUT**
- Slow random to **FOLD**
- Optional: patch **DELAY output** externally through reverb and bring it back to **CLIP** or **TRGT MOD**

### Result
The delay-derived shape source creates motion that feels spectral and ghostly rather than obviously LFO’d.

---

## 3. Segmented pad with hidden melody inside
**Goal:** a drone where different harmonic segments emerge as thresholds are crossed.

### Patch
- Sustained oscillator/chord into **IN**
- **TARGET = SLIDERs**
- Set TRGT sliders to a musically related contour
- **TARGET ORDER = SEQ** for more predictable motion
- **SHAPE source = TRGTs**
- **SLOPE** moderate
- **FOLD** low to medium

### Modulation
- Slow envelope or LFO to **THLDs/**
- Slow modulation to **SHIFT**
- Optional: modulate all targets using **TRGTs input**
- Use Macro threshold LFOs with very slow rates

### Result
The pad slowly animates across internal “zones,” almost like a wavetable scan controlled by threshold activity.

---

## 4. Frozen sorrow drone
**Goal:** suspended, broken, nearly-static texture with occasional motion.

### Patch
- Drone source into **IN**
- **TARGET = SLIDERs**
- Put several target sliders at zero
- Enable **HALT IF TARG=0**
- **SHAPE source = DIR** or **OUT**
- **SYNC = SOFT**

### Modulation
- Sparse gates to **HALT**
- Slow CV to **SHIFT**
- Very slow CV to **SLOPE**
- Slight movement on **THLDs/**

### Result
Parts of the waveform stall, hang, and then resume, giving eerie suspended harmonics and frozen emotional texture.

---

# Best self-patching tricks

These are especially powerful on Skorpion.

## 1. DIFF → SHAPE CV
Probably one of the best aggressive patches.

**Sound:**
- sharper transients
- unstable, spiky, tearing harmonics
- great for bass and percussion

---

## 2. TRGTs output → SHIFT CV
Lets the target sequencer also bias threshold crossing asymmetry.

**Sound:**
- internal recursive animation
- basses that seem to “talk”
- pads with subtle contour drift

Attenuate this if possible.

---

## 3. COUNT/ or DAC → FOLD CV
Since these reflect active thresholds, the amount of threshold activity changes fold amount.

**Sound:**
- dynamic harmonic escalation
- responsive growl
- self-energizing textures

**COUNT/** is more obvious.  
**DAC** is subtler and often more musical.

---

## 4. DELAY → SHAPE CV or TRGT MOD
Especially good when OUTPUT is in WIDE range.

**Sound:**
- spectral smear
- unstable stereo movement
- eerie self-related animation

Excellent for pads and strange percussion.

---

## 5. ABS(IN) → external modulation destination
Use ABS(IN) as a derived envelope-ish audio modulation source outside Skorpion, then send that back in somewhere else.

**Good return points:**
- FOLD CV
- SHIFT CV
- TRGT MOD
- THLDs/

---

## 6. G(IN>0) or ±G(DIR) for rhythmic logic
These are great utility outputs.

Use them to:
- trigger envelopes elsewhere
- switch CV paths
- clock logic
- derive rhythmic gates from the waveform itself

Then route those back to Skorpion or other modules.

---

# How to use the Macro Setup musically

The internal macro section is easy to overlook, but it’s very useful for “alive” patches.

## Best uses for distorted percussion
- Set short-to-medium Macro attack/release
- Use threshold LFO amount low-to-medium
- Put hardware normal modulation on **FOLD** and **SLOPE**
- Trigger Macro ENV per hit or phrase

This makes repeated percussion evolve slightly while staying coherent.

---

## Best uses for basslines
- Put **SHIFT** in LFO mode
- Put **SHAPE** in ENV mode
- Put **SLOPE** in LFO or ENV mode depending on whether you want wobble or punch
- Trigger Macro ENV from sequence accents

This gives a bass patch movement even if you don’t have extra external modulators.

---

## Best uses for pads
- Long attack and release on Macro ENV
- Slow threshold LFO rate
- Subtle amount on threshold LFOs
- Put **SHIFT** and **SHAPE** in LFO mode
- Put **FOLD** in ENV mode if you want bloom

The result is slow spectral emergence that feels composed rather than random.

---

# Switch settings that dramatically change character

## EQUALIZE THLDs
- **ON**: more classic wavefolder, more predictable, good for percussion and stable basses
- **OFF / JACK-controlled**: more unique irregularity, better for experimental bass/pad work
- **XOR**: excellent for rhythmic switching between classic and weird

---

## SYNC
- **HARD**: tight attacks, consistent bass transients, percussive precision
- **SOFT**: more organic, smeared resets, nice for pads
- **X**: freer, more chaotic behavior

---

## TARGET ORDER
- **SEQ**: more repeatable, phrase-like, musical
- **TIED**: more reactive and less predictable, good for wild basses and chaotic percussion

---

## OUTPUT SWITCH
- **DC**: rawest signal
- **FILTERS**: centered lows + widened highs, best for bass and spacious pads

---

# Three complete recipe patches

## Recipe 1: “Neuro Snarl Bass”
- Reese oscillator into IN
- Pitch CV also to 1V/OCT
- TARGET = SLIDERs
- TARGET ORDER = TIED
- SHAPE source = TRGTs
- SHAPE amount moderate positive
- FOLD medium-high
- SLOPE medium
- SHIFT slightly off noon
- OUTPUT in FILTERS wide mode
- DIFF → SHAPE CV
- Slow LFO → SHIFT
- Envelope → FOLD
- Envelope → SLOPE
- TRGT MOD from another oscillator or envelope

**Result:** vocal tearing, unstable phrase-like bass with stereo aggression and centered weight.

---

## Recipe 2: “Destroyed Techno Percussion”
- Sine or triangle VCO into IN
- Hard pitch envelope on oscillator
- HARD SYNC on Skorpion
- TARGET near 5V
- SHAPE source = DIFF
- Short env → SLOPE
- Slightly longer env → FOLD
- Random stepped CV → SHIFT
- CLIP fed from noise burst or another percussive source
- OUTPUT mostly wet

**Result:** industrial kick/tom/snare territory with brutal attack and strange overtone sprays.

---

## Recipe 3: “Cathedral Ghost Pad”
- Two detuned triangles/chord source into IN
- DRY IF NO THLDs on
- TARGET between CLIP and SLIDERs
- SHAPE source = DELAY
- SOFT SYNC
- OUTPUT wide with FILTERS
- Long Macro attack/release
- Threshold LFO amount subtle
- Slow LFO → SHIFT
- Slow LFO → TARGET
- DELAY → SHAPE CV
- External reverb after OUT L/R

**Result:** drifting, mournful, haunted stereo bloom with animated harmonic fog.

---

# Practical tips

## Use attenuation
Skorpion seems very sensitive to modulation depth. Many of the best sounds will come from **small amounts** of CV, especially on:
- SHIFT
- SHAPE
- THLDs/
- TRGT MOD

---

## Keep SHIFT near noon when exploring HALT
The manual specifically hints this gives best results, because SHIFT is summed with IN after FOLD.

---

## Use 1V/OCT for pitched bass work
The manual notes it controls slope and is necessary for equal timbre across different notes. If you want bass patches to stay consistent across a line, patch it.

---

## Don’t ignore CLIP input
This is one of the coolest features for unconventional sounds. Replacing the input-normalled clip signal with:
- drums
- another oscillator
- voice
- field recording-derived signal

can radically alter the folding behavior.

---

## WIDE is not just “stereo”
It also gives access to the delay behavior. Since DELAY can be used as a modulation-related source and SHAPE source, OUTPUT position can indirectly change timbre, not just width.

---

# Best modulation destinations by genre

## For distorted percussion
1. FOLD
2. SLOPE
3. SHAPE
4. TARGET / TRGT MOD
5. HALT

## For basslines
1. SHIFT
2. SHAPE
3. TARGET / TRGTs
4. THLDs/
5. OUTPUT wide/filter balance

## For atmospheric pads
1. SHIFT slow modulation
2. SHAPE source = DELAY / OUT / TRGTs
3. THLD LFOs via Macro Setup
4. TARGET slow modulation
5. OUTPUT into WIDE with FILTERS

---

# Final takeaway

The most unique sounds from Skorpion will usually come from **modulating relationships**, not just single parameters. The best pairings are:

- **FOLD + SLOPE** for transient character
- **SHIFT + THLDs/** for moving asymmetry and fold topology
- **TARGET + SHAPE source** for changing the actual contour logic
- **OUTPUT/DELAY + SHAPE** for spacious spectral motion
- **DIFF / COUNT / TRGTs self-patching** for recursive complexity

If you want, I can also turn this into:
1. a **quick-start cheat sheet**,  
2. **10 specific patch recipes with knob positions**, or  
3. a **self-patching-only guide for Skorpion**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)