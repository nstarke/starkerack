# worng Electronics — Vertex

- [Manual PDF](../../manuals/Vertex manual v1.00.pdf)

---

[Vertex Manual PDF](#)

## WORNG Electronics Vertex: using it for melodic components

The attached manual is for the **WORNG Electronics Vertex**, a **stereo VCA / stereo animation / CV-shaping module**. On its own, Vertex is **not a pitch source, sequencer, quantizer, or oscillator**, so it does not directly generate melodies. But in a Eurorack system, it can be extremely useful for making melodic parts feel more alive, more playable, and more spatial.

## What Vertex does musically

Vertex gives you:

- **Stereo amplitude control** for left and right signals
- **Voltage-controlled panning / balance**
- **Envelope shaping through CV clipping at unity**
- **DC coupling**, so it can process **CV as well as audio**
- The ability to turn **one mono source into stereo movement**
- The ability to control **two related modulation signals at once**

That means Vertex is best understood as a **melody enhancer and articulator**, not a melody generator.

---

## Core melodic use cases

## 1. Turn a mono melodic voice into a stereo melodic voice

If you already have:

- oscillator
- filter
- envelope
- VCA
- sequencer / keyboard / quantizer

you can patch the **final mono voice** into the **Left input** of Vertex. Since **L is normalled to R**, the same signal appears on both sides if R is unpatched.

Then:

- set **Gain** up
- use **Skew** as a manual pan control
- patch an **LFO**, envelope, random voltage, or another modulation source into **Skew CV**

### Result
Your melody stays the same pitch-wise, but becomes:

- animated in stereo
- rhythmically wider/narrower
- more expressive
- easier to separate in a mix

This is especially effective for:

- arpeggios
- plucked sequences
- repeating basslines
- lead melodies

---

## 2. Create dynamic panning tied to note articulation

A very musical trick from the manual is to use:

- your melodic **audio** into Vertex input
- the same **envelope** that shapes the note into **Gain CV**
- another modulation source into **Skew CV**

Because Vertex clips CV at approximately **unity gain**, stronger envelopes can change shape when skewed left or right. This means the stereo image is not just getting louder on one side — one side can feel like it has a slightly longer **hold** or stronger **presence**.

### Musical effect
For a melodic line, this can create:

- notes that bloom left then settle center
- accented notes that lean right
- motion that follows articulation rather than simple pan law
- a more psychoacoustic “apparent loudness” shift

This is more interesting than ordinary autopan because it can make each note feel differently shaped in space.

---

## 3. Use Vertex as a dual CV VCA for melodic modulation

Since Vertex is **DC coupled**, it can process modulation voltages. This opens up a lot of melodic applications.

For example, suppose you have:

- one envelope controlling **filter cutoff**
- one LFO or sequence controlling **wavefold amount**
- a melodic voice receiving both modulations

You can route two CVs through Vertex and use **Gain / Gain CV / Skew** to scale both simultaneously.

### Why this matters for melody
Melody is often shaped less by pitch alone and more by:

- brightness contour
- vibrato depth
- FM amount
- filter motion
- accent level

Vertex can control two related modulation paths at once, so a single gesture can make a melodic phrase become:

- brighter on one side
- more animated on accented notes
- more open during choruses
- narrower and calmer during verses

---

## 4. Control two parallel melodic timbre lanes

You can use Left and Right as **two different CV destinations** related to a melodic patch.

Example:

- **Left output** goes to filter cutoff modulation depth
- **Right output** goes to wavefolder or resonance modulation depth
- **Gain CV** receives your note envelope
- **Skew** sets the balance between those two modulation intensities

### Result
Each note can have a coordinated timbral profile:
- one side of the control gesture emphasizes brightness
- the other emphasizes texture or harmonic complexity

This is powerful for melodic phrasing because it makes a sequence speak with more nuance.

---

## 5. Animate counterpoint or paired melodic voices

If you have **two separate mono melodic lines**:

- voice A into Left
- voice B into Right

Vertex can act as a stereo performance VCA for the pair.

Then you can:

- open both together with **Gain**
- bias attention between them with **Skew**
- animate the relationship with **Skew CV**

### Musical uses
- move call-and-response lines across the stereo field
- emphasize one counter-melody over another
- make one voice feel foreground while the other recedes
- create living stereo interplay between two sequenced lines

This is especially nice when two voices share a clock but have different rhythmic densities.

---

## 6. Make envelopes themselves part of melodic expression

One of the most interesting parts of the manual is the explanation that pushing the **Gain CV Amount** beyond the point of unity doesn’t keep increasing gain; instead it effectively **clips the control signal**. With envelopes, this can transform a shape more like:

- **AD** into something closer to **AHD**

When combined with **Skew**, left and right can get differently clipped envelope responses.

### For melodic patches this means:
- staccato notes can become more legato on one side
- one side can feel more accented without higher peak level
- repeated notes can gain width and contour
- plucks can become spatially asymmetric in a very musical way

This is ideal for:
- mallet sounds
- acid-style lines
- plucky FM
- Buchla-style percussive melodic phrases
- evolving ambient melodies

---

## Patch recipes for melodic music

## Patch 1: Stereo lead with animated panning

**Needs**
- oscillator
- filter
- envelope
- sequencer / quantizer
- Vertex
- output mixer

**Patch**
1. Build a normal mono melodic voice.
2. Send the final audio output of the voice to **Vertex Left input**.
3. Leave **Right input unpatched** so Left normals to Right.
4. Set **Gain** high enough for full signal.
5. Start with **Skew** at noon.
6. Patch a slow triangle or sine **LFO** into **Skew CV**.
7. Raise **Skew CV Amount** slightly clockwise.

**What you get**
- centered mono melody becomes stereo
- notes drift in the stereo field
- excellent for leads and arpeggios

---

## Patch 2: Envelope-shaped stereo plucks

**Needs**
- mono melodic voice
- envelope
- Vertex

**Patch**
1. Audio from the melodic voice to **Vertex Left input**.
2. Same envelope used for note articulation to **Gain CV input**.
3. Set **Gain** low or off.
4. Set **Gain CV Amount** so the envelope opens the VCA fully.
5. Push **Gain CV Amount** a bit beyond the “normal” point if your envelope is strong enough.
6. Move **Skew** away from center a little, or modulate it.

**What you get**
- note shape becomes part of stereo imaging
- one side may feel like it has a longer sustain/hold
- very expressive melodic articulation

---

## Patch 3: Voltage-controlled panning for a bassline or sequence

**Patch**
1. Bassline audio into **Left input** only.
2. Set **Gain** fully clockwise.
3. Use **Skew** as manual pan.
4. Patch stepped CV, random CV, or a synced envelope into **Skew CV**.
5. Adjust **Skew CV Amount** for subtle or wide movement.

**What you get**
- a mono bass or riff gains life
- useful for keeping repeated melodic patterns interesting
- can be tempo-synced to musical phrases

---

## Patch 4: Dual modulation control for one melodic voice

**Needs**
- two modulation sources
- one melodic voice with at least two CV destinations

**Patch**
1. Modulation source A into **Left input**
2. Modulation source B into **Right input**
3. Vertex Left and Right outputs to two destinations on the melodic voice:
   - filter FM / cutoff depth
   - pulse width / wavefold / FM index / vibrato depth
4. Patch an envelope, keyboard pressure, fader CV, or sequencer accent to **Gain CV**
5. Use **Skew** to bias modulation emphasis between the two destinations

**What you get**
- one macro gesture controls melodic timbre in two dimensions
- expressive accents
- per-note timbral choreography

This is one of the best “melodic component” uses of Vertex even though it is not directly processing pitch.

---

## Patch 5: Two melodic voices, one stereo performance layer

**Patch**
1. Voice A audio to **Left input**
2. Voice B audio to **Right input**
3. Use **Gain** to control both together
4. Use **Skew** to feature one voice over the other
5. Modulate **Skew CV** with an LFO, envelope, or manual controller

**What you get**
- stereo conversation between voices
- performance-friendly balancing
- animated duet textures

Good for:
- canon lines
- harmonized sequences
- question/answer motifs

---

## Best companions for Vertex in melodic systems

Vertex works especially well with:

- **Sequencers**: to provide pitch and accent structure
- **Quantizers**: to ensure melodic CV is tonal
- **Oscillators / complex oscillators**: as the sound source
- **Envelope generators**: very important, because Vertex’s CV behavior is a big part of its character
- **LFOs**: for stereo motion and slow phrase animation
- **Function generators**: for more unusual envelope shapes
- **Filters / wavefolders / FM inputs**: because Vertex can shape dual CV paths going to them
- **Stereo effects** after Vertex: delay, reverb, chorus, resonator

A particularly strong chain is:

**sequencer → oscillator/filter/voice → envelope → Vertex → stereo delay/reverb**

That gives you a melodic line with built-in spatial articulation before it hits effects.

---

## What Vertex does not do

Based on the manual, Vertex does **not** provide:

- pitch sequencing
- quantization
- note generation
- sample & hold melody creation
- transposition memory
- tuning utilities
- oscillation or sound generation

So if your goal is specifically “create melodies,” Vertex needs to be paired with at least one of:

- sequencer
- keyboard/controller
- random source + quantizer
- oscillator/voice module

---

## Summary

The Vertex is best used in melodic music as a:

- **stereo animator** for mono melodic voices
- **voltage-controlled panner**
- **dual CV VCA** for shaping modulation tied to melodic phrasing
- **envelope sculptor** that can create apparent loudness and articulation differences between left and right
- **performance tool** for balancing two melodic voices or two modulation streams

Its most musically distinctive trick is that **overdriving the gain CV clips the control shape rather than boosting above unity**, which lets you create **different apparent envelope shapes** across a stereo image. That makes melodies feel wider, more dimensional, and more expressive without just turning one side up.

If you want, I can also turn this into a **“patch cookbook”** with:
1. **beginner melodic patches**,  
2. **ambient melodic patches**, and  
3. **techno / sequenced melodic patches**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)