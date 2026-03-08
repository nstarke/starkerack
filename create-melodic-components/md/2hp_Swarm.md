# 2hp — Swarm

- [Manual PDF](../../manuals/2hp_Swarm_v1-0.pdf)

---

[Manual PDF](https://www.twohp.com/modules/swarm)

# 2hp Swarm: using it for melodic parts

Based on the manual, **2hp Swarm** is a **hyper oscillator / supersaw-style voice source** designed to generate thick, animated pitched tones from a very small footprint. On its own, it is primarily an oscillator, but the manual also points to a few ideal companion modules for turning it into a complete **melodic voice**:

- **Swarm**: pitched sound source
- **EG**: envelope for note articulation
- **VCA**: amplitude control
- **MMF**: tone shaping / filtering
- **Lo-Fi**: coloration and character

## What Swarm does well musically

Swarm is built for **stacked oscillator textures**:

- **Freq** sets the main pitch and tracks **1V/oct**
- **Voices** changes how many oscillators are active
- **Detune** spreads those oscillators apart for width and motion
- **Wave toggle** switches between:
  - **Saw**: classic supersaw / trance / lead / pad character
  - **Pulse**: narrower, more hollow, reed-like or aggressive tone

### Voice count behavior
The manual gives useful detail here:

- fully CCW on **Voices** = **1 oscillator**
- center = **20 oscillators**
- fully CW = **dozens**
  - up to **88 oscillators for Saw**
  - up to **55 oscillators for Pulse**

That means Swarm can move from:

- a relatively simple mono oscillator
- to a very dense unison lead
- to a huge swarm pad/drone source

This makes it especially strong for **melodic hooks, trance leads, hardstyle stabs, lush harmonies, and animated basses**.

---

## Core melodic patch: Swarm as a playable synth voice

The most straightforward use is to build a standard subtractive-style monosynth voice.

### Patch
1. Send a **sequencer or keyboard 1V/oct CV** to **Swarm Freq input**
2. Send **Swarm OUT** to **VCA IN**
3. Send **EG OUT** to **VCA CV**
4. Send **gate/trigger** from your sequencer to **EG TRIG**
5. Send **VCA OUT** to your mixer/output

### Result
This gives you:

- pitch from your sequencer
- note starts/stops from the EG and VCA
- a playable melodic line with Swarm’s unison texture

### Good starting settings
- **Voices**: around 9–11 o’clock for a focused unison lead
- **Detune**: low to moderate, around 9–12 o’clock
- **Wave**:
  - **Saw** for trance, EDM, anthemic lines
  - **Pulse** for sharper, chiptune-ish, nasal, or edgy melodies

This is the minimum patch for **riffs, basslines, arpeggios, and lead melodies**.

---

## Better melodic patch: add MMF for classic synth movement

The manual strongly suggests **MMF** with Swarm, and musically that makes a lot of sense. Swarm is harmonically rich, especially in saw mode, so a filter gives you dynamic control over brightness.

### Patch
1. **Swarm OUT → MMF INPUT**
2. Choose one MMF output:
   - **LP** for smoother leads and basses
   - **HP** for thinner trance leads
   - **BP** for focused, vocal-like tones
3. **MMF output → VCA IN**
4. **EG OUT → VCA CV**
5. Optional: mult the same envelope or use another modulation source to **MMF FREQ CV** if available in your system

### Musical uses
- **Low-pass**: warm basslines, classic synth leads, pads
- **High-pass**: uplifting trance leads that sit above a mix
- **Band-pass**: more cutting melodic hooks

### Why this works
Swarm produces a lot of harmonic content. Filtering lets you:
- tame the density
- create build-ups and transitions
- animate repeated melodic phrases
- make different registers feel distinct

A simple 8-note sequence through Swarm can become much more expressive just by sweeping the filter.

---

## Expressive note shapes with EG

The manual describes **EG** as useful for shaping “super-saw stabs,” and that’s exactly one of Swarm’s strongest applications.

### Fast pluck / stab
Use:
- fast attack
- short decay
- moderate amplitude

This is great for:
- trance chords
- gated melodic stabs
- hard dance riffs
- percussive bass sequences

### Longer envelope
Use:
- medium attack
- longer decay

This is better for:
- legato melodies
- pad-like phrases
- swelling harmonic lines

Because Swarm can sound very big very quickly, even modest envelope shaping gives strong rhythmic definition.

---

## Using Voices as a musical performance control

One of the most interesting melodic uses of Swarm is that **Voices** acts like a macro density control.

### Practical musical applications

#### 1. Verse to chorus expansion
- keep **Voices** lower during sparse sections
- raise it for choruses or climaxes

This makes the same melody feel like it “opens up” without changing the notes.

#### 2. Bass to lead morph
- lower voices for bassline passages
- increase voices and detune for lead sections

#### 3. Accent selected notes
If you can modulate **Voices CV**, you can increase oscillator count on certain steps to emphasize accents in a sequence.

### Important tonal effect
As you add voices:
- the sound gets wider
- harmonics and beating increase
- pitch perception becomes more “ensemble-like”

This is excellent for emotionally larger melodic gestures.

---

## Using Detune musically

The manual notes:

- first half of the knob = **tasteful detune**
- second half = **chaotic detune**

That suggests two broad melodic zones.

### Low to moderate detune
Best for:
- melodic clarity
- basslines
- chord-like intervals implied by the swarm
- stable leads

Use this when the notes need to remain clearly defined.

### High detune
Best for:
- euphoric leads
- noisy risers
- unstable drones
- huge transitions

At extreme settings, pitch center becomes less precise, so it’s often better for:
- sustained notes
- breakdown textures
- dramatic fills

### Sequencing tip
A small amount of modulation to **Detune CV** can bring life to repeated phrases:
- slightly more detune on longer notes
- detune opening during phrase endings
- subtle LFO for constant motion

---

## Saw vs Pulse for melodic writing

The waveform switch is a major compositional choice.

## Saw mode
Best for:
- supersaw leads
- lush arps
- chordal illusions
- trance/hard dance hooks
- wide melodic pads

Because saw waves are bright and harmonically dense, this is likely the most iconic Swarm sound.

### Use saw when you want:
- width
- richness
- emotional “anthem” energy
- strong filter interaction

## Pulse mode
Best for:
- tighter basses
- more hollow melodies
- retro/electro tones
- sharper riffs

Pulse can cut differently in a mix and can feel more focused than saw despite still being stacked.

### Use pulse when you want:
- cleaner separation
- more nasal or woody tone
- less wash than saw
- strong rhythmic articulation

---

## Swarm for basslines

Even though Swarm looks like a lead machine, it should be excellent for **melodic bass content**.

### Bass patch
1. **Pulse** or **Saw** depending on brightness needed
2. Keep **Voices** lower to moderate
3. Use **Detune** lightly
4. Send through **MMF low-pass**
5. Shape with **EG + VCA**

### Result
You can get:
- rolling techno bass
- wide trance bass
- distorted rave bass if followed by Lo-Fi
- squelchy bass when MMF resonance is used creatively

For bass, less is often more:
- too many voices can blur the low end
- too much detune can weaken pitch definition

---

## Swarm for leads

This is where the module likely shines most.

### Lead patch recipe
- **Saw mode**
- **Voices** at medium-high
- **Detune** at low-medium
- **MMF high-pass or low-pass depending arrangement**
- **EG** set for fast attack and medium decay
- optional **Lo-Fi** after the VCA or filter

### Why it works
You get:
- width without needing multiple oscillators
- instant “produced” sound
- a large stereo-like psychoacoustic feel even in mono contexts due to beating and density

This is ideal for:
- trance melodies
- festival lead lines
- octave riffs
- arpeggiated hooks

---

## Swarm for chord-like melodic textures

Swarm does not appear to be a chord generator in the strict sense, but because of the stacked oscillators and detune spread, it can create **chord-adjacent massed harmony textures**.

### Ways to use it
- sustain single notes for lush pseudo-chord presence
- sequence simple melodies and let the swarm create harmonic thickness
- layer two Swarm takes or two separate melodic lines for very dense arrangements

This is especially useful if you want:
- big harmonic impact from minimal sequencing
- cinematic monophonic melodies
- thick drone-based tonal centers

---

## Adding Lo-Fi for character melodies

The manual recommends **Lo-Fi** as a companion and gives two broad directions:

- **digital mode** for crunch
- **analog mode** for wobble/vintage character

### Melodic uses

#### Digital mode
Good for:
- aggressive leads
- bit-crushed arps
- harsh rave melodies
- modern distorted hooks

This can help Swarm cut in a dense track.

#### Analog mode
Good for:
- woozy synth lines
- nostalgic melodies
- unstable tape-ish phrases
- warped ambient leads

This is a great pairing when you want the swarm sound to feel less pristine and more emotional or haunted.

---

## A few practical melodic patch examples

## 1. Trance supersaw lead
**Patch**
- Sequencer 1V/oct → Swarm Freq
- Gate → EG TRIG
- Swarm OUT → MMF INPUT
- MMF HP or LP → VCA IN
- EG OUT → VCA CV
- VCA OUT → mixer

**Settings**
- Wave: **Saw**
- Voices: medium-high
- Detune: low-medium
- EG: fast attack, medium decay
- MMF: slightly bright, maybe some movement

**Result**
Classic soaring lead for arps or main melody.

---

## 2. Hard dance stab
**Patch**
Same as above

**Settings**
- Wave: **Saw**
- Voices: medium
- Detune: moderate
- EG: very fast attack, short decay
- MMF: brighter cutoff
- Optional Lo-Fi after VCA

**Result**
Punchy rhythmic stabs with lots of mass.

---

## 3. Animated bassline
**Patch**
- Sequencer → Swarm Freq
- Swarm → MMF LP
- MMF → VCA
- EG → VCA CV

**Settings**
- Wave: **Pulse**
- Voices: low-medium
- Detune: low
- MMF cutoff: moderate to low
- resonance to taste

**Result**
A more controlled, musical bass where Swarm adds body without becoming too smeared.

---

## 4. Nostalgic warbly melody
**Patch**
- Swarm → VCA → Lo-Fi
or
- Swarm → MMF → VCA → Lo-Fi

**Settings**
- Wave: Pulse or Saw
- Voices: medium
- Detune: gentle
- Lo-Fi in analog mode

**Result**
A melodic line with movement and imperfection, useful for ambient, synthwave, or indie electronic styles.

---

## 5. Expanding sequence
Use a repeating melodic sequence and manually perform:
- **Voices**
- **Detune**
- filter cutoff on MMF

Start with:
- low voices
- low detune
- darker filter

Then build toward:
- more voices
- more detune
- brighter filter

**Result**
A full arrangement arc from a single simple melodic pattern.

---

## Best role of each module in a melodic system

### Swarm
Primary pitch source. Best for:
- leads
- basses
- drones
- thick arps
- melodic unison textures

### EG
Makes notes articulate musically. Best for:
- stabs
- plucks
- envelopes for melodic phrasing

### VCA
Essential for turning Swarm into an actual sequenced voice.

### MMF
Shapes brightness and movement; helps fit Swarm into a mix.

### Lo-Fi
Adds identity and vibe; useful when the clean supersaw sound feels too straightforward.

---

## Most complete melodic chain from the manual’s suggestions

A very strong full voice using only the pairings mentioned would be:

**Pitch CV / Gate source → Swarm → MMF → VCA → Lo-Fi → output**  
with  
**Gate → EG → VCA CV**

This gives you:

- pitch tracking
- note articulation
- subtractive tone shaping
- character processing

That is a complete melodic signal path for:
- basslines
- hooks
- arpeggios
- stabs
- soaring leads

---

## Summary

From the manual, **2hp Swarm** is best understood as a **compact supersaw / hyper-oscillator for melodic synthesis**. Its strength is not just in making a single waveform, but in giving you a **macro-controlled stack of many oscillators** that can range from focused and playable to huge and chaotic.

Used together with the modules suggested in the manual:

- **Swarm** provides the pitch and harmonic density
- **EG + VCA** turn it into a properly articulated melodic voice
- **MMF** sculpts it into basses, leads, and transitions
- **Lo-Fi** adds color, grit, or vintage instability

If your goal is melodic electronic music, this set is especially well suited for:

- trance leads
- supersaw riffs
- rave stabs
- wide mono basses
- animated arpeggios
- lush sustained hooks

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)