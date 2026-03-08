# 2hp — Delay

- [Manual PDF](../../manuals/Delay_Manual.pdf)

---

[Manual PDF](#)

# 2hp Delay — using it for melodic components

This manual covers a single module: **2hp Delay**.  
Even though it’s an effect, it can be very useful for building **melodic structure**, not just ambience. In a Eurorack patch, delay often becomes a **rhythmic pitch-support tool**: it can create repeated notes, implied counterpoint, evolving arpeggio-like patterns, and sustained harmonic beds from short melodic phrases.

## What the module does

The **Delay** is a **2 HP Eurorack delay processor** with:

- **Audio input and output**
- **Three main parameters**
  - **TIME**
  - **FDBK** (feedback)
  - **MIX**
- **CV inputs for all three parameters**
- Delay range from **milliseconds to nearly two seconds**
- Feedback capable of going to **infinity**

## Panel summary

From the manual:

1. **IN** — audio input, 10Vpp  
2. **TIME CV** — CV for delay time, 0–5V  
3. **TIME** — sets repeat interval  
4. **FDBK CV** — CV for feedback, 0–5V  
5. **FDBK** — sets number of repeats  
6. **MIX CV** — CV for dry/wet mix, 0–5V  
7. **MIX** — dry/wet balance  
8. **OUT** — audio output, 10Vpp  

## How Delay contributes to melody

A delay doesn’t generate pitch by itself, but it can strongly shape melodic content in these ways:

### 1. Creating repeated note phrases
Feed a melodic voice into Delay and set:

- **TIME** to a musically relevant interval
- **FDBK** to a few repeats
- **MIX** around 25–50%

This gives you repeating notes behind the original melody, making a simple sequence feel more complex and musical.

### 2. Turning short motifs into longer lines
A very short phrase from a sequencer can become a fuller melodic statement when delay repeats extend it. This is especially useful if your patch has:

- a quantized pitch sequence
- plucked envelopes
- short percussive voices

The delay fills the gaps, making sparse lines sound intentional and composed.

### 3. Creating call-and-response effects
Set the **TIME** so the repeat lands after the original phrase. With moderate feedback, the repeats act like an answer to the played line. This works well for:

- acid-style leads
- FM plucks
- filtered pulse melodies
- mallet-like voices

### 4. Producing pseudo-counterpoint
Longer delay times with lower mix can create a second layer that overlaps with new notes. If your incoming melody changes pitch while older repeats are still audible, you get the effect of multiple melodic lines interacting.

### 5. Building harmonic beds from monophonic material
With high **FDBK** and a longer **TIME**, a monophonic sequence can smear into a sustained texture. If the original line moves through scale tones, the delay can create overlapping pitch layers that imply harmony.

### 6. CV animation for evolving melodic texture
Because **TIME, FDBK, and MIX** all accept CV, you can animate the delay in sync with the rest of the patch:

- modulate **TIME** slowly for shifting rhythmic placement
- modulate **FDBK** to make some notes bloom into long tails
- modulate **MIX** to bring echoes in and out as part of arrangement

This is where the module becomes especially musical.

---

# Best melodic use cases

## 1. Echoed lead line
Patch:

- Oscillator/voice → Delay **IN**
- Delay **OUT** → mixer/output

Settings:

- **TIME**: short to medium
- **FDBK**: low to medium
- **MIX**: low to medium

Result:
- A lead becomes wider and more expressive without losing definition.

Good for:
- techno hooks
- ambient motifs
- Berlin-style step melodies

## 2. Arpeggio thickening
Feed an arpeggio or stepped sequence into Delay.

Settings:

- **TIME** synced by ear to the sequence pulse
- **FDBK** around 2–4 audible repeats
- **MIX** around 30–40%

Result:
- The arp sounds denser and more interlocked.
- Repeats fill empty spaces between notes.

## 3. Canon-style melodic overlap
Use a medium-long **TIME** so each note repeats after one or two steps of the sequence.

Result:
- Notes from earlier in the melody overlap with current notes.
- This creates a simple canon or round effect.

This works particularly well with:
- quantized diatonic melodies
- pentatonic sequences
- simple 3–5 note motifs

## 4. Drone from melody
Use:

- long **TIME**
- high **FDBK**
- medium/high **MIX**

Feed in occasional notes or a sparse sequence.

Result:
- A melodic phrase turns into a sustained tonal cloud.
- Very effective for ambient or intro sections.

## 5. Voltage-addressed arrangement movement
Use external CV:

- LFO or slow random to **MIX CV**
- envelope or sequencer gate-derived CV to **FDBK CV**
- stepped CV to **TIME CV**

Result:
- Certain notes become more echoed than others
- Some repeats stack into phrases
- The melodic texture changes over time without changing the source sequence

---

# Important musical behavior of each control

## TIME
This is the most compositionally significant control.

It sets the interval between repeats. For melodic use:

- **Short times**: thicken notes, slapback, doubling
- **Medium times**: rhythmic echo, phrase extension
- **Long times**: overlapping melody, ambient layering

### Musical tip
If you tune the TIME by ear relative to the tempo, echoes can land in useful subdivisions. Even though this manual does not mention clock sync, you can still manually dial in timings that feel like:

- dotted echoes
- off-beat responses
- phrase-length repeats

### CV on TIME
Using CV on delay time can create:
- shifting rhythmic relationships
- pitchy/glitchy time changes depending on the source and modulation depth
- expressive transitions

For melodic patches, subtle modulation usually works better than extreme modulation unless you want unstable, tape-like or fractured effects.

## FDBK
This controls how many repeats you hear.

For melody:

- **Low feedback**: just a few echoes, keeps phrase clarity
- **Medium feedback**: builds a repeating motif
- **High feedback**: turns phrases into looping melodic residue
- **Near infinity**: self-sustaining texture

### Musical tip
Use higher feedback on sparse sequences, lower feedback on dense ones.  
If the incoming line is already busy, too much feedback can blur pitch relationships.

### CV on FDBK
This is excellent for making only some notes “blossom” into repeating structures. For example:

- Send accented steps or envelopes to **FDBK CV**
- Stronger notes produce more repeats
- Unaccented notes stay dry and articulate

That creates phrasing and hierarchy in a melody.

## MIX
This determines how prominent the delayed signal is compared with the dry signal.

For melody:

- **Low mix**: support role, preserves note articulation
- **Mid mix**: clearly audible interplay between line and repeats
- **High mix**: original becomes less dominant; can create ghost-melody effects
- **Full wet**: useful as a parallel delayed line

### CV on MIX
One of the easiest ways to “arrange” the melodic space dynamically.  
For instance:

- Bring delay forward during transitions
- Pull it back during busy sections
- Use envelopes to make note tails emerge after each attack

---

# Patch ideas for melodic music

## Patch 1: Minimal techno riff enhancer
**Source modules needed:** sequencer, oscillator/voice, envelope/VCA, Delay

Patch:
- Sequencer pitch CV → oscillator pitch
- Gate → envelope → VCA
- Voice output → Delay IN
- Delay OUT → mixer

Settings:
- TIME: short-medium
- FDBK: low-medium
- MIX: low

Why it works:
- Preserves punch
- Adds repeated notes that reinforce the groove
- Makes a 1-bar riff feel more active

## Patch 2: Ambient overlapping melody
Patch:
- Quantized slow sequence → voice
- Voice output → Delay IN
- Delay OUT → reverb or mixer

Settings:
- TIME: long
- FDBK: medium-high
- MIX: medium-high

Optional modulation:
- slow LFO to MIX CV
- very slow random to TIME CV

Why it works:
- Notes overlap into suspended harmonies
- A simple melodic line becomes a floating harmonic texture

## Patch 3: Accent-sensitive echo melody
Patch:
- Voice → Delay IN
- Accent CV or envelope → FDBK CV

Settings:
- TIME: medium
- FDBK knob: low
- MIX: medium

Why it works:
- Only accented notes generate substantial repeats
- Repetition becomes part of phrasing
- Great for acid or sequenced electro lines

## Patch 4: Pseudo two-voice canon
Patch:
- Monophonic melodic voice → Delay IN
- Delay OUT → mixer

Settings:
- TIME: close to one beat or one step cycle by ear
- FDBK: low-medium
- MIX: medium

Why it works:
- The repeat enters like a second player echoing the melody
- Creates the illusion of polyphony from a single voice

## Patch 5: Wet-only melodic shadow
Patch:
- Send voice to Delay
- Set MIX high or fully wet
- Mix dry signal separately outside the module if possible

Why it works:
- The delayed line acts like an independent melodic shadow
- Very effective if the dry voice is centered and the delay is processed separately

---

# Practical performance advice

## Keep the source melody simple
Delay tends to reward simple melodic material:

- 3–7 note loops
- repeated motifs
- sparse arpeggios
- call-and-response phrases

If the source is too dense, the repeats may mask pitch clarity.

## Tune the TIME by ear
Because the module is not described as clock-syncable in the manual, treat TIME as a performance control. Sweep until the repeats sit in the groove.

## Use FDBK carefully
The manual notes that feedback can go to **infinity**. That means this module can enter a self-sustaining state. Musically, this is useful, but in performance:

- raise feedback gradually
- monitor output level
- be ready to pull back MIX or FDBK

## Animate one parameter at a time
For melodic clarity:
- modulate **MIX** first
- then add selective **FDBK** modulation
- use **TIME CV** more sparingly unless you want obvious time-warping effects

---

# Installation/specs from the manual

- **Format:** 2 HP Eurorack
- **Depth:** 47 mm, skiff friendly
- **Power:**  
  - +12V = 72mA  
  - -12V = 28mA  

Installation note from the manual:
- Red stripe corresponds to **-12V**
- On the module, the ribbon should be connected with the **red band facing the front**

---

# Bottom line

The **2hp Delay** is best thought of as a **melodic multiplier** rather than just an effect. It helps create:

- repeated note patterns
- phrase extension
- overlapping lines
- implied harmony
- evolving melodic texture through CV

If paired with a sequenced oscillator voice, quantizer, envelope, and VCA, it can turn very minimal note material into something much more musical and emotionally rich.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)