# 2hp — Pluck

- [Manual PDF](../../manuals/2hp_Pluck.pdf)

---

[Manual PDF](#)

## Module analyzed: Pluck

Pluck is a **2HP Karplus-Strong string synth voice** designed for **melodic, plucked, string-like sounds**. From the manual, it is a **complete sound source** with:

- **Trig input**
- **Damp CV + knob**
- **Decay CV + knob**
- **1V/Oct input**
- **Pitch knob**
- **Audio output**
- **4-voice polyphony**

That means this module is especially good at creating:
- plucked melodies
- pseudo-harp and mallet lines
- bass plucks
- ringing chordal arpeggios
- layered polyphonic trigger patterns from a single voice output

---

## What this module does musically

Pluck uses a **Karplus-Strong algorithm**, which is essentially a synthesized string model. In practice, that gives you:

- bright plucks
- muted string tones
- short percussive notes
- longer resonant string sounds
- bassy, dirty “half-strung” textures as the manual describes

Because it has **1V/Oct tracking**, it can be used like a melodic oscillator/voice. Because it has a **Trig input**, it behaves more like a self-contained plucked instrument than a continuously droning oscillator.

---

## Key performance behavior from the manual

A few details in the manual are very important for patching melodic material:

### 1. Trigger creates new notes
Each incoming trigger creates a new note using the current settings of:
- Pitch
- V/Oct
- Damp
- Decay

So the module “samples” those settings at note onset.

### 2. Four voice polyphony
It can generate **up to four notes simultaneously**, and when a fifth trigger arrives, the **oldest voice is replaced**.

Musically, this means:
- overlapping melodies work well
- arpeggios can smear into chord-like textures
- fast note sequences can build harmonic clouds
- long decay settings can create accidental harmony from monophonic trigger streams

### 3. Damp and Decay affect only new notes
This is crucial.

Per the manual, **Damp** and **Decay** only affect **newly generated notes**, not notes already ringing.

That means you can:
- sequence timbral variation per note
- make each new pluck brighter/darker
- make accents by increasing decay on certain steps
- create evolving melodies where older notes retain their own character

### 4. Pitch knob remains active on the most recently generated note
This is a very interesting detail. The manual says the pitch control remains active for the **most recently generated note**, allowing:
- vibrato
- pitch slew
- easier tuning while a note rings

So while older polyphonic voices stay where they were triggered, the newest note can still be “played” with the pitch control.

---

# How to use Pluck for melodic components

## 1. Basic melodic voice
This is the simplest patch.

**Patch:**
- Sequencer pitch CV -> **V/Oct**
- Gate or trigger sequencer -> **Trig**
- **Out** -> VCA, LPG, mixer, filter, or directly to output chain

**Result:**
A straightforward plucked melodic line.

**Tips:**
- Use shorter **Decay** for staccato lines
- Use longer **Decay** for harp-like overlap
- Use **Damp** lower for more muted tones
- Use **Damp** higher for brighter, harmonically rich notes

---

## 2. Polyphonic arpeggio texture
Since the module has **4-voice polyphony**, one sequencer can generate more than just a monophonic line.

**Patch:**
- Fast clocked pitch sequence -> **V/Oct**
- Matching triggers -> **Trig**
- Set **Decay** medium to long

**Result:**
As notes overlap, you get a shimmering arpeggiated texture that can imply chords.

**Why it works:**
Each trigger creates a new voice, and older voices continue ringing. With the right sequence, a simple melodic pattern becomes a harmonic bed.

**Best use cases:**
- ambient arps
- generative melodic figures
- pseudo-harp cascades
- Berlin-school pluck lines

---

## 3. Bass plucks
The manual specifically suggests it can move into “grungy half-strung bass.”

**Patch:**
- Low-register sequence into **V/Oct**
- Trigger pattern into **Trig**
- Lower **Damp**
- Medium-short **Decay**

**Result:**
Short, punchy bass notes with string character rather than pure analog oscillator tone.

**Variation:**
Add CV to **Decay** so some notes sustain longer than others. This gives a more “played” bassline feel.

---

## 4. Humanized melodic phrasing with Damp CV
Because **Damp CV** is bipolar and added to the knob position, you can animate tone on a per-note basis.

**Patch ideas:**
- Random stepped CV -> **Damp**
- Slow sequencer row -> **Damp**
- Accent CV -> **Damp**

**Result:**
Each note can be:
- brighter
- duller
- tighter
- more open

This is extremely useful for making repetitive melodic lines feel expressive.

**Musical application:**
- brighter notes on accented beats
- muted notes between accents
- alternating timbre in ostinatos
- pseudo-picking variation like a guitarist or harpist

**Manual range:**
- **-5V to +5V**

---

## 5. Dynamic note-length melody with Decay CV
Decay is one of the best modulation points for musical phrasing.

**Patch ideas:**
- Accent lane from sequencer -> **Decay CV**
- Random CV -> **Decay CV**
- Slow LFO -> **Decay CV**
- Euclidean accent pattern -> **Decay CV**

**Result:**
Some notes become short and dry, others bloom and ring.

Because **Decay only affects new notes**, you can get very nuanced melodic articulation:
- ghost notes
- accents
- phrase endings with longer sustain
- occasional blooming harmonic tails

This is one of the easiest ways to make Pluck feel “performed” rather than mechanically sequenced.

---

## 6. Chord illusion from a monophonic sequencer
Even though there is only one V/Oct input and one trigger input, the polyphony allows chord-like results.

**Patch:**
- Send a melodic sequence with medium/long decay
- Use repeated triggers and intervals in the sequence
- Let notes overlap

**Result:**
You can imply chords with:
- broken triads
- 1-5-8 patterns
- pedal-note figures
- repeated upper chord tones over changing bass roots

**Example sequence ideas:**
- C, G, E, G
- C, E, G, B
- root, 5th, 9th, 3rd
- octave displacement arpeggios

Because 4 notes can ring at once, Pluck can behave almost like a mini chord resonator when sequenced this way.

---

## 7. Vibrato and expressive pitch movement
The manual notes that the **Pitch knob remains active for the most recently generated note**.

This means after triggering a note, you can manually perform:
- slight vibrato
- subtle pitch bends
- tuning nudges
- glides on the newest note

**Musical use:**
- expressive leads
- live performance embellishment
- bending the final note of a phrase
- making a repeated pattern feel less rigid

If you’re hands-on with the system, this is a strong performance feature.

---

## 8. Generative melody voice
Pluck is a strong candidate for generative systems.

**Patch:**
- Random quantized CV -> **V/Oct**
- Irregular trigger source -> **Trig**
- Slow random voltage -> **Damp**
- Another slow random voltage -> **Decay CV**

**Result:**
An evolving, self-playing plucked instrument with tonal and rhythmic variation.

Because of the 4-voice overlap, even sparse generative triggers can create rich melodic/harmonic fields.

---

# Best pairings with other Eurorack module types

The manual only covers Pluck, but as a Eurorack musician, here’s how it works best with common companion modules to create melodic parts.

## Sequencer
A sequencer is the most obvious partner.

Use it to send:
- **pitch CV** to V/Oct
- **gate/trigger** to Trig
- optional modulation lanes to Damp/Decay

This gives you:
- basslines
- melodies
- arpeggios
- repeating motifs

## Quantizer
If using random or unquantized CV, a quantizer before **V/Oct** keeps the output musical and scale-locked.

Great for:
- generative plucks
- modal runs
- harmonic consistency

## Trigger sequencer / Euclidean trigger source
Since notes are initiated by triggers, rhythmic trigger design strongly shapes the melody.

Use this for:
- syncopation
- ratchets
- sparse note entries
- polyrhythmic pluck patterns

## Modulation source
LFOs, envelopes, random voltages, or sequencer CV lanes can animate:
- **Damp**
- **Decay**

This adds phrasing and timbral movement.

## Filter
Even though Pluck already has a strong timbral identity, a filter after the output can:
- soften brightness
- emphasize bass use
- create motion with filter envelopes
- place the sound better in a mix

## VCA / LPG
Pluck already produces decaying notes, but a VCA or LPG afterward can still help:
- shape overall dynamics
- add accenting
- shorten or gate the result further
- create more percussive articulation

## Delay / Reverb
Pluck excels with effects.

Use delay/reverb to turn simple melodic figures into:
- ambient string clouds
- shimmering arpeggios
- bell-like melodic trails
- cinematic harmonic beds

---

# Practical melodic patch recipes

## Patch 1: Harp arpeggio
**Connections**
- Sequencer CV -> V/Oct
- Clocked trigger pattern -> Trig
- Out -> Reverb

**Settings**
- Damp: high
- Decay: medium-long
- Pitch: tune to desired register

**Result**
Bright, sparkling plucked arpeggios with overlap.

---

## Patch 2: Muted ostinato
**Connections**
- 8-step sequencer -> V/Oct
- Trigger sequencer -> Trig
- Slow CV -> Damp

**Settings**
- Damp: lower range
- Decay: short to medium

**Result**
A tight, repetitive melodic phrase with subtle tonal variation.

---

## Patch 3: Polyphonic pseudo-chords
**Connections**
- Arpeggiator or sequencer -> V/Oct
- Fast regular triggers -> Trig
- Out -> Stereo delay / reverb

**Settings**
- Decay: long
- Damp: medium to high

**Result**
Overlapping notes create chord impressions from a single line.

---

## Patch 4: Expressive bassline
**Connections**
- Bass sequence -> V/Oct
- Gate pattern -> Trig
- Accent CV -> Decay CV

**Settings**
- Pitch low
- Damp low-medium
- Decay mostly short

**Result**
Punchy bass plucks with accented longer notes.

---

## Patch 5: Generative melodic texture
**Connections**
- Quantized random CV -> V/Oct
- Random trigger source -> Trig
- Slow random CV -> Damp
- Slow random CV -> Decay CV
- Out -> Reverb

**Settings**
- Decay medium-long
- Damp around center

**Result**
An evolving, self-playing melodic texture with harmonic smear.

---

# Performance tips

## Use decay to control harmonic density
Because Pluck is polyphonic, **longer decay = more overlap = more harmony**.

So if your melodic line feels too crowded:
- shorten Decay

If it feels too dry or empty:
- lengthen Decay

## Use damp to place the sound in the mix
- **Higher damp setting**: brighter, more present, more harmonics
- **Lower damp setting**: darker, more muted, more supportive

This makes Damp a great “arrangement” control.

## Be aware that old notes are replaced
With only **4 voices**, dense trigger streams can start cutting off earlier notes.

This can be used creatively:
- for rolling arps
- for controlled harmonic churn
- for pseudo-strumming

But if you want clearer sustained harmony, reduce trigger density or shorten the phrase.

## Exploit the newest-note pitch behavior
Since the newest note can still respond to the pitch control, you can manually add:
- microtonal bends
- vibrato
- phrase-end bends

That makes the module more performable than many tiny digital pluck voices.

---

# Limitations to keep in mind

From the manual:

- There is only **one audio output**, so polyphony is internally mixed
- **Damp** and **Decay** affect only newly triggered notes
- Polyphony is limited to **four voices**
- Voice allocation replaces the **oldest** note first

These are not drawbacks so much as characteristics to compose around.

---

# Summary

Pluck is best thought of as a **compact melodic string voice** for Eurorack. It is especially strong for:

- sequenced plucks
- basslines
- arpeggios
- generative melodies
- overlapping harmonic figures
- compact polyphonic textures from a single module

Its most musically useful features are:
- **1V/Oct pitch control**
- **triggered note generation**
- **4-voice polyphony**
- **per-note timbral articulation via Damp**
- **per-note sustain articulation via Decay**

If you pair it with even a basic sequencer and trigger source, it becomes a very flexible melodic tool. Add modulation to Damp and Decay, and it starts to sound expressive and alive rather than static.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)