# Bubblesound — HexVCA

- [Manual PDF](../../manuals/bubblesound.pdf)

---

[Manual PDF](https://www.bubblesound-instruments.com)

# Using the Bubblesound HEXvca for Melodic Eurorack Patching

The attached manual page is for the **Bubblesound HEXvca**, a **6-channel VCA and mixer** designed for both **audio and CV**. While it is not itself a sound source or sequencer, it is extremely useful for building **melodic structures** when paired with oscillators, envelopes, sequencers, LFOs, and trigger sources.

## What the HEXvca does

Key features from the manual:

- **6 independent VCAs**
- **3 mix outputs**
  - channels **1–3**
  - channels **4–6**
  - channels **1–6**
- Each VCA has switchable **linear or exponential CV response**
- **DC-coupled**, so it works for:
  - **audio**
  - **CV**
- **Normalized CV inputs** via jumpers on the back, allowing one or two envelopes/gates to affect multiple VCAs
- Can connect to a **HEXar** via ribbon cable for trigger/control integration
- Uses **SSM2164** VCA chips
- Compact: **7HP**, **30mm deep**

## Why this matters for melodic patching

A VCA is one of the most important modules in a melodic system because it shapes:

- **note articulation**
- **dynamic phrasing**
- **accent patterns**
- **modulation depth**
- **layered voices**
- **CV animation**

Since the HEXvca has **six channels** and is **DC-coupled**, it can control not only the loudness of oscillator voices, but also the amount of pitch modulation, filter modulation, vibrato, envelope depth, or even sequencer-derived CV.

---

# Musical ways to use the HEXvca

## 1. Build a standard melodic voice with better articulation

A basic melodic patch:

- **VCO** → **filter** → **HEXvca input**
- **Envelope generator** → **HEXvca CV input**
- **Keyboard/sequencer pitch CV** → **VCO 1V/oct**
- **Gate/trigger** → **envelope trigger**

This gives you the normal “note opens and closes” function of a synth voice.

### Tip
- Use **exponential response** for more natural loudness shaping on audio.
- Use **linear response** if you want cleaner, more precise control, especially for CV.

---

## 2. Create multiple melodic voices from one sequencer

With six VCAs, you can run multiple sound sources in parallel:

- VCO A → VCA 1
- VCO B → VCA 2
- Noise/sub/secondary oscillator → VCA 3

Then mix them at the **1–3 mix output**.

This lets you make:

- **layered mono leads**
- **thicker basslines**
- **stacked intervals**
- **dual-oscillator melodies with controlled blend**

You can give each oscillator its own envelope amount or use the normalized CV setup so one envelope shapes several channels at once.

### Musical result
One melody line can become a rich, orchestrated patch with dynamic control over each component.

---

## 3. Voltage-control your melodic mix

Because the HEXvca has submix outputs, it can act like a **voltage-controlled mixer**.

Example:

- Oscillator 1 = root tone
- Oscillator 2 = fifth above
- Oscillator 3 = octave layer

Patch them into channels 1–3, then use separate CVs to animate each level.

This allows:

- intervals fading in and out over time
- evolving chord-like single-note lines
- changing harmonic emphasis per note
- accents that bring in extra upper harmonics

This is great for **melodic techno**, **ambient arpeggios**, and **Berlin-school style sequencing**.

---

## 4. Use VCAs on modulation sources to shape pitch movement

Since the HEXvca is **DC-coupled**, you can use it on CV signals.

Example patch:

- LFO or envelope → HEXvca input
- Sequencer accent or envelope → HEXvca CV input
- HEXvca output → oscillator FM input or pitch modulation destination

Now the modulation amount changes over time.

### Musical uses
- vibrato only on certain notes
- pitch envelope only on accented steps
- controlled glide-like movement
- animated melodic instability

This is one of the best ways to make repetitive melodic lines feel alive.

---

## 5. Control transposition and melodic variation

You can also VCA-control **sequencer CV** before it reaches another destination.

Example:

- Secondary CV source (offset sequence, random voltage, slow envelope) → HEXvca input
- Gate pattern or envelope → HEXvca CV input
- HEXvca output mixed with main pitch CV

This can create:

- occasional melodic jumps
- accent-dependent transposition
- phrase-end rises
- selective addition of ornamentation

This is especially useful when you want a melody to feel composed rather than mechanically looped.

---

## 6. Make accents more musical

Classic accents are not just louder notes—they often also affect timbre and modulation depth.

With multiple HEXvca channels, one accent signal can control several things at once:

- VCA 1 = amplitude of the voice
- VCA 2 = filter envelope amount
- VCA 3 = FM amount
- VCA 4 = sub oscillator level

If the same accent envelope is normalized across channels, accented notes can become:

- louder
- brighter
- more harmonically complex
- more animated

This is a very effective way to add expression to melodic sequences.

---

## 7. Animate parallel melodic lines

If you have several melodic sources:

- main sequence
- transposed copy
- oscillator drone tuned to scale degree
- counter-line from another sequencer

you can run each through a different VCA and dynamically blend them.

The mix outputs make it easy to create:

- one submix for the lead
- another for accompaniment
- one combined output for recording or final processing

This supports more structured melodic composition inside the rack.

---

## 8. Pairing with the HEXar

The manual mentions ribbon-cable integration with the **HEXar**. Even without the HEXar manual page here, the implication is that the two are designed to work together efficiently, reducing front-panel patching.

If the HEXar is providing gates/triggers for multiple channels, then together they can form a very performance-friendly rhythmic/melodic control system:

- HEXar triggers multiple envelopes
- envelopes open HEXvca channels
- different oscillators or CV sources are mixed and articulated
- grouped outputs create melodic layers or voices

This could be especially powerful for:

- trigger-based melodic percussion
- arpeggiated voice switching
- multi-lane note articulation
- pseudo-polyphonic patches

---

# Practical melodic patch examples

## Patch 1: Dynamic mono lead

**Goal:** a more expressive single-note melody

- Sequencer pitch CV → VCO 1V/oct
- VCO saw output → filter → HEXvca ch. 1 input
- Gate → envelope
- Envelope → HEXvca ch. 1 CV
- HEXvca output → mixer/output

Add:
- LFO → HEXvca ch. 2 input
- Accent gate/envelope → HEXvca ch. 2 CV
- HEXvca ch. 2 output → VCO FM or filter CV

Result:
- the melody has normal articulation on ch. 1
- ch. 2 adds modulation only on selected notes

---

## Patch 2: Interval melody mixer

**Goal:** one melody that blooms into harmonized notes

- Main pitch CV → VCO 1
- Main pitch CV + precision adder offset → VCO 2
- Main pitch CV + octave offset → VCO 3
- VCOs into HEXvca channels 1, 2, 3
- Separate envelopes or modulation CVs into each VCA CV input
- Use mix output 1–3

Result:
- a melody that shifts between unison, fifths, and octaves
- harmonic density can change note by note

---

## Patch 3: Accent-driven melodic timbre

**Goal:** accents that reshape the whole note

- Oscillator → filter → HEXvca ch. 1
- Filter envelope CV source → HEXvca ch. 2
- FM source or wavefolder CV source → HEXvca ch. 3
- Accent envelope multed or normalized to control channels 1–3
- Outputs sent to their destinations, or audio mixed from the submix

Result:
- accented notes are louder and also brighter or more aggressive
- repeated melodic phrases feel much more intentional

---

## Patch 4: Controlled random ornamentation

**Goal:** melody with occasional variations

- Random stepped CV → HEXvca ch. 4 input
- Trigger pattern for selected notes → HEXvca ch. 4 CV
- HEXvca ch. 4 output mixed with pitch CV path via utility mixer

Result:
- only some notes receive random pitch decoration
- useful for generative melodic lines that still feel constrained

---

# Best roles for the HEXvca in a melodic system

The HEXvca is especially strong as:

- **voice amplitude control**
- **CV depth control**
- **submixer for layered oscillators**
- **accent distributor**
- **modulation animator**
- **performance mixer for melodic layers**

It is less about generating melody directly, and more about making melodic material feel:

- expressive
- dynamic
- layered
- articulated
- evolving

In practice, this means the HEXvca is a **core support module** for melodic composition in Eurorack.

---

# Summary

The **Bubblesound HEXvca** helps create melodic components by giving you six channels of control over both **audio and CV**, plus mix buses for combining related signals. In a melodic patch, it can:

- shape note loudness
- blend layered oscillators
- add harmonized intervals
- control modulation depth
- distribute accents across several parameters
- create evolving melodic phrasing

If you combine it with oscillators, envelopes, a sequencer, and possibly the **HEXar**, it becomes a very powerful module for turning simple note patterns into rich, musical phrases.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)