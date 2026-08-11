# xaoc Devices — Sopot

- [Manual PDF](../../manuals/DocFractaosEN-V1.5.pdf)

---

[Fractaos Manual PDF](https://kaona.fr/wp-content/uploads/2025/07/Manual_Fractaos_EN.pdf)

# Fractaos modulation ideas for distorted percussion, insane bass, and haunted pads

Fractaos is unusually deep because it’s not just “oscillator + filter.” You’re modulating:

- the **main fractal**
- the **primitive fractal**
- the **relationship between them**
- a **primitive-derived LFO/envelope**
- a **fractal filter / texture layer**
- **spread/detune behavior**
- and in some modes, the whole voice architecture changes

That means the best sounds come from **stacked modulation with intention**, not just wiggling one CV.

---

# First: what’s worth modulating on Fractaos

From the manual, the most important modulation destinations are:

- **Morph**: blends driver/follower in a complex way, not just crossfade
- **Spread**: detune between driver/follower, or chord spacing in Drone mode
- **Texture**: resonant/filter/formant/organic detune behavior
- **Chaos / Primitive Chaos**: often the most dramatic timbral motion
- **Speed / Amount**: controls the primitive-derived modulation/LFO behavior
- **Pitch CV**: obvious, but especially powerful with unstable fractals
- **Switch combinations**:
  - **Morph switch ON alone** with others OFF = **simplified FM mode**
  - **Loop/Trig** changes whether primitive motion is free-run or retriggered per note

Also note:
- **Depth** and **Primitive Depth** are stepped and **not CV modulatable**
- Drum/textures can only be the **main fractal**
- Primitive can only be one of the **14 geometric fractals**

So your live modulation focus should be on:
**Chaos, Primitive Chaos, Morph, Spread, Texture, Speed, Amount, Pitch**

---

# General patch philosophy

For Fractaos, strong patches usually use 3 modulation layers:

1. **Fast envelope or trigger-shaped CV**  
   For attack, hit, snap, growl, transient

2. **Medium rhythmic modulation**  
   Synced LFO, envelope follower, sequencer lane, random stepped CV

3. **Slow drift**  
   Slewed random, slow LFO, pressure, aftertouch, manual moves

A great rule for this module:

- use **Chaos** for instability
- use **Morph** for identity shift
- use **Texture** for “produced” or “alive” quality
- use **Spread** for width / aggression / chordal weirdness

---

# 1. Distorted percussive sounds

Fractaos has 5 dedicated drum fractals:
- Kick
- Tom
- Snare
- HiHat
- Cymbal

These are not samples; they’re real-time models. That means modulation can make them feel much more alive than static drum voices.

## Best modulation targets for drums

## A. Chaos CV for hit variation
This is probably the single most important drum modulation.

Patch:
- send a **random stepped CV** or **sample-and-hold per trigger**
- attenuate lightly
- route to **F-Chaos** (main fractal chaos)

Why:
- on drum fractals, Chaos changes roughness, instability, explosive character, internal detuning
- even small amounts can make repeated hits feel human or violently synthetic

Use for:
- snarls on snares
- alternate kick dirt
- varying hi-hat brightness/choke

**Tip:** clock a random source from the same trigger sequence driving the drum input.

---

## B. Texture CV for crushed, resonant drum tones
Texture is not just brightness. It affects:
- resonance
- formant detection/application
- micro-detuning
- filter intensity

Patch:
- envelope to **Texture CV**
- medium attenuation
- fast attack, short decay

Result:
- each hit “barks” or resonantly tears open at onset
- great for metallic snares, tearing hats, gnarly toms

If you want more destruction:
- keep **Texture knob already high**
- then modulate around that point with an envelope

That gives a more unstable, overdriven-feeling transient.

---

## C. Morph CV to add tonal tail onto drums
Drum curves can morph against a geometric primitive. The manual specifically notes:
- Morph can blend percussive attack with harmonic tail or note-like body
- FM has no effect on drum curves, but Morph still matters

Patch:
- choose a drum main fractal
- choose a geometric primitive like **Mandelbrot, Rule30, Koch, Sierpinski, Dragon**
- send envelope or velocity CV to **Morph**

What happens:
- low Morph = drum hit
- higher Morph = drum plus tonal/ringing/fractal sustain
- dynamic Morph = each hit opens into a pitched or metallic tail

Great pairings:
- **Kick + Fibonacci/Koch** for tuned industrial kicks
- **Snare + Rule30** for digital reese-snare hybrids
- **HiHat + Hilbert** for glitchy rectangular metallic hats
- **Tom + Dragon** for torn membrane/bass percussion

---

## D. Triggered primitive motion for per-hit animation
Use the switch logic:

- **Loop OFF**
- **Trig ON**

This makes primitive modulation retrigger per note/hit.

Then choose:
- **Morph ON** and/or
- **Chaos ON** and/or
- **Spread ON**

Now each trigger restarts the primitive-shaped modulation curve.

This is huge for percussion because it creates:
- identical attack contour with evolving spectral motion
- “designed transient” behavior
- almost like an internal modulation envelope per hit

Patch recommendation:
- Drum fractal main
- Primitive = **Lorenz**, **Hénon**, or **Rule30**
- moderate **Speed**
- moderate/high **Amount**
- switches: **Trig ON**, **Loop OFF**, **Chaos ON**, maybe **Morph ON**

Result:
- every hit blooms into internal fracture and dirt
- especially good for neuro-style snares and synthetic toms

---

## E. Pitch modulation for kick/tom aggression
The manual says Kick and Tom respond tonally to MIDI pitch.

Patch:
- send a sharp downward envelope via pitch CV path externally, if available in your system chain
- or sequence pitch changes rapidly over steps
- combine with Chaos modulation

Since Fractaos has 1V/oct inputs per voice, one powerful move is:
- send a **main pitch sequence**
- mult it
- send a **brief negative envelope offset** through a precision adder/mixer to create pitch drop on certain hits

This gives:
- harder kick punches
- rave tom drops
- jungle-style tuned perc runs

---

## Distorted percussion recipes

## Recipe: industrial kick
- Main fractal: **Kick**
- Primitive: **Koch** or **Fibonacci**
- Morph: low to medium
- Texture: medium-high
- Chaos: medium
- Spread: low
- Trig ON, Loop OFF, Chaos ON

Modulate:
- random CV to **F-Chaos**
- short envelope to **Texture**
- accent CV to **Morph**

Sound:
- body stays kick-like
- transient tears and tail becomes metallic/tonal
- ideal through external saturation/wavefolder

---

## Recipe: neuro snare
- Main: **Snare**
- Primitive: **Rule30** or **Dragon**
- Morph: medium
- Texture: high
- Chaos: medium-high
- Primitive Chaos: medium
- Speed: medium
- Amount: medium-high
- Trig ON, Loop OFF, Morph ON, Chaos ON

Modulate:
- stepped random to **F-Chaos**
- velocity/accent to **Morph**
- envelope to **Texture**

Sound:
- synthetic crack
- noisy digital body
- unstable metallic tail

---

## Recipe: broken hat machine
- Main: **HiHat** or **Cymbal**
- Primitive: **Hilbert** or **Sierpinski**
- Texture: high
- Chaos: medium-high
- Spread: low-medium
- Speed: medium-high
- Amount: medium

Modulate:
- Euclidean trigger variations
- sample-and-hold to **F-Chaos**
- subtle CV to **Spread**
- accent envelope to **Morph**

Sound:
- shifting metallic clusters
- artificial open/close tone changes
- beautiful when layered with analog hats

---

# 2. Crazy basslines for dubstep / DnB / neuro

This is where Fractaos looks especially dangerous.

For bass, the key features are:
- **simplified FM mode**
- **Chaos modulation**
- **Morph sweeps**
- **Texture resonance/formants**
- **Spread detune**
- unstable fractals like **Rule30, Lorenz, Hénon, Dragon**

---

## Core bass move: simplified FM mode
Manual setup:

- **Loop OFF**
- **Trig OFF**
- **Morph ON**
- **Spread OFF**
- **Chaos OFF**

This enables simplified FM mode.

Then:
- **Amount** becomes bipolar:
  - 0–50% = internal feedback
  - center = neutral
  - 50–100% = primitive modulates main fractal frequency

This is one of the best bass engines in the module.

## How to use it musically
- Keep bass notes low
- Set main fractal to something stable/aggressive:
  - **Cantor**
  - **Sierpinski**
  - **Koch**
  - **Rule30**
  - **Dragon**
- Use primitive:
  - **Rössler** for smoother motion
  - **Lorenz** for wildness
  - **Hénon** for instability
  - **Mandelbrot** for brightness

Now perform **Amount** slowly or sequence it with CV.

Results:
- below center = sharper, denser, feedback bass
- above center = metallic fractal FM growl
- near transition point = sweet spot for talking / ripping timbre shifts

**Important idea:** sequence or modulate **Amount** rhythmically to move between feedback bass and FM bass within a phrase.

---

## Best modulation targets for bass

## A. Morph CV for vowel/growl movement
Morph is not a simple blend; it changes how the two fractals interact.

Patch:
- synced triangle LFO, envelope, or sequencer lane to **Morph**
- medium attenuation
- slow for evolving growl
- fast per-note for talking bass

Best with:
- main = **Cantor, Dragon, Rule30, Koch**
- primitive = **Lorenz, Mandelbrot, Rössler**

Sound:
- bass opens and mutates instead of just filtering brighter
- more “resynthesis” than subtractive sweep

This is one of the strongest “dubstep vowel” controls in the module.

---

## B. Chaos CV for tearing bass edges
Chaos can be subtle on some fractals, extreme on others.

Patch:
- mod wheel / aftertouch / envelope / sequencer lane to **F-Chaos**
- use small attenuation first

Best fractals for bass chaos response:
- **Dragon**
- **Rule30**
- **Lorenz**
- **Hénon**
- **Logistic**
- **Hilbert**

Use:
- slow swept Chaos for evolving movement
- accented Chaos for specific aggressive notes
- random Chaos for “alive” reese movement

This creates:
- tearing harmonics
- unstable sidebands
- pseudo-formant breakups
- dirt without external distortion

---

## C. Spread CV for reese-like detune and widening
Outside Drone mode, Spread detunes driver and follower, up to +1 octave on follower.

Patch:
- slow LFO or envelope to **Spread**
- keep attenuation modest

Use cases:
- low amount: reese phasing / beating
- medium amount: ripping upper harmonic bloom
- envelope modulation: bass attacks widen then settle
- audio-rate-ish external modulation is probably too much, but medium speed can be nasty

For DnB:
- use low-mid Spread plus high Texture
- then modulate Chaos
- gives moving reese texture without relying only on filter detune

---

## D. Texture CV for talking and ripping resonances
Texture is essential for modern bass.

Patch:
- assign an envelope or synced LFO to **Texture**
- sweep around medium-high settings

Why it works:
- formant extraction / resonance emphasis gives vocal-like edge
- combined with Morph it can produce “talking” movement
- combined with Chaos it becomes savage

A very strong combo:
- **Texture as the macro vocal motion**
- **Morph as the internal identity shift**
- **Chaos as the destruction amount**

---

## E. Triggered modulation for note-synced bass articulation
Set:
- **Loop OFF**
- **Trig ON**

Then enable one or more of:
- Morph
- Spread
- Chaos

Now every note retriggers the primitive modulation shape.

This gives consistent, designed bass articulation:
- same growl contour every note
- great for sequenced neuro bass
- almost like a wavetable scan envelope, but stranger

Patch:
- 16th-note bassline into MIDI or 1V/oct + trig
- Primitive = **Lorenz** or **Hénon**
- Speed = synced by ear
- Amount = medium-high
- Morph switch ON
- Chaos switch ON

Result:
- each note bites, twists, then settles
- very useful for DnB “one-shot growl phrase” programming

---

## Bass patch recipes

## Recipe: talking dubstep bass
- Main: **Cantor** or **Koch**
- Primitive: **Mandelbrot** or **Rössler**
- Morph: medium
- Texture: high
- Spread: low-medium
- Chaos: low-medium
- Speed: slow-medium
- Amount: medium
- Trig ON, Loop OFF, Morph ON

Modulate:
- LFO to **Morph**
- envelope or second LFO to **Texture**
- accent lane to **Chaos**

Sound:
- vocal movement
- squelchy/formant-rich opening
- good for half-time wobble

---

## Recipe: neuro reese destroyer
- Main: **Rule30** or **Dragon**
- Primitive: **Lorenz**
- Spread: low-mid
- Texture: high
- Chaos: medium-high
- Primitive Chaos: medium
- Morph: medium-high
- Speed: medium
- Amount: medium-high
- Trig ON, Loop OFF, Chaos ON, Morph ON, maybe Spread ON

Modulate:
- slow CV to **Spread**
- sequencer lane to **Chaos**
- envelope to **Texture**
- subtle random to **Primitive Chaos**

Sound:
- layered beating
- internal tearing
- snarling upper mids
- works beautifully through external lowpass + distortion

---

## Recipe: FM sub/growl hybrid
- Use **simplified FM mode**
- Main: **Sierpinski** or **Koch**
- Primitive: **Rössler** or **Mandelbrot**
- Amount centered then pushed above center
- Texture: medium
- Spread: low
- Pitch: low register

Modulate:
- slow CV to **Amount**
- envelope to **Texture**
- performance control to **Chaos**

Sound:
- solid sub root
- moving metallic overtones
- can move from clean to mutant fast

---

# 3. Haunting atmospheric pads and drones

Fractaos is built for this. The six texture fractals plus Drone mode and chord Spread are where the module becomes a real atmosphere machine.

Texture fractals:
- Cloud
- Storm
- Aliasing
- String
- Ensemble
- Cluster

These are only available as the main fractal, which makes sense.

---

## Best approach for pads

Use:
- **Drone mode**
- slow modulation
- high Texture
- subtle Morph animation
- chordal Spread zone
- CV pitch offsets on voices if available

Drone mode changes architecture:
- 8 oscillators all run continuously
- Spread becomes:
  - unison zone
  - linear octave spread
  - predefined chords / microtunings

This is gold for pad work.

---

## A. Drone mode + chord scanning
The upper half of Spread in Drone mode scans predefined chords and tunings.

This means Spread becomes a macro harmonic control:
- unison cluster
- major/minor spreads
- sus/fifths
- 7ths
- add9/11/13
- just intonation
- 7-limit
- 19-TET
- Bohlen-Pierce subset

Patch:
- enable Drone
- main fractal = **Cloud**, **Ensemble**, **Cluster**, or **String**
- slowly modulate **Spread CV**
- use a slewed random or very slow LFO

Result:
- harmonic fields morph over time
- chord transitions smear due to detune slew
- eerie tuning systems create haunted, non-keyboard atmospheres

Best weird zones:
- **Just intonation**
- **7-limit flavor**
- **19-TET slice**
- **BP subset**

These are especially good if you want “beautiful but wrong.”

---

## B. Slow Morph modulation on texture fractals
Even though the main fractal is a texture, the primitive remains geometric.

Patch:
- main = **Cloud**, **Storm**, **String**, or **Cluster**
- primitive = **Hilbert**, **Rössler**, **Fibonacci**, or **Koch**
- slow LFO to **Morph**
- medium-low depth

What it does:
- injects a geometric skeleton into the noisy texture
- creates emergence/disappearance of tonal traces
- feels like spectral ghosts inside the pad

Great combinations:
- **Cloud + Fibonacci** = mournful, floating harmony
- **Storm + Hilbert** = broken digital weather
- **String + Koch** = bowed artifact haze
- **Cluster + Rössler** = unstable choral machine

---

## C. Very slow Chaos modulation for living pads
On texture fractals, Chaos changes internal motion and can create dramatic textural shifts.

Patch:
- very slow random or LFO to **F-Chaos**
- tiny attenuation
- optional second slow CV to **P-Chaos**

Why:
- too much fast modulation can make pads feel busy
- very slow Chaos changes create “breathing architecture”

This is especially effective with:
- **Storm**
- **Cloud**
- **Ensemble**
- **Cluster**

---

## D. Primitive as free-running modulation ecosystem
Set:
- **Loop ON**
- **Trig OFF**

Now the primitive-derived modulation runs freely.

Then enable:
- Morph and/or Chaos and/or Spread

This is ideal for pads because the motion is not tied to note events.

Patch:
- Drone mode ON
- Loop ON
- Morph ON
- Chaos ON
- Speed very low
- Amount medium

Result:
- independent internal life
- long non-repeating-seeming shifts
- evolving soundscape instead of cyclic synth pad

For best results:
- choose unstable primitive like **Lorenz** or **Hénon**
- keep amount moderate so it feels organic rather than seasick

---

## E. Texture modulation as spectral weather
Texture on texture fractals can get very expressive.

Patch:
- very slow triangle LFO or envelope follower to **Texture**
- keep base knob around medium-high
- modulate subtly around that point

Result:
- formants and resonances bloom and recede
- apparent distance changes
- pads go from soft wash to haunted vocal shimmer

If you have a joystick or expressive CV source:
- assign one axis to **Texture**
- assign the other to **Morph** or **Chaos**

That turns Fractaos into a live atmosphere instrument.

---

## F. Per-voice pitch offsets in Drone mode
Manual says 1V/oct pitch CVs of the 4 voices and MIDI notes can still transpose individual pairs in Drone mode.

That means you can:
- send slightly different pitch CVs to each voice
- create drifting clusters over the global 8-oscillator drone
- build pseudo-polytonal or suspended harmony

Patch ideas:
- send same root pitch to all four voices
- offset one voice +7 semitones
- offset another +12
- add subtle slewed random to one voice only

This creates huge, filmic moving harmonic beds.

---

## Pad recipes

## Recipe: haunted choir fog
- Drone mode ON
- Main: **Ensemble** or **Cluster**
- Primitive: **Fibonacci** or **Rössler**
- Texture: high
- Morph: low-medium
- Chaos: low
- Spread: upper chord zone, try just intonation or minor 7th
- Loop ON, Morph ON, Chaos ON
- Speed: very slow
- Amount: medium

Modulate:
- slow LFO to **Morph**
- subtle random to **Chaos**
- very slow CV to **Spread**

Sound:
- spectral choir
- shifting intonation
- ghostly consonance/dissonance

---

## Recipe: storm cathedral
- Drone mode ON
- Main: **Storm**
- Primitive: **Hilbert**
- Texture: high
- Chaos: medium
- Morph: low-medium
- Spread: 19-TET or BP subset
- Loop ON
- Speed: slow
- Amount: medium-high

Modulate:
- slow random to **Spread**
- slow envelope follower or LFO to **Texture**
- subtle CV to **Primitive Chaos**

Sound:
- weather, bells, broken harmonics, digital ruin
- very strong for dark ambient

---

## Recipe: broken string pad
- Main: **String**
- Primitive: **Koch** or **Fibonacci**
- Texture: medium-high
- Morph: medium
- Spread: add9/add11 in Drone mode
- Chaos: low-medium
- Loop ON, Morph ON
- Speed: slow

Modulate:
- slow LFO to **Morph**
- subtle random to **Spread**
- aftertouch to **Chaos** if using MIDI

Sound:
- fragile bowed/plucked illusion
- changing harmonic skeleton
- excellent with reverb

---

# 4. Specific modulation sources that pair well with Fractaos

Because Fractaos already has complex internals, it responds best to a few source types:

## Best external modulation sources
- **stepped random / sample & hold**
  - for Chaos and Primitive Chaos
- **short snappy envelopes**
  - for Texture and Morph on drums/bass
- **slewed random**
  - for pads, Spread, slow Chaos
- **sequencer modulation lanes**
  - for bass phrase design
- **pressure / aftertouch / mod wheel**
  - for performable Chaos/Texture movement
- **clocked LFO**
  - for dubstep wobble on Morph or Texture
- **Euclidean trigger accents**
  - to hit modulation VCAs before CV inputs

If you can place a **VCA on the modulation before Fractaos**, it becomes much more playable:
- trigger envelope opens VCA
- random CV passes through only on certain hits
- gives controlled chaos instead of constant chaos

---

# 5. Best fractal choices by goal

## For distorted percussion
- **Drum modes first**: Kick, Snare, Tom, HiHat, Cymbal
- primitives:
  - **Rule30**
  - **Dragon**
  - **Hilbert**
  - **Koch**
  - **Lorenz**

## For nasty bass
Main fractals:
- **Rule30**
- **Dragon**
- **Cantor**
- **Koch**
- **Sierpinski**
- **Hilbert**
- **Lorenz** for unstable experimental bass

Primitives:
- **Lorenz**
- **Hénon**
- **Rössler**
- **Mandelbrot**
- **Fibonacci**

## For haunted pads
Main fractals:
- **Cloud**
- **Storm**
- **String**
- **Ensemble**
- **Cluster**

Primitives:
- **Fibonacci**
- **Hilbert**
- **Rössler**
- **Koch**
- **Lorenz**

---

# 6. Three high-value modulation strategies

## Strategy 1: “accented destruction”
For drums or bass:
- steady sequence to pitch/gate
- accent trigger fires envelope
- envelope opens VCA carrying random CV
- VCA output goes to **Chaos** or **Texture**

Only accented notes get extra mutation.

This is perfect for:
- dubstep bass phrase punctuation
- snare fills
- broken kick patterns

---

## Strategy 2: “one macro, one damage, one drift”
Assign:
- **Morph** = macro movement
- **Chaos** = damage
- **Spread or Texture** = slow drift

This keeps patches musical.
If you modulate everything aggressively, Fractaos can become shapeless fast.

---

## Strategy 3: “stable main, unstable primitive”
For usable madness:
- pick a relatively stable main fractal
- pick a more unstable primitive
- use primitive motion to destabilize the sound indirectly

Examples:
- Main **Koch**, Primitive **Lorenz**
- Main **Sierpinski**, Primitive **Hénon**
- Main **Cloud**, Primitive **Hilbert**

This often sounds better than unstable-on-unstable.

---

# 7. Performance tips

- **Use presets for sound families**, not finished tracks  
  Fractaos seems ideal for storing starting points, then returning to LIVE and performing panel changes.

- In **LOAD mode**, you can align knobs to preset state and then jump back to LIVE. That’s very useful for recovering a patch and then improvising from it.

- In **MULTI mode**, you can combine:
  - one LIVE bass voice
  - one preset pad voice
  - one preset snare/perc voice
  - one extra texture voice

That could make Fractaos a whole mini track-generator inside one module.

- **Drone mode Spread is a feature, not just detune**  
  Treat it like harmonic composition control.

- **Texture is not just a finishing touch**  
  On this module it’s central to signature sound design.

---

# 8. My strongest recommendations if you want immediate results

## For distorted percussion
1. Start with a **Drum fractal**
2. Set **Trig ON / Loop OFF**
3. Modulate **Chaos**
4. Add envelope modulation to **Texture**
5. Use **Morph** to add pitched/fractal tail

## For dubstep / DnB bass
1. Try **simplified FM mode**
2. Sequence **Amount**, not just pitch
3. Modulate **Morph** for vowel motion
4. Add restrained **Chaos CV**
5. Use **Texture** as the formant/rip control

## For haunting pads
1. Use **Drone mode**
2. Choose **Cloud / Ensemble / Cluster / Storm**
3. Set **Loop ON**
4. Modulate **Spread** slowly through chord/tuning zones
5. Add very slow **Morph + Chaos** drift

---

# 9. Quick starter patches

## A. Dubstep wobble monster
- Main: Cantor
- Primitive: Lorenz
- Texture high
- Morph medium
- Spread low
- Chaos medium
- Trig ON, Loop OFF, Morph ON, Chaos ON
- LFO to Morph
- envelope to Texture
- sequencer lane to Chaos

## B. DnB reese
- Main: Rule30
- Primitive: Rössler
- Spread low-mid
- Texture high
- Chaos medium-high
- slow LFO to Spread
- random to Primitive Chaos
- lowpass and saturate externally

## C. Black-metal industrial snare
- Main: Snare
- Primitive: Dragon
- Morph medium
- Texture high
- Chaos high
- triggered random to Chaos
- short envelope to Texture

## D. Haunted film pad
- Drone ON
- Main: Cluster
- Primitive: Fibonacci
- Spread in Just Intonation or 7-limit
- Loop ON
- slow LFO to Morph
- slewed random to Spread
- subtle random to Chaos

---

If you want, I can also make you:
- a **“best fractals by genre” cheat sheet**
- a **CV patch plan using common modulation modules**
- or **10 exact Fractaos patches** for techno, dubstep, ambient, and IDM.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)