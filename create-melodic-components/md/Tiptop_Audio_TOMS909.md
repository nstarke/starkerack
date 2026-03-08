# Tiptop Audio — TOMS909

- [Manual PDF](../../manuals/Tiptop_Audio_TOMS909_ns.pdf)

---

[Manual PDF](https://tiptopaudio.com/manuals/TOMS909_manual.pdf)

# Tiptop Audio TOMS909: using it for melodic components

The **TOMS909** is primarily a **triple analog tom drum voice** based on the TR-909 tom circuits, but the manual makes clear that it can go well beyond percussion. Because each of the **Low, Mid, and High toms** has:

- **Tune**
- **Decay**
- **Accent**
- **Level**
- its own **Gate input**
- its own **Accent input**
- its own **audio output**
- and its own **VC Tune input with attenuator**

…it can be used as a **pitched percussive instrument**, a **3-note melodic voice cluster**, or a **modulated metallic texture generator**.

---

## What in the manual suggests melodic use?

The strongest clues are:

1. **Extended TUNE range**
   - The module is not restricted to fixed tom tones.
   - The manual explicitly says the Tune control can create:
     - low soft bass drum sounds
     - toms
     - “many other percussive sounds”

2. **Voltage control over tune/pitch for each drum**
   - Each tom has a dedicated **VC-TUNE input** and attenuator.
   - This means you can animate pitch with sequencers, LFOs, envelopes, or oscillators.

3. **Audio-rate modulation**
   - The manual specifically recommends patching a **VCO sine wave** into the tune CV inputs.
   - This is a classic way to create **pitched metallic spectra**, inharmonic tones, and tuned percussion timbres.

4. **Sequenced modulation**
   - The manual describes sequencing a VCO through a **Z8000 -> Z3000 -> VC-TUNE** chain.
   - That effectively turns the harmonic content of the toms into a **sequenced melodic parameter**.

5. **The note that VC-Tune is not 1V/Oct**
   - Important limitation: it is **not precision pitch tracking**.
   - So you should think of it as **quasi-melodic / tuned percussion / tonal modulation**, not as a keyboard-accurate oscillator voice.

---

# Best ways to use the TOMS909 melodically

## 1. Three tuned toms as a melodic percussion set

This is the most direct use.

### Patch concept
- Send separate trigger patterns to:
  - **LOW GATE IN**
  - **MID GATE IN**
  - **HIGH GATE IN**
- Take either:
  - individual outs for separate mixing/panning, or
  - **MIX OUT** for a summed signal
- Tune each drum to a stable pitch area using the **TUNE** knobs

### Musical result
You get a 3-note tuned percussion instrument. Think:
- low / mid / high “notes”
- tribal melodic figures
- pentatonic-feeling tom melodies
- call-and-response between registers

### How to make it more melodic
- Set **Decay** shorter for more defined pitch attacks
- Set **Decay** longer for more body and more obvious tone
- Pan low/mid/high across stereo if you have a mixer
- Program different rhythmic densities per tom

### Why it works
Even without exact volt/oct tracking, fixed tuning across three drums gives you a **repeatable interval structure**. This is enough for:
- ostinatos
- melodic fills
- pseudo-bassline plus upper accents
- tonal percussion riffs

---

## 2. Use gate sequencing to imply melody through register

The manual shows using a **Trigger Riot** to drive all three toms at different divisions. That same idea can be used to create melodic movement.

### Patch concept
- Low tom = root pulse
- Mid tom = offbeat answer
- High tom = faster ornament
- Tune them to musically related intervals by ear

Example:
- Low = tonic-ish
- Mid = fourth or fifth-ish
- High = octave-ish or ninth-ish bright accent

### Musical result
This creates **melody by orchestration**, rather than by traditional note sequencing.
You hear a phrase because the ear connects:
- pitch height
- rhythm
- accent
- decay shape

This is especially effective in:
- techno
- electro
- polyrhythmic minimal
- tribal / broken beat styles

---

## 3. Sequence the VC-TUNE inputs for moving pitch contours

Although the manual says **VC-TUNE is not 1V/Oct**, it is still highly useful for melodic animation.

### Patch concept
- Patch a CV sequencer row into:
  - **VC-L-TUNE**
  - **VC-M-TUNE**
  - **VC-H-TUNE**
- Use the corresponding attenuators to scale the pitch movement
- Trigger each tom with gates from a trigger sequencer

### Musical result
This gives:
- shifting tuned percussion
- rising/falling tom lines
- morphing melodic phrases
- unstable but musical pitch gestures

### Best practice
Because pitch tracking is not calibrated:
- use **small modulation amounts** for subtle interval movement
- tune by ear rather than expecting exact semitones
- use quantized CV only as a rough organizational tool, not for exact intonation

### Strong musical applications
- melodic fills
- pitch-bent tom runs
- evolving percussion hooks
- semi-tuned bass motifs from the low tom

---

## 4. Audio-rate FM for metallic melodic percussion

This is one of the most interesting uses described in the manual.

The patch tip specifically recommends:
- patching a **Z3000 sine wave**
- into all three **VC-TUNE** inputs
- and adjusting oscillator frequency

### What this does
At audio rates, modulation of tune creates:
- metallic overtones
- bell-like sidebands
- harsher or more harmonically rich attacks
- tuned-noise percussion colors

### Why this matters musically
This turns the TOMS909 from “drum module” into something closer to:
- tuned industrial percussion
- metallic marimba-like hits
- clangorous FM toms
- synthetic mallet voices

### Making it melodic
If the modulating oscillator is itself pitch-sequenced:
- the harmonic color changes in sync with the composition
- each hit can imply changing pitch centers
- the toms can move from drum role into tonal role

The manual explicitly suggests:
- clocking a sequencer
- sending sequenced CV to the VCO’s **1V/Oct**
- then using that VCO to modulate the TOMS909 tune CV inputs

That is a very powerful patch, because the **melody is not just in the drum pitch**, but in the **harmonic relationship between drum and modulator**.

---

## 5. Build harmonic relationships between Low, Mid, and High toms

Since each tom has independent Tune control, you can manually set them into interval relationships.

### Useful tuning strategies
By ear, try:
- **root / fifth / octave**
- **root / minor third / fifth**
- **root / fourth / minor seventh**
- close dissonant intervals for industrial tension

### Musical result
You can create:
- chord-like percussion voicings
- melodic triad fragments
- tuned fill systems
- pseudo-arpeggios when triggered in sequence

### Tip
Use:
- **longer decay** for more audible pitch
- **shorter decay** for more “plucked” tuned percussion

Short decay often works better for melodic clarity in dense mixes.

---

## 6. Accent as an expressive melodic parameter

The manual spends significant time on **Accent**, and this matters musically.

Accent does more than volume:
- it affects loudness
- it also changes the way the analog circuit is “hit”
- which slightly changes attack and noise content

So Accent acts like a primitive **performance articulation control**.

### Melodic use
Patch gates or CV into **ACCENT IN** while sequencing the toms.

This allows:
- stronger notes in a phrase
- phrase-end emphasis
- ghost notes vs accented notes
- dynamic melodic contour

### Why this is important
A melodic part is not just pitch; it is also:
- phrasing
- emphasis
- articulation

On TOMS909, Accent gives you a way to make repeated tuned hits feel like an intentional line rather than static percussion.

---

## 7. Use the Low tom as a bass voice

The manual notes that Tune can reach into **low-end bass drum / low percussion territory**. That implies the **Low tom** can often function as a quasi-bass instrument.

### Patch concept
- Trigger the **Low tom** in a repeating pattern
- Set:
  - lower Tune
  - medium/long Decay
  - carefully balanced Accent
- Optionally add subtle VC-TUNE modulation from a sequencer or envelope

### Musical result
You can get:
- thumpy bass ostinatos
- subby tuned hits
- acid-adjacent percussive bass pulses
- “bassline by drum synthesis”

This works best in styles where the bassline can be more percussive than sustained.

---

## 8. Use individual outs to build contrapuntal melodic layers

The module has:
- **LOW OUT**
- **MID OUT**
- **HIGH OUT**
- **MIX OUT**

For melodic work, the individual outputs are especially useful.

### Why
You can process each tom differently:
- low tom through saturation or lowpass filtering
- mid tom through delay
- high tom through reverb or ping-pong delay

### Musical advantage
Each tom can occupy a different melodic role:
- **Low** = bass motif
- **Mid** = main pulse/melodic answer
- **High** = ornament / sparkle / syncopation

This creates **multi-register melodic counterpoint** from one drum module.

---

# Practical melodic patch ideas

## Patch 1: Tuned tom melody trio
**Goal:** create a 3-note melodic percussion phrase

- Trigger source with 3 outputs -> Low/Mid/High Gate In
- Tune Low/Mid/High to a pleasing interval set by ear
- Set medium-short Decay
- Use individual outs or Mix Out
- Add slight Accent variation to one or two drums

**Result:** a playable tuned tom riff.

---

## Patch 2: Bass + answer + lead percussion
**Goal:** make the TOMS909 act like a mini melodic ensemble

- Low tom tuned low, medium decay, slower rhythm
- Mid tom tuned higher, syncopated rhythm
- High tom tuned bright, sparse accents
- Pan low left-center, mid center, high right
- Add accent pulses to high tom only

**Result:** a full melodic-percussive pattern with clear phrase structure.

---

## Patch 3: Sequenced pitch drift
**Goal:** add melodic variation over time

- Trigger each tom normally
- Send separate CV rows to each VC-TUNE input
- Keep attenuators low to moderate
- Use repeating but offset CV patterns

**Result:** each tom changes pitch over time, generating evolving melodic loops.

---

## Patch 4: Audio-rate harmonic percussion
**Goal:** create metallic melodic tones

- Sine VCO -> mult/stack -> all three VC-TUNE inputs
- Set VC-TUNE attenuators fairly high
- Sequence the VCO pitch from a CV sequencer
- Trigger toms in complementary rhythms
- Keep decay shorter for sharper metallic definition

**Result:** tuned industrial bells / metallic tom harmonics / animated melodic percussion.

---

## Patch 5: Tom arpeggiator
**Goal:** make the three toms behave like a chord arpeggio

- Tune Low/Mid/High as root/third/fifth by ear
- Trigger them sequentially:
  - Low on step 1
  - Mid on step 2
  - High on step 3
  - all together occasionally on step 4
- Add accent only to phrase boundaries

**Result:** a percussive arpeggio line.

---

# Strengths and limitations for melody

## Strengths
- Three independently tunable analog voices
- Dedicated CV tune per voice
- Great for tuned percussion and tonal rhythm
- Audio-rate modulation opens up rich melodic timbres
- Accent adds articulation and dynamics
- Individual outs enable layered melodic mixing

## Limitations
- **VC-TUNE is not 1V/Oct**
- Not intended as a precise chromatic oscillator
- Pitch may be better treated as **relative** rather than exact
- Best results come from **ear tuning** and **percussive phrasing**, not keyboard-style tonal expectation

---

# Best musical mindset for the TOMS909

The best way to think about this module is:

**not** as a conventional melodic synth voice, but as a:

- **tuned percussion instrument**
- **3-voice analog tonal drum bank**
- **metallic FM percussion source**
- **bass/mid/high melodic rhythm generator**

If you approach it that way, it can contribute a lot of melodic content:
- riffs
- bass pulses
- intervallic tom phrases
- shimmering metallic harmonics
- sequenced tonal percussion textures

In other words, the TOMS909 excels at **melody-through-rhythm, register, timbre, and articulation**.

---

# Most effective pairings with other modules

Based on the manual, the TOMS909 becomes especially melodic when paired with:

- **Trigger/gate sequencers**
  - for independent rhythmic phrasing of the 3 toms
- **CV sequencers**
  - for moving tune relationships over time
- **VCOs**
  - especially sine waves for audio-rate FM/timbre shaping
- **stereo delays/reverbs**
  - to enhance tonal and spatial perception
- **mixers/panners**
  - to separate the three toms into a melodic stereo image

---

# Bottom line

The **TOMS909** can absolutely create melodic material, especially if you use it as:

1. a **3-note tuned percussion set**
2. a **bass/mid/high interval voice cluster**
3. a **CV-modulated tonal drum instrument**
4. an **audio-rate FM metallic melody source**

Its melody is less about exact keyboard tracking and more about **pitched rhythm**, **interval relationships**, **accent phrasing**, and **harmonic modulation**. In a Eurorack system, that makes it extremely strong for expressive techno, electro, industrial, minimal, and experimental melodic percussion lines.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)