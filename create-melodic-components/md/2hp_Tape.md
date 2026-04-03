# 2hp — Tape

- [Manual PDF](../../manuals/2hp_Tape_Stop.pdf)

---

[Manual PDF – 2hp Tape Stop](https://www.twohp.com/modules/tape-stop)

# Using 2hp Tape Stop to Create Melodic Components

The attached manual is for the **2hp Tape Stop**, a **clock-synced tape-stop effect**. By itself, Tape Stop is not a pitch generator or oscillator, but it can still play a strong role in making **melodic material feel more expressive, rhythmic, and compositionally useful**. The manual also suggests pairings with **Lo-Fi, Play, Loop, and VCA**, and those combinations are especially relevant for melodic work.

## What Tape Stop does musically

Tape Stop simulates the classic effect of audio slowing down like a tape machine being stopped. In melodic patches, that means it can:

- create **pitch-fall endings**
- produce **phrase transitions**
- add **rhythmic pitch bends** when synced to clock
- turn static melodic lines into something more performative
- create **call-and-response textures** between dry and affected signals

Key features from the manual:

- **Audio input/output** for processing melodic audio
- **Clock input** to sync the stop time to your patch clock
- **Trig button/gate input** to activate the effect
- **Lag knob/CV** to control stop duration
- **Momentary or latching trigger modes**
- **50/50 boot mode** so dry signal remains audible alongside the effect

---

## Important musical behavior

### 1. Tape Stop works best on already-pitched material
Since this module processes incoming audio, the melodic source usually comes from somewhere else, such as:

- a sampled phrase
- a loop
- a bassline
- a lead voice
- a chord stab
- a sequenced melodic recording

So the melodic role here is less “generate notes” and more “reshape and animate notes.”

### 2. Clock sync makes pitch drops compositional
The manual says that when clocked externally, the **Lag** parameter steps through note values:

- Instant
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

That is very useful for melody because the slowdown can be aligned to phrase lengths. For example:

- a short 16th-note drop creates a glitchy melodic ornament
- a quarter-note drop creates a strong phrase accent
- a 1-bar or 2-bar drop creates a dramatic melodic ending

### 3. CV over Lag makes the effect performable
With **Lag CV (-5V to +5V)**, you can modulate how long the slowdown lasts. That allows:

- different phrase endings per bar
- alternating short and long tape drops
- evolving melodic transitions
- expressive fills triggered by CV sequencing

---

# Best module combinations from the manual

## 1. Tape Stop + Play
This is probably the most directly melodic pairing in the manual.

The manual says:

> “Stop samples with style by throwing Play before Tape Stop in the signal chain.”

### Why it works
**2hp Play** can provide pitched or melodic sample material, while **Tape Stop** adds expressive pitch-fall articulation to it.

### Melodic uses
- Trigger melodic one-shots and stop them mid-phrase
- Process vocal or instrumental stabs for descending ends
- Make repeated notes feel less mechanical
- Add “turntable stop” style transitions between melodic sections

### Patch idea
- **Play OUT → Tape Stop IN**
- Master clock → **Tape Stop CLOCK**
- Trigger pattern → **Play TRIG**
- Another gate source → **Tape Stop TRIG**

Now you can:
- trigger a melodic sample on the beat
- selectively tape-stop only some notes or phrase endings
- synchronize the stop duration to the groove

### Musical result
This is great for:
- hip-hop style beat transitions
- synth-pop fills
- lo-fi melodic warbles
- modern glitch melody accents

---

## 2. Tape Stop + Loop
This is one of the strongest pairings for building melodic structure.

The manual says **Loop** works well either before or after Tape Stop.

## Option A: Loop before Tape Stop
**Loop OUT → Tape Stop IN**

### Why this is useful
You record a melodic phrase into **Loop**, then use **Tape Stop** to process the playback.

### Musical applications
- end a looped melody with a synced pitch slowdown
- create degraded repeated phrases
- turn a stable repeating melody into something more performative
- create breakdowns by slowing a whole looped phrase

### Patch example
- Record a lead line or arpeggio into Loop
- Send Loop output to Tape Stop
- Clock Tape Stop from your master rhythm
- Trigger Tape Stop at the end of every 4 or 8 bars

### Result
Your melody remains recognizable, but gains long-form phrasing and transitions.

## Option B: Tape Stop before Loop
**Melodic source → Tape Stop → Loop**

### Why this is useful
Now you record the tape-stop gesture itself into Loop.

### Musical applications
- capture expressive slowdowns as part of the phrase
- chop and replay warped melodic material
- build a loop made from decelerated fragments
- create unusual pseudo-granular melodic textures

### Result
Instead of merely affecting a melody, you create a **new melodic sample language** based on slowed pitch gestures.

---

## 3. Tape Stop + Lo-Fi
The manual recommends Lo-Fi for adding wow, flutter, hiss, pops, and analog character.

### Why it matters melodically
Melodies often sound more emotionally compelling when they have instability and texture. Tape Stop already bends pitch downward; **Lo-Fi** adds small pitch instability and noise around it.

### Musical applications
- nostalgic lead lines
- degraded sampled keys
- broken cassette-style motifs
- dreamy melodic fragments

### Patch idea
- Melodic source → **Lo-Fi → Tape Stop**
- Use Lo-Fi for subtle wow/flutter
- Trigger Tape Stop only at phrase endings

### Result
The pitch material feels like it comes from old media rather than a clean digital source.

This is especially strong for:
- ambient
- vaporwave
- trip-hop
- cinematic interludes
- lo-fi house

---

## 4. Tape Stop + VCA
This pairing is about **mix control**, but that directly affects melody presentation.

The manual notes that if you want more control than the 50/50 mode, you can mult dry and wet signals into a **dual VCA**.

### Why this helps melodically
Mixing dry and wet versions lets you preserve pitch clarity while adding expressive falling pitch behind or around it.

### Melodic applications
- keep the original note audible while the stop effect trails downward
- fade between clean melody and warped melody
- emphasize only the ends of phrases
- create layered interval-like smears as dry and wet overlap

### Patch idea
- Mult melodic source
- One copy goes direct to VCA channel 1
- One copy goes to Tape Stop, then to VCA channel 2
- Mix the two channels

### Result
You can sculpt exactly how “melodic” versus “effected” the line feels.

This is much more useful than a simple insert effect if your goal is to keep strong pitch identity.

---

# Concrete melodic patch strategies

## 1. Phrase-ending tape falls
Use Tape Stop at the end of every melodic phrase.

### Patch
- Sequenced melodic voice or sample player into Tape Stop
- Clock into Tape Stop CLOCK
- Trigger Tape Stop only on the last note of a 4-bar phrase
- Set Lag to quarter, half, or whole note

### Effect
This creates a clear melodic punctuation, like a singer trailing off or a reel slowing down.

---

## 2. Ornament selected notes
Use short synced lag values like 32nd or 16th.

### Patch
- Fast melodic sequence into Tape Stop
- Trigger only occasional notes
- Keep Lag short

### Effect
Certain notes become pitch-dipping ornaments, similar to expressive bends or vinyl drag effects.

This works especially well on:
- arpeggios
- plucks
- repeated ostinatos

---

## 3. Build breakdowns from melodic loops
Use Loop and Tape Stop together for arrangement.

### Patch
- Record a melody into Loop
- Send Loop to Tape Stop
- Trigger Tape Stop for 1 or 2 bars before a section change

### Effect
The melody itself becomes the transition device into the next section.

---

## 4. Dry/wet counterpoint with 50/50 mode
The manual says holding **Trig during boot** enables **50/50 Mode**, so you hear dry signal while tape stopping.

### Why this matters musically
This creates a layered effect where:
- one version keeps pitch identity
- one version falls away

That can sound like:
- harmonized smearing
- decaying unison doubling
- ghosted melodic shadowing

For melodic content, this is one of the most useful hidden features in the manual.

---

## 5. Voltage-controlled phrase variation
Use CV into **Lag CV**.

### Patch concept
Send a slow modulation or stepped CV to Lag CV while using a regular trigger pattern.

### Effect
Each tape stop lasts a different rhythmic amount, which can make melodic phrases feel more alive and less repetitive.

If the CV source is sequenced, you can effectively “compose” different slowdown durations per phrase.

---

# Performance considerations

## Momentary vs Latching
The manual’s **Trig Toggle** changes behavior:

- **Momentary (down):** effect lasts while held/gated
- **Latching (up):** press once to start, again to stop

### For melody
- **Momentary** is better for tight rhythmic punctuation
- **Latching** is better for long breakdowns, drones, and gradual phrase collapse

---

## External clock is key for musical integration
Because the slowdown durations quantize to clock-related values, Tape Stop becomes much more compositionally useful when synced.

For melodic music, that means:
- phrase endings stay in time
- transitions feel intentional
- repeated tape gestures become part of the groove rather than random FX

---

# What each manual pairing contributes to melodic writing

## Lo-Fi
Adds unstable analog character to melodies before or after slowdown.

## Play
Supplies melodic samples or phrases that Tape Stop can reshape.

## Loop
Captures and repeats melodies, then allows Tape Stop to transform them structurally.

## VCA
Lets you blend clear pitch information with warped pitch tails for more controllable melodic presentation.

---

# Best overall melodic workflows

## Workflow 1: Sample-based melody
**Play → Tape Stop**

Use this when you want:
- triggered melodic snippets
- phrase punctuation
- stylized stop effects on leads or vocals

## Workflow 2: Loop-based phrase design
**Loop → Tape Stop**

Use this when you want:
- evolving repeated phrases
- arrangement transitions
- loop breakdown effects

## Workflow 3: Textured melody design
**Lo-Fi → Tape Stop**

Use this when you want:
- vintage melodic character
- unstable tape-like leads
- nostalgic pitch-drifting motifs

## Workflow 4: Controlled parallel melody/effect blend
**Mult source → dry path + Tape Stop wet path → VCA**

Use this when you want:
- precise wet/dry balance
- preserved melodic intelligibility
- more nuanced expressive effects

---

# Bottom line

The **2hp Tape Stop** is not a melody generator, but it is very effective as a **melodic articulation and phrase-shaping tool**. It works best when paired with a module that already contains or records pitched material:

- **Play** for melodic samples
- **Loop** for repeated melodic phrases
- **Lo-Fi** for tape-like color
- **VCA** for shaping the relationship between the original melody and the slowed version

Used this way, Tape Stop can turn simple melodic content into something more expressive, transitional, nostalgic, and rhythmically alive.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)