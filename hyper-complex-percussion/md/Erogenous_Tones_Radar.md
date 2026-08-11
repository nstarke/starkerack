# Erogenous Tones — Radar

- [Manual PDF](../../manuals/radar-instructions.pdf)

---

[Manual PDF / info page](http://erogenous-tones.com)

# Erogenous Tones RADAR for dense, hyper-complex percussion

RADAR is not a sound source by itself — it’s an **8-channel envelope/LFO generator**. That makes it extremely strong for **percussion architecture**: shaping drum voices, pinging filters/LPGs, modulating VCAs, creating clock-related motion, and building interlocked rhythmic systems.

Because it gives you **8 envelopes**, **repeating mode**, **AR/AD behavior**, **digital vs analog modeling**, **composite outputs**, and **quad/oct phase relationships**, it is ideal for:

- polymetric trigger shaping
- layered transient design
- evolving per-step drum articulation
- phase-shifted rhythmic modulation
- burst-like envelope-derived percussion
- pseudo-Euclidean and rotating accent systems

---

## What RADAR is best at for percussion

Think of RADAR as a **rhythm sculptor**, not just an envelope bank.

You can use it to:

- shape **kick, snare, hat, clap, tom, FM percussion, noise bursts**
- create **different envelope lengths** across voices for polyrhythmic feel
- generate **repeating envelopes as LFOs** that act like rhythmic modulators
- create **offset phase envelopes** in QUAD or OCT mode for rotating rhythms
- derive **composite accent patterns** using lane 4 and lane 8 max outputs
- use **analog vs digital behavior** to change whether retriggers snap or glide

If your goal is “densely rhythmic with hyper-complex percussion,” RADAR can become the **central articulation engine** for nearly every drum layer in the patch.

---

# Core concepts from the manual that matter most musically

## 1. Envelope Mode = 8 independent rhythm articulators
In **ENVELOPE MODE**, each of the 8 lanes can be its own:

- **AD envelope**
- **AR envelope**
- **Repeating envelope / LFO**

This is the most direct mode for complex percussion patches because each lane can control a separate part of the drum ecosystem.

Good uses:
- one lane per drum voice
- one lane for amplitude, another for pitch on the same drum
- one lane for transient click, another for body
- one lane for filter ping, one for distortion amount, one for decay length

---

## 2. Trigger normalization is very useful for cascaded rhythm systems
Each channel’s trigger input is **normalized to the next channel below it**.

That means one trigger stream can be distributed down multiple lanes until you patch over it.

This is fantastic for percussion because you can:
- send one master pattern into the top lane
- let several lower lanes inherit it
- then patch specific lanes differently to create divergence

This gives you a patch that feels related, but not repetitive.

---

## 3. Repeating mode can act like an LFO/clocked pulse shaper
Each lane can be set to **Repeating** mode.

That means you can turn envelopes into:
- cyclic percussion modulation
- ratchet-like motion
- rotating accent shapes
- independent modulation clocks

Because each lane can run at a different rise/fall time, you can make:
- one lane cycling in 5-beat-feel
- another in 7-beat-feel
- another in short fast bursts for hat chatter

Even without a dedicated trigger sequencer, repeating lanes can create living rhythmic motion.

---

## 4. Digital vs Analog modeling changes rhythmic feel
The manual’s distinction here is very important.

### Digital mode
- retriggers reset the envelope to zero immediately
- creates hard discontinuities
- repeating frequency is constant

For percussion this is:
- tighter
- sharper
- more machine-like
- more precise for aggressive rhythmic repetition

Use digital when you want:
- hard kicks
- snappy hats
- exact retrigger behavior
- glitchy, chopped accents

### Analog modeling
- retriggers do not always reset in the same way
- attack can begin from the current level
- short gates in AR may not reach full amplitude
- feels like capacitor charging/discharging

For percussion this is:
- more elastic
- more organic
- less identical from hit to hit
- great for “alive” drum articulation

Use analog when you want:
- hand-drum feel
- swelling accents
- softer retrigger overlap
- unstable or rolling percussion lines

A powerful strategy is to mix both:
- digital for kick/closed hat precision
- analog for toms, metallics, noise bursts, and modulations

---

## 5. Shape is a huge part of punch
The shape knob/CV moves between **LOG, LIN, and EXP**.

This matters for percussion more than people often realize.

### EXP attack / decay tendencies
Can produce:
- fast, snappy transients
- aggressive punch
- hard clicking articulation

Great for:
- kick attack
- tight hats
- pluck-like percussion
- VCA chopping

### LOG shape
Can produce:
- slower perceived onset or tail contour
- more bloom
- rounder percussion
- “air” around the transient

Great for:
- toms
- cymbal noise shaping
- resonant filter pings
- swelling accents

### LIN
Good neutral starting point for:
- balanced drum body
- clock-like modulation
- predictable response

The manual also notes **E/O** behavior:
- **Equal**: decay/release shape matches attack shape
- **Opposite**: release becomes the opposite contour

This is excellent for percussion design:
- a **LOG rise + EXP fall** can feel like a soft lift into a tight snap
- an **EXP rise + LOG fall** can give punch followed by a longer perceived body

---

# Best patch strategies for hyper-complex percussion

## Strategy 1: Use RADAR as a full drum articulation matrix
Patch several lanes to different destinations on the same drum voices.

Example for one kick voice:
- **Lane 1** → VCA amplitude envelope
- **Lane 2** → oscillator pitch for kick thump
- **Lane 3** → click transient VCA or filter cutoff
- **Lane 4** → distortion amount or wavefolder depth

Now the kick is no longer one static hit — it has:
- body
- pitch snap
- transient
- harmonic aggression

Do the same for snare:
- lane for noise VCA
- lane for body oscillator VCA
- lane for bandpass filter sweep
- lane for metallic ring modulation depth

This is how you get **punchy, unique, percussive drums** from otherwise simple voices.

---

## Strategy 2: One trigger source, many envelope interpretations
Since triggers normalize downward, send one trigger pattern to the top and use different RADAR modes per lane.

For example:
- Lane 1: AD, short, digital, EXP
- Lane 2: AR, analog, medium, LOG
- Lane 3: Repeating, synced by reset triggers
- Lane 4: AD, long release, opposite shape

All four react to the same pulse stream differently.

This creates:
- layered accents
- varied envelope density
- controlled rhythmic complexity without unrelated chaos

This is especially effective on:
- stacked hats
- clap layers
- multi-osc percussion clusters

---

## Strategy 3: Build polyrhythms with different envelope times
Even if several voices are triggered by the same clock division, the **envelope lengths** themselves can imply different meters.

Example:
- Kick envelope very short, every 4 beats
- Snare tail set to length suggestive of 3-beat grouping
- Metallic hit decay tuned to 5-beat cycle interaction
- Hat modulation repeating at a different period

This creates **polymetric perception** through articulation, not just trigger placement.

Practical patch:
- lane cycles in Repeating mode to modulate VCA or filter on a hat voice
- another lane cycles at a different rate to modulate pitch or tone
- a third lane triggers from sequencer but has AR behavior that responds to varying gate lengths

Result: the same programmed rhythm sounds much more complex.

---

## Strategy 4: Use QUAD mode for rotating 4-part percussion geometry
In **QUAD MODE**, 4 lanes are phase-offset by **90 degrees**.

This is extremely useful for:
- four interrelated percussion voices
- rotating accents
- circular rhythm illusions
- “one pattern chasing itself”

You can patch:
- lane 1 → kick accent
- lane 2 → snare timbre
- lane 3 → hat VCA
- lane 4 → percussion pitch or FM amount

Since they are phase-related, they create naturally interlocked movement.

Best use cases:
- techno percussion rings
- 4-on-the-floor plus rotating offbeat modulation
- cross-accented tom networks
- pseudo-African cyclic interlock patterns

The manual notes extra CV functions in QUAD mode:
- **SPEED**
- **GRAVITY**
- **SDELTA**

These are gold for advanced rhythm work.

### SPEED
Modulates the overall speed of the quad relationship.

Use it to:
- compress or expand all related modulations together
- create fills where all percussion motion speeds up
- slowly drift polyrhythmic relationships

### GRAVITY
Changes how the phase-related waves are attracted/repelled relative to lane 1.

Musically:
- can tighten the groove toward one pulse center
- or pull voices away from the center into more asymmetrical timing feel

This is amazing for:
- “swing beyond swing”
- rotating push/pull accents
- unstable but coherent percussion timing

### SDELTA
Offsets shape relationships across the lanes.

Use it to make:
- one lane snappy
- next lane more linear
- next lane bloomy
- next lane very sharp

That means one rotating phase system can also have **rotating timbral articulation**.

For drums, this is huge.

---

## Strategy 5: Use OCT mode for 8-step circular rhythm fields
In **OCT MODE**, all 8 lanes are phase-shifted **45 degrees** apart.

This is one of the best ways in the module to create complex rhythmic ecosystems.

Think of it like an 8-point wheel of envelope motion.

Patch ideas:
- all 8 lanes to 8 drum parameters
- or 8 VCAs opening 8 sound sources
- or 8 modulation inputs across 2–3 voices

This creates:
- phase-locked but offset rhythm webs
- dense interdependence
- highly animated percussion that still feels unified

Excellent for:
- glitch percussion matrices
- probabilistic-feeling but deterministic drum movement
- fast modular electro
- broken beat / IDM style articulation

Example:
- Lane 1: kick pitch
- Lane 2: kick saturation
- Lane 3: snare noise level
- Lane 4: snare body filter
- Lane 5: closed hat VCA
- Lane 6: open hat decay
- Lane 7: metallic FM amount
- Lane 8: clap width or reverb send VCA

Because the modulation phases are offset, every hit feels related but non-identical.

---

# Using RADAR to create complicated time signatures and patterns

## 1. Fake odd meters with cycle lengths
Set repeating envelopes with different speeds and use them to modulate:
- VCAs
- comparator thresholds
- trigger extractors
- logic modules
- sequential switches

For example:
- one repeating lane implies a 5-unit cycle
- another implies a 7-unit cycle
- another runs in 4

When these modulate percussion parameters, the resulting feel becomes **5 against 7 against 4**.

Even if your master clock is steady, the articulation creates shifting meter perception.

---

## 2. Use gate length to alter AR behavior
The manual says a **GATE input** can choose between AD and AR based on level, and in AR mode the envelope can continue attack while high.

This is fantastic for variable accents.

Patch different gate lengths from your sequencer or logic source:
- short gates = smaller attacks / shorter accents
- long gates = fuller rise / held peaks / longer tails

In analog mode, this can be especially expressive because short triggers may not reach full level.

Use this for:
- ghost notes vs accents
- flam-like dynamic differences
- evolving snare pressure
- hat openness tied to pattern length

This is a strong way to add “drummer-like” expression to rigid step patterns.

---

## 3. Trigger resets in repeating mode for ratchets and phrase turns
In Repeating mode, trigger inputs **reset the waveform**.

Use this with:
- clock divisions
- burst generators
- manual fills
- end-of-bar resets

Patch idea:
- Lane repeats at a fast rate to modulate hat VCA or filter
- occasional trigger reset from a larger phrase clock realigns it
- another lane runs at a nearby but different speed

This gives you:
- local rhythmic turbulence
- phrase-level re-synchronization
- patterns that feel like they mutate but return

Very effective for:
- IDM hats
- rolling metallics
- machine-gun fills that don’t stay static

---

## 4. Composite outputs for grouped accents
The manual says **Lane 4** and **Lane 8** can output a **max/composite waveform**:
- lane 4 = max of lanes 3 and 4
- lane 8 = max of lanes 6, 7, and 8

This is a powerful percussion utility.

Use these outputs as:
- accent buses
- grouped VCA control
- drum bus compression sidechain source
- layered transient macro-envelope

Why it’s useful:
Instead of summing and clipping, you get a “whichever is strongest wins” contour.

Applications:
- combine two related percussive envelopes into one accent line
- let several hat/tom envelopes drive one filter
- create a dynamic bus envelope for distortion or ducking
- extract a “dominant gesture” from multiple micro-rhythms

For hyper-complex patterns, this helps make the patch feel intentional rather than messy.

---

# Patch recipes

## Patch 1: 8-lane percussion laboratory
Use ENVELOPE MODE.

### Assignments
- Lane 1: Kick amplitude
- Lane 2: Kick pitch
- Lane 3: Snare noise amplitude
- Lane 4: Snare body amplitude or composite accent
- Lane 5: Closed hat amplitude
- Lane 6: Open hat decay CV
- Lane 7: Metallic percussion FM index
- Lane 8: Percussion bus distortion CV or composite bus accent

### Settings
- Kicks: digital, EXP-ish
- Snare body: analog, LIN to LOG
- Hats: digital, short AD
- Metallics: analog repeating or AD with unusual shapes

### Result
A tightly interrelated drum network with per-voice articulation and macro-accent options.

---

## Patch 2: Rotating 4-voice polyrhythm engine
Use QUAD MODE.

### Voices
- Lane 1 phase: kick voice accent
- Lane 2 phase: snare filter
- Lane 3 phase: hat VCA
- Lane 4 phase: tom pitch or noise level

### Modulate
- SPEED slowly from another LFO
- GRAVITY with stepped random or a manual CV
- SDELTA with a slow envelope

### Result
A 4-part rotating rhythm system where each voice breathes around the others with controlled complexity.

---

## Patch 3: OCT mode for hyper-dense hat and percussion cloud
Use OCT MODE and patch all 8 lanes into:
- 4 different hat/noise VCAs
- 2 filter cutoffs
- 1 wavefolder amount
- 1 reverb send VCA

All lanes are related but 45 degrees apart.

### Good move
Keep some envelopes very short and others medium-long. Use different shape contours.

### Result
A cloud of interlocked, phase-related percussive openings that sounds way more complex than a normal sequenced hat line.

---

## Patch 4: Humanized ghost-note snare system
Use ENVELOPE MODE.

- Lane 1: main snare VCA, digital AD
- Lane 2: snare noise layer, analog AR
- Lane 3: filter envelope, short EXP
- Lane 4: distortion or body resonance amount

Feed different gate lengths to the AR-controlled lane.

### Result
Main hits remain strong and consistent, while secondary layers vary in weight and contour, creating convincing ghost note behavior.

---

## Patch 5: Composite accent bus for drum glue
Use lane 3 and 4 as related envelopes, and set lane 4 to composite output.  
Use lane 6, 7, 8 similarly, with lane 8 in composite output.

Patch these composite outs to:
- filter cutoff on the drum bus
- VCA controlling parallel distortion
- compressor sidechain input if supported
- reverb send level for selected hits

### Result
Your dense percussion gets macro-dynamics and phrasing, not just micro-events.

---

# How to make percussion more punchy and unique with RADAR

## For punch
- use **digital mode**
- use **EXP-ish shapes**
- keep attack short
- use separate lanes for amplitude and pitch
- retrigger often for hard reset behavior
- modulate distortion, fold, or filter with a second envelope

## For uniqueness
- use **analog mode** on secondary layers
- exploit short AR gates that don’t fully rise
- mix different shapes across related voices
- use repeating lanes for internal motion
- use composite outputs as accent controllers
- phase-offset lanes in QUAD/OCT mode

## For percussive timbre design
RADAR is excellent at controlling:
- oscillator pitch drops
- filter pings
- LPG opening
- noise burst amplitude
- FM index bursts
- wavefolder stabs
- VCAs for transient click layers
- effects send bursts

A simple oscillator/noise source becomes a serious drum voice when RADAR handles multiple parameters at once.

---

# Advanced rhythmic ideas

## 1. Accent over one meter, timbre over another
Keep triggers in 4/4, but set repeating envelope rates or quad/oct modulation so timbre accents imply 5, 7, or 9 groupings.

This gives music that is playable and mixable, but rhythmically deep.

## 2. Use analog mode for “non-zero retrigger memory”
Because analog modeling can restart from the current level, repeated bursts create evolving contour depending on prior state.

That’s perfect for:
- drum rolls
- broken hats
- decaying ratchets
- asymmetrical fills

## 3. Separate transient and body envelopes
For every important drum:
- one lane for click/transient
- one lane for body
- one lane for pitch or filter
- one lane for character effect

This is the fastest way to get professional modular percussion.

## 4. Phrase-level reset logic
Use resets on repeating lanes only at larger phrase divisions. Let fast internal motion drift, then snap back every 8 or 16 bars.

This creates long-form rhythmic evolution without losing structure.

---

# Best practical workflow

## If you want maximum complexity:
Use **ENVELOPE MODE** first.

Why:
- all 8 lanes independent
- easier to assign across many drum functions
- easiest for mixed trigger sources
- best for “modular drum machine brain” behavior

## If you want rotating geometric rhythm:
Use **QUAD MODE**.

Why:
- immediate phase relationships
- coherent 4-lane interlock
- great for circular rhythmic feels

## If you want extreme phase-grid density:
Use **OCT MODE**.

Why:
- 8-way related motion
- ideal for dense percussion ecosystems
- strong for metallic, hat, noise, and FX modulation

---

# A strong performance setup

A good live/performance approach:

- **Lanes 1–2**: kick body + pitch
- **Lanes 3–4**: snare + composite accent
- **Lanes 5–6**: hats closed/open
- **Lanes 7–8**: metallic percussion + composite bus mod

Then perform with:
- shape changes
- switching AD/AR/repeating
- digital vs analog per lane pair
- output composite mode on 4 and 8
- phrase resets into repeating lanes
- external attenuation on shape CV and speed modulation

This gives you a playable system that moves from tight machine grooves to chaotic hyper-rhythm quickly.

---

# Bottom line

RADAR is excellent for hyper-complex percussion because it can be the:

- **amplitude engine**
- **pitch envelope bank**
- **accent generator**
- **rotating phase modulator**
- **composite rhythmic bus source**
- **humanizer / destabilizer**
- **polyrhythmic modulation core**

For dense rhythmic music, the most effective use is not “one envelope per voice,” but rather:

> **multiple RADAR lanes per percussion voice, plus repeating/phase-related lanes shaping the whole ecosystem.**

That’s where the module becomes truly powerful.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)