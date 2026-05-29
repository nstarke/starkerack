# Buchla and Tiptop Audio — 248t

- [Manual PDF](../../manuals/Buchla_&_Tiptop_Audio_248t.pdf)

---

[248t MARF Manual PDF](https://tiptopaudio.com/manuals/248t/Buchla_248_Manual_1977.pdf)

# Tiptop/Buchla 248t MARF: modulation ideas for distorted percussion, basslines, and atmospheric pads

The **248t MARF** is not just a sequencer. It is a **dual arbitrary CV/event generator** with per-stage control over:

- pitch/CV
- timing
- quantization
- glide/slope
- pulse outputs
- stop/sustain/enable behavior
- stage addressing
- external CV substitution

That means the most interesting results happen when you stop thinking of it as “16-step melody” and start thinking of it as a **programmable modulation brain**.

A big strength of the 248t is that it can generate:
- **pitched CV**
- **timing CV**
- **gates/pulses**
- **reference ramps**
- **stage-addressed movement**
- **externally injected CV per stage**

Those are perfect ingredients for aggressive rhythmic sound design and evolving textures.

---

# Quick mental model of what matters most

From the manual, the most creatively useful features are:

- **Two independent Function Generators (FG1 and FG2)**  
  Each can read the same 16 stages differently.

- **Per-stage voltage programming**
  - **Quantize / Continuous**
  - **Stepped / Sloped**
  - **Range: Full / Half / Limited**
  - **Source: Internal / External**

- **Per-stage timing programming**
  - selectable time ranges
  - **time source can be Internal or External**
  - each stage has its own interval time slider

- **Per-stage operating behaviors**
  - **Stop**
  - **Sustain**
  - **Enable**
  - **First / Last** loop points

- **Outputs**
  - ART pitch output
  - analog voltage output
  - time output
  - pulse 1 / pulse 2
  - all-pulses output
  - reference output (downward ramp over stage duration)

This gives you a module that can act like:
- a sequencer
- a clock divider / irregular rhythm source
- a CV animator
- a gated modulation matrix
- a patch-programmable phrase generator

---

# First: the best modulation mindset for the 248t

To get unique sounds, use the MARF in these three ways:

## 1. Use one FG for notes, the other FG for motion
For example:
- **FG1** = pitch sequence to oscillator
- **FG2** = filter cutoff, wavefolder amount, distortion tone, VCA decay, FM amount, sample rate, etc.

This is the easiest route to aggressive bass and evolving pads.

## 2. Use external CV inputs A/B/C/D as “modulation layers”
The manual says a stage can use **external CV instead of internal voltage/time settings**. That is huge.

This means stage-by-stage you can decide:
- use the slider value
- or swap in some external modulation source

So one sequence can selectively “invite in”:
- LFO bursts
- random voltage
- envelope output
- another sequencer
- audio-rate oscillator for chaos

That’s where the MARF gets weird.

## 3. Program timing as much as pitch
A lot of people use sequencers only for pitch. On the MARF, **time itself is compositional**.

Use per-stage interval time plus:
- stop
- sustain
- enable
- external time source
- global time multiplier

That creates:
- staggered grooves
- syncopated broken basslines
- choking percussion
- unstable evolving drones
- pseudo-granular rhythmic phrasing

---

# Best 248t features for your requested sound categories

---

# 1. Distorted percussive sounds

For percussion, the MARF excels at making **non-uniform trigger and modulation structures**.

## Core idea
Use the 248t to separately control:
- when a hit happens
- how long the hit lasts
- what its pitch/timbre is
- whether that hit is normal, accented, gliding, or externally modulated

## Great patch architecture
- **FG1 voltage out** → oscillator pitch / drum voice pitch / filter ping frequency
- **Pulse 1** → envelope trigger for VCA or LPG
- **Pulse 2** → accent path, distortion enable, wavefolder CV, second envelope, or noise burst VCA
- **Reference output** → directly to LPG CV for natural decay-ish per-hit contour
- **FG2 voltage out or time out** → modulate distortion tone / filter cutoff / FM amount

## Why this works
The manual notes:
- each stage can have **two independent pulse outputs**
- the **reference output** gives a **downward ramp over the interval time**
- **time output** gives CV from the interval slider

So every step can carry both **rhythmic** and **shape** information.

---

## Distorted kick / tom patch
Patch:
- sine or triangle VCO → VCA / LPG → distortion → mixer
- FG1 voltage out → oscillator pitch
- Pulse 1 → short envelope to VCA/LPG
- Pulse 2 → second envelope controlling distortion drive or wavefolder
- Reference output → exponential-ish decay destination, like filter cutoff or LPG CV
- Use **sloped** stages on certain hits

Programming suggestions:
- set most stages to **stepped**
- choose a few stages with **sloped** pitch for kick “doooom” downward pitch sweep character
- use **limited range** or **half range** for easier tuning of drum pitches
- assign **Pulse 2** only on accents
- vary **interval time** per stage so hits rush and drag slightly

What makes it nasty:
- patch **FG2 voltage out** to FM amount on the oscillator or to distortion CV
- make FG2 a shorter loop than FG1 using **First/Last**
- this creates repeating accent polymeters over the drum cycle

---

## Broken industrial snare / metallic hit
Patch:
- noise + oscillator mixed
- into bandpass or highpass filter
- into VCA
- into wavefolder or distortion

Use:
- Pulse 1 → trigger main snare envelope
- Pulse 2 → open a second VCA for noise burst or ring mod layer
- FG1 voltage → filter cutoff or oscillator pitch
- FG2 voltage → wavefolder / sample rate reducer / resonance / FM depth

Programming tricks:
- set some stages to **external source** for voltage and feed in random CV from S&H/noise
- use **quantize off** for non-musical metallic filter frequencies
- use **enable** on selected stages so the phrase waits for external gate conditions before continuing
- use **stop** stages to create sudden stutters and chokes

Very effective move:
- send **All Pulses Out** to clock another sequencer or logic module that modulates distortion parameters
- now every stage advance becomes an opportunity for secondary chaos

---

## Clicks, glitches, and fractured percussion
The MARF can get very strange if you use **very short time ranges** and stage addressing.

Patch idea:
- set some stages to very fast timing
- use **continuous/cont stage address** mode on one FG and strobe different positions
- clock the other FG conventionally

Patch:
- FG1 pulse output → trigger ultra-short envelope
- FG1 voltage output → VCA CV or LPG CV instead of pitch
- oscillator/noise/audio source remains static
- stage values become amplitude or timbre windows

Result:
- rhythmic amplitude carving
- almost wavetable-like percussive gestures
- jittery granular drum phrases

For more destruction:
- use **external voltage source** on selected stages and patch in audio-rate oscillator
- since the stage chooses external source by programming, only certain hits go berserk

---

## Percussion-specific modulation ideas
Here are especially good destinations for the MARF:

- distortion amount
- wavefolder symmetry/fold depth
- drum voice decay
- LPG decay
- filter resonance
- bandpass frequency
- FM amount
- noise VCA amount
- bitcrusher rate/depth
- sample rate reduction
- transient shaper/accent CV
- send amount to spring reverb or delay

---

# 2. Crazy basslines for dubstep / drum and bass

This is where the MARF is especially strong.

The main recipe for modern aggressive bass:
- stable phrase structure
- unstable timbre movement
- slides/glides
- per-hit accents
- rhythmic asymmetry
- selective quantization
- modulation relationships that don’t loop evenly

The 248t can do all of that.

---

## Core bassline strategy
Use:
- **FG1** = pitch
- **FG2** = timbre movement

Patch:
- FG1 voltage or ART out → main bass oscillator pitch
- Pulse 1 → envelope or LPG trigger
- Pulse 2 → accent envelope / distortion hit / FM burst / sub mute / re-trigger
- FG2 voltage → filter cutoff, wavetable position, FM index, fold amount, phase mod amount, resonance, or VCA level
- Reference output → ducking contour, LPG pluck, or sidechain-like movement
- Time output → another timbral parameter for note-length-correlated motion

---

## Use sloped stages for bass slides
From the manual:
- **Sloped/Stepped** is per stage
- slew time is based on that stage’s interval time

That is gold for bass music.

### Best use:
Program most bass notes as **stepped**, but set selected transition notes to **sloped**.

That gives:
- classic glide into target note
- grotesque pitch swoops
- “talking” bass phrase connections
- liquid DnB lead-in notes

### Extra trick:
Because slope time depends on **interval time**, longer stages produce longer slides.  
So you can compose the groove and the slide shape together.

This is a uniquely MARF behavior and it feels much more organic than global portamento.

---

## Wobble without sounding generic
Instead of a normal synced LFO wobble:

- use **FG2** as the wobble source
- assign different interval times to stages
- mark different loop boundaries than FG1
- occasionally substitute external CV using A/B/C/D on certain stages

Patch:
- FG2 voltage → multimode filter cutoff
- FG2 Pulse 1 → re-trigger a modulation envelope every few stages
- FG2 time output → distortion tone or wavefolder bias

Now the “wobble” is not repetitive LFO motion. It becomes a **composed modulation phrase**.

This works especially well for:
- reese basses
- vowel basses
- FM growls
- folded sub-mid basses

---

## Bass patch 1: Reese monster
Patch:
- 2 detuned saws or PWM squares
- into filter
- into soft clipper / wavefolder / distortion

Use:
- FG1 quantized voltage → oscillator pitch
- FG2 unquantized voltage → filter cutoff
- Pulse 1 → VCA envelope
- Pulse 2 → distortion accent CV or FM burst envelope
- Reference out → filter decay contour

Programming:
- FG1 in **half range** for musical bass note programming
- enable **quantize** on musical stages
- disable quantize on occasional transitional stages if you want ugly in-between slides
- use **sloped** notes selectively
- set FG2 loop shorter or longer than FG1 using First/Last markers

Result:
- bass notes stay anchored
- timbre cycles phase against pitch phrase
- pattern feels alive, not 8-step preset-ish

---

## Bass patch 2: Dubstep formant/growl line
Patch:
- complex oscillator / wavetable / FM voice
- bandpass or lowpass filter
- wavefolder/distortion after filter
- optional second filter for vowel movement

Use MARF like this:
- FG1 voltage → oscillator pitch
- FG2 voltage → wavetable position or FM index
- Time output from FG2 → filter cutoff
- Pulse 2 → trigger short envelope to second modulation destination, like formant sweep
- external input A → random stepped voltage
- set selected FG2 stages to **external source**, so only some timbre stages use randomness

Why this is powerful:
You get a phrase that is mostly controlled and repeatable, but certain bass hits “mutate” because stage-programmed external source injects new CV.

That’s excellent for:
- neuro bass
- metallic wobble
- formant screaming bass
- machine-like resampled phrases

---

## Bass patch 3: Stop/start savage groove
The manual’s **stop**, **sustain**, and **enable** functions are killer for bass.

### Stop
A stop stage waits until a start pulse arrives.

### Sustain
If a gate is high at start input, the stage holds.

### Enable
Stage pauses until voltage above 5V arrives at start input.

These are amazing for broken rhythmic basslines.

Patch:
- FG1 runs pitch line
- gate pattern from another sequencer, manual controller, logic module, or trigger pattern → FG1 start input
- certain stages programmed as **stop** or **enable**
- Pulse 1 still triggers voice
- FG2 continues separately or is also externally controlled

What happens:
- the phrase hangs on a stage
- then bursts forward when external rhythm allows it
- gives gated, syncopated, “breathe and lunge” bass motion

Perfect for:
- halftime dubstep
- techstep DnB
- broken neuro phrases
- pseudo-sidechained stop-go riffs

---

## Best bass modulation destinations from the 248t
Try patching the MARF into:

- oscillator pitch
- oscillator FM index
- oscillator wavefold amount
- wavetable position
- filter cutoff
- filter resonance
- comb filter frequency
- distortion drive
- distortion tone
- VCA level
- sub oscillator level
- noise layer level
- phase modulation depth
- LPG control
- delay send amount
- chorus depth
- stereo spread CV
- feedback amount on delay/filter

---

## Stage-address tricks for bass
The **Stage Address** section is especially good for advanced bass work.

From the manual:
- continuous mode sweeps through stages with the address control and stops internal clock
- strobe loads stage corresponding to current address value
- stage can be controlled by knob or external voltage

This means the 248t can become a kind of **voltage-scanned wavesequence/modulation table**.

### Try this:
- program 16 stages as different timbre values, not notes
- set FG2 to **continuous**
- patch an LFO, envelope, random CV, or audio-rate CV into external stage address
- use FG2 voltage out as filter/folder/FM modulation

Now you are “scanning” a programmed modulation shape instead of just clocking steps.  
That can sound like:
- talking bass
- tearing filter vowels
- scanning distortion colors
- unstable digital motion

For extreme bass:
- use envelope into stage address for attack-to-decay timbre travel
- use audio-rate oscillator into stage address for tearing discontinuous modulation

---

# 3. Haunting atmospheric pad sounds

The MARF is also great for pads because it can create **slow, non-uniform, semi-repeatable evolution**.

Pads get interesting when multiple parameters drift at different speeds with occasional structural surprises.

The MARF is built for that.

---

## Core pad strategy
Use very slow time ranges and separate the generators:

- **FG1** = pitch/harmonic center
- **FG2** = timbral evolution

Patch:
- FG1 quantized voltage → oscillator pitch or chord root CV
- FG2 continuous voltage → filter cutoff / wavetable position / morph / FM index
- Reference output → slow contour to LPG, filter, or reverb send
- Time output → modulation depth, stereo width, shimmer amount, or delay feedback
- Pulse outputs → occasional envelope resets, freeze functions, or reverb bloom triggers

---

## Use long stage times and sloped movement
The manual says time can range from very short to **up to 2 minutes**.

For pads:
- use long intervals
- set many stages to **sloped**
- use **continuous voltage** rather than quantized where timbre is concerned
- use **quantized** for pitch if you want harmonic clarity

This gives:
- slow glacial morphing
- note drift
- harmonic ambiguity
- ghostly transitions between states

---

## Pad patch 1: haunted chord bed
Patch:
- 2 or 3 VCOs or a polyphonic voice
- through LPG or lowpass filter
- into long reverb and modulated delay

Use:
- FG1 voltage → pitch CV or root note transposition
- FG2 voltage → filter cutoff
- FG2 time output → reverb send or delay feedback
- Reference output → subtle VCA/LPG contour
- Pulse 1 → trigger sparse envelope or shimmer burst every few stages

Programming:
- choose a key/scale if using quantize
- mark only a few stages with pulse outputs
- use unequal stage times so the phrase feels unmetered
- use **First/Last** loop points shorter on one FG than the other

Result:
- a pad that never quite comes back the same way
- harmonic movement and timbral movement drift against each other

---

## Pad patch 2: external-source spectral ghosting
This is one of the most powerful MARF tricks.

Use stage-programmed external voltage source for timbre.

Patch:
- external input A = slow random CV
- external input B = envelope follower from another sound
- external input C = sine LFO
- external input D = very slow manual CV/joystick/pressure source

Set selected stages to **external voltage source**.  
Now some stages use the programmed slider value, while others “open portals” to external modulators.

Patch FG2 voltage to:
- wavetable position
- wavefolder symmetry
- filter FM amount
- reverb tone
- granular density
- spectral morph

This creates a pad that has programmed structure but periodically becomes reactive and alive.

Excellent for:
- dark ambient
- haunted drone
- sci-fi beds
- decaying tape-memory textures

---

## Pad patch 3: frozen-time sustain architecture
Use **sustain** and **enable** to make pads breathe.

Patch:
- slow gate or manual controller to start input
- selected stages programmed as **sustain**
- some stages as **enable**
- long interval times
- sloped voltages

What happens:
- the pad arrives at a stage and lingers unnaturally
- then advances only when external condition changes
- creates suspended harmonic moments

Very useful for:
- performance-controlled drones
- evolving soundtrack textures
- ritual ambient structures
- live improvisation with pressure/foot controller/keyboard gate

---

# Advanced cross-modulation techniques

These are where the MARF becomes truly unique.

---

## 1. Use FG1 to make sound, FG2 to modulate FG1 timing indirectly
Patch:
- FG2 output → external input selected as **time source** on FG1 stages
- some stages of FG1 use internal time, some external time

Now pitch phrase timing changes according to another programmed function.  
This creates:
- rushing/dragging basslines
- unstable percussion grids
- swelling pad evolution

If external time CV is absent, the manual says it defaults to the fastest value of the selected range, so be deliberate.

---

## 2. Use Time Output as a hidden second sequencer
The manual states the time slider also produces CV at the **time output**.

This means each FG really gives you:
- pitch-like CV
- time-derived CV
- pulses
- reference ramp

The time sliders can therefore be programmed as a totally different contour than pitch.

Great uses:
- percussion decay sequence
- distortion amount sequence
- FM depth sequence
- reverb send sequence
- bass brightness sequence
- pad stereo width sequence

This is one of the most underused powers of the MARF.

---

## 3. Use All Pulses Out as a master chaos clock
Because **All Pulses Out** fires whenever a new stage is addressed, you can use it to drive:
- clocked random
- Bernoulli gates
- logic
- clock dividers
- envelope followers
- switched modulation

Then route those results back into:
- A/B/C/D external inputs
- start inputs
- stage addressing
- effect CVs

That creates a self-related ecosystem around the MARF.

---

## 4. Use mismatched cycle boundaries
Program:
- FG1 first/last = stages 1–8
- FG2 first/last = stages 3–13

Now both generators traverse the same stored 16-stage programming space but with different cycle windows.  
This gives extremely musical long-form variation without randomness.

Especially good for:
- bassline phrase evolution
- drifting accents in percussion
- pads that take a long time to truly repeat

---

## 5. Mixed quantized/unquantized stage programming
A very signature MARF trick:
- quantize some stages
- leave others continuous

Use this for bass:
- stable musical root notes on some stages
- ugly in-between bent notes on transitions

Use this for pads:
- clear harmonic anchor points
- drifting microtonal movement between them

Use this for percussion:
- discrete tuned drum hits alternating with inharmonic metallic offsets

---

# Patch recipes by genre target

---

## A. Distorted percussion patch recipe
**Goal:** industrial broken drum machine

Patch:
- VCO sine → wavefolder/distortion → LPG/VCA → mixer
- noise → VCA → mixer
- FG1 voltage → VCO pitch
- Pulse 1 → LPG/VCA envelope
- Pulse 2 → noise VCA envelope
- Reference out → LPG CV
- FG2 voltage → distortion drive
- FG2 time out → filter cutoff or fold symmetry

Programming:
- short to medium time ranges
- stage time variation for groove
- some sloped pitch stages for tom/kick dives
- pulse 2 only on selected accents
- external source on a few FG2 stages using random CV

Result:
- heavy kicks/toms/snare hybrids
- asymmetrical aggression
- animated distortion color

---

## B. Dubstep bass patch recipe
**Goal:** snarling syncopated growl bass

Patch:
- main oscillator + sub oscillator
- into multimode filter
- into wavefolder/distortion
- into VCA

MARF:
- FG1 ART/voltage → pitch
- FG2 voltage → filter cutoff
- FG2 time out → FM index
- Pulse 1 → VCA envelope
- Pulse 2 → distortion accent envelope
- Reference out → subtle ducking or second filter contour
- All Pulses Out → clock random source
- random source back to external input A
- selected FG2 stages set to external source

Programming:
- quantized bass notes in half range
- selective sloped transitions
- one or two stop/enable stages for dramatic hangs
- shorter loop on FG2 than FG1

Result:
- composed but mutating growl phrases
- classic bassline cohesion with non-repeating detail

---

## C. DnB reese patch recipe
**Goal:** rolling, tense, evolving low-end

Patch:
- two detuned saws
- lowpass filter
- saturation
- chorus/flanger optional

MARF:
- FG1 quantized voltage → pitch
- FG2 voltage → filter cutoff or chorus depth
- Time output → distortion tone
- Pulse 1 → short VCA envelope
- Pulse 2 → accent envelope to resonance/FM

Programming:
- mostly short stage times
- a few longer holds
- occasional sloped notes into phrase endpoints
- stop stage before drop resolution
- external start pulses from trigger sequencer for syncopation

Result:
- rolling bass with phrase punctuation
- long-form modulation that doesn’t sound loop-locked

---

## D. Haunted pad patch recipe
**Goal:** dark cinematic evolving texture

Patch:
- rich oscillator / wavetable source
- LPG or gentle filter
- large reverb
- modulated delay

MARF:
- FG1 quantized voltage → root/transposition
- FG2 continuous voltage → wavetable position
- Reference output → LPG/filter contour
- Time output → reverb send
- Pulse 1 → shimmer burst / freeze / envelope reset
- external inputs fed by slow random, envelope follower, sine LFO, manual CV
- selected stages on FG2 use external source

Programming:
- long stage intervals
- sloped on most timbral stages
- sparse pulse programming
- different first/last loops for the two FGs
- sustain stages controlled by external gate

Result:
- eerily structured but fluid pad motion
- occasional spectral intrusions from external sources
- strong “haunted machine” quality

---

# Best specific modulation destinations by sound goal

## For distorted percussion
Use MARF outputs to modulate:
- decay time
- pitch
- fold depth
- distortion drive
- resonance
- noise amount
- transient level
- LPG CV
- sample rate
- bit depth
- send to spring/delay

## For dubstep/DnB bass
Use MARF outputs to modulate:
- filter cutoff
- filter mode scan
- FM index
- wavefolder
- wavetable position
- phase modulation depth
- distortion drive and tone
- sub level
- stereo width
- comb filter frequency
- formant/vowel filter

## For atmospheric pads
Use MARF outputs to modulate:
- cutoff
- reverb send
- delay feedback
- wavetable position
- oscillator blend
- FM amount
- stereo image
- shimmer amount
- LPG level
- saturation tone
- granular density/position if using sampler modules

---

# Performance tips

## 1. Use presets as macro-scene changes
The manual says you can save and recall **12 presets**.  
This is extremely useful live.

Create:
- preset 1 = restrained groove
- preset 2 = distorted variation
- preset 3 = breakdown
- preset 4 = drop
- preset 5 = ambient wash

Since stage data includes slider positions and settings, presets can function like song sections.

---

## 2. Use manual stage advance for fills
The **advance** control on either FG is perfect for manual performance nudges:
- drum fill skip
- bass phrase mutation
- forcing unexpected pad harmonies

---

## 3. Use continuous stage addressing as a timbre macro
When stage address is in **continuous** mode, scanning stages can feel like moving through a custom wavetable of modulation states.

Great live gesture:
- patch a joystick or pressure controller to stage address external CV
- use FG2 voltage out for filter/folder/FM
- “play” timbre like an instrument

---

## 4. Keep one FG stable and abuse the other
For musical results:
- let one FG define the recognizable musical identity
- make the other FG do the dangerous stuff

Examples:
- stable bass notes, unstable filter motion
- stable percussion triggers, unstable distortion color
- stable pad root, unstable spectral movement

That prevents total chaos while still sounding unique.

---

# Practical “secret sauce” ideas

## Selective external source substitution
This is probably the most powerful sound-design trick in the manual.

Feed A/B/C/D with:
- random
- envelope follower
- audio oscillator
- slow LFO

Then on only a few stages, switch source to external.

That gives:
- occasional monstrous bass hits
- one snare in a bar that mutates
- pads that briefly become haunted
- controlled unpredictability

---

## Use time sliders as expression, not just duration
Because time output can be used separately, program stage times musically:
- short notes = brighter
- long notes = darker
- long notes = more reverb
- short hits = more distortion

This creates strong internal phrase coherence.

---

## Use limited range for bass and percussion
The manual notes:
- **Full range** = 0–10V
- **Half range** = 0–5V
- **Limited** = 2V spans with offsets

For bass, half/limited often feel better because:
- easier to dial pitch precisely
- less accidental huge jumps
- more “playable” musical range

For percussion:
- limited range is excellent for tuned drum zones

---

## Exploit unequal timing
The MARF’s stage times can make everything feel alive.

For bass:
- alternate short-short-long-short patterns
- then break them with stop/enable

For percussion:
- micro-variation in stage lengths humanizes and destabilizes grooves

For pads:
- unequal long durations make the harmony feel organic and non-gridlocked

---

# Best minimal starter patches

If you want immediate results, start here.

## Starter 1: nasty bass
- FG1 → pitch
- FG2 → filter cutoff
- Pulse 1 → amp envelope
- Pulse 2 → distortion accent
- use sloped notes sparingly
- shorter loop on FG2 than FG1

## Starter 2: broken drums
- FG1 → drum pitch
- Pulse 1 → main hit
- Pulse 2 → accent/noise burst
- Reference out → LPG decay
- FG2 → distortion tone
- program irregular stage times

## Starter 3: haunted pad
- FG1 → root pitch
- FG2 → wavetable/filter
- Time out → reverb send
- Reference out → slow LPG/filter shape
- long sloped stages
- external source on a few timbre stages

---

# Final advice

The 248t becomes special when you combine these four concepts:

1. **Pitch and timbre are sequenced separately**
2. **Timing is part of composition**
3. **Only some stages become externalized/randomized**
4. **Loop lengths and behaviors differ between the two FGs**

That combination is exactly how you get:
- **distorted percussive brutality**
- **dubstep/DnB basslines with movement and attitude**
- **haunting evolving pads that feel alive instead of looped**

If you want, I can also give you:
- **3 concrete patch diagrams** for these sound categories
- a **“best modules to pair with the 248t” list**
- or a **stage-by-stage example program** for bass, percussion, and pads.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)