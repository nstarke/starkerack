# Klavis — Grainity VCF

- [Manual PDF](../../manuals/Klavis_-_Grainity_User_Manual.pdf)

---

[Manual PDF](attachment)

# Klavis Grainity — using it to create melodic components in a Eurorack system

The **Klavis Grainity** is not just a filter. It’s really a **dual-path melodic spectral processor**:

- one side is a fairly standard **multimode analog VCF**
- the other is a **granular-style analog filter engine** whose filter state is stepped by the detected cycle of an input signal or by an external trigger/audio source

That makes it unusually good for generating **pitched overtones, subharmonics, interval relationships, chord-like layers, pseudo-sequenced filter motion, and harmonically related movement** from a simple oscillator line.

## What the module does best for melody

From a musician’s perspective, Grainity excels at turning a plain melodic source into:

- **tracked filter melodies**
- **harmonic doubles above the played note**
- **sub-octave / subharmonic reinforcement**
- **triad-like textures from one oscillator**
- **moving formant and flanging timbres that still follow pitch**
- **rhythmic melodic patterns tied to pitch or external clocks**
- **parallel voices** via its three outputs:
  - **M.VCF out**
  - **G.VCF out**
  - **Mix out**

Because both filters share the same **cutoff** and **resonance** controls, you can keep both paths musically related while using the granular side to introduce extra interval content.

---

## Core idea: how Grainity becomes melodic

The manual makes clear that the granular engine is stepped by:

- the **zero-crossings** of the input audio, or
- the **Detect** input instead

Then the module applies:

- a chosen **Structure** (predefined looping filter/phase pattern)
- optional **Track** retuning
- optional **Phase** offset
- optional **Division**

This matters musically because it means the granular section can behave like a **pitch-related pattern generator**, except it’s modifying filter states rather than outputting raw oscillator pitch.

### The most melodic controls are:

#### 1. **V/Oct input**
This applies to the shared cutoff of both filter sections.  
Use it with the same pitch CV as your oscillator to make the filter behavior follow the note line.

Best use:
- send your sequencer/keyboard pitch CV to both:
  - your VCO
  - Grainity **V/Oct**

That keeps the filtering and resonance behavior musically aligned with the note being played.

---

#### 2. **Track mode**
This is one of the most important melodic features.

When **Track** is enabled, Grainity detects the input pitch and retunes the granular cycling from **unison up to slightly above an octave**. The manual describes this as a kind of **virtual VCO for control only**.

Musically, this lets you create:

- **unison reinforcement**
- **fifths**
- **third-ish or sixth-ish harmonic relationships**
- **octave doubling**
- subtle **detuned melodic thickening**

A key example from the manual:
- if the incoming note is C
- and Track retunes the cycling toward G
- the granular filter cycles in a **3:2 relationship**

That’s huge for melody writing because it means one monophonic line can produce a musically related second layer.

---

#### 3. **Structure**
Structures are looping filter-state patterns of length:

- 2
- 3
- 4
- 5
- 6
- 8
- plus random structures

Longer structures tend to produce:
- more **subharmonics**
- deeper **sub-octave implications**
- more complex internal harmonic motion

Shorter structures tend to feel:
- more stable
- more intervallic
- easier to tune into melodic contexts

For melody:
- start with **2-step** and **3-step** structures
- then move to **4-step** and **5-step** if you want richer harmonic motion
- use **8-step** with external triggering for pattern-like melodic filtering

---

#### 4. **Division**
Division repeats each step before moving to the next.

Values shown by the display map to:
- 1, 2, 3, 4, 5, 8, 16, 32, 64, 128

This is extremely useful melodically.

Small divisions:
- create additional harmonic layers
- work especially well with **Track**
- can help form **3-note chord-like results from a single VCO**, per the manual

Large divisions:
- create **slow evolving rhythmic pitch-related filter patterns**
- especially when the source is pitched audio or when Detect is externally clocked

---

#### 5. **Phase / Frq control**
With **Track off**, this is **Phase**
- creates subtle tonal shifts
- flanging / phasing
- unison-like motion when modulated

With **Track on**, this becomes **Frq**
- retunes the granular cycling musically
- this is where you dial in interval relationships

For melodic work:
- with Track on, this is your **interval/harmony knob**
- with Track off and CV applied, this is your **animated doubling / chorus voice knob**

