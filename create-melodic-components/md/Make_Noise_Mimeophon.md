# Make Noise — Mimeophon

- [Manual PDF](../../manuals/mimeophon-manual.pdf)

---

[Make Noise soundhack Mimeophon Manual (PDF)](http://www.makenoisemusic.com/wp-content/uploads/2019/09/Mimeophon-Manual-v2021.pdf)

# Using the Make Noise Mimeophon to create melodic components

The attached manual is for the **Make Noise soundhack Mimeophon**, a stereo multi-zone delay/repeater. Even though it is “just” an effect on paper, the manual makes it very clear that Mimeophon can become a **melodic voice generator, harmonic processor, phrase looper, clock-derived pattern source, and pitch-shifting texture tool** when patched in a Eurorack system.

## What Mimeophon contributes melodically

From the manual, Mimeophon is especially useful for melody because it can:

- create **Karplus-Strong pitched tones** in **Zone 0**
- generate **pitched delay feedback** with **microRate**
- sync repeats to a master clock using **TEMPO**
- turn one melody into **polyrhythmic melodic canons**
- create **stereo melodic divergence** with **Skew**
- reverse and recontextualize phrases with **Flip**
- freeze loops with **Hold** and scan through them
- output a derived rhythmic clock from **Rate Out**

So rather than thinking of it only as a delay, think of it as a **melody multiplier**.

---

## Core features that matter for melodic patching

## 1. Zone determines musical scale of time

The manual describes 8 Zones:

- **Zones 0–1**: microsound, flange, Karplus, distortion, resonant/pitched behavior
- **Zones 2–4**: traditional delay/echo ranges
- **Zones 5–7**: looping phrases and long repeating structures

This means melodic use falls into 3 big categories:

- **Zone 0–1**: generate notes/timbres
- **Zone 2–4**: repeat notes rhythmically
- **Zone 5–7**: capture and reshape phrases/melodies

---

## 2. microRate is the most important melodic input

The manual says:

- **microRate tracks 1V/oct in Zone 0**
- in Zone 0 it is useful for **Karplus-Strong tone generation**
- in other zones it gives doppler modulation, chorus, vibrato, and flange

So in a melodic system, **microRate is effectively a pitch input when using Zone 0**.

That means:
- you can send sequencer pitch CV to **microRate**
- excite the input with a short transient/noise burst/envelope click
- Mimeophon behaves like a **plucked string oscillator**

This is one of the most direct ways the module becomes a melodic source rather than a processor.

---

## 3. Tempo sync turns echoes into harmonic/rhythmic melody structures

When **TEMPO** is patched, Rate chooses **divisions and multiplications** of the incoming clock, and changing Rate becomes free of doppler pitch glide.

That makes Mimeophon useful for:

- rhythmic melodic echoes
- canon-like note repetitions
- clock-locked arpeggio tails
- stereo subdivisions when **Skew** is enabled

If your source is already melodic, Tempo sync lets Mimeophon turn it into **structured repeating melodic patterns** that stay musically aligned.

---

## 4. Skew creates two related melodic timelines

With **Skew on**, left and right repeat rates diverge in opposite directions.

For melody, this is powerful because:
- one note stream becomes **two related melodic repeat grids**
- with stereo outputs, you get **counterpoint-like echo motion**
- with two mono signals patched independently, Mimeophon can behave almost like a **dual melodic repeater**

When clocked, this becomes especially musical because each side can land on different divisions/multiples of the same clock.

---

## 5. Hold turns it into a playable phrase memory

**Hold** freezes the buffer non-destructively:
- no new sound enters the feedback path
- all other controls remain active
- **Repeats** becomes a way to set the **start point** of the repeat

This makes long Zones very useful for melody:
- record a phrase
- press **Hold**
- move through Zones / Rate / Color / Halo / Flip
- scan different windows of the phrase
- derive new melodic fragments from older material

This is essentially **phrase resynthesis by navigation**.

---

## Best melodic use cases

## A. Karplus-Strong voice from Mimeophon alone

This is explicitly supported by the manual’s **Karplus String** patch.

### Patch concept
Use Mimeophon as a plucked string synth voice.

### How
- Go to **Zone 0**
- Patch a short transient into **Left input**
  - envelope click
  - noise burst
  - trigger-shaped transient
- Send **pitch CV** from a sequencer or keyboard to **microRate**
- Set:
  - **Rate** full CW
  - **Repeats** around 1:00
  - **Halo** fully CCW
  - **Mix** around 1:00
  - **Color** around noon

### Musical result
- Each trigger excites a resonant pitch
- **microRate** determines note pitch
- **Repeats** controls decay
- **Color** and **Halo** shape brightness/body

### Why this is melodic
This makes Mimeophon function like:
- a plucked string voice
- a tuned percussion voice
- a sequenceable resonator

This is probably the most important melodic takeaway from the manual.

---

## B. Turn a melody into a canon

### Patch concept
Feed a melodic voice through Mimeophon in **Zones 3–5**.

### How
- Patch oscillator/voice or full synth line into Mimeophon input
- Patch your master clock to **TEMPO**
- Set:
  - **Color** around 3:00 for neutral repeats
  - **Repeats** around noon
  - **Mix** to taste
  - choose **Zone 4 or 5**
- Adjust **Rate** to choose clock divisions/multiples

### Musical result
Your melody is repeated in time-locked patterns:
- quarter-note echoes
- dotted-feel echoes
- multiplied subdivisions
- phrase extensions

### Why this is melodic
You are not just adding ambience; you are creating:
- additional notes
- rhythmic answer phrases
- self-harmonizing melodic density

With the right source, Mimeophon becomes a **countermelody generator**.

---

## C. Stereo contrapuntal repeats with Skew

### Patch concept
Use **Skew** to split one melody into two related repeat rates.

### How
- Feed mono melody into **L input**
- Monitor both **L and R outputs**
- Patch clock to **TEMPO**
- Enable **Skew**
- Set Repeats moderately high
- Tune Rate for useful divisions

### Musical result
Left and right channels create:
- offset melodic responses
- staggered rhythmic answers
- widening stereo counterpoint

### Why this is melodic
A single monophonic line becomes a **two-voice spatial melody structure**.

This is great for:
- lead lines
- plucks
- marimba-type sequences
- vocal snippets

---

## D. Sequence Zones for note-by-note variation

The manual’s “Repeater Eater” patch suggests sequencing **Zone** while also sequencing audio material.

### Patch concept
Use stepped CV or a sequencer lane into **Zone CV**.

### How
- Feed a melodic or percussive melodic line into the input
- Sequence **Zone CV**
- Keep **Repeats** up enough for carryover between zones

### Musical result
Each note or step can jump between:
- Karplus-ish resonance
- flange-like short comb repeats
- normal echoes
- longer phrase repeats

### Why this is melodic
The melody gains **different repeat identities per note**.  
Short zones leave traces in longer zones, so earlier notes can bloom into later notes. This creates a **rhythmic/melodic lattice**.

This is one of the most compositional uses in the manual.

---

## E. Phrase looping and melodic excavation in Zones 6–7

The manual specifically notes that Zones 6 and 7 are long enough to retain material from earlier manipulations for minutes.

### Patch concept
Improvise in short zones, then mine the long zones for melodic material.

### How
- Play into Mimeophon while moving through shorter Zones
- Build up feedback and modulation
- Press **Hold**
- Remove modulation if desired
- Move to **Zone 7**
- Use **Repeats** to change start point
- Try **Skew** for drift
- Try **Flip** for reverse phrases

### Musical result
You can uncover:
- fragments of older melodies
- layered phrase memories
- accidental counterlines
- reversed motif variations

### Why this is melodic
Mimeophon becomes a **nonlinear phrase sampler**.

This is excellent for:
- ambient music
- generative melody
- live techno transitions
- evolving loop-based composition

---

## F. Reverse melody generation with Flip

The manual notes that in medium and large zones, **Flip** reverses playback.

### Patch concept
Send spoken, sung, or melodic material into Mimeophon and match Rate to phrasing.

### Musical result
You get reversed phrases that can still preserve cadence/rhythm.

### Why this is melodic
Reverse playback can create:
- melodic pickups
- swelling leads
- backward vocal hooks
- reversed answer phrases

If synced with TEMPO, these reversals can sit tightly in a composition.

---

## G. Harmonic enhancement with audio-rate microRate modulation

The manual’s **Octaviocho** and **Echoes Made of Sand** ideas show that feeding an oscillator into **microRate** creates harmonically related tones.

### Patch concept
Use a VCO waveform into **microRate** while also processing a voice.

### How
- Take sine/triangle from the same VCO driving your voice
- Patch it to **microRate**
- Choose Zones 1–5
- Adjust Repeats/Rate/Halo to taste

### Musical result
You get:
- octave-up fuzz
- subharmonic/related harmonic emphasis
- richer overtone structure
- more pitched edge to repeats

### Why this is melodic
This helps an existing melodic line produce **related harmonic content**, making it feel more like a second musical layer rather than plain delay.

---

## H. Clock generation from melody timing using Rate Out

The manual states that **Rate Out** outputs the current repeat clock, and under Skew it ORs both sides.

### Patch concept
Use Mimeophon’s Rate Out to drive other melodic events.

### Example uses
- clock a sequencer from **Rate Out**
- trigger envelopes for a second voice
- drive sample-and-hold for stepped pitch changes
- clock a quantizer source indirectly through repeat timing

### Why this is melodic
Now Mimeophon is not only processing melody—it is helping **generate the timing structure for other melodic voices**.

This is especially useful when:
- Tempo is externally clocked
- Rate chooses a division/multiple
- another sequencer follows that derived pulse

That creates nested melodic relationships.

---

## Practical melodic patch recipes

## 1. Plucked melodic lead
**Goal:** Use Mimeophon as the instrument.

- Triggered envelope or noise burst → **L Input**
- Sequencer pitch CV → **microRate**
- Trigger/gate sequence excites source
- Zone **0**
- Repeats around **1:00**
- Mix around **1:00**
- Halo low
- Color to taste

**Result:** sequenceable plucked notes.

---

## 2. Echo harmonizer for a lead synth
**Goal:** Turn one lead into multiple melodic events.

- Lead synth → **L Input**
- Clock → **TEMPO**
- Zone **4**
- Repeats at **12:00**
- Color around **3:00**
- Mix around **11:00 to 1:00**
- Adjust Rate to division/multiple

**Result:** synchronized repeating note patterns.

---

## 3. Stereo melodic canon
**Goal:** One melody, two repeat voices.

- Mono melody → **L Input**
- Clock → **TEMPO**
- Outputs L/R to mixer
- Enable **Skew**
- Moderate **Halo**
- Repeats at or above noon

**Result:** left/right phrases answer each other.

---

## 4. Reverse phrase hook generator
**Goal:** Create backward melodic motifs.

- Melody or vocal phrase → input
- Zone **4–6**
- Set Rate to approximate phrase length
- Engage **Flip**
- Use Hold if you want stable material
- Use Mix to blend

**Result:** reversed phrase layers for intros, breakdowns, and transitions.

---

## 5. Sequence-dependent melodic morphing
**Goal:** Different repeat behavior per note.

- Melodic sequence audio → input
- Stepped CV/sequencer lane → **Zone CV**
- Optional synced clock → **TEMPO**
- Repeats moderately high

**Result:** every note can occupy a different time/pitch texture regime.

---

## 6. Melodic loop mining
**Goal:** Build a phrase, then extract motifs.

- Play or sequence into Mimeophon
- Move around smaller zones while recording
- Raise Repeats
- Press **Hold**
- Switch to Zone **6 or 7**
- Use Repeats as start point selector
- Try Flip/Skew

**Result:** new melodies discovered inside older performance material.

---

## How Mimeophon works best with other Eurorack modules

Even though only Mimeophon is shown here, the manual implies several strong partnerships in a Eurorack system.

## Best companions for melodic use

### Sequencer
Use it for:
- pitch CV to **microRate**
- stepped modulation to **Zone CV**
- synced modulation to **Rate CV**

### Envelope/function generator
Use it to:
- create transient excitations for Karplus
- shape incoming audio
- dynamically modulate Color/Halo/Repeats

### Oscillator
Use it to:
- provide the melodic input signal
- feed audio-rate modulation into **microRate**
- create harmonic relation between source and repeater

### Clock source
Use it for:
- **TEMPO** sync
- tight rhythmic melodic repeats
- stable interlocking sequences

### Quantized random / sample and hold
Use it to:
- modulate Zone for structured variation
- create semi-random pitch on microRate
- derive generative melodies from Rate Out

### Mixer / stereo output module
Important because Mimeophon’s melodic power increases dramatically in stereo:
- Skew
- Halo
- Ping Pong
- left/right offset repeats

---

## Most musically important manual insights

These are the biggest takeaways for melody-making:

1. **Zone 0 + microRate = playable pitched voice**
2. **Tempo sync = repeat divisions/multiples without doppler**
3. **Skew = stereo split of melodic timing**
4. **Hold = frozen phrase for ongoing melodic modulation**
5. **Flip = reverse melody and phrase inversion**
6. **Long zones retain old musical information**, making phrase archaeology possible
7. **Rate Out** can propagate Mimeophon’s timing to the rest of the patch

---

## Best overall roles for Mimeophon in melodic music

Mimeophon can serve as:

- **Karplus synth voice**
- **tempo-synced melodic delay**
- **phrase looper**
- **reverse phrase processor**
- **stereo canon generator**
- **harmonic thickener**
- **clock-derived melodic hub**
- **generative phrase memory**

If you want a concise summary:

> Mimeophon is best used melodically when you either treat it as a **pitched resonator in Zone 0**, or as a **clocked phrase repeater/transformer in Zones 2–7**.

If you want, I can also turn this into:
- a **“5 best melodic patches” quick-reference sheet**
- a **module-to-module patch guide** if you upload more manuals
- or a **full system patch plan** for ambient, techno, or generative melody.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)