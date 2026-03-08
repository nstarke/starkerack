# Tiptop Audio — SD909

- [Manual PDF](../../manuals/Tiptop_Audio_SD909_ns.pdf)

---

[Manual PDF](https://www.tiptopaudio.com/909-2)

# Tiptop Audio SD909: using it for melodic components

The SD909 is fundamentally a **TR-909 snare voice**, but the manual makes clear it contains several parts you can repurpose musically:

- **pitched internal VCOs** for the snare body
- **voltage-controllable tune**
- **voltage-controllable binary noise source**
- **separate noise output**
- **accent input** that can be driven by gates or CV for dynamics

That means it is not just a drum hit module — it can become a source for **pitched lines, tuned percussion melodies, noisy basslines, metallic riffs, and articulated sequenced parts**.

## What in the module is useful melodically

From the manual, the most important features for melodic use are:

- **TUNE knob + VC-TUNE input**
  - controls the pitch of the internal snare oscillators
  - lets you sequence pitch externally
- **NOISE knob + VC-NOISE input**
  - changes the clocking frequency of the TR-909 noise generator
  - at lower settings it becomes more metallic and reveals clock artifacts
  - this can create pitched-adjacent or tonal/noisy textures
- **NOISE OUT**
  - gives you the raw noise source separately
  - useful as an oscillator-like source for filtering, pinging, or shaping into melodic material
- **ACCENT IN**
  - accepts gate/trigger or CV
  - lets you dynamically shape each note
  - accent also changes the balance between the noise and the “kick” body of the snare, which is very musical
- **GATE IN / Trigger button**
  - for rhythmic note events
- **LEVEL**
  - useful for balancing with other voices in a patch

## Important sonic behavior from the manual

A few manual notes matter a lot if you want melody rather than just drum hits:

1. **Tune only affects the internal VCOs**
   - so your “pitched” material mainly comes from the snare body, not the noise burst.

2. **Tone and Snappy affect the noise section**
   - **Tone** = noise length
   - **Snappy** = noise gain
   - for more obvious pitch, reduce the dominance of noise and let the VCO body speak clearly.

3. **Accent is part of the sound design**
   - on this snare, accent does not just make things louder; it also affects the body/noise balance.
   - that means accent sequencing can create expressive melodic phrasing.

4. **Lowering noise frequency gets metallic**
   - the manual explicitly says clocking noise will appear and that this is normal.
   - this is excellent for tuned-industrial or electro melodic parts.

---

# Best ways to use SD909 melodically

## 1. Tuned percussion line

This is the most direct melodic use.

### Patch idea
- Sequencer pitch CV → **VC-TUNE**
- Trigger sequencer → **GATE IN**
- SD OUT → VCA / mixer
- Optional accent trigger/CV → **ACCENT IN**

### Settings
- **Snappy**: low to medium
- **Noise**: around or below the marked 909 region
- **Tone**: shorter to medium
- **Tune**: set to a comfortable central pitch
- **Accent**: medium

### Result
You get a line of **pitched snare-body hits** that behaves like:
- tom melody
- synth-percussion sequence
- electro bass plucks
- tuned clicky lead

### Musical use
- Program scales by sending stepped CV to VC-TUNE
- Keep triggers short and regular for x0x-style tonal percussion
- Use accent on selected steps for groove and phrase emphasis

Because this is a drum circuit, expect the pitch to be **characterful rather than precision-1V/oct melodic**. It works best for:
- modal riffs
- percussive bass motifs
- atonal or semi-tonal sequences
- techno/electro hooks

---

## 2. Snare-bass voice

The internal oscillators can be pushed toward **low, punchy body tones**.

### Patch idea
- Pitch CV → **VC-TUNE**
- Gate pattern → **GATE IN**
- Accent sequence → **ACCENT IN**
- SD OUT → lowpass filter → VCA → mixer

### Settings
- **Tune**: lower range
- **Snappy**: low
- **Noise**: lower than “classic snare” balance
- **Tone**: short
- **Accent**: adjusted for punch

### Result
This turns the SD909 into a kind of:
- dirty analog bass drum synth
- short bass stab
- electro sub-percussion line

Because the snare body contains pitched oscillators, reducing the noisy part lets those oscillators behave more like a crude synth voice.

### Good genres
- electro
- industrial
- minimal techno
- EBM
- broken beat

---

## 3. Metallic pseudo-melody using VC-NOISE

The manual says lowering the noise frequency makes the sound more metallic and reveals the clock. That is a gift for experimental melody.

### Patch idea
- Trigger sequence → **GATE IN**
- Slow or stepped CV → **VC-NOISE**
- Another CV row → **VC-TUNE**
- Accent sequence → **ACCENT IN**
- SD OUT → bandpass filter or resonant lowpass

### Settings
- **Noise**: lower than normal
- **Snappy**: medium to high
- **Tone**: medium
- **Tune**: moderate
- **Accent**: medium-high

### Result
You get:
- metallic tuned hits
- robotic bell-ish phrases
- crunchy digital-sounding riffs
- industrial “snare synth” melodies

This works especially well if:
- VC-TUNE moves in small intervals
- VC-NOISE moves more slowly
- accents define phrase boundaries

Think of VC-NOISE as a **timbre melody lane** alongside pitch melody.

---

## 4. Raw NOISE OUT as a melodic source

The manual notes that the **NOISE OUT** is the pure, unfiltered TR-909 binary noise source. On its own, that is not a conventional oscillator, but in modular it becomes extremely useful.

## A. Filtered-noise melody
### Patch
- **NOISE OUT** → resonant filter audio input
- Envelope → filter cutoff and/or VCA
- Trigger sequence → envelope generator
- CV → filter cutoff

### Result
If your filter resonates strongly, you can “tune” the filtered noise into:
- whistling notes
- breathy leads
- tuned percussion
- hi-tech hats that imply pitch

This is especially effective with:
- bandpass filters
- high resonance lowpass filters
- LPGs for plucky response

## B. Noise as source for sample & hold / random melody
### Patch
- **NOISE OUT** → sample & hold input
- Clock → sample & hold trigger
- S&H output → oscillator pitch / VC-TUNE / filter cutoff

### Result
The SD909 becomes a **random CV source** for melodic generation.

## C. Noise into wavefolder/distortion/filter bank
### Patch
- **NOISE OUT** → waveshaper/distortion/filter bank
- sequenced VC over the processor
- envelope/VCA after it

### Result
You can create:
- vowel-like phrases
- tuned industrial drones
- noisy leads

---

## 5. Accent as melodic articulation

The accent system is unusually useful. The manual explains:

- without a cable in ACCENT IN, gate is normalized to accent
- with a cable patched, accent becomes independently controllable
- higher accent settings increase the difference between accented and unaccented hits
- accent can be controlled with CV, not just gates

This means accent can function like **velocity** in a melodic phrase.

### Musical uses
- stronger accents on downbeats
- CV accent contours for crescendos
- alternating soft/hard notes for call-and-response
- phrase shaping where accented notes also brighten or rebalance the noise/body tone

Because accent affects timbre as well as level, it can make a 1-note pattern sound like a melodic phrase even before pitch changes.

---

# Practical melodic patch recipes

## Patch 1: Electro tuned snare riff
**Goal:** a 4–8 step percussive melody

- Sequencer gate → **GATE IN**
- Sequencer pitch CV → **VC-TUNE**
- Accent track → **ACCENT IN**
- SD OUT → mixer

**Knobs:**
- Tune: noon-ish
- Snappy: 9–10 o’clock
- Noise: near or slightly below 909 mark
- Tone: short-medium
- Accent: around 909 mark

**Why it works:**
Less noise gives the tuned body more focus. Accent adds groove and timbral changes.

---

## Patch 2: Industrial bell sequence
**Goal:** metallic tonal sequence

- Trigger pattern → **GATE IN**
- Stepped CV → **VC-NOISE**
- Quantized CV or small modulation → **VC-TUNE**
- SD OUT → resonant bandpass filter → delay

**Knobs:**
- Noise: lower
- Snappy: medium-high
- Tone: medium
- Tune: medium-high
- Accent: medium

**Why it works:**
The lowered noise clock introduces metallic texture while tune gives body. Delay emphasizes the pseudo-pitched quality.

---

## Patch 3: Bassline from the snare body
**Goal:** punchy bass/percussion line

- Sequencer CV → **VC-TUNE**
- Gate sequence → **GATE IN**
- SD OUT → lowpass filter → VCA
- Envelope from same gate → VCA/filter
- Accent pattern → **ACCENT IN**

**Knobs:**
- Snappy: low
- Noise: low
- Tone: short
- Tune: low
- Accent: medium-high

**Why it works:**
You are minimizing the snare sizzle and using the body oscillator as a bass pluck.

---

## Patch 4: Noise melody generator
**Goal:** create melodic material elsewhere in the system using SD909

- **NOISE OUT** → sample & hold input
- Clock divider / rhythm trigger → sample & hold trigger
- S&H output → quantizer
- Quantizer output → another oscillator pitch
- Same rhythm or related rhythm → SD909 GATE IN

**Why it works:**
The SD909 contributes both percussion and a noise-derived melodic control source.

---

## Patch 5: Dual-layer melodic percussion
**Goal:** one module, two related musical lines

- SD OUT → main drum/percussion mix
- NOISE OUT → filter + VCA → FX return or second channel
- Shared triggers
- One sequencer row → **VC-TUNE**
- Another sequencer row → filter cutoff for NOISE OUT path

**Why it works:**
The snare body and raw noise become two coordinated voices:
- one for attack/rhythm
- one for pitched/noisy melodic color

---

# How to make the SD909 feel more melodic

## Reduce noise dominance
The manual repeatedly emphasizes balancing noise and oscillators. For melody:
- turn **Snappy** down
- keep **Noise** under control
- use **Tone** shorter

This exposes the VCO body.

## Use external filtering
A drum voice often becomes much more melodic through:
- lowpass filtering for bass/plucks
- bandpass filtering for tuned percussion
- resonant filtering for pitch emphasis

## Sequence accent separately
Independent accent makes phrases breathe. This is one of the strongest “musical” features in the module.

## Treat VC-NOISE as timbre pitch
It may not track musically like an oscillator, but it absolutely creates a second expressive dimension analogous to melodic movement.

## Use quantizers carefully
VC-TUNE is not described as precise tracking, so:
- use small pitch ranges
- try 3–5 note motifs
- embrace imperfect analog tuning
- think “pitched percussion” rather than keyboard synth

---

# Best companion modules for melodic use

The manual itself mentions shaping the NOISE OUT with other modules. In a Eurorack context, SD909 pairs well with:

- **quantizer**
  - to make VC-TUNE sequences more scale-like
- **sequencer with separate trigger/accent lanes**
  - for groove and articulation
- **filter**
  - crucial for turning noise or snare body into more focused tones
- **VCA + envelope**
  - especially for NOISE OUT patches
- **delay/reverb**
  - helps metallic and tuned-percussion patches bloom
- **wavefolder/distortion**
  - for aggressive industrial melodic lines
- **sample & hold / random**
  - to derive melodic CV from NOISE OUT

---

# Realistic expectations

The SD909 is **not a standard precision voice oscillator**. It is better thought of as:

- a **tunable analog percussion voice**
- a source of **pitched drum transients**
- a **metallic/noisy timbre oscillator**
- a **raw binary noise source** for synthesis duties

So the strongest melodic applications are:

- tuned percussion
- electro bass stabs
- metallic riffs
- noisy lead textures
- generative melody support via NOISE OUT

If you try to use it like a clean VCO playing exact equal-tempered lines, it will likely be frustrating. If you use it like a **characterful analog voice with pitchable attack and expressive accent**, it becomes very musical.

# Bottom line

The SD909 can contribute melodic material in three main ways:

1. **As a pitch-sequenced snare-body percussion voice via VC-TUNE**
2. **As a metallic timbre-melody source via VC-NOISE**
3. **As a raw noise source via NOISE OUT for filtered or generative melodic patches**

Its real strength is in **percussive melody**: lines that sit between drums and synths. In electro, techno, industrial, IDM, and experimental patches, that can be more inspiring than a conventional oscillator.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)