---

## Best melodic patch roles

## 1. Monophonic line enhancer

### Patch
- VCO saw or pulse -> **Input**
- Sequencer pitch CV -> VCO 1V/Oct and Grainity **V/Oct**
- **G.VCF out** or **Mix out** -> VCA -> output
- Enable **Track**
- Try a short **2-step or 3-step Structure**
- Low to medium **Division**
- Medium resonance

### Result
A lead or bassline gains:
- harmonically related extra content
- vocal/formant movement
- pseudo-interval doubling

This is probably the most immediate “melodic” use of the module.

---

## 2. One oscillator into a chord-like voice

The manual explicitly says careful use of **Track + Division** can create **3-note chords from a single VCO**.

### Patch
- Single VCO triangle/saw -> **Input**
- Same pitch CV -> VCO and Grainity **V/Oct**
- Enable **Track**
- Sweep **Frq**
- Try **Division 2, 3, 4, or 5**
- Try **3-step, 4-step, and 5-step Structures**
- Use **Mix out**
- Set M.VCF to **IN**, **LP2**, or **BP** depending on how much raw oscillator you want

### Why it works
You hear:
- the original tone or filtered original from M.VCF
- plus the harmonically offset granular component from G.VCF

This creates the perception of:
- root + interval + coloration
- or root + upper harmony + sub component

### Musical use
Great for:
- monophonic acid lines that imply chords
- modal drones
- arpeggios that sound fuller without multiple oscillators
- pseudo-polyphonic hooks

---

## 3. Bassline with subharmonic reinforcement

Longer structures generate stronger subharmonic behavior.

### Patch
- VCO square/saw -> **Input**
- Pitch CV to VCO and Grainity **V/Oct**
- Try **4-step, 5-step, or 6-step** structures
- Moderate resonance
- Track on or off depending on desired tightness
- Lower cutoff to emphasize low spectral motion
- Mix in some M.VCF lowpass output

### Result
The bassline becomes:
- thicker
- more vocal
- richer in implied lower tones
- more animated than a normal filter sweep

This is especially effective when the source octave is played a little higher, as the manual suggests for longer structures.

---

## 4. Parallel lead voice using the two outputs

Grainity really wants to be treated as a **dual voice shaper**.

### Patch
- VCO -> **Input**
- Pitch CV -> VCO + Grainity **V/Oct**
- **M.VCF out** to left mixer channel
- **G.VCF out** to right mixer channel
- Use different VCAs, envelopes, effects, or panning for each

### Result
You get:
- one more conventional filtered voice
- one more radical harmonically transformed voice

This can create:
- stereo melodic width
- call-and-response inside one patch
- a lead plus “ghost harmony”
- a dry/focused tone paired with an unstable overtone voice

The manual even notes that sometimes G.VCF can sound sufficiently unrelated to the source that the two outputs can be treated almost like independent channels.

---

## 5. Externally imposed melodic filtering with Detect

The **Detect** input is where Grainity becomes compositionally powerful.

It lets one signal define the granular stepping while another signal is being filtered.

That means you can separate:
- **what is heard**
from
- **what controls the melodic stepping**

### Patch concept
- Complex audio, chord, noise, percussion, or mixed voice -> **Input**
- Simple VCO or other pitch source -> **Detect**

### Melodic result
The heard sound inherits motion from the Detect source’s cycle pattern.

This is ideal for:
- imposing a melody onto a non-melodic source
- making chords behave more predictably
- deriving lead tones from noisy content
- turning drums into pitched rhythmic textures

---

## 6. Chord processing where one note guides harmony

The manual gives a direct recipe:
- feed the full chord to **Input**
- send one note, usually the **lowest voice**, to **Detect**

### Why this is musically useful
A full chord has too many zero-crossings and can make the granular section chaotic.  
Using one note on Detect makes the stepping stable and harmonically meaningful.

### Patch
- Three VCO chord mix -> **Input**
- Lowest note’s VCO -> **Detect**
- Shared pitch source for musical coherence
- G.VCF out or Mix out to VCA

### Result
You preserve chord richness while making the granular engine track a specific harmonic anchor.

This is excellent for:
- pads
- chord stabs
- melodic techno chord loops
- filtered organ-like riffs

---

## 7. Rhythmic melodic sequences from Detect triggers

Detect also accepts triggers, gates, LFOs, and audio.

