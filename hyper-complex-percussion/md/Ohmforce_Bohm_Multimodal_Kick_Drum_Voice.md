# Ohmforce — Bohm Multimodal Kick Drum Voice

- [Manual PDF](../../manuals/Bohm_Eurorack_Manual_Compiled.pdf)

---

[Manual PDF / Source](https://bohm-eurorack-manual.readthedocs.io/en/latest/index.html)

# Using Bohm for dense, hyper-complex percussion

Bohm is especially good for this because it is not just a single static kick voice: it is a **stereo dual-voice kick system** with **multiple models**, plus optional **Groove** and **Performer** expanders. That means you can treat it less like “just a kick” and more like a **central low-end percussion engine** for layered rhythmic architecture.

## What the module gives you musically

From the manual, the key strengths for complex rhythm design are:

- **Multiple kick models** with different architectures
- **Stereo dual-voice behavior**
- Controls for:
  - **HIT**
  - **VELOCITY**
  - **LENGTH**
  - **SUSTAIN**
  - **ATTACK**
  - **PITCH**
  - **CURVE**
  - **TRS DECAY**
  - **COLOR**
  - **FX**
  - **TRS TONE**
- **Groove expander** for a **secondary kick voice** suited to rumbles and layered percussion
- **Performer expander** for **DJ-style effects, ducking, and stereo processing**
- **Running modes**:
  - Studio Mode
  - Live Song Mode
  - Jam Mode

This makes Bohm ideal for building **nested rhythmic relationships** rather than a simple 4-on-the-floor kick.

---

# Core strategy: think of Bohm as 3 percussion roles

Use Bohm in three layers:

1. **Primary pulse**
   - The main downbeat anchor
   - Shorter, punchy, more defined

2. **Secondary low percussion**
   - Off-beat thumps, ghost kicks, tom-like low hits
   - Can come from alternate models or Groove voice

3. **Spatial/rumbled rhythmic tail**
   - Longer decays, stereo motion, FX, ducking
   - Creates density between primary hits

If you patch and sequence those layers independently, you can create the impression of a whole percussion section from one kick-centered ecosystem.

---

# Patch ideas for polyrhythms and complex time signatures

## 1. Polyrhythmic kick lattice

Use separate trigger streams to create interlocking cycles.

Example concept:

- Main Bohm voice: trigger every **5 steps**
- Groove voice: trigger every **7 steps**
- Accent CV or velocity modulation: cycle every **3 steps**
- Performer FX changes: cycle every **8 or 9 steps**

This creates a composite pattern that takes many bars to fully repeat.

### How to shape it
- Keep the **main voice** short:
  - lower **LENGTH**
  - moderate **ATTACK**
  - controlled **SUSTAIN**
- Set the **secondary/Groove voice** longer:
  - more **TRS DECAY**
  - more **COLOR**
  - subtle **FX**
- Modulate **PITCH** on only selected hits for pseudo-tom phrases

This works especially well for **5:7**, **4:5**, or **3:4:7** relationships.

---

## 2. Complex-meter kick phrasing

Instead of sequencing in 4/4, build phrases in meters like:

- **7/8**
- **9/8**
- **11/8**
- alternating **5/4 + 7/8**
- **3+3+2**
- **2+2+3**
- **4+4+3**

### Practical use on Bohm
Program your triggers so the strongest accents are not always on beat 1.

For example in **7/8**:
- Hit pattern accent structure: **3 + 2 + 2**
- Strong hit on step 1
- medium on step 4
- lighter on step 6

Then use:
- **VELOCITY** variation for accent hierarchy
- **ATTACK** for sharper accented hits
- **CURVE** to make some kicks snap and others bloom
- **PITCH** slightly lower on the first group to reinforce phrase boundaries

This gives the listener a strong internal pulse while still sounding asymmetrical.

---

## 3. Euclidean low-end percussion

If your trigger sequencer supports Euclidean rhythms, Bohm can become the anchor for very dense structures.

Try:
- Main kick voice: **5 hits over 13 steps**
- Groove layer: **7 hits over 16**
- Accent modulation: **3 over 8**
- FX bursts: **2 over 5**

### Why this works
Because Bohm has enough tone-shaping controls to differentiate each layer:
- shorter Euclidean streams become **dry punches**
- longer sparse streams become **sub punctuation**
- denser streams can be made **clickier and more percussive** with shorter sustain and more attack

You are not just varying timing; you are varying **spectral role**.

---

# Making the voice unique, punchy, and percussive

Even though Bohm is a kick module, you can push it into a broader percussion vocabulary.

## 1. Turn kicks into a family of tuned percussion

The manual notes that **PITCH** ranges roughly from **C1 to C2**, with adjustable pitch curves inspired by 808/909 behavior.

Use that musically:

- lower pitch = classic body/sub kick
- mid pitch = tom-like percussion
- high end of range = clicky attack drum or synth blip

### Technique
Sequence pitch changes across a phrase:
- Beat 1: low root kick
- Beat 3: slightly higher “tom”
- Beat 5: even higher accent hit
- Ghost notes: very short, higher-pitched taps

Then vary **CURVE**:
- steeper curve = more classic electronic punch
- softer curve = rounded low percussion

This gives you **melodic percussion**, which is excellent in odd meters.

---

## 2. Use ATTACK and LENGTH as rhythmic articulation controls

These are not just tone controls; they are groove controls.

### For punch
- Increase **ATTACK**
- Reduce **LENGTH**
- Keep **SUSTAIN** controlled
- Use shorter **TRS DECAY**

This makes hits feel more like precision drum machine transients.

### For dense rhythm beds
- Use alternating short and long hits
- Short hits act like punctuation
- Longer hits fill space between accents

Example:
- downbeats: short, sharp
- offbeats: longer, smeared, colored
- phrase-ending hit: long decay with FX

That contrast is what creates “hyper-complex” feel without total mud.

---

## 3. Use VELOCITY as a structural sequencer lane

If you can send variable accent or CV into velocity-related behavior, think of it as a compositional layer.

Use 4 velocity tiers:
- **high** = structural accents
- **medium** = groove support
- **low** = ghost hits
- **very low** = almost-clicks

Then map parameter response by model:
- some models may react with more attack
- some may react with more body
- some may change timbre strongly

This means a single trigger stream can become a **multi-level percussion line**.

---

## 4. Exploit model differences as “kit pieces”

Because Bohm includes multiple kick “models,” assign different models to different compositional purposes.

For example:
- Model A: tight, dry punch for meter definition
- Model B: boomy low-end support
- Model C: distorted or colored industrial accent
- Model D: click-forward transient percussion

In **Studio Mode**, explore immediate parameter changes to find:
- one model for anchor pulse
- one for syncopated secondary hits
- one for special fills

Then save programs if your workflow allows, since the module stores **up to 32 programs**.

---

# Using Groove for layered and rumble-heavy complexity

The manual says Groove adds a **secondary kick voice for techno rumbles and layered percussion**. This is extremely useful for dense rhythm.

## 1. Separate transient from tail
Use:
- **Main Bohm voice** = transient and impact
- **Groove voice** = longer low-end tail or off-beat rumble

This gives you cleaner control over rhythmic density.

### Patch idea
- Main voice on the grid
- Groove voice delayed or sequenced in between grid points
- Main voice: low sustain, sharp attack
- Groove: more decay, more color, more FX

Result:
- the main voice defines meter
- the Groove layer creates rolling momentum

---

## 2. Create call-and-response between voices

In odd meter, alternate the voices as if they were two drummers.

In **11/8**, for example:
- Main voice accents: steps 1, 4, 7
- Groove voice answers: steps 3, 6, 9, 11

Then tune them slightly apart with **PITCH** and vary **COLOR** so they occupy different low-frequency identities.

This becomes more like **interlocking hand drums or taiko logic**, but in electronic kick form.

---

## 3. Build pseudo-ratchets with layered short hits
If your sequencer can create fast repeated triggers:
- send the first trigger to main Bohm
- subsequent flams/repeats to Groove
- shorten both voices

This makes percussive bursts that feel like:
- machine-gun kicks
- low tom rolls
- granular impact clusters

Especially effective before bar transitions or phrase resets in complex meters.

---

# Using Performer for rhythmic motion and stereo complexity

The manual says Performer adds **DJ-style effects, ducking, and stereo processing**.

## 1. Turn ducking into groove architecture
Ducking is not just for mix cleanup. In dense percussion, it can become a rhythmic sculptor.

Use ducking to:
- carve space after major accents
- make long Groove tails pulse around the main kick
- exaggerate asymmetrical meter

For example:
- every strong hit ducks the stereo tail
- weaker hits do less ducking
- this creates macro-accent structure across a 7/8 or 13-step phrase

---

## 2. Use stereo processing to separate polyrhythms
Put different rhythmic functions in different stereo behaviors:
- centered = main structural pulse
- widened/processed = secondary or off-grid material

This helps dense patterns remain intelligible.

A practical idea:
- main kick dry and center
- Groove/performance-processed tails wider
- FX emphasized only on every 5th or 7th event

This creates the sensation of multiple percussion layers moving at different rates.

---

## 3. Use FX as phrase punctuation, not always-on decoration
With complicated rhythms, constant effects can blur the structure.

Instead:
- dry for most of the bar
- apply **FX** only at:
  - phrase ends
  - metric pivots
  - fill moments
  - polyrhythm intersections

That makes complexity feel intentional rather than messy.

---

# Best running modes for this goal

## Studio Mode
Use this first.

Because parameter changes happen immediately, it is ideal for:
- dialing in contrasting kick personalities
- finding the exact attack/sustain balance
- testing model behavior under rapid modulation
- building a library of saved rhythmic voices

Best for:
- designing kits for odd-meter percussion
- tuning layered rumble vs punch
- discovering how models respond to accents

## Live Song Mode
Use this when you want:
- preplanned kick changes
- different sections with different meter emphasis
- reliable transitions between pattern families

Good for arrangements like:
- intro in 5/4
- main section in 7/8
- breakdown with sparse 3-against-4 pulse
- climax with layered polymeter

## Jam Mode
Best when you want performable instability.

Use it for:
- mutating pattern emphasis live
- improvising fills
- switching which voice dominates
- riding FX and color for tension

For hyper-complex percussion, Jam Mode is likely best when the sequencing is external and Bohm becomes the expressive sound-shaping center.

---

# Patch recipes

## Recipe 1: Odd-meter industrial kick ensemble
Goal: sharp, asymmetrical percussion in 7/8

- Sequence main voice in **3+2+2**
- Set:
  - short **LENGTH**
  - medium/high **ATTACK**
  - low/moderate **SUSTAIN**
  - controlled **COLOR**
- Add Groove on offbeats with:
  - longer **TRS DECAY**
  - lower pitch
  - subtle **FX**
- Use Performer ducking on strong accents only

Result:
- articulated phrase divisions
- heavy but readable low-end
- aggressive machine-percussion feel

---

## Recipe 2: Polymetric techno rumble engine
Goal: long-cycle interaction

- Main voice: 4-step regular pulse
- Groove voice: 5-step cycle
- Accent/velocity: 7-step cycle
- FX modulation: 9-step cycle

Sound design:
- Main voice = clean punch
- Groove = longer rumble tail
- Every 7th accent = extra pitch drop or color shift
- Every 9th event = FX splash or stereo widening

Result:
- evolving phase relationships over many bars
- still club-functional, but much more intricate than straight techno

---

## Recipe 3: Low tom + kick hybrid system
Goal: make Bohm act like multiple drum instruments

- Use one model as a classic kick
- Use another setting or voice as a higher-pitched low tom
- Sequence alternating pitches within one phrase
- Shorten sustain on higher notes
- Increase attack on accented tom-like hits
- Use color variation to separate the “drums”

Pattern example in 11 steps:
- 1 = low kick
- 3 = high tom hit
- 5 = low kick
- 7 = ghost tap
- 8 = high tom accent
- 11 = long tail phrase ending

Result:
- one module behaves like a mini percussion battery

---

## Recipe 4: Hyper-dense ghost-note engine
Goal: lots of activity without losing punch

- Main accents: high velocity, short decay
- Ghost hits: low velocity, shorter length, slightly higher pitch
- Keep ghost hits quieter and thinner
- Use Groove only for selected reinforcement hits
- Add Performer stereo or ducking to prevent overlap mud

The trick is **spectral hierarchy**:
- loud hits = low and full
- ghost hits = smaller, brighter, shorter

That makes density possible.

---

# Composition tips specifically for complex rhythm music

## Use contrast, not maximum density everywhere
If every hit is huge, complex rhythm turns to mush.

Instead:
- accents big
- inner notes small
- fills bright and short
- rumbles reserved for transitions or support

## Let timbre mark the meter
In odd signatures, listeners need cues.

Use:
- lower pitch on the first beat of a cycle
- sharper attack on group boundaries
- more color on phrase endings
- extra FX only at long-cycle resets

## Build long-form repetition cycles
For true hyper-complex feel:
- trigger cycle length
- velocity cycle length
- pitch cycle length
- FX cycle length

Make each a different number of steps so the full phrase evolves slowly.

## Keep one stable reference layer
Even with heavy polymeter, keep one voice acting as the listener’s anchor.
Usually:
- shortest
- driest
- most centered
- least processed

Then let everything else mutate around it.

---

# Practical sound design checklist

When dialing in Bohm for punchy complex percussion:

- **Need more impact?**
  - raise **ATTACK**
  - shorten **LENGTH**
  - reduce excessive **SUSTAIN**

- **Need more definition in dense patterns?**
  - shorten decays
  - separate main and secondary roles
  - use stereo/ducking to create space

- **Need more variation?**
  - change **model**
  - modulate **PITCH**
  - vary **CURVE**
  - use **VELOCITY** in tiers

- **Need more rumble without losing clarity?**
  - let Groove handle tails
  - keep main voice dry and punchy
  - use Performer ducking to shape overlap

- **Need more “percussion” than “kick”?**
  - tune some hits higher
  - shorten them
  - use attack-heavy settings
  - alternate tonal roles across the phrase

---

# Final approach

If your goal is **densely rhythmic, hyper-complex percussion**, use Bohm as:

- a **kick anchor**
- a **layered low percussion pair**
- a **stereo rhythmic texture generator**

The real power is in separating functions:
- **main pulse**
- **secondary counter-rhythm**
- **tail/rumble/space**
- **accent/effect punctuation**

With external sequencing, odd meters, and differing trigger cycle lengths, Bohm can become the low-frequency heart of a very advanced rhythmic patch. The module’s controls let you move beyond straight kick duty into **tuned low percussion, ghost-note structures, industrial impacts, rumble counterpoint, and evolving polymetric low-end architecture**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)