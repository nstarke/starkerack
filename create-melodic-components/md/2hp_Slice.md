# 2hp — Slice

- [Manual PDF](../../manuals/2hp_Slice.pdf)

---

[2hp Slice Manual PDF](https://twohp.com/modules/slice)

# Using 2hp Slice to Create Melodic Components

The attached manual is for **2hp Slice**, a **beat repeat / glitch engine**. On its own, Slice is not a pitch-generating oscillator or quantizer, but it can be used very effectively to create **melodic rhythm, pitched textures, repeating motifs, and variation** when paired with sound sources, samplers, loopers, and modulation.

## What Slice does musically

Slice takes incoming audio and, when triggered, **repeats small clock-synced chunks** of that audio. Because the repeat size is tied to the clock, it can produce:

- rhythmic stutters
- granular-like time slices
- glitch fills
- pitch-like artifacts when the slices get very short
- evolving repeated motifs from already melodic material

### Key controls relevant to melodic use

- **Audio In / Audio Out**
  - Feed Slice any melodic audio: oscillator voice, sample playback, looped phrase, or full voice chain.
- **Clock In**
  - Sets the rhythmic base for all repeat divisions.
  - Works from **10 BPM to audio rate**, which is very important: at slower rates you get musical rhythmic repeats; at faster rates you can enter more tone-like or timbral territory.
- **Trig Gate In / Trig Button**
  - Activates the repeat effect.
  - Threshold: **0.4V**
  - Can operate in:
    - **Latching mode**: repeat stays on after trigger until toggled off
    - **Momentary mode**: repeat is active only while gate is high
- **Size Knob**
  - Sets repeat length relative to the clock.
  - Range includes:
    - 2 bars
    - 1 bar
    - 1/2
    - 1/4
    - 1/4 triplet
    - 1/8
    - 1/8 triplet
    - 1/16
    - 1/16 triplet
    - 1/32
    - 1/64
    - 1/128
    - 1/256
- **Triplet Toggle**
  - Includes/removes triplet divisions from the available size range.
- **Size CV**
  - CV control over repeat size
  - Range: **-5V to +5V**

## How Slice contributes to melody

Slice is best thought of as a **melodic transformer**, not a melody source. It works especially well in these roles:

### 1. Turning a simple phrase into a melodic hook
If you send a melodic line, arpeggio, bassline, or vocal phrase into Slice, it can isolate tiny rhythmic fragments and repeat them. This creates:

- repeated notes from a single transient
- syncopated melodic fragments
- “hook” moments from longer phrases
- fills that sound intentional and compositional

A plain 4-note line can become much more interesting if Slice grabs a short segment at the end of every bar.

### 2. Creating apparent pitch shifts with very short slices
When repeat times get extremely short, repeated audio can begin to sound **pitched** or “resonant,” especially with harmonically rich material. This can create:

- metallic tuned blips
- buzzy pseudo-oscillator tones
- rising or falling glitch tones when modulating Size
- melodic percussion from non-melodic material

This is especially strong when the incoming audio has clear harmonic content, such as:
- saw or square oscillator voices
- vocal samples
- plucked sounds
- drum hits with tone

### 3. Producing rhythmic melody from non-melodic audio
If you feed drums or noise bursts into Slice and clock it tightly, short repeated sections can create tonal-feeling motifs. With careful timing, this becomes a kind of **percussive melody** or **pitched glitch lead**.

---

# Pairing ideas from the manual

The manual explicitly recommends pairing Slice with:

- **2hp Rnd**
- **2hp Play**
- **2hp Drum Machine**
- **2hp Loop**

Below is how each pairing can help generate melodic components.

---

## 1. Slice + Play: strongest melodic pairing

The manual specifically mentions **Play** as a sampler companion and suggests multing modulation to **Slice Size** and **Play pitch**.

### Why this is strong
Play already gives you sample-based tonal content:
- vocals
- chops
- melodic samples
- breakbeats
- instrument one-shots

Slice then rhythmically repeats sections of that audio, while Play can shift pitch. This combination can create:

- pitched vocal chops
- chopped sample melodies
- rising/falling glitch leads
- pitched call-and-response phrases

### Patch idea: linked pitch and slice length
The manual suggests:
- mult one CV source to:
  - **Slice Size CV**
  - **Play pitch**

### Musical result
- **longer slices = lower pitch**
- **shorter slices = higher pitch**

This creates a natural-feeling mapping where:
- slower, longer repeats feel deeper and more stable
- shorter, faster repeats feel brighter and higher

That can produce very expressive melodic movement from even a single sample.

### Example patch
- Play output → Slice audio input
- Master clock → Slice clock input
- Gate pattern → Slice trig input
- Sequenced or random CV multed to:
  - Play pitch
  - Slice Size CV

### Result
A sampled phrase becomes a playable melodic-glanular instrument. You can get:
- rhythmic riffs
- pitch-synced glitch fills
- evolving top lines

---

## 2. Slice + Loop: building melodic loops from repeats

The manual highlights using Loop with Slice to:
- capture beat repeats
- pitch them up/down
- reverse them
- use Frippertronics-style looping

### Why this matters melodically
Slice produces short repeat gestures; Loop can **freeze and preserve** those moments. Once captured, they become reusable melodic material.

### Musical uses
- capture a particularly good Slice repeat and turn it into a looped melodic phrase
- pitch the loop for harmonic movement
- reverse the captured repeat for a contrasting melody
- layer a stable loop underneath live Slice improvisation

### Patch workflow
- Melodic source → Slice
- Slice out → Loop in
- Trigger Slice for interesting fragments
- Record the best moments in Loop
- Repitch or reverse the loop

### Result
This turns transient glitch moments into:
- repeatable hooks
- atmospheric pitched textures
- melodic beds
- transitional FX that still feel harmonic

This is one of the best ways to use Slice in a song structure, because it lets you move from improvisation to fixed musical phrases.

---

## 3. Slice + Rnd: generative melodic variation

The manual recommends **Rnd** for both clocking and modulating Slice.

### Why this helps
Rnd can provide:
- clock-synced gates
- clock-synced CV

That means Slice can receive:
- regular or semi-random triggers
- moving Size CV
- variation synchronized to tempo

### Melodic potential
Rnd doesn’t directly create tonal pitch unless routed elsewhere too, but paired with a melodic source it can create:
- generative phrase slicing
- changing subdivisions that form melodic motifs
- evolving glitch arpeggios from static audio
- randomized fill behavior

### Good melodic strategy
Use Rnd to modulate **both**:
- Slice Size CV
- the pitch of your source voice or sampler

This creates correlation between:
- where the phrase is sliced
- what pitch the phrase is playing

### Result
You get semi-composed generative melodies that feel related rather than chaotic.

---

## 4. Slice + Drum Machine: percussive melody and fills

The manual frames this pairing mostly around drum fills, hi-hat triplets, and repeat rises. That sounds rhythmic rather than melodic, but in practice it can be very melodic too.

### How drums become melodic
If the Drum Machine includes tuned percussion, toms, tonal hats, or resonant sounds, Slice can:
- isolate short tonal drum segments
- create pitched-sounding rolls
- make ratcheting fills that imply melody
- turn a groove into a hook through repetition

### Best uses
- repeat just the tail of a tonal snare/clap
- create triplet hat bursts that interact with a bassline
- use short slice values for rising “laser” fills

### Result
You may not get conventional note-sequence melody, but you get **melodic percussion**, which is often what makes electronic arrangements feel alive.

---

# Best practical melodic patch strategies

## A. Chopped lead line
Use Slice after a complete melodic voice.

**Patch:**
- Oscillator + VCA + filter + envelope voice → Slice in
- Clock → Slice clock
- Gate sequence for fills → Slice trig
- Modulation → Slice Size CV

**What happens:**
Slice creates repeating fragments of your lead only at selected moments, adding hooks and phrase accents.

**Best for:**
- techno leads
- IDM stutters
- glitch-pop vocals
- bassline fills

---

## B. Vocal/sample melody instrument
Use Play into Slice.

**Patch:**
- Play out → Slice in
- Main clock → Slice clock
- Random or sequenced gate → Slice trig
- Shared CV → Play pitch + Slice Size CV

**What happens:**
A single sample becomes an animated melodic instrument.

**Best for:**
- vocal chops
- sample house
- hyperpop-style glitches
- breakbeat edits

---

## C. Granular pseudo-oscillator
Drive Slice with harmonically rich sustained audio and use very short repeat sizes.

**Patch:**
- Sustained oscillator drone or sample → Slice in
- Fast clock → Slice clock
- Gate held high or latching mode engaged
- Manually scan Size

**What happens:**
At short divisions, the repeated micro-segment can produce tuned or quasi-tuned textures.

**Best for:**
- glitch leads
- metallic pads
- artificial plucks
- experimental melodies

---

## D. Capture-and-compose method
Use Slice for discovery and Loop for arrangement.

**Patch:**
- Melodic source → Slice → Loop
- Trigger Slice manually or with sequencer
- Record appealing fragments into Loop
- Repitch/reverse the loop

**What happens:**
Improvised glitch events become stable compositional elements.

**Best for:**
- building hooks
- turning accidents into motifs
- live performance resampling
- ambient/glitch composition

---

# Important performance behaviors

## Latching vs momentary gate mode

This matters a lot for melodic phrasing.

### Latching mode
- One trigger turns Slice on
- Next trigger turns it off

**Use for:**
- sustained chopped passages
- turning a whole phrase into a repeated texture
- performance toggling between clean and glitched sections

### Momentary mode
- Slice is active only while gate stays high

**Use for:**
- short fills
- ratchets
- transient note repeats
- precise rhythmic punctuation

To change modes:
- **hold the Trig button while powering up the module**

For melodic work, **momentary mode** is usually better for tight phrase control, while **latching mode** is better for dramatic section changes.

---

# Triplets and melodic feel

The **Triplet toggle** is deceptively powerful for melody.

### With triplets enabled
You get:
- swing-like subdivisions
- polyrhythmic melodic stutters
- more expressive fills
- less rigid machine-grid phrasing

### With triplets disabled
You get:
- cleaner binary divisions
- more techno/electro precision
- easier synchronization with straight sequenced melodies

For melodic variation, turning triplets on can make a static phrase feel much more human or “musical.”

---

# Clocking considerations for melodic results

Since Slice is clock-dependent, the clock choice strongly affects how melodic it feels.

## Slow clock
- broader rhythmic repeats
- phrase-level looping
- musical and recognizable motifs

## Medium clock
- ratchets and note subdivisions
- sequence embellishment
- arpeggio-style rhythmic chopping

## Very fast clock
- timbral/pitch-like artifacts
- granular textures
- buzzy melodic effects

If your goal is **recognizable melody**, stay in slower to medium divisions. If your goal is **pitched glitch texture**, use faster clocks and tiny slice sizes.

---

# Limitations to understand

Slice is not:
- a quantizer
- a traditional pitch sequencer
- a V/Oct oscillator
- a harmonic processor

So it does not generate conventional note melodies by itself.

Instead, it excels at:
- **reframing existing melodic material**
- **extracting motifs**
- **creating rhythmic pitch illusions**
- **adding expressive glitch phrasing**
- **transforming samples or loops into melodic texture**

That makes it especially useful in systems where you already have:
- a sampler
- a looper
- a melodic voice
- a random CV source
- a sequencer

---

# Best overall “melodic system” from this manual

If using only the module relationships shown in the manual, the strongest melodic chain is:

**Play → Slice → Loop**

with **Rnd** providing modulation and timing.

### Why this works
- **Play** provides pitched/sample content
- **Slice** creates rhythmic micro-repetition and glitch phrasing
- **Loop** captures and transforms the best moments
- **Rnd** adds evolving movement

### This system can produce
- vocal chop melodies
- evolving sample leads
- repeated micro-hooks
- pitched glitch textures
- looped ambient melodic fragments
- generative top lines

---

# Summary

## Most melodic use cases for Slice
1. **As a stutter effect on an existing melodic voice**
2. **As a sample-chopper with Play**
3. **As a glitch phrase generator captured by Loop**
4. **As a pseudo-pitched texture device with short repeat sizes**
5. **As a rhythm-to-melody transformer using synced CV from Rnd**

## Best pairings from the manual for melody
- **Play**: best for direct melodic/sample work
- **Loop**: best for capturing and reusing melodic fragments
- **Rnd**: best for generative variation
- **Drum Machine**: best for melodic percussion and fills

If you want, I can also turn this into:
- a **set of concrete patch recipes**
- a **beginner/intermediate/advanced usage guide**
- or a **“best melodic patches for 2hp Slice” cheat sheet**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)