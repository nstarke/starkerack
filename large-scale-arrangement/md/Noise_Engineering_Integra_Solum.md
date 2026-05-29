# Noise Engineering — Integra Solum

- [Manual PDF](../../manuals/Integra Solum Manual - Noise Engineering Documentation.pdf)

---

[Manual PDF / documentation](https://manuals.noiseengineering.us/is/)

# Using Noise Engineering Integra Solum to build full-length Eurorack songs

Integra Solum is easy to misunderstand as “just” a clock divider / trigger source. But for song construction, that is exactly the kind of module that can turn a cool loop into an arrangement.

Its real strength is not only making rhythms — it is making **structured time divisions**, **section changes**, **rotating variations**, and **parallel trigger streams** that can control multiple layers of a patch over longer spans.

## What Integra Solum does well

From the manual:

- Dual rotating clock divider
- 16 trigger outputs total, in two groups of 8
- Both sides can share one clock or run independently
- Both sides can share reset or reset independently
- 3 modes per side:
  - `/2N` = powers-of-two divisions
  - `N` = sequence of eight
  - `/2N+1` = odd divisions
- `Shift` rotates output order
- “Wack mode” adds randomized behavior
- Outputs are trigger outputs, 0–5 V, triggering around 3.4 V

That means it can act as:

- a master **section clock brain**
- a **drum arrangement source**
- a **phrase variation generator**
- a **fill / break generator**
- a **modulation scheduler**
- a **song form coordinator**

---

# Why this module is useful for full songs

A full song usually needs more than a repeating 1-bar pattern. It needs:

- intro
- groove entry
- tension / subtraction
- variation
- fills
- breakdown
- return
- ending

Integra Solum helps because it naturally produces **events at different time scales**.

For example, from one master clock you can derive triggers that happen:

- every 2 steps
- every 4 steps
- every 8 steps
- every 16 steps
- every 32 steps

Those longer divisions are exactly what creates arrangement.

Instead of asking:
> “How do I make a song?”

you can patch:
> “What should happen every 8 bars? Every 16 bars? Every 32 beats? What should rotate at the end of each phrase?”

Integra Solum gives you those timing landmarks.

---

# Core song-building idea

Use Integra Solum in **layers of time**:

- **Fast events**: hats, accents, ratchets, melodic note clocks
- **Medium events**: kick pattern variations, bass phrase resets, chord changes
- **Slow events**: mute/unmute, filter opening, switching sequencer pages, changing effect sends, transitions between sections

A full-length song emerges when those layers interact over time.

---

# Best roles for each side

Because Integra Solum is dual, a very practical use is:

## Side A: “musical pattern timing”
Use one side for things the listener clearly hears as rhythm or phrase structure:
- drums
- bass resets
- melodic step advances
- fills
- phrase endings

## Side B: “arrangement and transitions”
Use the other side for slower or more hidden control:
- switch sequential switch routes
- trigger envelope bursts for transitions
- advance sequencer pages
- open VCAs for different voices
- change quantizer root
- enable effect sends
- trigger sample changes

This split makes the patch feel more song-like instead of just busy.

---

# Understanding the modes musically

## 1. `/2N` mode: powers of two
This is the most useful mode for arrangement.

Musically, use it for:
- phrase boundaries
- 2-bar / 4-bar / 8-bar / 16-bar changes
- kick dropouts every few bars
- opening a filter every 8th or 16th cycle
- switching sections

This is the “song form” mode.

### Example uses
- Output 1: every 2 clocks
- Output 2: every 4 clocks
- Output 3: every 8 clocks
- Output 4: every 16 clocks

Even if you don’t know exactly which jack corresponds to which division in practice, patch and listen: some outputs will clearly be slower and ideal for arrangement timing.

---

## 2. `N` mode: sequence of eight
This behaves more like a moving one-of-eight trigger stream.

Musically, use it for:
- stepping through drum voices
- driving an 8-stage melodic accent structure
- sending one trigger to a sequential switch to create scene changes
- creating “which lane is active now?” behavior

This is the “ordered pattern evolution” mode.

### Example uses
- Trigger one of 8 VCAs in succession
- Route one trigger across 8 modulation destinations via switch logic
- Clock a switch that changes oscillator timbre every phrase step

Very useful for making arrangement feel intentional rather than random.

---

## 3. `/2N+1` mode: odd divisions
This is where groove starts becoming less square.

Musically, use it for:
- polymetric accents
- fills that don’t align every bar
- asymmetrical modulation
- variation in percussion layers
- non-obvious phrase resets

This is the “keep the loop from becoming static” mode.

### Example uses
- Trigger a clap accent every 3 or 5 cycles
- Fire a noise burst into reverb on an odd division
- Advance a secondary melody at an odd interval against a 16-step main line

Odd divisions are excellent for full-length songs because they create **longer composite cycles** before repeating.

---

# Wack mode for arrangement

Wack mode is particularly valuable for transitions and anti-loop fatigue.

From the manual:

- `/2N` becomes probabilistic divide-by-two behavior
- `N` generates one random trigger at each step
- `/2N+1` gives independent 50% chance per output per clock

This means Wack mode is not just “random chaos.” It is **controlled variation**.

## Good musical uses for Wack mode
- fills at the end of phrases
- semi-random percussion texture during breakdowns
- changing note density in arpeggios
- evolving hi-hat accents
- conditional stabs or FX hits

## Best practice
Don’t leave everything in Wack mode all the time. Use it in **specific sections**:
- intro texture
- pre-drop tension
- breakdown instability
- final chorus variation
- outro decay

That way it sounds like arrangement, not drift.

---

# Patch strategies for full-length songs

## 1. Build a verse/chorus structure with mutes and VCAs

### What you need
- Integra Solum
- master clock
- multiple voices
- VCAs or mute modules
- envelopes

### Patch concept
- Clock both sides from one master clock
- Use Side A in `/2N` mode for phrase timing
- Use slow outputs to trigger envelopes that open VCAs for different voices
- Use Side B to rotate or switch variation triggers

### Song behavior
- Intro: only kick + texture voice open
- Verse: bass VCA opens every 8 or 16 beats
- Chorus: lead voice and open hats come in on a slower divider trigger
- Breakdown: gate closes bass and kick, leaves FX and melody fragments
- Final section: all VCAs opened, plus Wack-mode percussion accents

This is one of the cleanest ways to turn a patch into sections.

---

## 2. Use it as a “scene change trigger” for sequential switches

Sequential switches are one of the strongest song-form tools in Eurorack.

### Pair with
- Doepfer A-151
- Noise Engineering Vice Virga / Confundo Funkitas style logic tools
- any sequential switch
- switchable sequencers or sample players

### Patch concept
Use slow Integra Solum outputs to:
- advance a sequential switch
- switch between:
  - different bass CV sequences
  - different drum trigger patterns
  - different modulation routings
  - different quantizer roots
  - different effect send levels

### Result
The patch changes “scene” every phrase.

### Example
- Scene 1: intro
- Scene 2: verse groove
- Scene 3: chorus
- Scene 4: breakdown
- Scene 5: return
- Scene 6: final chorus with extra percussion

Integra Solum becomes a song section conductor.

---

## 3. Drive drum arrangement over many bars

A common issue in Eurorack is a great 1-bar drum loop that never develops.

### Patch concept
Let your core drum sequencer handle the main beat, but use Integra Solum to create:
- clap entrances
- tom fills
- crash triggers
- hat density changes
- kick dropouts
- snare flam triggers
- end-of-phrase noise bursts

### Pair with
- drum modules
- logic modules
- burst generators
- VCAs
- mute matrix
- OR combiner / trigger mixer

### Specific approach
- Main sequencer = kick/snare fundamentals
- Integra Solum outputs = arrangement overlays
- `/2N` outputs trigger crash or fill every 16 or 32 steps
- `N` mode rotates through toms or percussion lanes
- Wack mode drives occasional hat and rim variations

This creates the feeling of a drummer or arranger intervening over time.

---

## 4. Reset sequencers to create phrases

Resets are one of the most important arrangement tools in modular.

### Pair with
- melodic sequencer
- bass sequencer
- Euclidean sequencer
- quantizer
- clocked modulation source

### Patch concept
Use Integra Solum outputs not only as note triggers, but as:
- sequencer reset triggers
- modulation reset triggers
- envelope re-sync triggers

### Why this matters
A patch often sounds “songless” because multiple clocks run freely with no phrase boundaries.

Use slow Integra Solum triggers to:
- reset the bass sequencer every 16 steps
- reset the melody every 32 steps
- reset a modulation LFO every 64 steps

Now phrases line up and sections feel intentional.

---

## 5. Use Shift as a live arrangement control

The Shift/Offset control rotates outputs. This is very useful live.

Instead of repatching, you can rotate which output is considered first in the cycle.

## Musical result
- fills happen in different places
- accents shift forward/backward
- phrase emphasis changes
- drum lane ordering changes
- switch progression changes

If one side is controlling a sequence of section actions, rotating it effectively rearranges the order of events.

### Practical use
During performance:
- keep one side stable for core groove
- manually move Shift on the other side to create evolving arrangements

This is a strong way to make a 6-minute performance feel composed.

---

## 6. Separate clocks for macro and micro time

Because each side can be clocked independently, you don’t have to run both from the same pulse.

### Powerful approach
- Side A gets 16th-note clock
- Side B gets bar clock, phrase clock, or divided clock from another module

### Why
Now one side handles local rhythm while the other handles large-scale arrangement.

### Example
- Side A: hats, percussion, melodic triggers
- Side B: every bar or every 2 bars triggers section changes, filter swells, switch advances

This creates hierarchy in the patch, which is key to song form.

---

## 7. Create intros and outros by gradual layer activation

Full-length songs often need gentle entry and exit.

### Patch concept
Use progressively slower outputs to bring in layers one by one:
- drone starts immediately
- kick starts after a few bars
- bass enters after 8 bars
- hat enters after 16 bars
- lead enters after 32 bars

You can do this with:
- trigger-to-gate modules
- sample & hold plus comparator
- sequential switches
- latching VCAs / gate-controlled VCAs

Similarly for outros:
- remove hats first
- then lead
- then bass
- leave kick + delay tail
- then only texture

Integra Solum gives the timing skeleton for that.

---

# Module combinations that work especially well

## With trigger sequencers
Examples:
- Steppy
- Numeric Repetitor
- Varigate
- Pam’s Pro Workout
- Euclidean Circles

Use Integra Solum as the **macro arranger** above the trigger sequencer.

The sequencer makes the groove.
Integra Solum decides when the groove changes.

---

## With melodic sequencers
Examples:
- Metropolix
- René
- Mimetic Digitalis
- Moskwa
- Voltage Block plus quantizer

Use Integra Solum to:
- reset phrases
- switch stored sequences
- transpose sections
- enable alternate clocks
- trigger different envelopes for note articulation

This helps transform a cool riff into verse/chorus development.

---

## With quantizers
Examples:
- Scales
- Bard Quartet
- O_C
- ADDAC quantizers

Use slow trigger outputs to:
- change root note
- switch scale
- transpose melody up for chorus
- move bass from tonic pedal to progression tones

One of the fastest routes to “song” is harmonic change.
Integra Solum can schedule those changes.

---

## With sequential switches
This may be the single best pairing.

Use it to switch:
- CV patterns
- trigger lanes
- modulation destinations
- audio sources
- filter inputs

Now every phrase can be a different arrangement state.

---

## With logic modules
Examples:
- AND / OR / XOR logic
- Compare 2
- Joranalogue logic tools
- Ladik logic modules

Logic multiplies the usefulness of Integra Solum.

### Example
- Main snare trigger AND a slow divider trigger = only occasional snare accent
- Kick trigger XOR odd division = changing syncopation
- Melody gate OR random Wack trigger = occasional grace notes

This creates controlled song evolution.

---

## With VCAs and envelope generators
This is essential.

Triggers only matter musically if they open or shape something.
Use Integra Solum to trigger:
- accent envelopes
- amplitude envelopes
- filter envelopes
- effect send envelopes
- ducking or sidechain pulses

For song construction, think in terms of:
- when does this part enter?
- how strongly?
- for how long?
- on what phrase cycle?

---

## With effects
Use slow outputs to animate effects over sections:
- send more snare to reverb every 8 bars
- open delay feedback during fills
- trigger freeze or hold functions
- switch between dry and wet paths
- clock modulation on delay/reverb parameters

Effects automation is one of the easiest ways to create progression without changing notes.

---

# Concrete full-song patch examples

## Patch 1: Techno arrangement engine

### Modules
- drum voices
- bass voice
- lead voice
- 1 main trigger sequencer
- 1 melodic sequencer
- Integra Solum
- mute VCAs
- filter
- delay/reverb
- sequential switch

### Patch
- Main clock to Integra Solum and trigger sequencer
- Side A `/2N`: phrase triggers
- Side B `N`: route through sequential switch for section changes

### Use
- Output A1: occasional open hat accents
- Output A2: clap enable every phrase
- Output A3: crash trigger every 16 steps/bars
- Output A4: reset bass sequence every 32 steps
- Output B outputs: advance switch selecting 1 of 4 lead modulation states

### Song structure
- 0:00–0:45 intro: kick + filtered percussion only
- 0:45–1:30 bass enters on a slow divider event
- 1:30–2:15 lead enters when switch reaches scene 2
- 2:15–2:45 breakdown: mute kick using gate logic, enable Wack percussion
- 2:45–4:00 full groove return, Shift slightly rotated for new accents
- 4:00–end gradual layer subtraction

---

## Patch 2: Generative ambient song with recurring form

### Modules
- 2–3 voice patch
- quantizer
- clocked random
- envelopes
- VCAs
- reverb
- sequential switch
- Integra Solum

### Patch
- Side A in `N` mode controls which voice is active each step/phrase
- Side B in `/2N` mode resets melodic and modulation cycles
- Wack mode on one side for sparse random texture triggers

### Result
- recurring phrase markers create recognizable form
- random textures keep it evolving
- resets keep it from turning into an endless drift

This is great for long-form ambient where “song” means recurring sections rather than verse/chorus.

---

## Patch 3: Bassline + melody song form

### Modules
- bass sequencer
- melody sequencer
- quantizer
- two voices
- mixer
- VCA
- switch or precision adder
- Integra Solum

### Patch
- Side A controls bass phrase resets and accents
- Side B controls melody transposition and section changes

### Use
- A slow output resets bass every 16 steps
- Another output opens bass accent envelope at phrase start
- Side B triggers precision adder transposition:
  - section 1 = root
  - section 2 = +5th
  - section 3 = relative minor / alternate root
- another slow output enables melody only in chorus sections

Now your song gains harmonic and textural development without needing a DAW-style arranger.

---

## Patch 4: Drum fill and transition machine

### Modules
- main drum sequencer
- sample player or noise voice
- burst generator
- logic
- reverb
- Integra Solum

### Patch
- Main groove stays stable
- Integra Solum handles only transitions:
  - fill trigger
  - crash trigger
  - reverse cymbal / noise swell
  - delay send burst
  - kick mute for one beat before drop

### Why it works
Many songs are defined less by the loop and more by the transitions between loops.
Integra Solum can specialize in that role and dramatically improve song feel.

---

# Practical workflow for writing a song with Integra Solum

## Method 1: Build from the longest timescale first
1. Set master clock
2. Patch slow Integra Solum outputs to section-change functions
3. Define:
   - intro length
   - phrase length
   - breakdown point
   - return point
4. Then fill in drums and melody

This works better than starting with a dense groove and trying to “arrange” later.

---

## Method 2: Reserve one side only for arrangement
This is a great discipline.

- Side A = groove support
- Side B = song form only

Do not spend all outputs on drums.
Keep at least a few outputs for:
- mutes
- resets
- switch advances
- effect moments
- harmonic changes

That is usually the missing ingredient in Eurorack songs.

---

## Method 3: Use one “event” per phrase
For each phrase boundary, decide one thing that changes:
- add hat
- remove bass
- transpose melody
- open filter
- trigger fill
- change switch state
- enable random mode

If each phrase has one clear event, the listener hears progression.

Integra Solum excels at creating these phrase events.

---

# Important performance ideas

## Manual interaction matters
A full song in Eurorack often comes from a combination of:
- automated structure
- live intervention

On Integra Solum, live actions can include:
- changing mode
- rotating Shift
- entering/exiting Wack mode
- changing which side shares a clock/reset
- muting outputs downstream

These actions can act like arrangement moves:
- verse to chorus
- stable groove to fill-heavy section
- breakdown to full density return

---

## Use reset intentionally
Reset is one of the strongest “section marker” gestures in modular.
A reset can make the whole system feel like it has arrived at a new chapter.

Use resets:
- at drop returns
- at end of breakdowns
- at start of melody sections
- when changing clock relationships

---

# Limitations to be aware of

Integra Solum is not a full song arranger by itself.

It does not:
- store songs
- chain patterns explicitly
- remember section order
- output pitch CV
- mute audio directly

So to make full songs, you should pair it with:
- VCAs
- switches
- logic
- sequencers
- quantizers
- mixers
- effects

Think of it as a **structural timing generator**, not a complete composer.

That said, structural timing is often exactly what a modular patch lacks.

---

# Best song-building use cases in one sentence each

Integra Solum is especially good for:

- turning bar-level loops into phrase-level arrangements
- making different voices enter and leave on longer cycles
- creating fills and transitions automatically
- resetting sequencers into recognizable song phrases
- controlling section changes via switches
- adding non-repeating long-form variation with odd divisions
- using Wack mode to inject controlled instability

---

# A simple “full song” starter patch

If you want one practical patch to try immediately:

## Modules
- clock source
- kick, snare, hat voices
- bass voice
- lead voice
- melodic sequencer
- sequential switch
- 4 VCAs or mute channels
- Integra Solum

## Patch
- Clock to both Integra Solum sides
- Side A `/2N`
  - one output to hat accents
  - one to bass sequencer reset
  - one to crash
  - one to fill trigger
- Side B `N`
  - outputs to sequential switch selecting:
    1. bass only
    2. bass + drums
    3. add lead
    4. breakdown modulation state
    5. full chorus
- Use VCAs to open/close layers based on switch outputs
- At breakdown, engage Wack mode on one side for hats and percussion only
- Rotate Shift for the final section

That can easily produce a 4–8 minute performance with clear form.

---

# Final thought

Integra Solum helps create full-length songs because it gives you a way to think beyond the loop.

In Eurorack, the jump from “great pattern” to “great song” usually comes from adding:
- phrase boundaries
- section changes
- controlled entrances and exits
- resets
- fills
- long-cycle variation

Integra Solum is extremely strong at all of those.

If you treat it not as a divider but as a **song clock architecture module**, it becomes much more powerful.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)