# Ohmforce — Bohm Multimodal Kick Drum Voice

- [Manual PDF](../../manuals/Bohm_Eurorack_Manual_Compiled.pdf)

---

[Manual PDF / source](https://bohm-eurorack-manual.readthedocs.io/en/latest/index.html)

# Using Bohm, Groove, and Performer to create melodic components

Even though **Bohm** is fundamentally a **stereo dual-voice kick module system**, the manual suggests a lot of ways it can be pushed beyond simple kick duties and into **pitched, melodic, and tonal percussion** territory.

## Big picture

These modules work together as a kind of **performance-oriented drum synth voice cluster**:

- **Bohm** is the main sound engine.
- **Groove** adds a **secondary kick voice**, useful for layering, rumbles, and supporting tonal material.
- **Performer** adds **DJ-style effects, ducking, and stereo processing**, which can turn simple hits into animated rhythmic/melodic phrases.

Because Bohm has:
- multiple synthesized **kick models**
- a controllable **PITCH**
- adjustable **pitch curves**
- timbral controls like **COLOR**, **FX**, and **TRS TONE**
- support for **CV input calibration**

…it can be treated not just as a kick drum, but as a **pitched percussion oscillator/envelope voice**.

---

## 1. Bohm as a melodic percussion voice

The manual notes that **PITCH ranges roughly from C1 to C2**, with pitch behavior inspired by classic **808/909** style kick curves. That tells me Bohm is ideal for:

- **bassline fragments**
- **tom-like tuned percussion**
- **pitched kick melodies**
- **sub-bass accents**
- **one-note or limited-range riffs**

### Practical melodic use
You can sequence Bohm’s trigger input rhythmically, then use:
- **PITCH** for the note center
- **CURVE** to control how the pitch falls or bends
- **LENGTH / SUSTAIN / TRS DECAY** to move between short percussive notes and longer booming tones
- **COLOR / TRS TONE / FX** to emphasize harmonics so the pitch reads more clearly in a mix

### What kind of melody?
Because the pitch range is relatively narrow, Bohm excels at:
- **modal bass ostinatos**
- **2–5 note repeating patterns**
- **industrial/techno tuned kick riffs**
- **electro low-end hooks**
- **pitched call-and-response with another oscillator**

Instead of expecting full keyboard-style melody, think:
> “low-register tonal rhythm instrument”

That’s often more musically effective in Eurorack anyway.

---

## 2. Using different kick models as different “instruments”

The manual says Bohm includes multiple kick drum **models**, each based on different drum machine architectures, and that controls behave differently depending on the selected model.

That is extremely useful for melody because different models will emphasize different things:

- some models will give a **cleaner sine-like fundamental**
- some will have more **click/attack**
- some will produce more **midrange body**
- some may support more obvious **pitch drops** or resonant tails

### Melodic strategy
Use different models for different musical roles:

- **Model A**: deep sub note voice
- **Model B**: punchy tuned tom sequence
- **Model C**: resonant note with more harmonics for audible melody
- **Model D**: noisy attack-heavy note for percussive arps

In practice, if one model does not “sing” enough melodically, switch models before trying to force it with EQ or processing.

---

## 3. Groove as a second melodic layer

The manual says **Groove adds a secondary kick voice for techno rumbles and layered percussion**.

That means Groove is very useful for **countermelody by layering**.

## Ways to use Groove melodically

### A. Root + accent tuning
- Tune **Bohm** to the tonal center or root note.
- Tune **Groove** slightly above or below.
- Alternate triggers between them.

Result:
- a two-note low melody
- great for techno, EBM, industrial, dub, broken beat

### B. Pitch-separated body and tail
- Use Bohm for the **main pitched attack**
- Use Groove for a **lower or longer rumble tail**

This creates the illusion of a more complex note:
- the attack says one pitch
- the resonance implies another
- together they feel melodic and cinematic

### C. Layered interval relationships
Try tuning the two voices to:
- unison
- octave
- fifth
- minor third for darker material

Even with limited pitch range, interval layering makes the kick system feel like a small **2-voice bass synth**.

### D. Trigger offset melodies
If your sequencer can send slightly offset triggers:
- trigger Bohm on the downbeat
- trigger Groove slightly later

This creates:
- flam-like tonal gestures
- rolling “bass fills”
- pseudo-delay note effects without needing an actual delay

---

## 4. Using envelope shape to imply melody

With drum synths, “melody” is often as much about **contour** as exact note pitch.

Bohm gives several contour-related controls:
- **ATTACK**
- **LENGTH**
- **SUSTAIN**
- **CURVE**
- **TRS DECAY**

These can be used to make repeated pitches sound like different notes or phrases.

### Examples

#### Short vs long notes
A repeated note becomes a phrase if you alternate:
- short, dry hits
- long resonant booms

#### Different pitch-fall curves
A note with steep downward curve reads differently from:
- a flatter curve
- a long glide
- a punchy 909-style snap

#### Attack shaping
Sharper attack gives more “consonant-like” articulation.
Softer attack makes the note feel rounder and more legato.

So even a 2-note sequence can become expressive if:
- note 1 = short, hard, bright
- note 2 = longer, softer, darker

That is melodic writing through **timbre and envelope**, not just pitch.

---

## 5. Performer as the “melody animator”

Performer adds:
- **DJ-style effects**
- **ducking**
- **stereo processing**

This is especially powerful if you want Bohm/Groove to contribute melodic content in a mix without muddying everything.

## How Performer helps melodic use

### A. Ducking clarifies pitch phrases
Low-frequency melodic percussion can blur easily.
Use **ducking** so longer tails from Bohm or Groove make space for:
- the next hit
- the other layered voice
- external melodic modules

This lets low-end patterns feel like **articulated notes** instead of a wash.

### B. Stereo processing creates movement
A mono kick is often perceived as purely rhythmic.
Stereo motion can make the same sound feel more like a **musical phrase**.

Use stereo effects to:
- widen tails
- exaggerate transitions between notes
- separate attack from ambience

This can make tuned kick riffs feel surprisingly “composed.”

### C. DJ-style effects for fills
Performer can turn simple 1- or 2-note material into evolving melodic events via:
- transitions
- drops
- effect throws
- phrase-ending emphasis

That means you can build melodic structure from a very minimal sequenced source.

---

## 6. Using the running modes musically

The manual mentions three running modes:

- **Studio Mode**
- **Live Song Mode**
- **Jam Mode**

These matter a lot for melodic use.

### Studio Mode
Best for:
- sound design
- tuning by ear
- exploring how each model responds to pitch and curve changes
- finding “sweet spots” where the drum starts to behave like a bass voice

Use this mode to create:
- tuned kick patches
- bass drum notes with stable pitch centers
- layered tonal presets

### Live Song Mode
Best for:
- sequenced kick changes
- switching between prepared tonal/percussive roles
- arranging melodic transitions in a set

This suggests you can prepare programs where Bohm changes from:
- standard kick
- tuned bass hit
- rumble note
- metallic percussive accent

That’s extremely useful in live techno or electro sets.

### Jam Mode
Best for:
- improvising with pitch and timbre
- performing note-like changes by ear
- using tactile modulation to morph from drum groove to bass phrase

Jam Mode sounds ideal for:
- live low-end improvisation
- breakdowns where the kick becomes the bassline
- spontaneous melodic layering with Groove

---

## 7. Program storage as a melodic composition tool

The manual states memory includes:
- **system settings**
- up to **32 programs**

That means you can design an entire melodic/percussive architecture around stored presets.

## Example program organization
You could dedicate programs like this:

1. **Clean root kick**
2. **Fifth-tuned layer**
3. **Long sub-boom**
4. **Punchy tom-like note**
5. **Dark distorted bass hit**
6. **Breakdown rumble texture**
7. **Wide stereo melodic kick**
8. **Transition/fill effect patch**

Then in performance, switch between them as if Bohm were a hybrid of:
- drum synth
- bass module
- performance FX unit

That’s a very powerful live composition approach.

---

## 8. CV and calibration matter for musical tuning

The manual mentions calibration for:
- knobs
- CV inputs
- optional **3V pitch calibration**

This is important if you want **reliable melodic behavior**.

### Why calibration matters
If you are using external CV to control pitch:
- uncalibrated inputs can make intervals inconsistent
- the usable note range may drift
- layered Bohm/Groove tuning can become muddy

### Best practice
If you want Bohm to act melodically:
1. Run the calibration process.
2. Check pitch response carefully.
3. Build patterns that stay inside the module’s strongest tracking range.
4. Tune by ear for musical intervals rather than assuming perfect 1V/oct keyboard behavior.

Given the manual’s pitch description, I would treat Bohm as:
- **tunable**
- **musically controllable**
- but probably best used for **limited-range melodic percussion**, not precision full-range tonal synthesis

That is not a weakness—it’s actually where a lot of compelling Eurorack music lives.

---

## 9. Concrete patch ideas

## Patch 1: Tuned techno bass kick
- Bohm as main voice
- Tune PITCH to track root note
- Use medium **CURVE**
- Increase **SUSTAIN** and **TRS DECAY**
- Reduce attack click if you want clearer tonality
- Sequence sparse triggers in a bassline rhythm

Result:
- a bass/kick hybrid line

---

## Patch 2: Dual-voice interval riff
- Bohm = root
- Groove = fifth or octave
- Alternate triggers between voices
- Use slightly different LENGTH and COLOR settings

Result:
- a low-register 2-voice riff built entirely from percussion voices

---

## Patch 3: Rumble melody
- Bohm handles short attack notes
- Groove provides long decaying tuned rumble
- Performer adds ducking so tails don’t swamp the next notes
- Add stereo processing for width

Result:
- atmospheric melodic techno low-end phrases

---

## Patch 4: Pitched tom sequence
- Choose a model with a strong audible body
- Shorten SUSTAIN
- Raise pitch into the upper part of Bohm’s range
- Use multiple trigger steps with different velocities

Result:
- tom melody / tribal tuned percussion line

---

## Patch 5: Live breakdown morph
- Start with Bohm as straight kick
- In Jam Mode, raise pitch and alter CURVE
- Bring in Groove for tonal layering
- Use Performer effects to expand into stereo
- End with ducked long tails and sparse triggers

Result:
- the kick gradually transforms into the breakdown bass motif

---

## 10. Best musical roles for this system

Used together, these modules are especially good for:

- **melodic techno**
- **industrial**
- **electro**
- **EBM**
- **dub techno**
- **leftfield rhythm music**
- **cinematic low-end design**

They are less likely to replace:
- a full-range VCO melody voice
- a polyphonic harmonic module
- a precision keyboard bass synth

But they are excellent for:
- **low-end hooks**
- **pitched percussion motifs**
- **bass/kick hybrids**
- **performance transitions**
- **stereo rhythmic melody textures**

---

## Final takeaway

The Bohm ecosystem can create melodic material by treating the kick engine as a **tuned percussion synthesizer** rather than just a drum source.

- **Bohm** provides the core pitched voice.
- **Groove** adds a second tunable layer for intervals, rumbles, and counter-rhythms.
- **Performer** shapes those sounds into clearer musical phrases through ducking, stereo movement, and effects.

The most effective approach is not to force these modules into traditional “lead synth” roles, but to exploit their strengths:
- strong low-end pitch
- expressive pitch envelopes
- layered drum synthesis
- preset-based performance changes
- live morphing between rhythm and tone

In other words, this system is ideal for building **melody out of drums**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)