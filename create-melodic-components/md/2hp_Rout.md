# 2hp — Rout

- [Manual PDF](../../manuals/Rout_Manual.pdf)

---

# [Manual PDF](#)

Based on the attached manual, the module shown is **Rout**, a **2hp voltage-controlled gate router/switch**. It does **not generate pitch directly**, but it can be very useful in building **melodic structures** by routing rhythmic gate information to different destinations in a patch.

## What Rout does
Rout takes **one gate/trigger input** and sends it to **one of four outputs**.

### Key functions
- **INPUT**: incoming gate/trigger
- **SEL CV**: voltage control for selecting which output is active
- **SEL knob**: manual selection of output 1–4
- **OUT 1–4**: the selected output passes the input gate
- **LEDs**: show which output currently has voltage

### Specs relevant to patching
- **Input threshold**: 2.5V
- **Output range**: 0–5V gate/trigger
- **SEL CV range**: 0–5V

---

## How Rout can help create melodic components

Since Rout is a **gate distributor under CV control**, its melodic use comes from deciding **which sequencer, envelope, voice, or modulation path gets triggered** at a given moment.

## 1. One rhythm, multiple pitched voices
Patch:
- Master clocked gate pattern → **Rout INPUT**
- **OUT 1–4** → trigger inputs of **four different voices** or **four different envelopes** controlling four oscillators

Result:
- A single rhythm gets sent to different voices over time
- If each voice is tuned to a different note, chord tone, or register, Rout turns one trigger pattern into a **melodic line with timbral or harmonic movement**

Example:
- OUT 1 → bass voice
- OUT 2 → root note lead
- OUT 3 → fifth
- OUT 4 → octave accent

Use **SEL CV** from an LFO, stepped random, or sequencer row to choose which note/voice is active.

---

## 2. Route one trigger stream to different sequencers
Patch:
- Gate pattern → **Rout INPUT**
- Each **Rout output** → clock/advance input of a different pitch sequencer

Result:
- Only one sequencer advances at a time
- You can effectively switch between different melodic phrases depending on the selected output

This is a strong way to create:
- verse / chorus variations
- call-and-response melodies
- fills and alternate note orders

For instance:
- OUT 1 → sequencer with bass motif
- OUT 2 → sequencer with higher inversion
- OUT 3 → sequencer with sparse phrase
- OUT 4 → sequencer with dense ornamentation

The melody changes because different pitch sources are being stepped.

---

## 3. Route triggers to different envelope shapes for one oscillator
Patch:
- One VCO provides the audio pitch
- Several envelopes or function generators shape the VCA/filter differently
- Trigger source → **Rout INPUT**
- **OUT 1–4** → different envelope generators

Result:
- Same oscillator pitch sequence, but each note articulation changes depending on routed gate destination
- This creates perceived melodic phrasing:
  - plucked notes
  - long sustained notes
  - accented filter pops
  - ghost notes

Even if pitch stays the same, articulation can make the line feel much more melodic.

---

## 4. Create melody by switching quantizer/sample-and-hold triggers
Patch:
- Random or stepped CV → quantizer input
- Gate stream → **Rout INPUT**
- **OUT 1–4** → different sample-and-hold or quantizer trigger paths, or different track-and-hold stages

Result:
- Rout determines **when** and **where** new pitch values are captured
- This can create alternating melodic behavior:
  - one output grabs notes frequently
  - another only occasionally
  - another triggers transpositions
  - another updates a harmony line

This is especially useful for semi-generative melodic systems.

---

## 5. Use Rout as a phrase selector for transposition events
Patch:
- Main melodic sequencer runs continuously
- Trigger pattern into **Rout INPUT**
- Each Rout output sends a trigger to a different transpose event, precision adder gate, sequential switch, or CV preset recall

Result:
- The same melody can jump between harmonic contexts
- You can use outputs to trigger:
  - root position
  - minor third transpose
  - fifth transpose
  - octave jump

That makes Rout a **harmonic phrase router**, even though it only routes gates.

---

## 6. Send one trigger stream to different percussion-like pitched voices
If your system includes tuned percussion modules or pinged filters:
- INPUT = regular trigger pattern
- OUT 1–4 = different tuned resonant voices

Result:
- One trigger source becomes a melody by striking different tuned modules
- Great for:
  - marimba-style lines
  - West Coast bongo melodies
  - pseudo-sequenced modal percussion

Because the selection can be under CV control, the melodic order can be static or animated.

---

## 7. Controlled melodic variation with SEL CV
The biggest musical feature is **voltage control over output selection**.

Feed **SEL CV** with:
- **Stepped random** for generative melodic routing
- **Sequencer CV row** for repeatable phrase switching
- **Slow triangle/sine LFO** for cyclical movement across destinations
- **Manual CV controller** for live performance fills and transitions

Because SEL CV expects **0–5V**, it pairs well with many Eurorack modulation and sequencer sources.

### Musical outcomes
- Repeatable output order = structured melody
- Randomized output order = generative melody
- Slowly changing selector = evolving phrase orchestration
- Fast CV changes = glitchy ratcheting destination shifts

---

## Practical melodic patch ideas

## Patch 1: Four-note melodic distributor
- Clock divider or trigger sequencer → Rout INPUT
- OUT 1–4 → four envelope generators
- Each envelope controls a different VCA for four tuned oscillators

Tune oscillators to:
- C
- E
- G
- B

Now Rout turns one rhythm into an arpeggiated chord spread across four voices.

Control:
- SEL knob manually for fixed note choice
- SEL CV from a sequence for melodic order

---

## Patch 2: Phrase switching lead
- Gate sequencer → Rout INPUT
- OUT 1–4 → clock inputs on four pitch sequencers
- Outputs of pitch sequencers mixed or switched into one voice path

Each sequencer contains a different phrase.
Rout determines which phrase advances, creating larger melodic form from small patterns.

---

## Patch 3: Bassline with accents and octave jumps
- Main gate pattern → Rout INPUT
- OUT 1 → standard bass envelope
- OUT 2 → same bass voice plus octave transpose trigger
- OUT 3 → accent envelope
- OUT 4 → fill/reset event

This creates a bassline with evolving melodic contour from one simple gate stream.

---

## Patch 4: Generative melody hub
- Master trigger source → Rout INPUT
- SEL CV from stepped random
- OUT 1 → trigger main sequencer advance
- OUT 2 → trigger sample-and-hold for new pitch
- OUT 3 → trigger transpose event
- OUT 4 → trigger second voice harmony envelope

This makes Rout the central decision-maker for melodic behavior.

---

## Strengths of Rout in melodic patching
- Very compact at **2hp**
- Excellent for **reusing one trigger source** across many melodic destinations
- Adds **variation and structure** without needing a second trigger sequencer
- CV control makes it easy to fold into generative or performative systems
- Useful in both **polyphonic** and **single-voice evolving** patches

---

## Limitation to keep in mind
Rout is a **gate router**, not a pitch router or CV switch for melodic voltages.  
So by itself, it does not create notes. Its melodic value comes from routing **events** that affect:
- when notes happen
- which voice plays
- which phrase advances
- which articulation/transposition is triggered

In other words, Rout is best thought of as a **melody structure tool**, not a melody source.

---

## Summary
**Rout** is ideal for creating melodic components by:
- distributing one rhythm to different tuned voices
- selecting which sequencer or phrase advances
- varying articulation across notes
- triggering transposition or harmony events
- adding CV-controlled variation to otherwise static melodic material

If you upload the other module manuals too, I can analyze **how they work together as a complete melodic system** and suggest specific multi-module patches.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)