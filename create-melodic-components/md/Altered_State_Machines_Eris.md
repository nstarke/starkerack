# Altered State Machines — Eris

- [Manual PDF](../../manuals/Eris _ Altered State Machines.pdf)

---

[Manual PDF / Product Page](https://alteredstatemachines.net/eris)

# Using the Altered State Machines Eris to Create Melodic Components

From the provided manual, the module shown is:

- **Altered State Machines Eris**
- **4×4 matrix mixer**
- **DC-coupled**, so it can mix both **audio** and **CV**
- Up to **4× gain per channel**
- Includes an **Aux input/output**
- Aux is summed with **Output 1** and can be softly muted
- Rear switch for **unity or x2 gain** on Aux input

Because Eris is DC-coupled and has a true matrix architecture, it is especially useful for building **melodic control structures**, not just audio submixes. In a melodic Eurorack patch, Eris can act as a **CV router, pitch combiner, transposition hub, feedback mixer, or voice distributor**.

---

## What Eris does musically

A 4×4 matrix mixer means:

- You have **4 inputs**
- You have **4 outputs**
- Each input can be sent to **any or all outputs**
- The amount sent is controlled by a knob at each crosspoint

So in melodic use, you can treat Eris as a way to combine and distribute:

- pitch CV
- envelopes
- LFOs
- sequencer rows
- offsets
- random voltages
- audio oscillators

This makes it useful for creating melody by **mixing pitch sources**, **sending related variations to multiple voices**, and **creating movement around a central tonal idea**.

---

## Best melodic uses for Eris

## 1. Create harmonized pitch lines from one or more sequencers

If you patch pitch-related CV into several inputs, Eris can create multiple related melodic outputs.

### Example patch
Inputs:
- **Input A**: main pitch sequencer
- **Input B**: slow offset CV or precision adder output
- **Input C**: random stepped voltage
- **Input D**: envelope or LFO for pitch animation

Outputs:
- **Output 1**: main voice pitch
- **Output 2**: second oscillator pitch
- **Output 3**: bass voice pitch
- **Output 4**: transposed lead or FM index control

### Result
Each output becomes a different weighted combination of the same sources. That means:

- Voice 1 can play the basic melody
- Voice 2 can play a related intervallic variation
- Voice 3 can get a simplified or lower-register version
- Voice 4 can become a more animated melodic derivative

This is one of the strongest uses of Eris: **turning a few CV sources into a family of melodies**.

---

## 2. Build a modulation matrix for melodic motion

The manual explicitly says Eris can be used as a **modulation matrix**, and this is very important for melodic work.

Patch in modulation sources such as:

- a slow triangle LFO
- a stepped random source
- an envelope
- a sequencer lane

Then send them in different amounts to destinations like:

- oscillator 1 pitch
- oscillator 2 pitch
- filter cutoff
- wavefolder amount

### Why this helps melody
Melody is not just note order. It also comes from:

- slight pitch drift
- phrase-based transposition
- varying brightness
- changing articulation

Eris lets one modulation source influence several melodic voices in different proportions. That creates **coherence**, which is often more musical than using unrelated modulation everywhere.

---

## 3. Use it as a pitch variation network

Since Eris is DC-coupled, one very practical use is **mixing pitch CV**. This lets you create:

- transpositions
- interval stacks
- octave shifts
- unstable melodic variants

### Example
Inputs:
- **A**: quantized melody
- **B**: +1V offset
- **C**: slow random CV
- **D**: keyboard or pressure CV

Outputs:
- **Out 1**: original melody
- **Out 2**: melody + octave
- **Out 3**: melody + small random deviation
- **Out 4**: melody + performance control

If your downstream oscillators need accurate 1V/oct tracking, you’ll usually want to send Eris outputs into a **quantizer** or carefully calibrate your scaling by ear, since matrix mixers are creative tools first and precision utilities second.

Still, for melodic composition, this is extremely powerful.

---

## 4. Generate chord-like structures across several voices

Eris can distribute one melodic CV source to several voices while adding different amounts of supporting voltages.

### Patch concept
Inputs:
- **A**: root melody
- **B**: fixed interval offset
- **C**: another interval offset
- **D**: slow macro modulation

Outputs:
- **1**: root
- **2**: root + interval 1
- **3**: root + interval 2
- **4**: root + animated extension

Run each output into a separate quantizer channel or separate oscillators, and you get **parallel melodic structures** that can resemble chords, counterpoint, or clustered harmony.

This works especially well for:
- triads spread across three oscillators
- drone + melody combinations
- canon-like pitch relations
- evolving harmonic beds

---

## 5. Morph between melodic roles in performance

Because Eris has knobs at every routing point, it is highly playable.

You can perform melody changes by:
- bringing one sequencer into several outputs
- fading in random voltage to destabilize pitch
- reducing one modulation path while increasing another
- moving a bassline into a lead register structure

This is especially useful in live techno, ambient, and experimental patches where melody evolves by **mix balance** rather than by replacing sequences.

---

## 6. Use the Aux path as a melodic layer return or drone injection

The manual says:

- the **Aux input** is summed with **Output 1**
- then both are sent to the **Aux output**
- there is a **mute** for the Aux input
- Aux gain can be set to **unity or x2**

This suggests a few melodic uses.

### A. Bring in a drone or second melodic line
Patch:
- Main melodic mix on Output 1
- Drone oscillator, sub voice, or effect return into Aux input
- Use Aux mute to softly bring the extra layer in and out

This is excellent for:
- introducing a fifth or octave drone
- adding reverb-returned melody
- dropping in a secondary motif without clicks

### B. Feedback-based melodic coloration
If you have an effect that emphasizes pitch, like:
- delay
- resonator
- shimmer reverb
- tuned feedback path

you can send Eris output to that effect and return it to the Aux input. Since Aux is summed with Output 1, this creates a **melodically reinforcing return path**.

### C. Percussive melodic accent
The manual mentions using Aux to mix a kick with the main signal, but for melodic work you could instead use it for:
- plucked voice accents
- a bass reinforcement line
- a manually introduced counter-melody

The clickless mute makes this ideal for performance.

---

## 7. Create cybernetic feedback melodies

The manual specifically mentions use in a **cybernetic feedback circuit**.

In melodic terms, this can mean:

- sending a pitch-related or audio signal through effects
- returning it into Eris
- cross-mixing it with modulation or oscillators
- allowing the system to influence itself

### Melodic applications
- self-evolving semi-tonal loops
- unstable resonant melodies
- pitch-fed-back filtered sine structures
- recursive transpositions

If you use feedback with pitch CV, be careful. Small changes can become extreme quickly. But with controlled amounts, Eris can create **organic, evolving melodic systems** that sound less programmed than a typical sequencer patch.

---

## 8. Multi-voice distribution from one melodic source

One of the simplest but strongest uses:

- Send one sequencer into Input A
- Route it to all four outputs in different amounts
- Add one or two other CV sources across the matrix
- Feed outputs to four oscillators, or to oscillator pitch plus timbral destinations

This turns a single melody into:
- lead
- harmony
- bass
- ornament

That is a very “musician-friendly” use of Eris in a compact system.

---

# Practical melodic patch recipes

## Patch 1: Four related melodies from one sequence

**Inputs**
- A: main sequencer CV
- B: stepped random
- C: slow triangle LFO
- D: manual offset voltage

**Outputs**
- 1: lead voice pitch
- 2: bass voice pitch
- 3: pluck voice pitch
- 4: modulation to wavefolder or filter

**How to set it**
- Send A strongly to outputs 1, 2, 3
- Add a little B to outputs 2 and 3
- Add C to output 3 only
- Add D to output 1 for live transposition

**Musical result**
A coherent melodic ecosystem: one recognizable line, one variation, one animated ornament.

---

## Patch 2: Matrix-generated harmony

**Inputs**
- A: quantized root melody
- B: offset representing a harmonic interval
- C: another interval offset
- D: envelope or phrase CV

**Outputs**
- 1: root
- 2: third/fifth-related line
- 3: higher extension
- 4: expressive transposition

**Tip**
Use quantizers after Eris if you want the harmonic relationships to stay locked to a scale.

---

## Patch 3: Live melodic performance hub

**Inputs**
- A: sequencer row 1
- B: sequencer row 2
- C: pressure or joystick CV
- D: random source

**Outputs**
- 1: lead pitch
- 2: bass pitch
- 3: filter contour CV
- 4: FM or wavefold amount

**Performance method**
Use the matrix knobs like a mixing desk for composition:
- fade from row 1 into row 2
- inject pressure into pitch
- add random only at phrase endings
- create breakdowns by stripping outputs back to one source

---

## Patch 4: Aux-based melodic overlay

**Main path**
- Build your central melodic voice at Output 1

**Aux path**
- Send a second oscillator, drone, or effected return to Aux input
- Take Aux output as your final melodic sum
- Use mute switch for clean entry/exit

**Result**
A second musical layer appears and disappears smoothly, ideal for:
- choruses
- breakdown transitions
- ambient widening
- lead reinforcement

---

# Strengths of Eris for melody

- **DC-coupled**, so it works with pitch and modulation CV
- **4×4 matrix format** encourages related, structured variation
- **Gain up to 4x** can amplify weak control sources
- **Aux path** adds a performable melodic layer or return
- Good for both **precise composition** and **experimental generative patching**

---

# Things to watch out for

## 1. Pitch precision
Matrix mixers can be used for pitch CV, but if you need exact tonal intervals, you may want:
- a quantizer after the outputs
- carefully tuned offsets
- testing by ear with your oscillators

## 2. Gain staging
Since each channel can amplify up to 4x, it is easy to push CV or audio beyond expected ranges. That can be useful, but be intentional.

## 3. Feedback caution
For cybernetic/feedback patches, start with low levels. Melodic feedback can become noisy or unstable very fast.

---

# Conclusion

Even though Eris is presented as a matrix mixer, it is very well suited to **melodic patch design** in Eurorack. Its biggest strength is not simply mixing signals, but creating **families of related control voltages and audio layers**. That makes it valuable for:

- harmonized voices
- melodic variation
- transposition systems
- modulation matrices
- live melodic performance mixing
- feedback-based generative melody

If you pair it with sequencers, quantizers, oscillators, and effects, Eris can become the central “relationship builder” that turns a few simple sources into rich melodic structures.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)