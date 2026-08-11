# Doepfer — A-151 Quad Sequential Switch

- [Manual PDF](../../manuals/A151_man.pdf)

---

[Doepfer A-151 Quad Sequential Switch Manual (PDF)](https://doepfer.de/a100_man/A151_man.pdf)

# Doepfer A-151 Quad Sequential Switch — Sound Design Ideas

The **Doepfer A-151** is a **4-step sequential switch**. Every trigger advances the connection from the common jack to the next of four I/O jacks. That sounds simple, but in a modular patch it becomes a **rhythm router, waveform scanner, modulation sequencer, pattern breaker, and timbral animator**.

A few key things from the manual that matter musically:

- It is **bi-directional**:
  - **4 inputs → 1 output**
  - or **1 input → 4 outputs**
- It advances on the **rising edge** of a trigger at **Trig In**
- A pulse to **Reset In** returns it immediately to **step 1**
- **Version 2** adds a **2 / 3 / 4 step switch**
- Early versions handle about **-8V to +8V**
- Later versions handle the full **A-100 range: -12V to +12V**
- Very fast triggering can create **audio-rate switching effects**, which is where things get especially wild

---

## What the A-151 is best at

Think of the A-151 as a way to make one thing become many things over time:

- one oscillator becomes a rotating set of waveforms
- one envelope becomes a rotating set of destinations
- one audio path becomes a rotating set of distortions
- one clock becomes evolving phrasing through reset tricks
- one sustained sound becomes a shifting pad through stepped timbre changes

Because it is a **hard switch**, not a crossfader, the sonic results can be:
- abrupt
- glitchy
- percussive
- formant-like
- aggressive
- rhythmically complex

That makes it especially good for:
- **distorted percussion**
- **dubstep / DnB bass movement**
- **haunted evolving atmospheres**

---

# General modulation strategies

## 1. Trigger it at musically meaningful rates
Use different trigger sources into **Trig In**:

- **Clock divider** for rhythmic pattern switching
- **Gate from sequencer** for note-by-note changes
- **LFO square** for slower movement
- **Envelope end-of-cycle / trigger out** for self-evolving patches
- **VCO square wave** for audio-rate timbral destruction

This one choice massively changes the character:
- **slow triggers** = structural variation
- **medium triggers** = rhythmic articulation
- **audio-rate triggers** = new composite timbres / digital tearing / harshness

---

## 2. Use Reset In for pattern control
Reset is one of the most important creative features.

If you clock the A-151 in 4-step mode but send a reset every 3 clocks, you get:
- **1 → 2 → 3 → reset**
instead of
- **1 → 2 → 3 → 4**

That means:
- uneven phrasing
- accents that feel “broken”
- loop lengths that don’t match the main clock
- pseudo-polyrhythms

For bass music, this is gold.

Try:
- reset every **5th**, **7th**, or **irregular** pulse
- reset from a **probability gate**
- reset from a **manual gate button** during performance

---

## 3. Use the 2/3/4 step switch musically
If your version has the step switch:

- **2-step** = alternating A/B behavior, great for kick/snare, wobble/open-close
- **3-step** = asymmetry, instantly more interesting
- **4-step** = full cycle variation

A strong performance trick:
- patch a 4-source timbre chain
- switch between **2-step** and **3-step** during playback
- the whole groove shifts without changing pitch sequencing

---

## 4. Remember it is bi-directional
This is huge.

### 4 inputs → 1 output
Use when you want to **select between sound sources** or modulation sources.

### 1 input → 4 outputs
Use when you want one source to **strike different destinations in sequence**.

For example:
- one trigger routed to 4 different envelopes
- one envelope routed sequentially to 4 modulation targets
- one audio source routed to 4 different processing chains

This is where patches become animated and “composed.”

---

# Patch ideas for distorted percussive sounds

## 1. Rotating drum voice architecture
Use one trigger sequence to advance the A-151 while one noise/oscillator source feeds the common input.

### Patch
- Put a sound source into **O/I**
  - white noise
  - sine or triangle oscillator
  - short FM blip source
- Patch **I/O 1–4** to four different processing chains:
  1. LPG or VCA with short decay
  2. wavefolder or distortion
  3. bandpass filter with high resonance
  4. ring mod or FM input path
- Use the outputs of those chains to your mixer or combine downstream depending on routing scheme

Alternative approach:
- send **4 sound sources** into **I/O 1–4**
- take **O/I** as the selected output

### Result
Each hit rotates to a different timbre:
- kick-ish thud
- metallic crack
- tearing snare
- noisy zap

### Make it more brutal
- Trigger A-151 with the same rhythm driving your percussion envelope
- Use a reset every 3 or 5 triggers
- Add distortion after the A-151 output so the abrupt switching creates transients that get exaggerated

This can create really strong **industrial percussion** and **broken beat textures**.

---

## 2. Sequential transient designer
Route one trigger source to different envelope generators or decay shapes.

### Patch
- Put a trigger stream into **O/I**
- Route **I/O 1–4** to:
  1. short snappy envelope
  2. medium decay envelope
  3. ultra-short click envelope
  4. envelope with attack for reverse-like swell
- Each envelope controls either:
  - VCA amplitude
  - filter cutoff
  - FM index
  - distortion amount

### Result
Each note has a different contour. Even a simple oscillator becomes:
- punch
- slap
- bite
- smear

For distorted percussion this matters a lot, because distortion responds differently to different envelope shapes.

---

## 3. Audio-rate switched noise percussion
The manual specifically notes very fast trigger rates can create audio-frequency modulation.

### Patch
- Send **noise** or a harmonically rich oscillator into **O/I**
- Put 4 different filtered versions of the sound on **I/O 1–4**, or vice versa
- Trigger **Trig In** with:
  - fast square LFO
  - audio-rate VCO square output

### Result
You get:
- tearing digital-like edges
- zippering textures
- metallic alias-style percussion
- strange formant bursts

Add:
- short VCA envelope after the switch
- hard clipping
- resonant HPF/BPF

This produces fantastic:
- snare layers
- glitch hats
- neuro percussive stabs

---

## 4. Rotating feedback percussion
If your system supports careful feedback patching:

### Patch
- Source oscillator/noise into A-151
- Each stage feeds a different effect:
  1. clean
  2. overdrive
  3. filter feedback loop
  4. wavefolder
- Mix some output back into the input path

### Result
The A-151 changes the topology of the feedback path on each hit. This can yield:
- unstable clanks
- explosive hits
- screaming transients
- “machine breaking” sounds

Keep levels under control. This can get loud fast.

---

# Patch ideas for dubstep / drum & bass basslines

## 1. Waveform scanner bass
This is directly suggested by the manual: switch between VCO waveforms.

### Patch
- Patch one oscillator’s **saw, pulse, triangle, sub** into **I/O 1–4**
- Take **O/I** to filter → VCA → distortion
- Trigger **Trig In** from:
  - sequencer gate
  - clock division of the note rhythm
  - fast LFO for rolling movement

### Why it works
Each waveform hits the downstream distortion and filter differently:
- saw = bright/aggressive
- pulse = nasal/hollow
- triangle = smoother body
- sub = weight

### Bass music trick
Run the switched waveform into:
- wavefolder
- aggressive lowpass with resonance
- parallel clean sub underneath

The A-151 becomes a **hard-stepped wavetable selector**.

---

## 2. Sequential modulation-source selector for wobble bass
Instead of switching audio, switch **control voltages**.

### Patch
Send 4 modulation sources into **I/O 1–4**:
1. slow triangle LFO
2. envelope with snappy attack
3. stepped random
4. inverted envelope or slewed random

Take **O/I** to:
- filter cutoff CV
- wavetable position CV
- FM amount CV
- VCA CV amount
- distortion CV if available

Trigger the A-151 from the bass rhythm.

### Result
Every note or every beat has a different movement pattern:
- wobble
- stab
- glitch
- growl

This is one of the best uses of the module for **neuro / reese / dubstep** style design.

---

## 3. Sequential distortion topology
Use the A-151 to select different pre- or post-distortion paths.

### Patch
Bass source into **O/I**, then switch among 4 different routes:
1. direct to overdrive
2. filtered before distortion
3. wavefolded before distortion
4. ring mod or FM sidechain before distortion

Or reverse:
- 4 different parallel processing outputs into **I/O 1–4**
- **O/I** to final VCA/mix bus

### Result
One bassline becomes many basslines:
- guttural
- nasal
- crunchy
- ripped apart

### Performance note
Resetting at odd intervals creates those “mutating but still looped” bass phrases common in DnB.

---

## 4. 3-step bass phrasing against 4/4 drums
If your version has the **3-step mode**, use it constantly.

### Patch
- Sequence a normal 16-step bassline
- Advance the A-151 every quarter note or every note gate
- Put 3 different modulation or audio variants on steps 1–3

### Result
Because the timbre cycle is 3 while the bar is 4, the phrase drifts:
- bars feel less repetitive
- accents move
- bass seems to “evolve” without changing notes

This is excellent for:
- rolling DnB
- halftime dubstep
- broken neuro phrases

---

## 5. Audio-rate trigger for monstrous bass grit
This is one of the most extreme uses.

### Patch
- Bass oscillator waveforms into the A-151
- Trigger **Trig In** from another VCO square wave
- Tune the trigger VCO to harmonic or inharmonic relationships

### Result
The switching itself becomes part of the spectrum:
- harsh digital edge
- phasey tearing
- vocal-like movement
- unstable upper harmonics

Then run through:
- lowpass filter with envelope
- heavy saturation
- sub oscillator in parallel

This can produce **devastating reese-style textures**.

---

# Patch ideas for haunting atmospheric pads

The A-151 is often thought of as rhythmic, but it can be excellent for pads if you use it more slowly and structurally.

## 1. Rotating filter character pad
The manual gives an example of switching filter outputs. This is perfect for atmospheres.

### Patch
- Send one rich drone or chord source into a multimode filter
- Patch several filter outputs into **I/O 1–4**
  - lowpass
  - bandpass
  - highpass
  - notch or second filter output
- Take **O/I** to reverb and delay
- Trigger A-151 slowly:
  - very slow clock
  - manual gate
  - sparse random pulse

### Result
The pad shifts between spectral personalities:
- warm
- hollow
- distant
- ghostly

With enough reverb, the hard switching becomes a dramatic timbral scene change rather than a click.

---

## 2. Sequential envelope-to-modulation routing
Use one modulation source and send it to different destinations in sequence.

### Patch
- Put a slow envelope or LFO into **O/I**
- Send **I/O 1–4** to:
  1. filter cutoff
  2. oscillator PWM
  3. FM depth
  4. effect send or reverb CV

Trigger the switch very slowly.

### Result
The same movement migrates through the patch:
- first brightness rises
- then pulse width drifts
- then FM bloom appears
- then the reverb tail swells

This makes a patch feel **alive and intentional**, not just “LFO on everything.”

---

## 3. Chord or oscillator layer selector
If you have multiple sound sources or chord voicings:

### Patch
- Put 4 different related timbres into **I/O 1–4**
  - detuned saw layer
  - sine + fifth
  - filtered noise layer
  - FM bell-ish layer
- Take **O/I** into a shared ambience chain
- Trigger occasionally or from sparse random

### Result
The pad morphs between identities while staying in one harmonic world.

For haunting sounds, keep the source relationships close:
- same root
- octave/fifth clusters
- slight detuning differences

---

## 4. Reset for phrase-based ambience
Use reset as a “return to memory.”

### Patch
- Advance slowly through 4 timbral stages
- Send a reset at the start of every 8 or 16 bars

### Result
The atmosphere wanders, then returns to a recognizable opening state. This creates:
- narrative motion
- tension and release
- cinematic structure

---

## 5. Unstable spectral shimmer with audio-rate switching
For darker ambient or horror textures:

### Patch
- Feed four slightly different versions of a drone into **I/O 1–4**
  - one filtered
  - one ring modded
  - one wavefolded lightly
  - one with feedback delay coloration
- Trigger A-151 at medium to high rate with a square LFO or oscillator
- Put the output through long reverb

### Result
You get:
- spectral flutter
- metallic shimmer
- broken choir textures
- uncanny digital halo

Use attenuation if needed, especially if working with older A-151 voltage limits.

---

# Best modulation sources to pair with the A-151

## For percussion
- clock dividers
- trigger sequencers
- burst generators
- random gates
- envelope triggers
- audio-rate square VCOs

## For bass
- note gates from sequencer
- swung clocks
- reset patterns from logic
- stepped random CV sources
- envelopes and function generators
- synced LFOs

## For pads
- very slow square LFO
- manual gate/button
- Bernoulli/probability gate
- end-of-rise/end-of-cycle triggers
- sparse generative clocks

---

# Important sonic behaviors to exploit

## Hard switching clicks can be useful
Because the A-151 is switching abruptly, transitions may click depending on the material.

Usually that’s a problem, but for your goals it can be an advantage:
- added attack on percussion
- nasty transient on bass
- haunted artifact in ambient patches

If you want cleaner results:
- switch at envelope zero-crossing moments
- place a VCA after the switch
- filter after switching
- use slower or masked transitions with reverb/delay

---

## Switching modulation is often more powerful than switching audio
A lot of people first use sequential switches for audio selection, but for complex music, CV switching is often deeper.

Examples:
- different envelopes to one filter
- different LFOs to one wavetable position
- one envelope routed to changing destinations
- different sequencer rows selected per note

This gives movement without needing four totally separate voices.

---

## Audio-rate triggering is a signature trick
The manual explicitly points out that very fast trigger repetition can create audio-frequency effects.

This is one of the A-151’s secret weapons:
- pseudo-waveshaping
- digital-sounding aggression
- composite waveform generation
- metallic timbral breakup

For bass music and experimental percussion, this is one of the most valuable techniques in the module.

---

# Three full patch recipes

## 1. Distorted neuro snare machine
**Goal:** metallic, crushed, changing snare hits

- Noise + sine osc mixed together
- Into A-151 common I/O
- Four destinations:
  1. bandpass filter
  2. wavefolder
  3. hard clipper
  4. ring mod input chain
- Trigger A-151 from 16th-note clock
- Envelope/VCA after switch with short decay
- Heavy compression or saturation after VCA
- Reset every 3 or 5 hits

**Result:** rotating snare identities with aggressive transient differences

---

## 2. Dubstep bass mutator
**Goal:** filthy evolving bassline

- VCO waveforms to A-151 inputs:
  1. saw
  2. pulse
  3. sub
  4. FM output or second detuned VCO
- A-151 output to lowpass filter → distortion → VCA
- Trigger from note gate or divided clock
- Send another A-151 or modulation source to switch between filter-envelope shapes
- Use 3-step mode for drift
- Reset at phrase boundaries

**Result:** constantly shifting bass timbre with coherent musical repetition

---

## 3. Haunted pad engine
**Goal:** dark evolving cinematic texture

- Rich oscillator or chord source into multimode filter
- Filter outputs into A-151
- A-151 output into chorus/delay/reverb
- Advance switch every few seconds with slow square LFO
- Route reset from sparse random or bar-start pulse
- Add a second slow modulation source to detune or FM depth

**Result:** spectral scene changes that feel ghostly and alive

---

# Practical warnings from the manual

- If you have an **older version**, watch signal range:
  - roughly **-8V to +8V**
- **Version 2** can handle **-12V to +12V**
- If something behaves strangely, excessive voltage may be the cause
- Fast switching can be intentionally dirty, but also unpredictable depending on source material and downstream gain staging

---

# Final creative advice

The A-151 is most exciting when you stop thinking of it as just a utility and start treating it like a **compositional timbre sequencer**.

For your goals:

- **Distorted percussion:** switch audio paths and envelope shapes per hit
- **Dubstep / DnB bass:** switch waveforms, modulation sources, and distortion chains with resets for phrase control
- **Haunting pads:** switch filter outputs and slowly migrate modulation destinations

If you want, I can also give you:
1. a set of **10 specific patch recipes** using common Eurorack modules, or  
2. a **genre-focused patch sheet** for **dubstep**, **drum & bass**, or **dark ambient** built around the A-151.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)