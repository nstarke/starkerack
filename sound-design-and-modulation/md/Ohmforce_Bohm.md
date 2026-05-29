# Ohmforce — Bohm

- [Manual PDF](../../manuals/Bohm documentation.pdf)

---

[Manual PDF / Bohm Documentation](#)

# Creative Modulation Ideas for **Ohm Force Bohm**  
*A Eurorack musician’s take on how to push Bohm beyond “just kicks”*

Bohm is marketed as a stereo dual-voice kick system, but the manual makes it clear it can do much more if you treat it like a playable synth voice + rhythmic layer generator + sidechain/effects hub. The biggest takeaway is:

- **Bohm voice** can be pitched and sustained with **HIT as a gate**
- **Groove** is not just a rumble generator; it’s a second rhythmic synth voice with envelope logic
- **Performer** can turn the whole thing into a ducking / filtering / beat-roll performance processor
- Different **models reinterpret controls differently**, so modulation feels very different model-to-model

That means you can get:
- **distorted percussion**
- **talking / tearing basslines**
- **pseudo-pads and haunted drones**
- **industrial tops, reese-adjacent lows, broken techno thumps, DnB stabs**

---

## Best core ideas from the manual

Before patch recipes, here are the most important modulation facts from the manual:

### 1. **HIT can be a trigger or a gate**
This is huge. If **HIT stays high**, the sound sustains. That means Bohm can act more like a bass synth/drone voice than a one-shot kick.

Use this for:
- bass notes
- held drones
- long evolving atmospheric tones
- pitch-tracked lines

---

### 2. **PITCH can track 1V/oct**
The manual says for proper pitch tracking:
- set **PITCH knob fully CCW**
- set **PITCH attenuverter fully CW**
- choose proper **Pitch CV range** in system settings: `0..1V`, `1..2V`, or `2..3V`
- make sure sequencer is **1V/oct**

This is essential for:
- dubstep bass riffs
- DnB subs
- melodic industrial percussion
- pad/drone harmonics

---

### 3. **CURVE matters a lot**
The pitch envelope curve moves from:
- **808-style** counterclockwise
- **909-style** clockwise

The manual notes that fully CCW reaches the fundamental frequency quicker. That means:
- shorter, more solid bass pitch center
- better bassline tuning
- more stable held-note behavior

While clockwise can give:
- more exaggerated punch / dive
- more synthetic attack
- more aggressive transient motion

Modulate or perform this manually for big character changes.

---

### 4. **COLOR is often a wavetable motion control**
On many models, **COLOR** is not simply “brightness.” It often controls:
- wavetable position
- position over time
- transient harmonic content
- sound source blend on Groove

This is probably one of the best CV destinations for “alive” sounds.

---

### 5. **Groove is a second voice, not just an effect return**
Groove has:
- its own trigger input: **CLOCK**
- relative **PITCH** and **LENGTH**
- **COLOR** source blending
- **2 / 3 / 4 taps** shaping an envelope
- **TAPS CV output**

That means Groove can become:
- a tuned secondary bass layer
- a metallic top layer
- an evolving rumble envelope source
- a modulation generator via **TAPS out**

---

### 6. **Performer can process kick, input, or both**
Performer has:
- external stereo input
- ducking on every **HIT**
- effect modes like **DJ Filter**, **HP**, **LP**, **Beat Roll**, **Slip Roll**
- channel selector: **ALL / KICK / INPUT**

This opens up a lot:
- sidechained pads
- pumping drones
- beat-repeat resampling
- filtered industrial atmospheres

---

---

# Best models for the sounds you want

## For distorted percussion
Use:
- **FM-2X**
- **OLP4**
- **VX-T**
- **PX3**
- **SP-6**
- **WT-4**

### Why
- **FM-2X / OLP4** = sharper synthetic FM attack, industrial metal
- **VX-T** = strong transient shaping
- **PX3** = weird, hard, experimental with object-hit layers
- **SP-6 / WT-4** = layered transient and wavetable body

---

## For dubstep / DnB basslines
Use:
- **FM-2X**
- **HZ-1**
- **VX-T**
- **XT-88**
- **OLP4**

### Why
- **FM-2X** = very strong bass transient and FM bark
- **HZ-1 / VX-T** = clean-to-nasty wavetable motion
- **XT-88** = user wavetable/sample import for custom bass timbres
- **OLP4** = weird FM motion and metallic bass growl

---

## For haunting atmospheric pads / drones
Use:
- **PM-K1**
- **HZ-1**
- **VX-T**
- **XT-88**
- **WT-4**
- Groove + Performer together

### Why
- **PM-K1** can become roomy, resonant, ambient, especially with long held gates
- **HZ-1 / VX-T / WT-4** can be softened into wavetable drones
- **XT-88** can use custom wavetables and layers
- Performer ducking/filtering can make things breathe

---

# Modulation strategies by sound type

# 1. Distorted percussive sounds

## A. Industrial metallic kick/snare hybrid
### Try on:
- **FM-2X**
- **OLP4**
- **VX-T**

### Patch:
- Send regular triggers to **HIT**
- Send a fast random or stepped CV to:
  - **ATTACK CV**
  - **TRS DECAY CV**
  - **TRS TONE CV**
- Send a slower LFO to **COLOR CV**
- Use **VELOCITY CV** with random accents
- Set Bohm FX variation to:
  - **HARD**
  - **WAVEFOLD**
  - **BITCRUSH** if available
  - **DECIM** if available

### Why it works
- **ATTACK** affects transient intensity
- **TRS DECAY** changes click/toc length
- **TRS TONE** changes dark/bright transient color
- **COLOR** moves the oscillator/wavetable body
- **VELOCITY** gives non-repeating impact

### Extra trick
Use a clock divider/multiplier so one modulation source changes every 2, 3, or 5 hits rather than every hit. That creates repeatable “machine language” percussion instead of chaos.

---

## B. Broken hardcore kick with tearing top
### Try on:
- **PX3**
- **SP-6**
- **WT-4**

### Patch:
- Trigger **HIT** with your main rhythm
- Send a sequenced CV to **PITCH CV** for tuned percussion jumps
- Modulate **COLOR CV** with a medium-speed envelope or LFO
- Modulate **FX CV** with random stepped voltage
- Turn **LENGTH** fairly short
- Turn **CURVE** toward 909 side for more punch movement
- Layer Groove lightly with high **COLOR**

### Why it works
These models combine wavetable kick body and transient/sample layering. When pitch and color move together, they stop reading as a standard kick and start becoming hard-edged drum voices.

### Performance move
Make the **FUNCTION CV** randomize in Studio mode between takes. Since Bohm randomization is designed around “sweet spots,” you can quickly discover distorted percussion presets.

---

## C. Glitch percussion via Groove taps
### Patch:
- Main beat to **HIT**
- Faster clock, like 16ths or triplets, to **Groove CLOCK**
- Modulate **TAPS CV**
- Modulate Groove **COLOR**
- Put Groove FX on **HP** or **BP**
- Keep Groove **VOL** fairly high
- Use irregular tap settings on **2 / 3 / 4**

### Why it works
Groove repetitions are **retriggered**, not delayed copies. That means the groove voice acts like a sequenced percussion synth. With HP/BP filtering and changing tap levels, it becomes a clattery glitch layer rather than a normal rumble.

### Best use
- industrial hats from a kick source
- neuro-ish ghost percussion
- broken beat tops

---

# 2. Crazy basslines for dubstep / drum and bass

# First, the setup for proper bass playing
Per manual:
- **PITCH knob full CCW**
- **PITCH attenuverter full CW**
- set **Pitch CV** system range properly
- use **1V/oct** sequencer
- use longer **LENGTH** or hold **HIT gate**

This is the main unlock for turning Bohm into a bass synth.

---

## A. FM growl bass
### Best model:
**FM-2X**

### Patch:
- Send a pitch sequence to **PITCH CV**
- Send matching gates to **HIT**
- Set **LENGTH** fairly long
- Use medium **SUSTAIN**
- Modulate:
  - **ATTACK CV** with envelope or velocity
  - **TRS TONE CV** with a slow triangle LFO
  - **COLOR CV** with another slow/moderate LFO
  - **FX CV** with manual performance or sequencer lane
- In variations, explore **RATIO**

### Why it works
FM-2X gives you:
- sub carrier
- modulator-driven attack/growl
- wavetable-dependent tone changes
- ratio variation for harmonic character shifts

### What to listen for
- low ratios = heavier sub and weight
- higher ratios = more edge / metallic bark
- ATTACK modulation = changes how hard the FM bites
- TRS DECAY/TONE = changes the growl contour

### Dubstep move
Patch an LFO or envelope to **ATTACK CV** and sync it to phrase length. You’ll get “opening” growls on selected notes without losing low-end consistency.

---

## B. Wobble / vowel-adjacent bass
### Best models:
- **HZ-1**
- **VX-T**
- **WT-4**
- **XT-88**

### Patch:
- Pitch sequence into **PITCH CV**
- Gates into **HIT**
- Long **LENGTH**
- Moderate **SUSTAIN**
- Slow/tempo-synced LFO into **COLOR CV**
- Another LFO into **FX CV**
- Optional stepped random into **CURVE CV**
- Performer FX set to **DJ FILTER** or **LP**
- Use Performer channel set to **KICK** or **ALL**

### Why it works
On these wavetable-oriented models, **COLOR** often sweeps harmonic position over time. This behaves a lot like a wavetable sweep or moving tone contour. Add Performer filtering and you get pseudo-formant movement.

### Make it more aggressive
- Add Groove as a higher pitched layer
- Set Groove **PITCH** above center
- Use Groove **COLOR** to blend noise/grit/sub components
- Filter Groove with **BP** or **DIST**
- Keep Bohm as the sub anchor

This gives a bass patch with:
- Bohm = body/sub
- Groove = grit/motion/top harmonics

That’s a very dubstep/neuro concept.

---

## C. Reese-ish stereo bass stack
### Best models:
- **XT-88**
- **WT-4**
- **HZ-1**
- **OLP4**

### Patch idea:
- Bohm voice: long bass note sequence
- Groove clock: fast subdivisions
- Groove **PITCH** slightly above or below center
- Groove **LENGTH** around center or longer if repetition source is active
- Bohm and Groove stereo width up
- Modulate Bohm **COLOR**
- Modulate Groove **COLOR**
- Use Performer **DJ FILTER** with moderate resonance

### Why it works
It won’t be a classic detuned dual saw reese, but it can create a similar feeling:
- wide moving low-mid texture
- animated upper harmonics
- unstable stereo edge
- filtered motion

### Advanced trick
Use **Panning** system settings:
- Bohm hard left
- Groove hard right
- Performer center or one side

Now process left/right externally with separate Eurorack chains for serious stereo destruction.

---

## D. Machine-gun DnB stabs
### Best models:
- **FM-2X**
- **OLP4**
- **PX3**

### Patch:
- Short gates into **HIT**
- Fast sequenced pitch line
- High **ATTACK**
- Short/medium **LENGTH**
- Random accents into **VELOCITY**
- Modulate **CURVE** per phrase
- Modulate **TRS TONE**
- Use hard distortion mode
- Add Groove taps in sync with 16ths

### Why it works
This gives sharp, tuned impacts that sit between kick, bass, and tom. Great for:
- jump-up stabs
- techstep bass punctuation
- industrial fills

---

# 3. Haunting atmospheric pad sounds

This is the most non-obvious use of Bohm, but the manual directly supports it because:
- **HIT can sustain with a gate**
- **PITCH can track**
- **Performer ducks and filters external audio**
- Groove can create evolving envelopes and texture layers

The key is to stop thinking “kick” and think “held digital resonant voice.”

---

## A. Bohm as a dark drone/pad oscillator
### Best models:
- **HZ-1**
- **WT-4**
- **XT-88**
- **PM-K1**
- **VX-T**

### Patch:
- Send long gates or manually hold **HIT**
- Use very long **LENGTH**
- Medium/high **SUSTAIN**
- Lower **ATTACK**
- Slow LFO into **COLOR CV**
- Very slow random or triangle into **CURVE CV**
- Small pitch modulation from a slow random source into **PITCH CV** in addition to your base note
- Use Bohm FX lightly
- Use Performer **LP** or **DJ FILTER**
- Add external reverb after Bohm

### Why it works
A held Bohm tone with wavetable motion can become a haunting sustained sound, especially when pitch dive behavior is minimized and the transient is tamed.

### Important
For cleaner sustained notes:
- keep **CURVE** more toward the side that stabilizes pitch sooner
- lower transient emphasis
- avoid overly short **LENGTH**

---

## B. PM-K1 haunted drum room
### Best model:
**PM-K1**

This model is totally different:
- **PITCH** = drum size/tension
- **ATTACK** = beater volume
- **TRS TONE** = beater reverberation decay
- **SUSTAIN** = ambient mic volume
- **LENGTH** = room size
- **FX** = stereo spread of ambient mic

### Patch:
- Send sparse gates to **HIT**
- Long gate lengths
- Low **ATTACK**
- High **SUSTAIN**
- Long **LENGTH**
- High **FX** for stereo spread
- Modulate **PITCH** slowly
- Modulate **TRS TONE** with slow random CV

### Result
This can create:
- ghostly resonant drum rooms
- cinematic low thuds
- ritual ambient percussion
- almost-tom, almost-space, almost-pad textures

This is probably the fastest path in Bohm to “haunting.”

---

## C. Pad made from Groove envelope + external sound
### Patch:
- Feed a stereo drone/oscillator into **Performer IN**
- Set Performer ducking moderate
- Send sparse or rhythmic triggers to **HIT**
- Set Performer FX to **LP** or **DJ FILTER**
- Use Bohm only lightly, or even nearly silent
- Set **TAPS OUT** system setting to:
  - **GROOVE**
  - or **PERF**
- Use that CV output to modulate an external VCA/filter/reverb send

### Why it works
Now Bohm becomes the rhythmic ghost controlling another sound source:
- the pad breathes with the kick
- Groove envelope creates non-standard swells
- Performer ducking gives transparent or exaggerated pumping

This is excellent for:
- haunted pads behind broken beats
- sidechained cinematic wash
- evolving dub-techno atmospheres

---

## D. Granular-feeling haunted loops with Performer
### Patch:
- Feed texture, radio noise, field recording, or resampled ambience into **Performer IN**
- Set channel mode to **INPUT** or **ALL**
- Use **SLIP ROLL** or **BEAT ROLL**
- Trigger **HIT** sparsely
- Use synced Performer FX switching if desired
- Modulate **DUCK**
- Modulate **FX**
- Mix in Bohm quietly as a low pulse

### Why it works
Performer can stutter and resample input around hits, which turns static ambience into ghost rhythm. Great for:
- dark DnB intros
- haunted breakdowns
- IDM-ish shattered atmospheres

---

# Cross-modulation ideas using Bohm’s own outputs and logic

## 1. Use **TAPS OUT** as a modulation source
The manual says TAPS output can emit:
- **GROOVE** envelope
- **I BOHM** inverted Bohm envelope
- **PERF** performer envelope
- **BOHM** Bohm envelope

This is one of the coolest features.

### Uses:
- send to external filter cutoff for synced movement
- send to VCA controlling noise layer
- send to reverb send amount
- send to wavefolder depth
- use **I BOHM** to create inverse movement against the kick

### Great patch
- Set TAPS OUT = **I BOHM**
- Route to external oscillator VCA
- Now your external drone swells in the spaces *between* the kick hits

That’s instant haunted atmosphere.

---

## 2. Groove as modulated bass grit layer
The Groove section has:
- repetition
- kick reverb
- noise
- grit + sub

Since **COLOR** blends these, slow CV on Groove COLOR can morph from:
- rhythmic repeat
- to hiss/noise texture
- to gritty low-end layer

This is extremely useful for neuro / bass music hybrid patches.

---

## 3. Performer ducking as rhythmic spectral carving
The **DUCK BS** variation sets a band split frequency:
- lows duck
- highs preserved

This is powerful and easy to miss.

### Use it for:
- keeping air/transients from an external pad while clearing room for Bohm low-end
- subtle sidechain instead of full pumping
- rhythmic bass/pad integration

For haunting pads, this is often better than full-range ducking.

---

# Specific patch recipes

# Patch 1 — “Neuro Kick Bass Monster”
### Goal
Aggressive bassline with attack bark and moving upper harmonics

### Model
**FM-2X**

### Patch
- sequencer pitch -> **PITCH CV**
- gate sequence -> **HIT**
- velocity lane/random accents -> **VELOCITY CV**
- envelope/LFO -> **ATTACK CV**
- slow LFO -> **TRS TONE CV**
- manual or sequenced modulation -> **FX CV**
- Groove CLOCK -> 16ths
- Groove COLOR around grit/noise area
- Groove PITCH slightly above center
- Groove FX = **DIST**
- Performer FX = **DJ FILTER**
- Performer CHN = **KICK**

### Notes
Keep Bohm as the sub/fundamental and Groove as the upper dirt.

---

# Patch 2 — “Broken Factory Percussion”
### Goal
Metallic industrial percussion line

### Model
**OLP4** or **PX3**

### Patch
- Euclidean triggers -> **HIT**
- stepped random -> **PITCH CV**
- random gate accents -> **VELOCITY CV**
- slow random -> **TRS DECAY CV**
- fast attenuated random -> **ATTACK CV**
- Bohm FX = **HARD** or **WAVEFOLD**
- short **LENGTH**
- Groove clock at odd division
- Groove FX = **HP**

### Notes
This produces a line that sits between tuned drum hits and machine noise.

---

# Patch 3 — “Dubstep Wobble Pad”
### Goal
A sustained, wobbling dark harmonic bed

### Model
**HZ-1**, **WT-4**, or **XT-88**

### Patch
- hold **HIT** high with long gate
- root pitch to **PITCH CV**
- slow sine LFO -> **COLOR CV**
- second slower triangle -> **FX CV**
- tiny slow random -> **PITCH CV** mixed in
- Performer IN <- external reverb return or texture source
- Performer DUCK moderate
- Performer FX = **LP**
- CHN = **ALL**

### Notes
This works best if you reduce the attack transient and let wavetable movement do the talking.

---

# Patch 4 — “Ghost Chamber”
### Goal
Haunted cinematic percussive ambience

### Model
**PM-K1**

### Patch
- sparse triggers/gates -> **HIT**
- slow random -> **PITCH CV**
- slow random -> **TRS TONE CV**
- high **SUSTAIN**
- long **LENGTH**
- high **FX** width
- external shimmer or long reverb after Bohm

### Notes
This makes spectral low-end drum ghosts and ritual room tones.

---

# Patch 5 — “Self-Pumping Atmosphere”
### Goal
Pad that breathes around Bohm hits

### Patch
- external pad/oscillator/mixer send -> **Performer IN**
- Bohm plays sparse kick or bass pulses
- set **TAPS OUT** = **PERF** or **I BOHM**
- send TAPS OUT to external filter/VCA controlling a second drone
- Performer DUCK moderate to high
- Performer DUCK BS set so highs remain
- Performer FX = **DJ FILTER**

### Notes
This makes the whole system feel like one breathing instrument.

---

# Best modulation sources to pair with Bohm

## Great CV types for Bohm
Because many parameters are macro controls, Bohm responds best to **musical**, not purely chaotic, CV.

Use:
- **slow triangle / sine LFOs** for COLOR and FX
- **stepped random** for VELOCITY, ATTACK, PITCH jumps
- **envelopes** for ATTACK and FX
- **burst/ratchet clocks** for Groove CLOCK
- **sample & hold** for transient tone changes
- **sequenced CV lanes** for COLOR movement phrase-by-phrase

---

## Best parameter pairings

### For bass
- **PITCH + COLOR**
- **PITCH + FX**
- **ATTACK + TRS DECAY**
- **COLOR + Performer filter**

### For percussion
- **ATTACK + TRS TONE**
- **PITCH + VELOCITY**
- **CURVE + LENGTH**
- **Groove COLOR + TAPS CV**

### For atmospheres
- **COLOR + FX**
- **PITCH + CURVE** very slowly
- **Performer DUCK + DJ FILTER**
- **TAPS OUT -> external VCA/filter**

---

# Underused manual features that are especially creative

## 1. **Load snapshots with pots positions**
This means you can create families of radically different bass/percussion/pad states and recall them like presets for a set.

Use it for:
- section changes in a live DnB set
- switching from kick to bass drone instantly
- verse/chorus transitions

---

## 2. **Program knob modes: Latch / Relative / Override**
If you want one control always live during performance:
- set that parameter to **OVR**

Example:
Keep **COLOR** on override in a live bass patch so you always have hands-on “wobble depth.”

---

## 3. **Panning modes**
Hard-pan:
- Bohm left
- Groove right
- Performer center or opposite side

Then process channels separately outside Bohm. This is killer for:
- stereo bass mangling
- asymmetrical distortion
- pseudo-mid/side destruction

---

## 4. **Post EQ**
Since Bohm and Groove can get very bass-heavy or harsh, Post EQ can be used like global voicing:
- cut excess mud
- boost bite
- tame fizz

Very useful if you build dubstep/DnB patches that overload the low mids.

---

# My strongest recommendations

If I were using Bohm for your goals, I would focus on these 5 workflows:

## 1. **Use HIT as a gate**
This is the biggest key to turning Bohm into:
- bass synth
- drone
- pad voice

## 2. **Treat Groove as a separate texture oscillator**
Not just rumble. Use it as:
- tops
- grit
- ghost notes
- bass harmonics

## 3. **Use Performer as part of the sound design, not just end-of-chain**
Especially:
- DJ FILTER
- LP/HP
- ducking
- beat/slip roll on input or kick

## 4. **Modulate COLOR constantly**
On Bohm and Groove both. This is where a lot of movement lives.

## 5. **Use TAPS OUT as a real modulation source**
It can animate the rest of your rack and make Bohm the rhythmic brain of a larger patch.

---

# Quick starting recipes

## Fast distorted percussion starter
- Model: **PX3**
- Short LENGTH
- High ATTACK
- Medium TRS DECAY
- Random VELOCITY
- Slow COLOR modulation
- FX distortion mode
- Groove HP filtered tops

## Fast dubstep bass starter
- Model: **FM-2X**
- PITCH track enabled
- HIT as gate
- Long LENGTH
- Moderate SUSTAIN
- LFO on COLOR
- Envelope on ATTACK
- Performer DJ FILTER

## Fast haunted pad starter
- Model: **WT-4** or **PM-K1**
- Long gate to HIT
- Long LENGTH
- High SUSTAIN
- Slow COLOR or PITCH modulation
- Performer LP
- external long reverb
- TAPS OUT to modulate another drone layer

---

# Final thought

Bohm is most interesting when you stop asking it to be a kick drum and instead patch it like:
- a **bass voice with transient architecture**
- a **dual-voice percussion synth**
- a **stereo drone generator**
- a **sidechain and resampling performance processor**

If you want, I can also turn this into:
1. a **set of specific patch sheets**,  
2. a **genre-focused guide** for **dubstep / neuro / industrial techno / dark ambient**, or  
3. a **“best CV inputs by model” cheat sheet**.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)