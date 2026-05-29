# Pittsburgh Modular — Synthesizer Box

- [Manual PDF](../../manuals/Synthesizer Box - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF / Source](https://pittsburghmodular.com/synthesizer-box)

# Pittsburgh Modular Synthesizer Box: using one semi-modular voice to build full-length Eurorack songs

The **Pittsburgh Modular Synthesizer Box** is a discontinued but very capable **complete analog semi-modular voice**. From the manual, it includes:

- **Complex waveform oscillator**
- **Waveform mixer**
- **Voltage-controlled multi-mode lopass gate**
- **Wide-range LFO**
- **ADSR envelope**
- **Glide**
- **Linear VCA**
- Full internal normalization with patch points to override routings

Specs from the manual:

- **28hp**
- **36.5mm deep**
- **+12V 125mA / -12V 95mA**
- No +5V required

What makes it especially useful for songwriting is that it already contains the whole “single-voice chain”:

**Pitch CV → oscillator → LPG/filter/VCA shaping → final VCA**

That means with the right surrounding modules, it can act as:

- the **main lead voice**
- the **bass voice**
- a **percussion voice**
- a **textural or transitional voice**
- a **resample source** for an entire arrangement

The challenge of full-length Eurorack songs is rarely “how do I make a cool sound?”  
It’s usually:

1. **How do I create sections?**
2. **How do I vary energy over time?**
3. **How do I recall or re-enter motifs?**
4. **How do I move one voice through different roles in the arrangement?**

This module is actually very good for that, because it has enough internal routing to be playable, but enough patchability to recontextualize during a song.

---

# 1. What the Synthesizer Box is best at in a song context

## A. Strong monophonic identity
The oscillator includes:

- triangle
- saw/blade selection
- square
- sub oscillator
- waveform modulation
- FM input with exp/linear option

This gives one voice a lot of timbral range without changing modules. For song structure, that matters because one voice can evolve across sections while still sounding like the same instrument.

Example:

- **Verse:** triangle + a little sub
- **Pre-chorus:** blade + PWM/modulation
- **Chorus:** saw/blade + square + sub into LPG/VCA
- **Breakdown:** triangle with audio-rate FM or pinged LPG

That is exactly how you make one modular voice feel like a “song instrument” rather than a loop.

## B. The lopass gate is a secret arranging tool
The LPG has 3 modes:

- **VCA**
- **LPG**
- **Lowpass filter**

This is huge for structure.

You can use the same oscillator patch and change only the LPG mode to create arrangement contrast:

- **VCA mode** = clean, direct, more synth-bass or stable lead behavior
- **LPG mode** = plucky, organic, percussive, dynamic
- **Lowpass mode** = more classic subtractive filter sweeps and tension-building

That means one sequence can become three different sections.

## C. Internal modulation normals reduce patch complexity
The manual notes:

- oscillator **FM CV** is internally patched from the **LFO triangle**
- oscillator **MOD CV** is internally patched from the **LFO triangle**
- LPG **MOD CV** is internally patched from the **envelope output**
- VCA **CV IN** is internally patched from the **envelope**
- VCA **IN** is internally patched from the **LPG OUT**

This makes it easy to set up a “default playable voice,” then use external modules only where song form needs more control.

That’s ideal for song-building because you can reserve precious external modulation/sequencing for **macro changes**.

---

# 2. Core limitation: it is one voice, not a whole song by itself

To make full-length songs, you’ll want to pair it with modules that solve these arrangement problems:

- **song sequencing / section recall**
- **rhythmic variation**
- **mixing and muting**
- **effects and spatial change**
- **recording / looping / resampling**
- **additional voices or layered samples**
- **performance controls**

The Synthesizer Box can be the emotional center of a track, but full song structure usually comes from the system around it.

---

# 3. The most useful companion modules for full-length songwriting

## A. A sequencer with pattern memory or song mode
This is the single biggest upgrade for turning loops into songs.

Best companions:

- **Metropolix**
- **Hermod+**
- **Five12 Vector Sequencer**
- **Eloquencer**
- **NerdSEQ**
- **Winter Modular Eloquencer**
- **Intellijel Metropolis/Metropolix**
- **Keystep Pro** if you’re okay with external sequencing

Why: you need to be able to define:

- intro
- verse
- pre-chorus
- chorus
- bridge
- breakdown
- outro

For the Synthesizer Box, this sequencer should output:

- **1V/Oct** to **1V/O IN**
- **gate** to **ENV IN**
- optionally an extra modulation lane to:
  - **FM CV IN**
  - **MOD CV IN**
  - **LPG CV IN**
  - **VCA CV IN**
  - **BLADE IN**

A good song sequencer lets the same voice play **different musical roles per section**, which is the key to full songs.

---

## B. A trigger/gate variation source
Even with one melody sequence, changing gate behavior changes the section.

Useful modules:

- **Pamela’s New Workout / Pro Workout**
- **Temps Utile**
- **Mutable Grids**
- **Euclidean Circles**
- **Shakmat Time Wizard / clock tools**
- **logic modules** like Compare 2, Klavis Logica XT, Joranalogue Compare 2

Use these to vary:

- envelope triggers
- LPG pings
- rhythmic accents
- ratchets
- occasional fills

The Synthesizer Box responds especially well to **LPG pinging** and **short envelope articulation**, so rhythmic variation alone can create section changes without rewriting pitch material.

---

## C. A matrix mixer or CV mixer
This is underrated for songwriting.

Great options:

- **4ms VCA Matrix**
- **AI Synthesis Matrix Mixer**
- **Doepfer A-138m**
- **Happy Nerding 3xMIA**
- **Frap 321**
- **Befaco A*B+C**

Why: the oscillator has multiple outputs and multiple modulation destinations. A matrix mixer lets you create “scene-like” relationships:

- LFO to pitch FM lightly in verse
- same LFO to waveform MOD strongly in chorus
- envelope to LPG in one section
- extra sequencer lane to LPG in another
- random source to BLADE IN only in fills

This creates evolving arrangements without repatching.

---

## D. A performance mixer with mutes and sends
If you want full songs, you need to mix like you’re arranging.

Examples:

- **WMD Performance Mixer**
- **Befaco Hexmix**
- **Tesseract Tex Mix**
- **Cosmotronic mixer**
- **Happy Nerding PanMix**
- **ALM Mega-Tang**
- **XOH / output module** plus submixers

Why this matters with the Synthesizer Box:
Even if it’s your only true synth voice, you may pair it with:

- drum modules
- sample playback
- a second oscillator/voice
- effects returns
- resampled loops

A mixer with **mutes**, **aux sends**, and **submixes** is one of the main ways Eurorack becomes “song-capable.”

---

## E. Effects with CV or preset switching
Arrangement needs space changes.

Strong companions:

- **Make Noise Mimeophon**
- **Strymon Magneto**
- **Xaoc Sarajewo**
- **Happy Nerding FX Aid Pro**
- **Erbe-Verb**
- **Nautilus**
- **Desmodus Versio**
- **Sealegs**

Use effects to create section identity:

- dry and close in the verse
- wider delay in pre-chorus
- huge reverb wash in breakdown
- dub-style send throws for transitions
- feedback rises into chorus

The Synthesizer Box’s waveform complexity and LPG plucks are especially good into delay and reverb.

---

## F. A sampler / looper / recorder
This is maybe the most practical “song-finishing” companion.

Examples:

- **1010 Bitbox**
- **Rossum Assimil8or**
- **Morphagene**
- **Lubadh**
- **Nebulae**
- **Arbhar**
- external pedal/DAW recorder if preferred

Why: one voice can only play one thing at once. To build full arrangements, record the Synthesizer Box as:

- bass loop
- lead line
- arp
- drones
- transitional noise swells

Then play those back while the module moves on to the next role.

This is one of the strongest ways to make full-length songs from a single great voice.

---

# 4. Best ways to use the Synthesizer Box across different song roles

## Role 1: Bass voice
The module is excellent for bass because of:

- sub oscillator
- square and saw/blade blending
- VCA mode for punch
- glide for portamento basslines
- filter/LPG for articulation

### Patch idea
- Sequencer pitch → **1V/O IN**
- Gate → **ENV IN**
- Oscillator **MIX OUT** → **LPG IN** or leave normalized
- LPG in **VCA** or **LPG** mode
- **VCA OUT** to mixer

### Song use
- **Verse:** simple sub-heavy mono bass
- **Chorus:** add square and blade, more envelope depth
- **Bridge:** open filter more or add FM
- **Outro:** reduce to triangle + sub

For full-length structure, automate or sequence:

- note density
- glide amount
- envelope timing
- sub amount
- LPG mode

---

## Role 2: Lead voice
The blade wave and modulation options make it strong for expressive leads.

### Patch idea
- Keyboard or sequencer CV → **1V/O IN**
- Gate → **ENV IN**
- Slow LFO or sequenced CV → **MOD CV IN**
- Pressure/aftertouch/expression CV → **FM CV IN** or **LPG CV IN**
- Delay/reverb on aux send

### Song use
- Keep the melody recurring, but change articulation:
  - short LPG plucks in verse
  - sustained VCA lead in chorus
  - filtered legato in bridge
  - highly modulated lead in final chorus

This is classic songwriting inside modular: same melodic identity, different sound treatment.

---

## Role 3: Percussion / plucked voice
The manual specifically highlights **PING mode** on the LPG.

That means this voice can be turned into:

- bongos
- woodblock-like sounds
- plucks
- metallic pings
- synthetic toms
- tuned percussion

### Patch idea
- Short trigger pattern → **LPG CV IN** with LPG in **PING** mode
- Oscillator tuned to desired pitch
- Minimal sustain from ADSR or bypass envelope entirely
- Modulate **BLADE IN** or **FM CV IN** for transient complexity

### Song use
Use this as:
- intro hook percussion
- rhythmic motif in verses
- fill generator between sections
- breakdown pluck sequence

Very often a full song needs a recurring “signature texture.”  
A pinged Synthesizer Box patch can be that.

---

## Role 4: Drone / atmosphere / transition source
Because the oscillator offers mixed waveforms and the VCA/LPG can be externally driven, it can easily become a long evolving drone.

### Patch idea
- No gate sequence, or hold gate open
- LFO → **MOD CV IN**
- Very slow CV from external source → **FM CV IN**
- **MIX OUT** through LPG lowpass mode
- Reverb/delay heavy send

### Song use
- intro pad/drone
- pre-drop tension
- bridge ambience
- outro decay

This helps connect sections so the piece feels like a song, not isolated loops.

---

# 5. Specific strategies for making full-length songs with this module

## Strategy 1: One sequence, many orchestrations
Instead of writing six different sequences, write **one strong motif** and reuse it.

Example arrangement:

- **Intro:** triangle wave only, long delay
- **Verse:** same notes as bass, sub + square
- **Pre-chorus:** same notes an octave up with glide
- **Chorus:** same notes with blade wave + open LPG
- **Breakdown:** same sequence slowed or sparsified, ping mode
- **Final chorus:** combine original bass playback sample with live lead version

The Synthesizer Box excels here because one pitch sequence can sound like a different instrument just by reconfiguring wave mix and LPG mode.

---

## Strategy 2: Use sampling/resampling to turn one voice into many layers
This is probably the most effective real-world approach.

### Workflow
1. Program bassline on Synthesizer Box
2. Record it into sampler/looper
3. Repatch Synthesizer Box as lead
4. Record a lead phrase
5. Repatch as percussion or drone
6. Use mixer to arrange the layers in and out

Now one module becomes a whole track’s sonic fingerprint.

This is especially effective because the module has a distinctive tone that helps all recorded layers feel cohesive.

---

## Strategy 3: Build sections with modulation scenes
Use switches, sequential switches, preset managers, or CV mixers to create section changes.

Helpful modules:

- **Noise Engineering Vice Virga**
- **Doepfer sequential switch**
- **Tenderfoot quad switch**
- **Verbos Sequence Selector**
- **Make Noise Morph 4**
- **macro CV controllers** like Planar 2, Tetrapad/Tete

### Example scene mapping
- **Scene A (Verse):**
  - little FM
  - little waveform mod
  - LPG mode
  - short decay

- **Scene B (Pre-chorus):**
  - more resonance in lowpass mode
  - slower envelope
  - more delay send

- **Scene C (Chorus):**
  - sub on
  - square and blade up
  - VCA mode
  - stronger VCA envelope

- **Scene D (Breakdown):**
  - triangle only
  - high reverb send
  - sparse triggers

This gives modular the equivalent of arrangement automation.

---

## Strategy 4: Separate pitch variation from timbral variation
A common mistake is changing everything at once. Songs work better when some things stay stable.

With the Synthesizer Box:

- let **pitch sequence** remain recognizable
- change **waveform blend**
- change **LPG mode**
- change **modulation depth**
- change **effects send**
- change **register**
- change **rhythm/gates**

That creates narrative continuity.

---

## Strategy 5: Use the oscillator outputs independently
From the manual, the oscillator provides:

- **TRI OUT**
- **S/B OUT**
- **SQR OUT**
- **MIX OUT**

This is very useful beyond the default voice path.

### Examples
- Send **MIX OUT** to the internal LPG/VCA chain for the main voice
- Simultaneously send **SQR OUT** to an external wavefolder or distortion
- Send **TRI OUT** to a separate filter for a sub-layer
- Use **S/B OUT** as a raw audio source for sampling

This can create pseudo-multitimbral results from one oscillator during recording or in parallel processing.

---

## Strategy 6: Create transitions, not just patterns
Songs feel complete because of transitions.

Use the Synthesizer Box to generate:

- rising FM tension before section changes
- LPG pings as fills
- glide slides into downbeats
- resonance/filter sweeps in lowpass mode
- sudden drop to triangle-only minimalism
- burst of blade-wave modulation into chorus

Good modules for transition control:

- envelope followers
- function generators
- burst generators
- manual gate buttons
- sequential switches
- clock dividers/multipliers

A simple but effective technique:
- assign a manual controller or macro knob to increase:
  - LPG frequency
  - effects send
  - oscillator modulation depth  
  over 4–8 bars before a chorus.

---

# 6. Example full-song setups

## Setup A: Techno / Electro track
### Other modules
- Drum voice(s) or drum sampler
- Pamela’s New Workout
- Metropolix
- Delay/reverb
- Performance mixer
- Sampler/looper

### Synthesizer Box role
Primary bass/lead hybrid voice

### Arrangement
- **Intro:** filtered noise/drums only, Synthesizer Box enters as pinged LPG stab
- **Section 1:** bassline in VCA mode, sub oscillator on
- **Section 2:** same pattern with blade modulation and more reverb throws
- **Breakdown:** resampled bass loop continues, live module becomes high-register FM lead
- **Drop:** return to bass role, add square wave and tighter envelope
- **Outro:** strip back to LPG plucks and delay tails

Why it works:
one voice carries the identity, but resampling lets it appear in multiple roles.

---

## Setup B: Ambient / Berlin-school style song
### Other modules
- Long sequencer
- Clock divider
- Reverb/delay
- Stereo mixer
- Quantizer
- Looper

### Synthesizer Box role
Evolving melodic centerpiece

### Arrangement
- **Intro:** drone from triangle/blade through lowpass mode and reverb
- **Main section:** sequenced melody with moderate glide
- **Variation:** transpose sequence, increase LFO-to-MOD amount
- **Bridge:** remove gate, sustain a drone while sampled previous melody keeps repeating
- **Final section:** reintroduce sequenced melody with sub and added FM shimmer

Why it works:
repetition with timbral evolution is enough for long-form ambient music.

---

## Setup C: Indie / synth-pop modular performance
### Other modules
- External MIDI-to-CV or Keystep Pro
- Drum machine or sample drums
- Chord sampler/polyphonic source
- Mixer with sends
- Delay and chorus/reverb

### Synthesizer Box role
Bass in verse, lead in chorus

### Arrangement
- **Verse:** monophonic bass under drums and pads
- **Pre-chorus:** open filter/LPG and add glide
- **Chorus:** octave shift up, more blade/square, same motif becomes lead hook
- **Verse 2:** back to bass, but with rhythmic gate variation
- **Bridge:** use ping mode for sparse plucks
- **Final chorus:** bass sampled and looping while live voice handles lead

This is one of the most practical uses of the module in song form.

---

# 7. Best patching ideas specifically suggested by the manual

## A. Exploit the internal LFO normals, then override when needed
Per manual:

- LFO triangle is normalized to **FM CV**
- LFO triangle is normalized to **MOD CV**

This means you can immediately get movement without extra cables.

For songwriting:
- keep internal LFO modulation for the “default section”
- patch external CV to override it in special sections

For example:
- verse uses internal LFO wobble
- chorus overrides **MOD CV IN** with sequencer automation for precise timbral accents

---

## B. Use the BLADE wave as your “chorus timbre”
The manual describes the **BLADE** wave as a unique complex saw, modulated via **MOD CV** and further manipulated at **BLADE IN**.

That suggests a strong arrangement tactic:
- keep **SAW** for stable sections
- switch to **BLADE** for heightened sections

This is a very musical way to make choruses feel larger.

---

## C. Exploit the three LPG modes as section states
This module almost gives you three different tone-shaping modules:

1. **VCA mode** for clean dynamics
2. **LPG mode** for pluck and organic tone
3. **LOPASS mode** for filter sweep drama

A full song can be built around rotating these modes.

---

## D. Use the wide-range LFO at audio rate
The manual says the LFO is suitable for **audio-rate frequency modulation**.

That means section escalation can include:
- gentle slow modulation in verse
- audio-rate FM in climax or breakdown
- return to subtle modulation after peak

Audio-rate shifts are powerful when used sparingly as arrangement moments.

---

# 8. A practical “song blueprint” using only a few extra modules

Let’s say your system contains:

- **Synthesizer Box**
- **Pamela’s New Workout**
- **Metropolix**
- **FX Aid Pro**
- **small mixer**
- **Bitbox or Morphagene**
- **drum voice or external drum machine**

## Patch
- Metropolix pitch → **1V/O IN**
- Metropolix gate → **ENV IN**
- Pamela modulation lane → **LPG CV IN**
- Pamela second lane or Metropolix mod lane → **MOD CV IN**
- **VCA OUT** → mixer channel
- mixer send → FX Aid
- record phrases into Bitbox

## Arrangement plan
### Intro
- triangle only
- no sub
- long reverb
- sparse gates

### Verse
- sub + square
- LPG mode
- short ADSR
- dry mix
- low note density

### Pre-chorus
- increase glide
- switch to saw/blade
- open LPG frequency more
- add delay send
- maybe thin drums briefly

### Chorus
- blade + square + sub
- VCA mode for punch and stability
- stronger envelope
- doubled by sample of previous section
- brighter FX return

### Breakdown
- sample carries bass loop
- live module repatched for pinged plucks or FM lead
- minimal drums
- more reverb

### Final chorus
- bring back live bass or lead
- stack with resampled material
- stronger modulation depth
- use manual performance gestures

### Outro
- remove sub
- triangle/drone tail
- fade to delay/reverb

That is a complete song architecture from one main Eurorack voice.

---

# 9. Common mistakes when trying to make songs with this module

## Mistake 1: Treating it only as a “cool voice patch”
If you only dial in one sweet spot and leave it there, you’ll get a loop.

Fix:
- pre-plan 3–4 versions of the same patch for different sections

## Mistake 2: Using modulation only for sound design, not arrangement
Modulation should mark form.

Fix:
- assign separate modulation behaviors to verse, chorus, and breakdown

## Mistake 3: No recording/resampling
One mono voice can’t carry every layer live at once.

Fix:
- sample your own module early and often

## Mistake 4: No mute/transition strategy
A great pattern with no entry/exit plan stays a pattern.

Fix:
- build transitions using mutes, sends, switchable mod routings, and fills

## Mistake 5: Rewriting pitch when timbre would have been enough
Many songs rely on repeated motifs.

Fix:
- use recurring sequences and vary orchestration instead

---

# 10. Best module pairings by songwriting goal

## If you want structured songs
Pair with:
- **Vector Sequencer**
- **Hermod+**
- **NerdSEQ**
- **Metropolix**

## If you want performable live arrangements
Pair with:
- **WMD Performance Mixer**
- **Planar 2**
- **Mute switches**
- **Pamela’s New Workout**

## If you want one voice to become a whole track
Pair with:
- **Bitbox**
- **Assimil8or**
- **Morphagene**
- **Lubadh**

## If you want rich transitions and evolving sections
Pair with:
- **Mimeophon / Magneto / FX Aid**
- **matrix mixer**
- **sequential switch**
- **function generator**

## If you want the module to cover bass, lead, and percussion
Pair with:
- **quantized sequencer**
- **clocked trigger source**
- **sampler**
- **mult/effects**
- **possibly a wavefolder or distortion**

---

# 11. Final takeaway

The **Synthesizer Box** is not just a starter semi-modular voice. It can be a **song engine** if you stop thinking of it as “one patch” and start thinking of it as **one recurring character** in an arrangement.

Its strengths for full-length composition are:

- enough oscillator complexity to support multiple section identities
- a very flexible **LPG / filter / VCA** stage
- internal normalization for quick setup
- enough patch points to integrate into larger systems
- excellent ability to move between:
  - bass
  - lead
  - percussion
  - drone
  - transition FX

The most effective way to use it for full songs is:

1. **Sequence it with pattern memory**
2. **Use rhythmic variation and section-based modulation**
3. **Exploit LPG mode changes**
4. **Resample it into loops or phrases**
5. **Arrange with mutes, effects sends, and transitions**
6. **Reuse motifs while changing orchestration**

That is how a great Eurorack voice stops being “a nice loop machine” and becomes part of a real, beginning-to-end composition.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)