This lets you step structures at **sub-audio rates**, making Grainity act like a **timbral sequence generator**.

### Patch
- Sustained oscillator or drone -> **Input**
- Clock / trigger sequence -> **Detect**
- Structure: **4-step, 5-step, 6-step, or 8-step**
- Division: low values first
- V/Oct tracking from your pitch source
- Track usually off unless experimenting

### Result
Each trigger advances the granular filter structure, creating:
- repeating melodic timbre phrases
- pseudo-arpeggiation
- rhythmic tonal accents
- sequence-like formant patterns

If the input is a sustained pitched note, this can sound like a **melodic sequence without changing oscillator pitch**.

That’s very useful for:
- sequenced drones
- Berlin-school style movement
- gated pad figures
- evolving ostinatos

---

## 8. Use M.VCF “IN” mode to blend dry pitch with granular harmony

The multimode side has an **IN** option that passes the unaltered input.  
The manual specifically notes this can be useful mixed with G.VCF.

### Why this matters for melody
One of the easiest ways to keep the result musical is to retain a stable pitch center.

### Patch
- Oscillator -> Input
- M.VCF set to **IN**
- Mix toward center
- G.VCF supplying the movement/harmonic complexity
- Modulate Mix CV for changing emphasis

### Result
You get:
- stable root definition from the dry input
- animated overtone and interval content from G.VCF

This is one of the best patches for:
- hooks
- basslines
- melodic arps
- anything where you want “weird” but still clearly pitched

---

## 9. Animate melodic notes with Phase modulation

With **Track off**, the Φ/Frq control becomes **Phase**.

The manual describes this as producing:
- subtle tonal variation
- phasing/flanging
- unison-like effects when CV modulated

### Patch
- Melodic oscillator -> Input
- Slow LFO / random slew / vector modulation -> Φ/Frq CV
- Track off
- Use a stable short structure
- Mix some M.VCF with G.VCF

### Result
Your melody becomes:
- wider
- chorus-like
- gently detuned
- more animated without losing pitch identity

This is a strong patch for:
- lead lines
- pads
- melodic plucks
- synth-pop style chorus movement

The manual specifically recommends irregular evolving signals for chorus-like results.

---

## 10. Create “melody from percussion”

This is unusual but musically interesting.

The manual suggests two ways:

### A. Use a VCO on Detect
- Percussion -> Input
- Tuned VCO -> Detect

Now the percussive sound takes on pitched granular stepping, which can produce a melodic impression.

### B. Use the drum trigger on Detect
- Percussion audio -> Input
- Drum trigger/gate -> Detect

Now the structure changes once per drum hit.

### Musical applications
- tuned percussion lines
- melodic hats
- bass drum harmonic accents
- hybrid drum+melody parts in techno/IDM

---

## 11. Mixed music or loops as melodic material

The manual suggests extracting rhythmic events from a full mix and feeding those to Detect.

In a modular music-making context, this translates well to:
- drum loops
- stems
- resampled phrases

### Patch
- Loop or mix -> Input
- Filtered band / comparator / gate extractor -> Detect

### Result
The granular filter stepping can lock to prominent features in the loop, creating:
- musically reactive filtering
- pitch-related rhythmic melody artifacts
- loop-derived harmonic motion

This is more experimental, but very powerful.

---

# How to think about the three outputs musically

## 1. **M.VCF out**
Use for:
- the stable melodic anchor
- traditional subtractive filtering
- dry or semi-dry pitch reference
- second voice in stereo

Best modes for melody:
- **LP2** for gentle shaping
- **LP4** for focused bass/lead control
- **BP** for vocal mids
- **IN** for preserving pitch center while blending G.VCF

---

## 2. **G.VCF out**
Use for:
- harmonic transformations
- pseudo-chords
- subharmonic bass enrichment
- flanged or formant melodic lines
- aggressive timbral melody

This is usually the “character” output.

---

## 3. **Mix out**
Use for:
- immediately playable melodic sounds
- balancing clarity and complexity
- CV morphing between stable and unstable voices

This is the most performance-friendly output.

---

# Best practical melodic patches

## Patch 1: Harmonic lead from one oscillator
- Saw VCO -> Input
- Pitch CV -> VCO and Grainity V/Oct
- Track on
- Structure 2A, 2b, 3A, or 3b to start
- Division 1 or 2
- M.VCF = IN or LP2
- Mix around noon to 2 o’clock toward G.VCF

