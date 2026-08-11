# Kaona Instruments — Fractaos

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Fractaos Manual PDF](https://kaona.fr/wp-content/uploads/2025/07/FRCTAOS_manual_1.5_ENG.pdf)

# Fractaos modulation ideas for distorted percussion, basslines, and haunted pads

Fractaos is unusually deep for a Eurorack oscillator because it’s not just “an oscillator with FM.” It’s really:

- 4 voices
- 8 real-time fractal oscillators in driver/follower pairs
- per-voice resonant fractal filtering
- internal primitive-driven modulation/LFO behavior
- CV over the most important movement controls

That means the best sounds usually come from **stacking several small motions at once** rather than one huge modulation source.

---

# First: understand what is most worth modulating

From the manual, the most modulation-friendly panel parameters are:

- **Morph**
- **Spread**
- **Texture**
- **Speed**
- **Amount**
- **Chaos**
- **Primitive Chaos**
- **Pitch**

And the switches decide **where the primitive-derived modulation goes**:

- **Morph**
- **Spread**
- **Chaos**
- plus **Loop/Trig** behavior for whether it acts like a looping LFO or note-retriggered contour

## Important limitation
These are **not CV-modulatable**:
- **Depth**
- **Primitive Depth**

So for live patching, treat Depth settings as your “static engine configuration,” then animate:
- chaos
- morph
- texture
- spread
- speed/amount

That’s where the sound comes alive.

---

# Big-picture patch philosophy for Fractaos

## 1. Use the primitive as an internal motion source
The primitive isn’t just a second oscillator. It also creates internal motion. The switches let you decide whether that motion affects:
- morphing
- spread/detune
- chaos

This is one of the module’s strongest features.

## 2. Treat Texture like a spectral violence / atmosphere control
Texture does a lot at once:
- fractal filter resonance
- formant extraction/detection
- micro-detuning
- filter intensity

So in practice:
- low Texture = more direct oscillator identity
- medium Texture = vocal/formant/organic complexity
- high Texture = unstable, spectral, resonant, sometimes noisy behavior

## 3. Spread is context-sensitive
- **Normal mode:** detunes driver/follower in each voice
- **Drone mode:** becomes a global 8-oscillator spread/chord/microtuning control

That makes Spread one of the best performance parameters on the module.

## 4. Chaos is not generic “randomness”
Each fractal responds differently to Chaos. Some become unstable, some become richer, some just get slightly rougher. So the best approach is:
- pick a fractal family for the musical role
- then find its sweet-spot chaos window

---

# Best fractals by use case

## For distorted percussion
Best starting points:
- **Rule30** — granular, dense, percussive
- **Collatz** — stepped and jerky, rhythmic
- **Dragon** — beating and expressive under chaos
- **Hénon** — unstable/experimental
- **Lorenz** — complex drifting, irregular
- **Drum models:** **Kick, Tom, Snare, HiHat, Cymbal**

Also try morphing Drum curves with geometric primitives for hybrid percussion.

## For dubstep / DnB bass
Best starting points:
- **Mandelbrot** — bright, crystalline, harmonically rich
- **Cantor** — gapped saw/pulse character
- **Sierpinski** — strong odd harmonics
- **Dragon** — moving/internal beating
- **Rule30** — nasty bass texture
- **Koch** — brassy low register
- **Fibonacci** — warmer foundation
- **Hilbert** — stepped rectangular spectral behavior

## For haunted atmospheric pads
Best starting points:
- **Cloud**
- **Storm**
- **String**
- **Ensemble**
- **Cluster**
- **Lorenz**
- **Rössler**
- **Julia**
- **Fibonacci**

For pads, the texture fractals as the main fractal are especially important because they’re intentionally noisy/atmospheric.

---

# Core modulation techniques that work especially well on Fractaos

## 1. Slow CV into Texture
This is one of the best “free complexity” moves.

Use:
- a slow triangle LFO
- random slewed voltage
- very slow envelope
- offset + attenuated modulation

Why it works:
Texture changes not only filter intensity but also formants and micro-detuning, so even tiny movement sounds rich.

### Great for:
- evolving pads
- speaking bass growls
- metallic percussion tails

---

## 2. Envelope to Chaos
Use a fast-decay envelope into **F-Chaos** or **P-Chaos**.

Why:
A burst of chaos at the attack makes sounds feel:
- struck
- ripped
- unstable
- snarling

This is excellent for:
- distorted kicks
- tearing bass attacks
- noisy transient design

### Patch idea
- Trigger source -> envelope generator
- Envelope out -> Fractaos **F-Chaos CV**
- Set attenuator low-medium
- Keep base Chaos moderate
- Let the envelope briefly push it over the edge

Result:
clean-ish body with violent transient articulation.

---

## 3. Gate-triggered primitive modulation
Use:
- **Loop OFF**
- **Trig ON**

Now each new note retriggers the primitive contour from the beginning.

If **Morph**, **Spread**, or **Chaos** are enabled, each hit/note gets its own animated shape.

This is one of the best methods for:
- punchy bass plucks
- animated percussion
- articulated sequences

---

## 4. Looping primitive modulation for unstable movement
Use:
- **Loop ON**
- optional **Trig ON** if you want note-synced restarts

Now the primitive becomes a looping LFO.

Great for:
- wobble basses
- fluttering spectral percussion
- living drones
- breathing pads

---

## 5. Audio-style aggression without classic audio-rate CV: use simplified FM mode
The manual’s “simplified FM mode” is huge for aggressive sounds.

Set:
- **Loop OFF**
- **Trig OFF**
- **Morph ON**
- **Spread OFF**
- **Chaos OFF**

Now **Amount** becomes bipolar:
- **0–50%:** internal feedback
- **center:** neutral
- **50–100%:** primitive 2 modulates main fractal frequency

This is your primary route to:
- tearing reese-like basses
- metallic attacks
- snarling dubstep timbres
- overdriven, deformed waveforms

### Important note
FM does **not** work when the main fractal is a **Texture** fractal, and does not affect **Drum** curves.

---

# Sound design recipes

---

# 1. Distorted percussion and hybrid drums

Fractaos is unusually good at percussion because you can combine:
- actual drum models
- geometric fractals
- primitive-triggered contouring
- chaos bursts
- texture resonance

## A. Distorted kick drum
### Start here
- Main fractal: **Kick**
- Primitive: **Dragon** or **Rule30**
- Depth: medium-high
- Primitive Depth: medium
- Chaos: low-medium
- Primitive Chaos: medium
- Morph: low to low-mid
- Texture: medium
- Speed: medium-fast
- Amount: low-medium

### Switches
- **Loop OFF**
- **Trig ON**
- **Morph ON**
- optionally **Chaos ON**
- **Spread OFF**

### Why this works
- Kick provides the body
- Primitive adds evolving harmonic contamination
- Retriggered modulation gives each hit a consistent motion contour
- Chaos modulation adds snap/rip at the start

### Improve it further
Patch:
- trigger mult -> Fractaos trig + external fast envelope
- external envelope -> **Texture CV**
- another envelope or accent CV -> **F-Chaos CV**

This gives:
- attack-dependent filter/formant bite
- aggressive transient dirt
- more “broken speaker” energy

### For harder industrial kicks
Try:
- more Texture
- more Morph
- primitive = **Cantor** or **Collatz**
- pitch lower
- higher Chaos on accented hits

---

## B. Snare from hell
### Start here
- Main fractal: **Snare**
- Primitive: **Rule30**, **Hénon**, or **Collatz**
- Morph: medium
- Texture: medium-high
- Chaos: medium-high
- Primitive Chaos: medium-high
- Speed: medium-fast
- Amount: medium

### Switches
- **Loop OFF**
- **Trig ON**
- **Morph ON**
- **Chaos ON**
- maybe **Spread ON** in small doses

### Result
You get:
- percussive shell/noise from Snare
- digital tearing from primitive modulation
- unstable noise sprays from chaos
- flamming metallic edges via spread modulation

### Advanced trick
Sequence pitch slightly even on Snare. The manual says pitch shifts color/resonance/internal filtering strongly on Snare/HiHat/Cymbal. Tiny pitch sequences can create a whole kit from one patch.

---

## C. Metallic hi-hats and fractured tops
### Start here
- Main fractal: **HiHat** or **Cymbal**
- Primitive: **Hilbert**, **Rule30**, or **Koch**
- Texture: high
- Chaos: medium
- Primitive Chaos: high
- Morph: medium-high
- Spread: low-medium
- Speed: fairly fast
- Amount: medium-high

### Switches
- **Loop OFF**
- **Trig ON**
- **Spread ON**
- **Morph ON**

### Why
Spread modulation on short metallic voices introduces oscillating detune and can create:
- shaken hat texture
- digital sizzle
- unstable cymbal wash

### Patch improvement
Use random stepped CV with attenuation into:
- **P-Chaos**
- or **Morph**

Now every hit gets a slightly different color without losing the patch identity.

---

## D. Percussion that turns into a note
One of Fractaos’s coolest manual-noted features is using **Morph** with Drum curves to blend percussion with the second geometric fractal.

### Patch
- Main fractal: **Kick**, **Tom**, or **Snare**
- Primitive: **Fibonacci**, **Mandelbrot**, or **Koch**
- Morph: medium-high
- Trig ON, Loop OFF, Morph ON

### Effect
You can create:
- percussive attack + pitched sustain
- drum-to-bass hybrids
- “hit becomes note” sounds
- tuned tom stabs

This is excellent for modern bass music fills.

---

# 2. Crazy basslines for dubstep / drum and bass

Fractaos can do bass very well if you focus less on “traditional analog FM bass” and more on:
- morph movement
- attack chaos
- spread detune
- texture/formants
- simplified FM mode

## A. Talking/growling bass
### Start here
- Main fractal: **Cantor**, **Mandelbrot**, **Dragon**, or **Rule30**
- Primitive: **Rössler**, **Dragon**, or **Hilbert**
- Pitch: low register
- Depth: medium-high
- Primitive Depth: medium
- Chaos: medium
- Primitive Chaos: medium
- Morph: around center
- Texture: medium-high
- Speed: synced to groove
- Amount: medium-high

### Switches
- **Loop ON**
- **Morph ON**
- **Spread ON**
- optional **Chaos ON**
- **Trig** optional depending on whether you want phrase resets

### Why
This creates multiple interlocked movements:
- spectral shape changing from Morph modulation
- detune throbbing from Spread modulation
- chaos-driven internal roughness
- filter/formant animation from Texture

### Best external modulation
Patch an LFO or sequencer lane into:
- **Texture CV** for vowel/growl emphasis
- **Morph CV** for phrase evolution
- **Pitch CV** for slides or stepped riffs

### Dubstep move
Clock a stepped random or sequenced CV into Texture while the internal primitive loops on Morph. That gives macro movement plus internal motion.

---

## B. Reese / tearing DnB bass
### Start here
- Main fractal: **Sierpinski**, **Cantor**, **Koch**, or **Mandelbrot**
- Primitive: **Dragon**, **Rössler**, or **Fibonacci**
- Spread: medium
- Morph: low-mid
- Texture: low-medium to medium
- Chaos: low-medium
- Primitive Chaos: medium
- Pitch: low

### Switches
- **Loop ON**
- **Spread ON**
- **Morph OFF**
- **Chaos OFF** initially

This gives you animated detune between driver/follower. It’s not a classic supersaw detune; it’s stranger and often gnarlier.

### Make it nastier
Then add:
- a little **Chaos ON**
- slow CV to **Texture**
- envelope to **F-Chaos**

This keeps body and adds attack abrasion.

### External processing recommendation
Fractaos will sound huge through:
- wavefolder
- distortion
- lowpass or bandpass filter
- VCA with envelope follower sidechaining

But even before external processing, Spread + Texture is already very “reese-adjacent.”

---

## C. Simplified FM bass monster
This is one of the most important bass modes on the module.

### Set exactly
- **Loop OFF**
- **Trig OFF**
- **Morph ON**
- **Spread OFF**
- **Chaos OFF**

### Then
- Main fractal: **Cantor**, **Mandelbrot**, **Koch**, **Sierpinski**, or **Dragon**
- Primitive: **Dragon**, **Hilbert**, **Rössler**, or **Fibonacci**
- Turn **Amount** around center and above
- Increase until the tone becomes metallic, unstable, or tearing

### Sound zones
- Below center: more self-feedback, denser/deformed
- Near center: neutral
- Above center: more proper fractal FM

### Bassline patch tip
Use a sequencer with:
- pitch CV into a voice
- gate/trig into trig input
- accent envelope into **Texture**
- slower modulation into **P-Chaos**

This produces bass phrases with stable pitch but moving overtone violence.

### For neuro / hyper-bass
Automate **Amount** itself with CV while in FM mode. Small CV moves near the center crossing point can dramatically change the spectral behavior.

---

## D. Stab bass / bass plucks
### Start here
- Main fractal: **Koch**, **Fibonacci**, **Cantor**, or **Hilbert**
- Primitive: **Dragon** or **Rössler**
- Texture: medium
- Morph: low-medium
- Chaos: low-medium
- Speed: medium-fast
- Amount: medium

### Switches
- **Loop OFF**
- **Trig ON**
- **Morph ON**
- optional **Chaos ON**

This makes each note speak with an internal motion envelope rather than a static tone.

### Extra patching
Use external envelope into **Spread CV** for pitch-tear on every hit.

Subtle version:
- low attenuation
- very fast decay

Extreme version:
- moderate attenuation
- medium decay

Result:
a “rip” or “bark” at note onset.

---

## E. Bass that mutates per step
Fractaos loves sequencer modulation lanes.

Use a sequencer row or CV track to step-modulate one of:
- Texture
- Morph
- F-Chaos
- P-Chaos
- Amount

Best combination:
- one stepped lane to **Texture**
- one slewed/random lane to **P-Chaos**
- internal primitive modulating **Morph**

That gives:
- step-specific tone
- overall living movement
- controlled unpredictability

---

# 3. Haunting atmospheric pads and drones

This is where Fractaos gets very special because of:
- Texture fractals
- Drone mode
- 8-oscillator chord spread
- slow primitive movement
- formant and resonance behavior

## A. Haunted drone pad
### Start here
- Enable **Drone**
- Main fractal: **Cloud**, **Storm**, **String**, **Ensemble**, or **Cluster**
- Primitive: **Julia**, **Rössler**, **Fibonacci**, or **Hilbert**
- Depth: medium-high
- Primitive Depth: medium
- Chaos: low-medium
- Primitive Chaos: low-medium
- Morph: low-medium
- Texture: medium-high
- Speed: very slow
- Amount: low-medium

### Spread in Drone mode
Use Spread in its three zones:

#### Zone 1: near 0
- 8 oscillators in unison
- dense central mass
- good for ominous mono-drones

#### Zone 2: 0.02–0.50
- gradual 8-oscillator widening up to +1 octave
- excellent for slowly opening a drone over time

#### Zone 3: 0.50–1.00
- chord and microtuning scan
- this is absolute gold for haunted harmonic beds

### Best pad performance move
Very slowly sweep Spread through the Drone chord region while also slowly modulating Texture.

This changes both:
- tuning relationships
- spectral identity

The result feels composed rather than merely filtered.

---

## B. Ghost choir / broken organ
### Start here
- Main fractal: **Ensemble**, **Cluster**, or **String**
- Primitive: **Fibonacci**, **Julia**, or **Koch**
- Morph: around center
- Texture: high
- Chaos: low
- Primitive Chaos: low-medium
- Speed: very slow
- Amount: medium

### Switches
- **Loop ON**
- **Morph ON**
- **Spread OFF**
- optional **Chaos ON** very lightly

### Why
Texture plus slow Morph modulation creates formant/vocal drift without requiring an actual vocal filter.

### Add external CV
- slow random into **Texture CV**
- slow triangle into **Morph CV**

Use tiny amounts. On Fractaos, subtle is often more eerie than extreme.

---

## C. Storm ambience with unstable harmonics
### Start here
- Main fractal: **Storm**
- Primitive: **Lorenz** or **Rule30**
- Texture: high
- Chaos: medium-high
- Primitive Chaos: medium
- Speed: very slow to slow
- Amount: medium-high

### Switches
- **Loop ON**
- **Chaos ON**
- optional **Morph ON**

The manual notes Storm can evoke thunder/dense rain depending on Amount, Chaos, Depth, and Texture. Modulating Chaos and Texture slowly is the key.

### Patch method
- very slow random CV -> **F-Chaos**
- another slow CV -> **Texture**
- manual Spread sweeps in Drone mode chord zone

This creates weather systems, not just pads.

---

## D. Evolving chord cloud in Drone mode
### Start here
- Drone ON
- Main fractal: **Cloud** or **Cluster**
- Primitive: **Fibonacci** or **Rössler**
- Spread in Zone 3 chord area
- Texture: medium-high
- Speed: very slow
- Amount: low-medium

### Then perform:
- move Spread through:
  - Maj triad spread
  - Min triad spread
  - Major 7th
  - Minor 7th
  - Just intonation
  - 7-limit flavor
  - BP subset

The microtuning options especially will produce eerie, alien, haunted harmony.

### Best modulation addition
Use a slow CV into Pitch while in Drone mode for whole-cloud transposition. If you have four pitch CV sources, you can offset the four voice pairs separately while the 8-oscillator spread remains global.

---

# Best CV sources to pair with Fractaos

Fractaos rewards particular modulation types.

## Best for percussion
- short decay envelopes
- accent envelopes
- stepped random
- burst generators
- trigger-synced sample & hold

Use these on:
- Chaos
- Texture
- Morph
- Spread

## Best for bass
- tempo-synced LFOs
- sequencer modulation lanes
- envelopes with adjustable decay
- slewed random
- manual controller CV

Use these on:
- Texture
- Amount
- Morph
- Chaos

## Best for pads
- ultra-slow LFOs
- smooth random
- looping envelopes
- manual joystick or fader
- quantized slow CV for Drone Spread chord selection

Use these on:
- Texture
- Morph
- Pitch
- Chaos very lightly

---

# Modulation destinations ranked by musical usefulness

## For distorted percussion
1. **F-Chaos**
2. **Texture**
3. **Morph**
4. **Spread**
5. **P-Chaos**

## For bass music
1. **Texture**
2. **Amount**
3. **Morph**
4. **F-Chaos**
5. **Spread**

## For atmospheric pads
1. **Spread** in Drone mode
2. **Texture**
3. **Morph**
4. **Pitch**
5. **P-Chaos / F-Chaos** in very small amounts

---

# High-value switch combos

## 1. Retriggered animated note
- Loop OFF
- Trig ON
- Morph ON

Best for:
- plucks
- kicks
- snare hybrids
- bass stabs

## 2. Wobble machine
- Loop ON
- Morph ON
- Spread ON

Best for:
- dubstep movement
- chorused bass
- unstable drones

## 3. Attack violence
- Loop OFF
- Trig ON
- Chaos ON

Best for:
- drum transient corruption
- bass attack tear
- broken digital edge

## 4. Simplified FM
- Loop OFF
- Trig OFF
- Morph ON
- Spread OFF
- Chaos OFF

Best for:
- metallic basses
- harsh stabs
- distorted synth tones

## 5. Full internal turbulence
- Loop ON
- Morph ON
- Spread ON
- Chaos ON

Best for:
- extreme sound design
- horror drones
- glitch percussion
- mutant bass FX

Use attenuation and restraint here; it can get wild quickly.

---

# Three complete patch examples

## Patch 1: DnB reese destroyer
**Goal:** aggressive moving bass

### Panel
- Main: Cantor
- Primitive: Dragon
- Chaos: 35%
- Primitive Chaos: 45%
- Depth: 60%
- Primitive Depth: 45%
- Morph: 30%
- Spread: 40%
- Texture: 35%
- Speed: slow-medium
- Amount: 45%
- Pitch: low

### Switches
- Loop ON
- Spread ON
- optional Morph ON

### CV
- slow triangle LFO -> Texture CV
- accent envelope -> F-Chaos CV
- sequencer mod lane -> Morph CV

### Result
Wide, growling, moving bass with attack abrasion and phrase evolution.

---

## Patch 2: Broken industrial snare
**Goal:** distorted percussive hit with synthetic tail

### Panel
- Main: Snare
- Primitive: Rule30
- Chaos: 55%
- Primitive Chaos: 60%
- Depth: 40%
- Primitive Depth: 50%
- Morph: 50%
- Spread: 15%
- Texture: 60%
- Speed: fast
- Amount: 50%

### Switches
- Loop OFF
- Trig ON
- Morph ON
- Chaos ON

### CV
- trigger -> Fractaos trig
- fast envelope -> Texture CV
- stepped random -> P-Chaos CV

### Result
Snare hit with tearing digital edge, unstable brightness, and a weird tonal residue.

---

## Patch 3: Haunted microtonal fog
**Goal:** eerie ambient drone

### Panel
- Drone ON
- Main: Cluster
- Primitive: Fibonacci
- Chaos: 20%
- Primitive Chaos: 15%
- Depth: 70%
- Primitive Depth: 45%
- Morph: 35%
- Texture: 65%
- Speed: very slow
- Amount: 30%
- Spread: Zone 3, around Just intonation / 7-limit / BP subset

### Switches
- Loop ON
- Morph ON
- maybe very light Chaos ON

### CV
- slow random -> Texture CV
- ultra-slow triangle -> Morph CV
- manual performance on Spread

### Result
A drifting harmonic cloud with slightly uncanny tuning and spectral vocal-like motion.

---

# Practical performance tips

## 1. Keep one hand on Texture
If I had to choose a single performance knob on Fractaos for live interest, it would often be **Texture**. It can move the sound from:
- defined
- to resonant
- to organic
- to unstable
without simply acting like a plain filter sweep.

## 2. Use Chaos for transients, not only constant dirt
Especially for percussion and bass, Chaos is often strongest when it is:
- moderate at rest
- pushed by envelope/accent CV on attack

That preserves body while adding violence.

## 3. For bass, don’t overdo Morph immediately
Too much Morph can dissolve the core note. Start lower than you think, then add modulation. Bass usually hits harder when the center of gravity remains audible.

## 4. Use Drum curves with Morph for hybrid hits
This is one of the module’s signature tricks:
- drum transient
- geometric sustain
- fractured hybrid tone

Perfect for:
- neuro percussion
- cinematic impacts
- weird tom/bass hits

## 5. In Drone mode, Spread is compositional
On many modules, detune spread is just width. Here it becomes:
- interval architecture
- chord selection
- microtonal atmosphere

That’s much more powerful than typical unison spread.

---

# Best “quick-start” settings by genre

## Distorted percussion quick start
- Main: Snare / Kick / HiHat
- Primitive: Rule30 / Dragon / Collatz
- Trig ON
- Loop OFF
- Morph ON
- Chaos ON
- Texture medium-high
- envelope to F-Chaos or Texture

## Dubstep / DnB quick start
- Main: Cantor / Mandelbrot / Sierpinski / Rule30
- Primitive: Dragon / Rössler / Hilbert
- Loop ON
- Morph ON or Spread ON
- Texture medium
- Chaos medium
- sequencer CV to Texture
- try simplified FM mode for the nastiest tones

## Haunted pad quick start
- Main: Cloud / Cluster / Ensemble / Storm
- Primitive: Fibonacci / Julia / Rössler
- Drone ON
- Loop ON
- Morph ON
- very slow Speed
- medium-high Texture
- Spread in Zone 3 chord range
- very slow random CV to Texture

---

# Final takeaway

The most unique thing about Fractaos is that it doesn’t sound best when treated like a normal oscillator plus filter. It excels when you think in layers:

1. choose a fractal with the right native behavior  
2. choose a primitive with contrasting motion  
3. decide whether that motion should affect Morph, Spread, or Chaos  
4. use CV to animate Texture, Chaos, and Amount in restrained but purposeful ways  
5. for percussion, use retriggered modulation  
6. for bass, use simplified FM, Texture movement, and Spread  
7. for pads, use Drone mode and chord/microtuning Spread sweeps

If you want, I can also turn this into:
- a **cheat sheet of best fractal pairings**
- a **set of 20 patch recipes**
- or a **“what to patch into each CV input” guide**

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)