# Pittsburgh Modular — Synthesizer Box

- [Manual PDF](../../manuals/Synthesizer Box - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF](https://pittsburghmodular.com/s/Synthesizer-Box-Manual.pdf)

# Pittsburgh Modular Synthesizer Box: modulation ideas for extreme percussion, filthy bass, and haunted atmospheres

The **Synthesizer Box** is especially good for sound design because it is **internally normalized like a semi-modular voice**, but almost every important point can be overridden. That means you can start with the normal signal path for fast results, then break it apart for more aggressive or unusual patching.

## What matters most for modulation on this module

From the manual, the most important modulation opportunities are:

- **Oscillator FM**
  - Internal default: **LFO triangle → FM**
  - Switchable **linear/expo FM**
  - External override via **FM CV IN**
- **Oscillator waveform modulation**
  - Internal default: **LFO triangle → MOD CV**
  - Affects:
    - **square wave PWM**
    - **blade wave shape morphing**
  - External override via **MOD CV IN**
- **Blade input**
  - Additional manipulation of the **blade** waveform via **BLADE IN**
- **LPG CV**
  - Internal default: **Envelope out → LPG CV**
  - Can operate in:
    - **VCA**
    - **LPG**
    - **Lowpass filter**
  - Has **MOD/PING** behavior switch
- **VCA CV**
  - Internal default: **Envelope out → VCA CV**
  - Override via **VCA CV IN**
- **Glide**
  - Hardwired between **1V/O IN** and oscillator for sliding phrases
- **LFO**
  - Has **triangle and square outputs**
  - Wide range, including **audio-rate FM territory**

That combination gives you the raw materials for:
- tearing, unstable attacks
- basses with moving harmonics
- ringing LPG percussion
- pitch-diving drum sounds
- pseudo-duophonic layered timbres via multiple oscillator outs
- slow evolving drones/pads

---

# General sound-design strategies on this module

Before the specific patches, here are the big ideas:

## 1. Use the internal routings, then override one thing
The module already gives you:
- LFO to oscillator FM
- LFO to oscillator MOD
- envelope to LPG
- envelope to VCA
- LPG to VCA

This means one of the easiest ways to get unusual results is:
- leave most of the internal normalization intact
- patch just **one external feedback or cross-modulation path**

That preserves musicality while adding chaos.

## 2. The LPG is your secret weapon
The **lopass gate** is not just a filter or VCA. In LPG mode it adds a very natural, woody, decaying contour. But when driven hard with harmonically rich waves, it can become:
- snappy and clicky
- rubbery
- thumpy
- oddly distorted in a very organic way

For percussive and bass sounds, this is arguably the most characterful section of the module.

## 3. The blade wave is likely your “aggression” source
The **blade wave** is described as a unique complex saw that responds to modulation and can be further altered via **BLADE IN**. This is exactly the sort of waveform you want for:
- snarling basses
- scraping growls
- metallic percussion
- eerie textures

## 4. Audio-rate modulation is the key to dirt
Because the LFO has a **high range** and is described as suitable for **audio-rate frequency modulation**, you should absolutely use it not only as an LFO but as a second audio-ish modulation source.

That’s how you get:
- distortion without a distortion module
- tearing sidebands
- metallic grit
- vocal-ish bass movement

---

# Patch ideas for distorted percussive sounds

## 1. LPG ping kick / tom / wood-hit
This module is very well suited for percussive pings.

### Patch
- Set oscillator to a low or mid frequency
- Use **MIX OUT → LPG IN**
- Set LPG to **PING**
- Set LPG mode to **LPG**
- Patch a trigger/gate sequence into **ENV IN**
- Patch **ENV OUT → LPG CV IN** if you want explicit control rather than relying on normalization
- Use **LPG OUT → VCA IN**
- Use **VCA OUT** as final output

### Settings
- Envelope:
  - Attack very low
  - Decay short to medium
  - Sustain low/off
  - Release short
- LPG frequency around low-mid
- Resonance only matters in lowpass mode, so ignore it in LPG mode
- Oscillator mix:
  - start with **triangle + sub**
  - then add square or blade for grit

### Why it works
In **PING** mode, the module converts incoming modulation into a short excitation. This makes the LPG behave almost like a struck acoustic object.

### To make it dirtier
- Add **square wave** into the mix
- Switch saw/blade to **blade**
- Turn up **MOD CV** so the blade is moving during each strike
- Put LFO in **high range** and let it modulate oscillator waveform or FM

### Variations
- **Kick**: low pitch, mostly triangle/sub, short decay
- **Tom**: slightly higher pitch, some square, medium decay
- **Wood block / knock**: higher pitch, blade wave, short LPG decay, pinged hard

---

## 2. Broken industrial snare / clap-ish hit
Use noise-like harmonic motion from FM and waveform animation rather than actual noise.

### Patch
- Mix **square + blade**
- Set LFO to **high range**
- Use LFO **TRI OUT → FM CV IN**
- Use LFO **SQR OUT** or a gate pattern into **ENV IN**
- Route **MIX OUT → LPG IN → VCA IN**
- LPG mode:
  - start in **LOPASS** for sharper spectral shaping
  - try **LPG** for a more acoustic smack

### Settings
- Oscillator pitch in upper-mid range
- FM amount moderate to high
- Try **linear FM** first for metallic textures
- Set waveform MOD amount medium-high
- Envelope decay short
- VCA envelope short-medium

### Why it works
A single oscillator under fast FM can create noisy, splashy upper partials. Filtering or LPG striking turns that into a synthetic snare-like transient.

### Make it more distorted
- Patch **S/B OUT back into BLADE IN**
- Keep the level controlled at the source mixer
- This can create unstable, ripping harmonic folding behavior
- If too extreme, reduce saw/blade level before feeding back

This is one of the best “illegal” patches on a module like this: mild self-patching for internal abuse.

---

## 3. Zappy electro percussion with pitch envelope illusion
There’s no dedicated pitch envelope, but you can fake one.

### Patch
- External envelope or triggerable CV source → **FM CV IN**
- If you only have the Synthesizer Box:
  - mult **ENV OUT**
  - one copy goes to normal VCA duties
  - second copy goes to **FM CV IN**
- Use oscillator as source into LPG or VCA

### Settings
- Use **expo FM** for punchier pitch sweep character
- Keep FM attenuator fairly low at first
- Envelope:
  - fast attack
  - short decay
  - zero sustain
  - short release

### Result
You get a quick falling-pitch thwack that works for:
- kicks
- laser toms
- zaps
- synthetic congas

### Trick
Use **triangle wave only** for classic electro percussion, then blend in **blade** for the distorted version.

---

## 4. Metallic percussion using audio-rate waveform modulation
This module’s waveform modulation is special because it affects:
- **square PWM**
- **blade morph**

### Patch
- Set LFO to **high range**
- Patch **LFO TRI OUT → MOD CV IN**
- Use **square** or **blade** heavily in the mix
- Send **MIX OUT → LPG IN**
- Set LPG to **LOPASS** or **LPG**
- Trigger envelope normally

### Why it works
Audio-rate PWM and wave-morphing can create inharmonic overtones, which read like:
- metal
- broken circuitry
- bent cymbal-like textures
- machine chatter

### Extra move
Patch **LFO SQR OUT → ENV IN** for repeated machine-gun pulses while triangle output modulates timbre.

---

# Patch ideas for crazy dubstep / drum & bass basslines

## 1. Basic reese-ish bass
A true Reese usually uses detuned oscillators, but you can get into related territory with internal harmonic motion and modulation.

### Patch
- Use **square + blade + sub**
- Patch **MIX OUT → LPG IN**
- LPG mode = **VCA** or **LOPASS**
- Patch envelope normally to VCA
- Use **LFO TRI OUT → MOD CV IN**
- Optionally also send modulation to **FM CV IN**

### Settings
- Pitch low
- Glide medium
- Blade selected rather than plain saw
- MOD amount medium
- LFO rate synced slow-medium for wobble phrases
- LPG in **lowpass** for bass sculpting
- Filter frequency moderate, resonance low to moderate

### Why it works
The moving blade plus PWM-like square motion creates internal beating and spectral animation that can mimic multi-oscillator movement.

### Performance tip
Sequence long notes with **glide** on. That sliding motion is essential for DnB and dubstep phrasing.

---

## 2. Talking wobble bass
This module can do vocal-ish sounds by combining:
- filter/LPG movement
- waveform morphing
- moderate FM

### Patch
- Oscillator mix: mostly **blade**, some **square**, some **sub**
- **MIX OUT → LPG IN**
- LPG in **LOPASS**
- Envelope to VCA as usual
- LFO triangle internally or externally to **MOD CV IN**
- Patch another modulation source or the same LFO to **LPG CV IN**
- If possible from your system, use two related-but-different modulation sources:
  - slow one to LPG cutoff
  - faster one to MOD CV

### Settings
- LFO to MOD: medium-high
- LPG cutoff fairly low
- Resonance moderate
- FM low to medium, often better in **linear FM**
- Glide medium-high

### Why it works
The oscillator’s harmonic structure changes while the filter shape moves, creating formant-like vowel motion.

### To make it nastier
- Switch from triangle-heavy to more square/blade
- Push FM harder
- Use **audio-rate LFO** for short sections
- Momentarily switch LPG from **LOPASS** to **LPG** for more plucky articulation

---

## 3. Neuro-style tearing bass
This is one of the most promising sounds on this module.

### Patch
- Use **blade** as primary wave
- Add sub for weight
- Set LFO to **high range**
- Patch **LFO TRI OUT → FM CV IN**
- Patch another mod source to **MOD CV IN**, or leave internal LFO normalled there if helpful
- **MIX OUT → LPG IN**
- LPG in **LOPASS**
- Moderate resonance
- **LPG OUT → VCA IN → VCA OUT**

### Settings
- Start with **linear FM**
- Increase FM until harmonics begin to shred
- Then sweep between **linear** and **expo** to compare:
  - **linear** = more metallic, sideband-rich, controlled
  - **expo** = more unruly, aggressive, screaming
- Keep cutoff moving slowly with envelope or another CV
- Use glide on sequenced notes

### Secret sauce
Patch **ENV OUT → LPG CV IN** and let the envelope smack the filter on each note while FM is already active. This creates a pronounced front-edge “bark” to each bass note.

### Further abuse
Try:
- **S/B OUT → BLADE IN**
- or **SQR OUT → BLADE IN**

This can create feral harmonic interactions that sound much larger than a single oscillator voice.

---

## 4. Machine bass with rhythmic internal modulation
Good for stuttering DnB bass figures.

### Patch
- Sequence pitch into **1V/O IN**
- Use **LFO SQR OUT** as a rhythmic source elsewhere in your system, or to clock related modulation
- Use **LFO TRI OUT → MOD CV IN**
- Envelope into VCA normally
- LPG in **VCA** mode for cleaner amplitude, or **LOPASS** for movement

### Settings
- Short to medium envelopes
- Glide only on selected notes
- Oscillator mix:
  - sub high
  - square medium
  - blade medium-high
- Filter/LPG cutoff low-mid

### Result
A punchy, articulate bass that still has internal motion. Good when you want more note definition than full chaos.

---

## 5. Distorted bass without an external distortion module
The Synthesizer Box can fake distortion by stacking harmonic complexity before filtering.

### Patch recipe
- Turn up multiple waveforms in the mixer:
  - triangle low
  - square medium-high
  - blade high
  - sub to taste
- Apply:
  - moderate **audio-rate FM**
  - medium waveform modulation
- Run the result into:
  - **LPG in lowpass mode** with resonance just below self-emphasis
  - then into **VCA**

### Why this distorts
You are not clipping in the conventional pedal sense; instead you are:
- increasing harmonic density
- creating sidebands with FM
- reshaping the spectrum dynamically
- then filtering it for focus

That often reads as “modular distortion,” especially in bass contexts.

---

# Patch ideas for haunting atmospheric pads and drones

This is a monophonic voice, so don’t think “poly pad.” Think:
- evolving drone
- pseudo-pad texture
- eerie sustained atmosphere
- layered timbral wash

## 1. Slow haunted drone
### Patch
- Use **triangle + blade** with a little sub
- Set LFO to **low range**
- Let internal LFO routing modulate FM and/or MOD
- Use **MIX OUT → LPG IN**
- Set LPG to **LOPASS**
- Use a long gate into **ENV IN**
- Envelope:
  - long attack
  - medium-long decay
  - sustain high
  - long release
- **LPG OUT → VCA IN → VCA OUT**

### Settings
- FM amount very low
- MOD amount low-medium
- LPG cutoff fairly low
- resonance low to medium
- glide medium if sequencing note transitions

### Why it works
The blade wave’s slow morphing adds ghostly harmonic motion, while the lowpass gate/filter gently shapes the brightness over time.

---

## 2. Hollow choir-like texture
### Patch
- Prioritize **triangle + square PWM**
- Use LFO triangle to **MOD CV IN**
- Keep FM low or off
- Filter in **LOPASS**
- Slow envelope

### Why it works
PWM-like movement on the square can create a hollow, vocal quality. Blending triangle smooths it out.

### Extra move
Slightly open the filter and use a little resonance for a breathy, formant-adjacent character.

---

## 3. Unstable cinematic dread drone
### Patch
- Use mostly **blade**
- Add a little square
- Set LFO to **high range but low modulation depth** into **FM CV IN**
- Also use a very slow modulation source to **LPG CV IN**
- Hold long notes or manually drone the oscillator

### Why it works
Tiny amounts of audio-rate FM create subtle inharmonic shimmer and dread. It stops sounding like a normal analog oscillator and starts sounding haunted.

### Important
Keep FM amount low. Too much and it becomes bass/industrial. Tiny amounts are where the eerie magic lives.

---

## 4. Self-animated evolving texture
Use the normalized routings as a self-contained ambient machine.

### Patch
- No special patching required initially
- LFO internally modulates oscillator FM and waveform
- Envelope controls LPG and VCA
- Just patch:
  - pitch CV to **1V/O IN**
  - gate to **ENV IN**
  - audio from **VCA OUT**

### Then refine
- Put LFO in **low range**
- Set envelope to long attack/release
- Use blade wave with some triangle
- LPG in **LOPASS**
- Moderate resonance

### Result
Very playable atmospheric lines with internal motion and no cable complexity.

---

# Best modulation sources and destinations on this module

## Most powerful destinations
### 1. MOD CV IN
Best for:
- vocal bass movement
- metallic percussion
- animated drones
- PWM aggression

Because it affects both:
- square width
- blade morph

this is one of the richest destinations on the module.

### 2. FM CV IN
Best for:
- tearing bass
- synthetic percussion
- unstable atmospheres
- clangorous textures

Try both **linear** and **expo** every time:
- **linear** for more deliberate, “designed” motion
- **expo** for more unstable, raw behavior

### 3. LPG CV IN
Best for:
- plucks
- pings
- spectral articulation
- dynamic natural decay
- vowel-like bass movement

### 4. BLADE IN
Best for:
- weirdness
- feedback-adjacent patches
- external audio-rate modulation
- turning the oscillator into something more complex than a basic VCO

If you want “unique,” this is one of the first jacks to experiment with.

---

# Self-patching ideas

These are especially useful because the module exposes multiple oscillator outs.

## 1. SQR OUT → BLADE IN
Creates aggressive harmonic interaction.
Great for:
- neuro bass
- metallic percussion
- tearing leads

## 2. S/B OUT → FM CV IN
Use carefully. This can get wild quickly.
Great for:
- screaming bass
- unstable drones
- dirty acid-adjacent tones

## 3. TRI OUT → LPG CV IN
Can create smoother internal animation than square/blade-based modulation.

## 4. MIX OUT → external attenuator/VCA → back to BLADE IN or FM CV IN
If your rack has attenuation, this becomes much more controllable and can produce very sophisticated chaos.

---

# Genre-focused recipes

## Distorted percussion quick recipe
- Wave: blade + square
- LFO: high range
- LFO TRI → FM CV IN
- Envelope fast
- LPG: PING + LPG mode
- Short decay
- Output from VCA OUT

## Dubstep wobble quick recipe
- Wave: sub + blade + square
- Glide: medium
- LFO slow-medium to MOD CV
- LPG in lowpass mode
- Moderate resonance
- Envelope to VCA and LPG
- Sequence long slides and syncopated gates

## DnB reese/growl quick recipe
- Wave: sub + square + blade
- FM: moderate, linear first
- MOD: medium-high
- Filter/LPG lowpass
- Short-medium amp envelope
- Fast note changes with occasional glide
- Try self-patching SQR OUT → BLADE IN

## Haunted pad quick recipe
- Wave: triangle + blade
- LFO low range
- Very low FM depth
- Slow waveform modulation
- LPG lowpass mode
- Long attack/release
- Sustain high

---

# Practical performance tips

## Use the sub oscillator strategically
The sub is one octave below and can massively reinforce bass patches. But too much sub can mask the timbral movement. For filthy bass:
- get the midrange growl right first
- then add sub until the weight appears

## Use LPG mode switching as a performance gesture
The three LPG modes dramatically reshape the voice:
- **VCA** = cleaner, more straightforward
- **LPG** = organic, woody, percussive
- **LOPASS** = strongest spectral sculpting

Switching modes mid-performance can make a bassline jump from:
- tight and dry
- to round and acoustic
- to filtered and speaking

## High-range LFO is not just an LFO
Treat it like a bonus oscillator/modulator. That’s where many of the “how is this one voice doing that?” sounds will come from.

## Glide is essential for bass genres
Especially for:
- dubstep bends
- DnB transitions
- menace-filled mono leads
- portamento into growls

---

# A few especially strong example patches

## Patch 1: Filthy dubstep growler
- Pitch CV → **1V/O IN**
- Gate → **ENV IN**
- Mix mostly **blade**, some **square**, some **sub**
- **LFO TRI OUT → FM CV IN**
- Internal or external modulation to **MOD CV IN**
- **MIX OUT → LPG IN**
- LPG mode = **LOPASS**
- **LPG OUT → VCA IN**
- **VCA OUT** to mixer
- Glide around 10–11 o’clock
- Linear FM first, then test expo

## Patch 2: Distorted synthetic snare
- Oscillator in upper-mid register
- Square + blade in mix
- **LFO high range → MOD CV IN**
- **ENV OUT → FM CV IN**
- **MIX OUT → LPG IN**
- LPG in **LOPASS**
- Fast envelope
- Moderate resonance
- Output from VCA

## Patch 3: Ghost drone
- Triangle + blade
- Slow gate or sustained trigger to ENV
- Long A/R, high sustain
- LFO low range to MOD
- Tiny amount of FM
- LPG in lowpass mode
- Low cutoff, low-mid resonance
- Optional: **TRI OUT → BLADE IN** very lightly if you have attenuation

---

# Final thoughts

The Synthesizer Box may look like a compact classic voice, but the real personality comes from combining:

- **blade waveform**
- **waveform modulation**
- **switchable linear/expo FM**
- **audio-rate LFO**
- **LPG in ping/lopass modes**
- **self-patching through BLADE IN, FM CV IN, and LPG CV IN**

If your goal is:
- **distorted percussion**: abuse **PING**, fast envelopes, and audio-rate modulation
- **dubstep / DnB bass**: use **blade + sub**, FM, moving waveform modulation, and glide
- **haunting atmospheres**: use slow blade morphing, tiny FM, and long LPG/VCA shaping

If you want, I can also turn this into:
1. a **set of 10 named patches with knob starting positions**, or  
2. a **signal-flow cheat sheet** for the Synthesizer Box.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)