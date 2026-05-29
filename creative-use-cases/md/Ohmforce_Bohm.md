# Ohmforce — Bohm

- [Manual PDF](../../manuals/Bohm documentation.pdf)

---

[Manual PDF](https://ohmforce.com/wp-content/uploads/2025/03/Bohm_manual.pdf)

# Creative patch ideas for the Ohm Force Bohm system

Bohm is much more than a kick module. Reading through the manual, it’s really a **performance-oriented stereo kick workstation** with three distinct roles:

- **Bohm core** = main kick voice with pitch/gate behavior, CV-able macro control, model switching, snapshots
- **Groove expander** = secondary voice / rumble / top / envelope generator
- **Performer expander** = stereo sidechain, live FX bus, and external audio processor

That means you can use it as:

- a kick drum
- a bass synth
- a stereo transient processor
- a ducking hub
- a clock-relative rhythm shaper
- a live scene-recall instrument

Below are practical and creative ways to combine it with other Eurorack modules.

---

## 1. Turn Bohm into a playable bass voice

The manual makes it clear that Bohm can **track pitch at 1V/oct** if you:

- set **PITCH knob fully CCW**
- set **PITCH attenuverter fully CW**
- choose the correct **Pitch CV range** in system settings: `0..1V`, `1..2V`, or `2..3V`
- use **1V/oct**
- keep **LENGTH long enough** or use a **gate** at `HIT`

### Patch idea
Use a pitch sequencer or keyboard controller to play Bohm melodically while still behaving like a kick/bass hybrid.

### Great pairings
- **Intellijel Metropolix**
- **Make Noise René**
- **Winter Modular Eloquencer**
- **Arturia BeatStep Pro**
- Any **MIDI-to-CV** module with stable pitch output

### Why it’s interesting
Because Bohm’s models are not just simple sines. Many are wavetable/FM/sample-layered engines, so you can get:
- 808 basslines
- FM acid-ish low end
- industrial tuned tom/bass hits
- per-note kick changes in a groove

### Extra trick
Send:
- **pitch CV** to `PITCH`
- **gate** to `HIT`
- **velocity/accent CV** to `VELOCITY`

Now you have a dynamic bass instrument that still has kick articulation.

---

## 2. Use Groove as a modular techno rumble designer

Groove isn’t just a delay. It creates **clock-triggered repetitions**, reverb/noise/grit-sub layers, and a **tap-based envelope**. This is huge.

### Patch idea
Clock Groove at **16ths** or **triplets**, and trigger Bohm only on quarter notes. Use Groove to build:
- rolling techno rumble
- kick tops
- pumping noise wash
- sub-synced ghost hits

### Great pairings
- Clock source: **Pamela’s Pro Workout**, **Tempi**, **Shakmat Clock O’Pawn**
- Trigger sequencer: **Steppy**, **Varigate**, **Euclidean Circles**
- CV modulation for `TAPS`: **Stages**, **Zadar**, **Batumi**, **Ochd**

### Creative move
Use Groove `COLOR` to morph between:
- kick repetitions
- reverb-based body
- noise
- grit + sub

Then automate it with a slow CV to create a kick that evolves from tight to cavernous over 16 or 32 bars.

### Best companion modules
- **Filter** after Bohm output: for deep rumble sculpting
- **Stereo compressor**: glue the entire kick ecosystem
- **Saturation/waveshaper**: turn rumble into dirt

Examples:
- **SSF Stereo Dipole**
- **WMD Overseer**
- **Bastl Ikarie**
- **Joranalogue Fold 6**
- **Noise Engineering Ruina series**

---

## 3. Exploit the TAPS output as a modulation source

One of the most underrated features in the manual: Groove provides a **TAPS CV output**. System settings also let that output become:

- `GROOVE` envelope
- `I BOHM` inverted Bohm envelope
- `PERF` Performer ducking envelope
- `BOHM` non-inverted Bohm envelope

This means Bohm can act like a **rhythmic CV brain** for the rest of your system.

### Patch ideas

#### A. Animate a hi-hat VCA
Send `TAPS OUT` to a VCA controlling noise or hats.
- Kick triggers the groove envelope
- Groove taps create hat swells synced to kick structure

#### B. Sidechain external bass without a compressor
Set `TAPS OUT` to `I BOHM` or `PERF` and patch into:
- a VCA CV input
- a low-pass gate CV
- the level CV of a mixer channel

Now your modular bassline or drone ducks rhythmically.

#### C. Modulate filter cutoff rhythmically
Send `TAPS OUT` to:
- filter cutoff CV
- wavefolder amount
- delay feedback CV

This gives your entire patch a kick-related breathing pattern.

### Great pairings
- **VCAs**: Veils, Quad VCA, Tallin
- **Filters**: Belgrad, Ikarie, QPAS
- **Mixers with CV**: Mutamix, Tangle Quartet, Happy Nerding 3xVCA
- **Envelope followers / dynamics tools** to stack modulation behavior

---

## 4. Use Performer as your modular sidechain and DJ bus

Performer is not just an insert effect. It is a **ducking processor and performance effects bus** for external stereo audio.

### Core concept
Feed another part of your patch into Performer `IN`, and Bohm will duck it on each `HIT`.

This means you can sidechain:
- pads
- drones
- stereo loops
- a whole submixer
- granular clouds
- chord voices

### Great pairings
- **Stereo voice**: XPO, Ensemble Oscillator, Odessa, Plaits into stereo effects
- **Stereo mixer**: Xer Mixa, Cosmix Pro, Listen Four, Mixup + stereo FX
- **Sampler / loopers**: Morphagene, Lubadh, Bitbox, Squid Salmple

### Patch ideas

#### A. Full live techno bus
Patch your melodic bus into Performer `IN`, then let Bohm create all the pumping.

Use:
- `DUCK` for depth
- `DUCK TIME` variation for release length
- `DUCK SMTH` to preserve some transient
- `DUCK BS` to duck only lows for more transparent sidechaining

This is extremely useful if you want a “mastering-style” pump without dedicating a compressor.

#### B. DJ filter transitions
Set Performer FX to:
- `DJ FILTER`
- `LP`
- `HP`
- `BEAT ROLL`
- `SLIP ROLL`

Now Bohm becomes your transition/performance module for the rest of your patch.

Excellent with:
- **stereo sampler**
- **drum bus**
- **granular texture source**

#### C. Process only the kick or only the input
The `CHN` variation lets you choose:
- `ALL`
- `KICK`
- `INPUT`

So you can:
- filter only the external music while kicks stay clean
- roll/stutter only the kick
- process everything together for breakdowns

This makes it function like a compact live DJ section inside the rack.

---

## 5. Build a self-ducking drone patch

The manual specifically notes:
- Performer can duck external input
- Groove can sustain as a drone with `GRV ENV = SUSTAIN`
- `PERF VOL` can be set to affect only Bohm or Bohm+Groove
- Groove can become effectively continuous in some cases

### Patch idea
Create a sustained drone from another voice and let Bohm periodically carve holes in it.

### Setup
- Patch drone voice into Performer `IN`
- Trigger Bohm with a sparse rhythm
- Set `DUCK` fairly high
- Set `DUCK BS` low enough that highs remain more present
- Use long `DUCK TIME`

### Great drone sources
- **Instruō Cs-L**
- **Make Noise DPO**
- **4ms Ensemble Oscillator**
- **Mutable Rings / Resonator voices**
- **Sine bank / chord modules**
- **Granular processors**

### Result
You get a huge, breathing cinematic low-end structure where the kick doesn’t merely sit on top — it physically sculpts the other sound.

---

## 6. Use Bohm snapshots like scene memory for live improvisation

Bohm has **32 programs** with **16 steps** each, plus:
- snapshot save/load
- `LOAD W/ POTS`
- Song mode
- Jam mode
- per-knob behavior: `LATCH`, `REL`, `OVR`

This is ideal with sequencers or controllers that can fire step advances.

### Patch idea
Use Bohm as a **scene-recall rhythm engine** while the rest of your system remains semi-improvised.

### With other modules
- Use a trigger sequencer to advance `FUNCTION`
- Use a manual gate button module or controller for cueing
- Clock everything from one master source

### Great pairings
- **Pam’s Pro Workout** for sending structured triggers
- **Tetrapad / Tête**, **Pressure Points**, **Planar 2**, **Faderbank** for manual transitions
- **Stillson Hammer**, **Eloquencer**, **Hermod** for arranged changes

### Smart live setup
Set some knobs to `OVR` inside the program:
- `COLOR`
- `FX`
- maybe `PITCH`

Now snapshots recall the overall kick architecture, but you retain hands-on control of the “money parameters.”

---

## 7. Combine Bohm with logic and probability modules for generative kick variation

Because Bohm responds to:
- `HIT`
- `VELOCITY`
- `FUNCTION` CV randomization in Studio mode
- lots of parameter CV inputs

…it can benefit hugely from modular logic.

### Patch idea
Create an evolving kick system where:
- kick triggers remain stable
- accents vary
- model variations randomize occasionally
- Groove taps reshape on phrase boundaries

### Great pairings
- **Mutable Branches / compare/probability**
- **Pam’s probability/skips**
- **Shakmat Time Wizard**
- **Joranalogue Compare 2**
- **Klavis Logica XT**
- **Marbles**
- **Turing Machine + Pulses**

### Example
- Main quarter note trigger to `HIT`
- Random accent gate opens a VCA sending CV to `VELOCITY`
- Slow random stepped voltage to `COLOR`
- Every 16 bars, pulse `FUNCTION CV` in Studio mode for randomization
- Save favorite results as snapshots

This turns Bohm into a generative kick laboratory.

---

## 8. Patch Bohm through resonators for tuned kick architecture

Because Bohm is rich in transients and tuned low-frequency content, it works brilliantly as an exciter.

### Patch idea
Send Bohm’s output to:
- resonator
- comb filter
- physical modeling module
- tuned delay

### Great pairings
- **Mutable Rings**
- **2hp Pluck**
- **Comb filters**
- **Karplus processors**
- **Mimeophon** with tuned settings
- **Sealegs**
- **Data Bender** for glitch tails

### Results
- metallic industrial kicks
- tuned boomy toms
- dub-techno bass clouds
- resonant ghost harmonics around the kick

### Extra idea
Use the **Bohm envelope from TAPS OUT** to modulate the resonator damping/brightness.

---

## 9. Feed Bohm into a LPG or VCA for alternate transient shaping

Even though Bohm has internal envelopes, using an external dynamics stage gives another layer of articulation.

### Patch idea
Route Bohm into:
- VCA controlled by another envelope
- LPG for woody damping
- transient shaper/EQ

### Great pairings
- **Optomix**
- **LxD**
- **Tallin**
- **SSF Vortices** for saturation
- **Mutable Streams** or similar dynamics module

### Why bother?
You can:
- choke the tail
- emphasize the punch
- make kicks more percussive and woody
- create “gated industrial” kicks

This is especially useful on the more sample-layered or FM-heavy models.

---

## 10. Use external CV recorders or motion sequencers to animate macro controls

Bohm’s controls are macro-based and model-dependent. That means a single CV modulation can produce lots of meaningful movement.

### Best CV targets
- `COLOR`
- `CURVE`
- `TRS DECAY`
- `TRS TONE`
- `FX`
- Groove `COLOR`
- Groove `TAPS`
- Performer `DUCK` / `FX`

### Great pairings
- **Make Noise Maths**
- **Xaoc Zadar**
- **Intellijel Quadrax**
- **Batumi**
- **Mimetic Digitalis**
- **Voltage Block**
- **Acid Rain Maestro**
- **Planar 2** for recorded gesture control

### Patch idea
Record one manual gesture with Planar 2 or Voltage Block to sweep:
- Bohm `COLOR`
- Groove `COLOR`
- Performer `FX`

Now one movement transitions the whole drum ecosystem from dry punch to huge rave wash.

---

## 11. Build layered kick ecosystems with external analog kick modules

Bohm is already dual voice with Groove, but it becomes monstrous when layered with a third kick.

### Great companion kick/percussion modules
- **SSF Ultra-Kick**
- **WMD Crater**
- **Jomox ModBase 09**
- **Bastl Kickall**
- **Hexinverter Mutant Bassdrum**
- **Noise Engineering Basimilus Iteritas Alter** as click/top/metal layer

### Patch approaches

#### A. Bohm = sub/fundamental, external module = click
Use Bohm for weight and long body.
Use another kick module for midrange click.
Mix externally or send one through Performer input.

#### B. Bohm = main kick, external module = ghost kick
Send the other kick through Performer input so Bohm ducks it rhythmically.

#### C. Bohm Groove = rumble, external module = dry 909 attack
Very strong for modern techno.

---

## 12. Use Bohm as the central low-end voice in a stereo effects network

Bohm outputs **true stereo audio**. That’s unusual for a kick module and worth exploiting.

### Great stereo effects
- **Mimeophon**
- **Sealegs**
- **Nautilus**
- **Desmodus Versio**
- **Aurora**
- **FX Aid XL**
- **Timiszoara**
- **Xaoc Sarajewo** for delay networking

### Patch ideas

#### A. Stereo widening + post-FX rumble
Use Bohm model `STEREO` variation to widen, then feed into stereo reverb/delay.

#### B. Split panning by source
Use the system **PANNING** settings:
- Bohm left
- Groove right
- Performer center or opposite side

Then process the channels separately downstream.

This is powerful if you have:
- dual mono filters
- separate distortion paths
- independent channel VCAs

### Example
Hard-pan Bohm left and Groove right, then:
- distort left harder
- filter right darker
- recombine in mixer

Now your kick system has internal width and movement rather than just a centered thump.

---

## 13. Leverage PM-K1 for acoustic-space hybrid percussion

The **PM-K1** model is unusual: it’s a physical model of an acoustic bass drum, with controls for:
- drum size/tension
- beater volume
- beater reverb decay / tone
- room size
- ambient mic volume
- stereo spread

### Patch idea
Use PM-K1 not as a club kick but as a **cinematic percussion anchor**.

### Pair with
- **Field recordings**
- **Granular textures**
- **Tape emulation / wow-flutter**
- **Spring reverb**
- **Transient designer**
- **Random trigger skips**

### Great companion modules
- Morphagene
- Arbhar
- Lubadh
- Rings / Elements-type resonators
- Spring reverb or reverb tank interface

Because PM-K1 ignores many standard controls, it behaves like a different instrument entirely — perfect for ambient, soundtrack, experimental techno intros, or acoustic-electronic hybrids.

---

## 14. XT-88 as a custom kick/sample laboratory

The **XT-88** model lets you load:
- up to 16 custom wavetables
- up to 256 samples
- user WAVE files
- custom layering samples

### Patch idea
Create your own signature percussion engine by loading:
- vinyl clicks
- foley hits
- metal textures
- modular recordings
- field-recorded impacts
- vocal consonants

Then use Bohm’s macro controls to transform them into playable kicks.

### Great workflow
Pair Bohm with:
- a desktop editor workflow
- DAW resampling
- field recorder
- other Eurorack samplers for source generation

### Smart sound design trick
Make your own layer folders:
- “Clicks”
- “Hard tops”
- “Dust”
- “Industrial”
- “Wood”
- “Broken speaker”
- “Rave transient”

Then use snapshots to create genre-specific sets.

---

## 15. Create polyrhythmic low-end systems with independent HIT and CLOCK streams

Important manual detail:
- Bohm main voice is triggered by `HIT`
- Groove voice is triggered by `CLOCK`

They don’t have to be the same rhythm.

### Patch idea
Use different rhythmic divisions for each.

### Example setups
- `HIT` = quarter notes
- `CLOCK` = 16ths
- or `CLOCK` = dotted 8ths
- or triplet clock against straight kick

### Great pairings
- Clock divider/multiplier
- Euclidean trigger generator
- Trigger delay
- Logic modules

Examples:
- **Pam’s**
- **Tempi**
- **Rotating Clock Divider**
- **Euclidean Circles**
- **Shakmat Time Wizard**
- **Doepfer trigger tools**

### Result
Groove becomes a rhythmic “afterimage” of the kick rather than a static tail.

---

## 16. Use Performer beat roll/slip roll as a modular breakdown machine

The Performer FX modes include:
- `BEAT ROLL`
- `SLIP ROLL`

These are performance-oriented and excellent in live modular where most systems lack DJ-style loop effects.

### Patch idea
Feed a whole drum/percussion submix into Performer `IN`.
Let Bohm provide the kick and ducking.
Then punch in beat roll for transitions.

### Great pairings
- Drum submixer
- Sample drums
- hats and percussion bus
- stereo loop sources

Modules:
- **Bitbox**
- **Squid Salmple**
- **Assimil8or**
- **Erica Sample Drum**
- **WMD/SSF percussion modules**
- **Stereo mixer before Performer**

This can replace a lot of external mixer DJ FX tricks inside the rack.

---

## 17. Pair Bohm with envelope-following or audio-reactive modules

Because Bohm is highly transient and structured, it is a fantastic source for:
- envelope followers
- transient extractors
- comparators
- audio-to-CV tools

### Patch idea
Use Bohm audio to derive modulation for the rest of your patch.

### Great pairings
- **Envelope follower**
- **Comparator**
- **PLL**
- **Transient detector**
- **Clock extractor**

### Uses
- kick audio opens bass VCA
- rumble amplitude controls reverb depth elsewhere
- kick transient clocks another sequence
- ducking envelope derived from audio complements CV envelope

This is especially nice if you don’t want to use TAPS OUT and want audio-reactive behavior instead.

---

## 18. Make Bohm the master “drop” controller with manual controllers

Because the module has performance-oriented controls and scene memory, it pairs really well with hands-on controllers.

### Great pairings
- **Planar 2**
- **Tetrapad/Tête**
- **Pressure Points**
- **Faderfox external MIDI to CV**
- **Joystick or macro controller**
- **Manual gate buttons**

### Patch idea
Map different control sources to:
- Bohm `COLOR`
- Bohm `FX`
- Groove `VOL`
- Performer `DUCK`
- Performer `FX`

Now one hand can:
- increase kick aggression
- raise rumble
- deepen sidechain
- sweep DJ filter
- then recall a new kick snapshot

That’s an entire live techno performance workflow centered around Bohm.

---

## 19. Process Bohm through spectral or unusual processors

Because Bohm models cover FM, physical modeling, wavetable and layered samples, they respond differently to niche processors.

### Interesting companions
- **Frequency shifter**
- **Spectral processor**
- **Ring mod**
- **Bitcrusher**
- **Granular delay**
- **Resampling looper**
- **Multiband distortion**

### Patch ideas
- Send only Groove through a frequency shifter for metallic side-rumble
- Use a spectral processor on Performer input while Bohm ducks it
- Resample Bohm hits into a looper, then feed them back into Performer

This creates recursive drum architecture.

---

## 20. Build a full “one-rack techno engine” around Bohm

If I were designing a compact system around Bohm, I’d pair it with:

### Essential supporting module types
- **Master clock / trigger sequencer**
- **Pitch sequencer**
- **Modulation source**
- **Stereo effect**
- **Mixer with VCAs**
- **Filter/distortion**
- **Sampler or texture voice**
- **Performance controller**

### Example dream companions
- **Pamela’s Pro Workout** — clocks, modulation, probability
- **Metropolix** — pitch and rhythmic bass sequencing
- **Zadar or Maths** — deep modulation
- **Ikarie / Stereo Dipole** — stereo tonal shaping
- **Mimeophon / FX Aid XL / Sealegs** — atmosphere
- **Planar 2** — performance gestures
- **Bitbox / Morphagene** — stereo material into Performer input
- **Veils / Quad VCA** — extra control and sidechaining

With that, Bohm can sit at the center as:
- kick
- bass
- sidechain processor
- transition effect
- scene memory brain

---

# Best module pairings by goal

## For hard techno
- distortion / saturation
- clock sequencer
- stereo filter
- sampler for industrial layers
- manual controller

**Examples:** Crater, Ruina, Pam’s, Ikarie, Bitbox, Planar 2

## For dub techno / deep techno
- stereo delay
- resonator
- ducked pad source
- warm filter
- slow CV modulators

**Examples:** Mimeophon, Rings, Ensemble Oscillator, QPAS/Ikarie, Batumi

## For live performance
- trigger sequencer for `FUNCTION`
- controller for macro moves
- stereo mixer/submix
- sampler loops into Performer

**Examples:** Hermod, Tetrapad, Cosmix Pro, Squid Salmple

## For experimental percussion
- resonator
- granular processor
- comparator/logic
- custom sample workflow for XT-88

**Examples:** Arbhar, Data Bender, Compare 2, Morphagene

---

# A few especially strong patch recipes

## Recipe 1: Modern techno kick station
- Quarter notes to `HIT`
- 16ths to Groove `CLOCK`
- Groove `COLOR` around repetition/reverb blend
- Performer ducks a stereo drone
- TAPS OUT to VCA controlling hats
- External stereo filter after Bohm output

Result: full kick/rumble/pump ecosystem from one hub.

## Recipe 2: Bassline + kick hybrid
- Sequencer pitch CV to `PITCH`
- Gate to `HIT`
- Accent lane to `VELOCITY`
- Long `LENGTH`
- FM-2X or OLP4 model
- External distortion and low-pass filter after output

Result: kick that plays notes and still slams.

## Recipe 3: Breakdown machine
- Drum bus into Performer `IN`
- Kick from Bohm internal voice
- `CHN = INPUT` or `ALL`
- Use `DJ FILTER` / `BEAT ROLL`
- Cue snapshot changes for sections

Result: modular DJ-style transitions without external mixer FX.

## Recipe 4: Generative industrial percussion
- Sparse random triggers to `HIT`
- Independent Euclidean clock to Groove
- Random stepped CV to `COLOR`
- Envelope to `TRS TONE`
- Function randomization occasionally in Studio mode
- Process through resonator or brutal distortion

Result: self-evolving industrial kick landscapes.

---

# Final thoughts

Bohm is best treated not as “a kick module,” but as a **low-end performance instrument**. The most interesting combinations come from treating its parts separately:

- **Bohm core** for punch, tuning, and snapshots
- **Groove** as rhythmic envelope/rhythm texture generator
- **Performer** as sidechain bus and transition processor

If you want, I can also make you any of these next:

1. a **10-patch “starter cookbook”** for Bohm  
2. a **best companion modules shopping list by budget**  
3. a **genre-specific guide** for techno / electro / industrial / ambient  
4. a **small-case performance system built around Bohm**  

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)