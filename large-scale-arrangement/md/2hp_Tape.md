# 2hp — Tape

- [Manual PDF](../../manuals/2hp_Tape_Stop.pdf)

---

[Manual PDF / Source](https://www.twohp.com/modules/tape-stop)

# 2hp Tape Stop: using it to turn loops and patterns into full-length songs

The **2hp Tape Stop** is a **performance transition and phrasing module**. On paper it’s “just” a clock-synced tape-stop effect, but in a song-building context that is exactly what makes it valuable: it gives you a **repeatable, musical way to mark sections, create tension, reset energy, and signal arrangement changes**.

A lot of modular patches get stuck at the “cool 8-bar loop” stage because everything is always on, always cycling, and changing too continuously. Tape Stop helps because it creates **clear, section-defining events**:
- intros
- breakdowns
- transitions
- fills
- fake endings
- drops
- outros

It is especially useful because it can be:
- **manually performed** with the Trig button
- **gated from other modules** via the Trig input
- **clock-synced** so the slowdown length matches the structure of your patch
- **CV controlled** with the Lag CV input
- used in **momentary or latching** mode
- set to **50/50 dry/wet at boot**, which makes it much more arrangement-friendly

---

## What the module does, in practical musical terms

From the manual:

- **Audio in/out**: 10 Vpp
- **Clock input**: syncs tape-stop timing to external clock
- **Trig button / Trig gate input**: starts the tape-stop effect
- **Lag knob**: sets stop length from instant to 4 seconds, or clock divisions/bars when clocked
- **Lag CV**: modulates stop length
- **Momentary vs latching toggle**:
  - **momentary** = effect lasts while held/gated
  - **latching** = one trigger starts, another stops
- **50/50 mode on boot**: hold Trig while powering on for dry/wet blend of 50%

This means Tape Stop can behave as:
1. a **live DJ-style brake effect**
2. a **bar-length transition tool**
3. a **section marker controlled by sequencer gates**
4. a **dynamic send effect** when combined with mixers/VCAs
5. a **structural disruption device** that makes repeating material feel arranged

---

# Why Tape Stop is good for song structure

A full song usually needs:
- **contrast**
- **phrasing**
- **section boundaries**
- **energy management**
- **returns**
- **moments of surprise**

Tape Stop is not a composition module by itself, but it is excellent at creating **boundaries between sections**. In a modular system, these boundaries often matter more than adding yet another oscillator or sequencer.

Think of it like this:

- Your sequencers and voices make the **content**
- Your mixers, VCAs, switches, and mutes make the **arrangement**
- Tape Stop makes the **transitions feel intentional and musical**

A repeated pattern becomes a “verse” or “chorus” when it is **introduced, interrupted, paused, dropped, or resumed in a controlled way**. Tape Stop gives you a very recognizable language for doing that.

---

# Best roles for Tape Stop in a song

## 1. End-of-phrase transition
Patch your full drum bus, melodic bus, or full mix through Tape Stop and trigger it every:
- 4 bars
- 8 bars
- 16 bars

This creates a recurring structural cue. Even if the pattern content is almost unchanged, listeners perceive a larger arrangement.

### Example
- 16-bar groove plays normally
- on bar 16, Tape Stop slows the entire drum bus for an 8th or quarter note
- bar 17 comes back with:
  - open filter on bass
  - hi-hats added
  - new melody transposition

That one tape-stop event tells the ear: **“new section.”**

---

## 2. Breakdown generator
Instead of muting everything abruptly, use Tape Stop on:
- full mix
- drum bus
- melodic bus
- sampler loop bus

Then bring back only selected parts.

### Example breakdown flow
- Full groove playing
- Trigger Tape Stop on the whole mix for a half-note or whole-note stop
- During the slowdown:
  - mute kick
  - leave reverb tail
  - bring in pad drone
- Restart only bass + pad
- Reintroduce drums 8 bars later

This works because Tape Stop provides a **musical deceleration**, not a hard mute. That makes the arrangement feel composed rather than patched.

---

## 3. Fake ending / restart
A great song trick in modular is making the audience think the piece is ending.

### Patch idea
Run the master bus through Tape Stop in **latching mode**.

At the apparent “end”:
- trigger Tape Stop with a long lag (whole note, 2 bars, or 4 bars if clocked)
- simultaneously reduce other voices via VCAs or mutes
- let the sound collapse
- then relaunch clocked material with a new variation

This creates:
- tension
- drama
- a “second act”
- room for a new melody or denser percussion layer

---

## 4. Transitional fill substitute
If your system lacks dedicated drum fill modules or probability logic, Tape Stop can function as a fill event.

Instead of adding more notes, create variation by **interrupting time itself**.

### Example
Every 8 bars:
- tape-stop the drum bus for a 16th or 8th
- at the same moment:
  - switch to alternate snare pattern
  - advance sequencer to a new page
  - transpose bass line

This is especially effective for techno, electro, synthwave, ambient breaks, and live improvised sets.

---

## 5. Intro/outro builder
Many modular pieces start too suddenly and end too abruptly. Tape Stop can help both.

### Intro
Begin with:
- only texture, pad, or noise
- a loop or melodic fragment through Tape Stop
- repeated momentary stops synced to clock

This gives a “warped startup” feel before the beat fully appears.

### Outro
At the end of the song:
- send entire mix through Tape Stop
- trigger progressively longer lag values
- remove percussion layers underneath
- let delays/reverbs decay
- final long stop = ending

This produces a much more convincing ending than simply muting the master.

---

# How to combine Tape Stop with other modules to build songs

The manual itself suggests pairings with:
- **2hp Lo-Fi**
- **2hp Play**
- **2hp VCA**
- **2hp Loop**

Those are all useful arrangement partners. More broadly, here is how to combine Tape Stop with common Eurorack categories.

---

## 1. With sequencers: create section changes

Use a sequencer, trigger sequencer, or gate sequencer to send triggers to Tape Stop at specific phrase lengths.

### Good partners
- trigger sequencers
- clock dividers
- Euclidean sequencers
- sequential switches
- song mode sequencers
- gate programmers

### Song use
Program Tape Stop triggers only at:
- end of bar 8
- end of bar 16
- just before chorus/drop
- final bar before breakdown

This gives your patch a **macrostructure**.

### Strong technique
Use a **clock divider**:
- /16, /32, /64, /128 outputs
- route one division into Tape Stop trig
- route another division to pattern change/reset

Now your patch has **periodic form**:
- every 16 bars: transition
- every 32 bars: bass pattern changes
- every 64 bars: melody resets

That’s the skeleton of a full song.

---

## 2. With VCAs and mixers: control where the effect applies

This is one of the most important uses.

Tape Stop is more song-useful when you don’t always put the entire mix through it. Use VCAs, mixers, aux sends, and submixes.

### Put Tape Stop on:
- drum bus only
- bass bus only
- melody bus only
- sample loop only
- full mix only during major transitions

### Why this matters
Full songs need **selective contrast**. If the whole patch gets tape-stopped constantly, the trick gets old. But if:
- verse = melody only gets tape-stopped
- pre-drop = drums only get tape-stopped
- breakdown = full mix gets tape-stopped

then the effect becomes part of arrangement language.

### Great patch
- mult lead synth signal
- one copy dry to mixer
- one copy through Tape Stop to second mixer channel
- use VCAs to crossfade dry/wet
- optionally engage 50/50 mode for more natural blend

This makes Tape Stop feel less like an insert effect and more like a performable texture layer.

---

## 3. With samplers and loopers: transform loops into sections

This is perhaps the most direct path to full songs.

If you use a sampler, phrase looper, or sample player, Tape Stop can turn a repetitive loop into a staged performance.

### Good partners
- 2hp Play
- 2hp Loop
- Morphagene
- Arbhar
- Bitbox
- Assimil8or
- Rossum, Make Noise, 1010music, etc.

### Song use
- play a stable vocal chop, field recording, pad loop, or drum loop
- apply Tape Stop only at section ends
- restart or replace sample after slowdown
- switch sample banks during or immediately after the stop

This feels like a DJ moving between scenes or clips.

### Example song arrangement
- Intro: ambient loop through Tape Stop
- Verse: drum loop enters dry
- Pre-chorus: apply short tape stop to loop every 4 bars
- Chorus: new sample loaded, no Tape Stop
- Breakdown: long tape stop on full sampled texture
- Outro: one final stop and decay

Tape Stop helps conceal abrupt sample switching and makes section handoffs sound deliberate.

---

## 4. With clock dividers/multipliers: make transitions land musically

Because Tape Stop has a **clock input**, it can quantize its lag timing into useful musical lengths:
- instant
- 32nd
- 16th
- 8th
- quarter
- half
- whole
- 2 bars
- 4 bars
- 8 bars
- 16 bars

This is huge for song construction.

### Why
Without sync, transitions can feel arbitrary. With sync, they become part of the groove architecture.

### Powerful uses
- short values for fills
- 1 bar for pre-drop brake
- 2–4 bars for breakdown entry
- 8–16 bars for ambient collapse or outro

### Song strategy
Map different sections to different lag lengths:
- verse transition = 8th note
- chorus entry = quarter note
- breakdown = 2 bars
- ending = 8 bars

Now one module provides a recognizable but evolving transition vocabulary.

---

## 5. With logic and gate utilities: automate structure

Logic modules are amazing for getting beyond loops.

### Patch ideas
- use **AND** so Tape Stop only triggers when both:
  - phrase reset pulse occurs
  - performance gate is high
- use **OR** so either a manual button or a sequencer can trigger it
- use **probability/skipping** so some section transitions stop and others don’t
- use **burst generators** to create repeated stop/release gestures

This gives you larger-form variation without manually repatching.

---

## 6. With sequential switches: create A/B song sections

A sequential switch can move between:
- two melodies
- two drum patterns
- two basslines
- dry vs processed routing

Tape Stop is ideal for masking the moment of change.

### Example
- 8 bars of pattern A
- Tape Stop on full mix for quarter note
- switch to pattern B during the slowdown
- release into new section

This is one of the best ways to create “verse/chorus” contrast in modular.

---

## 7. With filters and envelopes: exaggerate transitions

Tape Stop gets stronger if something else changes at the same time.

### During tape stop, also:
- close lowpass filter
- increase reverb send
- reduce kick VCA
- slow LFO rate
- open noise wash
- fade in drone

This makes transitions feel cinematic.

### Example
At the end of 16 bars:
- trigger Tape Stop on drums
- trigger envelope that closes bass filter
- open reverb send on lead
- switch melody octave

By combining several coordinated changes, a loop becomes an arranged section.

---

## 8. With effects chains: build distinctive song identities

The manual suggests pairing with **Lo-Fi**, which is smart: wow/flutter/noise plus Tape Stop gives an old machine aesthetic.

Other strong partners:
- reverb
- delay
- chorus
- distortion/saturation
- granular processors
- compressors on buses

### Example chains
- **Sampler → Lo-Fi → Tape Stop → Reverb**
  - nostalgic intros, degraded breakdowns
- **Drum bus → Saturation → Tape Stop**
  - aggressive drop transitions
- **Pad → Tape Stop → Huge reverb**
  - ambient sectional boundaries
- **Full mix → Tape Stop → Delay feedback tail**
  - dramatic endings

For full songs, these combinations help each section have a distinct emotional quality.

---

# Specific song-building patch concepts

## Patch 1: Techno arrangement engine
### Goal
Turn a 2–3 pattern techno patch into a 6-minute performance.

### Modules involved
- kick, hats, clap voices
- bass voice
- lead/stab voice
- clock source
- clock divider
- trigger sequencer
- mixer/submix
- Tape Stop
- VCAs/mutes
- reverb/delay

### Routing
- drum bus through Tape Stop
- bass and lead dry to mixer
- clock to Tape Stop clock input
- /64 pulse from divider to Tape Stop trig input
- manual override trigger button for live fills

### Structure
- bars 1–16: drums and bass
- bar 16: short tape stop on drums only
- bars 17–32: add lead
- bar 32: quarter-note tape stop on full drum bus, mute kick under it
- bars 33–48: breakdown, only hats + delay lead
- bar 48: long tape stop on full mix
- bars 49–64: full drop with bass variation
- final section: progressively longer tape stops every 16 bars for outro

### Why it works
You’re using Tape Stop as a recurring phrase marker, not a gimmick.

---

## Patch 2: Ambient-to-beat evolving song
### Goal
Create a piece that slowly transforms from texture to rhythm and back out.

### Modules
- granular/sample source
- looping module
- melodic voice
- drum voice or soft pulse
- Tape Stop
- clock
- random CV
- VCA mixer
- reverb

### Routing
- granular/loop source through Tape Stop
- drums bypass Tape Stop initially
- random stepped CV to Lag CV for changing stop length
- clock sync connected

### Structure
- Intro: sparse loop repeatedly tape-stopped in momentary mode
- Mid section: melody enters dry, loop still stopping occasionally
- Beat enters after 2 minutes
- Main section: only loop bus gets stopped every 8 bars
- Breakdown: full mix through Tape Stop for 2 bars while reverb blooms
- Return: drums come back dry, loop reduced
- Outro: long synced stop on ambient bus, then silence

### Why it works
The piece has directional movement because Tape Stop marks transitions between density levels.

---

## Patch 3: Modular “verse/chorus” song
### Goal
Create pop-like section differentiation.

### Modules
- two melodic sequences
- bass sequence
- drum pattern A/B
- sequential switch
- Tape Stop
- utility mixer
- VCAs
- filter
- delay/reverb

### Routing
- melodic sequence A/B switched by sequential switch
- drum pattern A/B switched separately
- full melodic bus through Tape Stop
- clocked lag set to quarter or half note

### Structure
- Verse: sequence A, reduced drums
- Transition: tape-stop melodic bus
- Chorus: sequence B, brighter filter, fuller drums
- Transition back: tape-stop full mix briefly
- Verse 2
- Bridge: long tape stop + no kick + sustained pad
- Final chorus: all parts active
- Outro: repeated shorter stops, then final long stop

### Why it works
Tape Stop becomes your “section punctuation mark.”

---

## Patch 4: Performance sampler song
### Goal
Use prepared samples/clips and make transitions feel live.

### Modules
- sample player
- drums
- bass
- Tape Stop
- VCA
- cue mixer or performance mixer
- trigger controller/pads

### Routing
- sample player through Tape Stop
- dry sample multed to second channel
- 50/50 mode enabled on Tape Stop
- manual pad controller to Trig input

### Performance method
- trigger Tape Stop at end of sample phrases
- switch sample bank during slowdown
- bring in bass underneath
- use longer lag for vocal sample transitions, shorter lag for drum fills

### Why it works
This is close to DJing with phrases, but still modular.

---

# Using momentary vs latching for arrangement

## Momentary mode
Best for:
- fills
- brief transitions
- hands-on performance
- rhythmic pumping stop effects
- “grab and release” phrasing

### Song use
Use momentary on:
- drums during turnarounds
- lead synth at the end of vocal-like phrases
- loops during intro texture work

It feels expressive and playable.

---

## Latching mode
Best for:
- full breakdowns
- longer dramatic stops
- section changes
- sustained transitions

### Song use
Use latching when you want:
- one trigger to begin the section collapse
- time to mute/unmute/repatch/switch patterns
- another trigger to release into the next section

This is better for macro-arrangement.

---

# Using Lag CV to keep transitions from getting repetitive

A common problem in modular is that transitions become too predictable. Lag CV helps.

## Patch ideas
- send slow random CV to Lag CV
- send stepped CV from a sequencer row
- send envelope to create longer stops at stronger accents
- use attenuator/offset to constrain values to useful ranges

### Song benefit
Different sections can have different stop lengths automatically:
- verse = short and subtle
- chorus = tighter and punchier
- breakdown = much longer
- outro = longest

That gives the song contour.

---

# Using 50/50 mode musically

The manual notes:
> Holding the Trig button at boot up sets dry/wet mix to 50%.

This is very useful for arrangement.

## Why 50/50 mode matters
A fully wet tape stop can be dramatic, but it can also remove too much clarity. In a song context, 50/50 mode lets the audience still hear:
- pulse
- note identity
- section continuity

while getting the slowdown gesture.

## Best uses
- on melodic bus
- on vocals/samples
- on full mix in subtle genres
- on intros and transitions where total collapse would be too extreme

If you want even more control, the manual’s suggestion of using a **VCA with separate dry/wet paths** is excellent.

---

# Practical full-song workflow with Tape Stop

Here’s a very workable method.

## 1. Build three states, not one loop
Before using Tape Stop, define:
- **State A**: minimal groove
- **State B**: main groove
- **State C**: breakdown or alternate groove

Tape Stop works best when it transitions between pre-planned states.

---

## 2. Decide where the effect lives
Choose one:
- full mix
- drum bus
- melodic bus
- sample bus

Don’t overcommit too early. Usually **drum bus** or **melodic bus** is more flexible than full mix.

---

## 3. Clock it
Patch the master clock to Tape Stop’s clock input.

This is critical if you want:
- repeatability
- section timing
- song-friendly transitions

---

## 4. Assign section lengths
Use divider pulses or sequencer triggers for:
- every 8 bars
- every 16 bars
- every 32 bars

These pulses can:
- trigger Tape Stop
- switch patterns
- mute channels
- transpose sequences

Now your modular patch is beginning to behave like a song machine.

---

## 5. Reserve different lag times for different formal roles
For example:
- **16th / 8th** = fill
- **quarter / half** = transition
- **1 bar / 2 bars** = breakdown entry
- **4+ bars** = ending or ambient collapse

This creates a consistent arrangement language.

---

## 6. Layer another change with every tape stop
Never rely on Tape Stop alone for the full song effect.

At each stop, also do one or more of:
- mute kick
- change sequence
- transpose bass
- open filter
- switch samples
- alter clock division
- change probability density
- increase reverb send

That is how transitions become sections.

---

# Genre-specific ideas

## Techno
- tape-stop drum bus every 16 or 32 bars
- long stop before drop
- pair with mutes and filter sweeps

## House
- short synced stops at phrase ends
- use on drum bus or sampled chords
- fake vinyl/tape DJ transitions between sections

## Ambient
- apply to loopers and textures
- use long bar-based lag values
- combine with reverb and Lo-Fi coloration

## Hip-hop / beat tape
- use 50/50 mode
- route sampled phrases or full beat bus through it
- trigger at scene changes for cassette-stop character

## Synthwave / electro
- use on full mix sparingly for dramatic breakdowns
- pair with chorus, delay, and nostalgic sample material

## Experimental
- CV the lag heavily
- use logic and random triggers
- alternate between synchronized and manual gestures
- place before or after loopers for extreme time-feel disruption

---

# Limitations to keep in mind

Tape Stop will not, by itself:
- create melodies
- store song sections
- sequence arrangements
- mix multiple layers
- perform mutes for you

So for full-length songs, it works best alongside:
- sequencers with resets/pages/song mode
- mixers/performance mixers
- VCAs
- mutes
- switches
- clock dividers
- samplers/loopers
- effects

Think of Tape Stop as a **section punctuation module**, not a complete arrangement brain.

---

# Best complementary module types for full-song writing

If your goal is complete songs, Tape Stop is especially strong with:

- **performance mixers**: bring parts in/out around stops
- **clock dividers**: place transitions every 8/16/32 bars
- **switches**: move between verse/chorus material
- **VCAs**: separate dry/wet or animate buses
- **samplers/loopers**: transition clips and phrases
- **logic/probability**: automate when transitions happen
- **reverb/delay**: make stop events bloom into space
- **filters**: shape energy around transitions
- **macro controllers**: one gesture changes several things at once

---

# Bottom line

The **2hp Tape Stop** is not a song generator, but it is a very effective **song-finishing module**.

Its real power in Eurorack is that it helps convert:
- loops into phrases
- phrases into sections
- sections into performances

Use it to:
- mark 8/16/32 bar boundaries
- create breakdowns and drops
- hide pattern or sample switching
- build intros and outros
- perform fake endings and restarts
- differentiate verse/chorus/bridge states
- make transitions feel musically intentional

If you combine it with **clocked structure, VCAs/mutes, pattern switching, and submixes**, Tape Stop can be one of those deceptively small modules that makes the difference between a cool patch and an actual full-length song.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)