**Sound:** lead with interval color and extra vocal edge.

---

## Patch 2: Chord-implying bass
- Square VCO -> Input
- Pitch CV -> VCO and V/Oct
- Track on
- Structure 4A–4F or 5A–5d
- Division 2–4
- M.VCF LP4
- Moderate resonance

**Sound:** monophonic bass that implies stacked harmony.

---

## Patch 3: Sequenced timbre melody
- Sustained oscillator/drone -> Input
- Trigger sequencer -> Detect
- Structure 8A–8F
- Division 1
- Track off
- Modulate cutoff via envelope or slow CV

**Sound:** rhythmic melodic phrase from filter-state sequencing rather than note changes.

---

## Patch 4: Chord stabilizer
- Mixed 3-VCO chord -> Input
- Lowest VCO -> Detect
- Pitch CV shared
- Track on
- Structure 3-step or 4-step
- Blend M.VCF and G.VCF

**Sound:** rich chord with controlled harmonic animation instead of chaos.

---

## Patch 5: Chorus lead
- VCO -> Input
- Track off
- Slow random or slewed S&H -> Φ/Frq CV
- Structure all-pass or short low-pass family
- M.VCF + G.VCF mixed

**Sound:** pitch-stable melody with animated ensemble feel.

---

# Recommended workflow for writing melodic parts

## Start simple
Use:
- one clean VCO
- short structures
- low division
- Track on
- M.VCF set to IN or LP2

This gives you a strong reference point.

## Then add complexity in this order
1. adjust **Frq/Track** for interval feel
2. change **Structure**
3. increase **Division**
4. add **Phase/Frq CV**
5. introduce external **Detect**
6. separate **M.VCF** and **G.VCF** into different channels

That progression helps keep the patch musical instead of immediately chaotic.

---

# Best pairings with other module types

Even though only Grainity is present here, these are the module partners it most obviously wants for melodic work:

## With a VCO
Essential. Grainity shines with:
- saw
- pulse
- triangle
- sync tones
- additive or complex waves

Simple wave to Detect, complex wave to Input is directly recommended in the manual.

## With a sequencer
Needed for:
- pitch CV to VCO and Grainity V/Oct
- trigger patterns to Detect
- modulation lanes to Struct / Div / Mix / Φ/Frq

## With a mixer or mult
Very useful for:
- splitting one VCO to Input and Detect
- mixing chords to Input while sending one voice to Detect
- blending M.VCF and G.VCF externally

## With modulation
LFOs, random, envelopes are great on:
- Mix CV
- Struct CV
- Div CV
- Φ/Frq CV
- FM
- Q CV

## With VCAs
Important if you want the two outputs to behave as two separate melodic voices.

---

# Performance tips

## 1. Use Mix as a macro control
Because Mix crossfades between conventional and granular filter voices, it’s a powerful live performance control for bringing in harmonic complexity.

## 2. Keep M.VCF as a pitch anchor
If the G.VCF becomes too abstract, keep some dry or lightly filtered signal in the mix.

## 3. Track + low division is the sweet spot
For clearly melodic use, this is often where the best interval-like results live.

## 4. Use longer structures for bass and drones
These are better for subharmonic or evolving textures than for precise fast melodies.

## 5. Detect is the secret weapon
Whenever the input is too busy:
- use a simpler correlated source on Detect

That turns Grainity from chaotic to compositionally useful.

---

# Summary

The **Klavis Grainity** is best understood as a **melodic harmonic filter instrument**, not merely a special-effect VCF.

It can be used to create melodic components by:

- tracking incoming pitch with **V/Oct**
- generating harmonic relationships using **Track**
- building interval and chord-like textures using **Structure + Division**
- separating control from sound using **Detect**
- blending stable and transformed tones with **M.VCF / G.VCF / Mix**
- creating pseudo-sequences from trigger-driven structure stepping
- adding chorus, formant, and subharmonic motion to otherwise plain melodic lines

If I were using it in a patch, I’d treat it as a way to get **more melody out of less source material**:
- one oscillator becomes a layered lead
- one bassline becomes harmonically richer
- one chord becomes animated but controlled
- one drone becomes a sequence

That is where Grainity seems most musically valuable.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)