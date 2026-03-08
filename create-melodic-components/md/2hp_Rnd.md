# 2hp — Rnd

- [Manual PDF](../../manuals/2hp_Rnd.pdf)

---

[Manual PDF](#)

# Using 2hp Rnd to Create Melodic Components

The attached manual is for the **2hp Rnd**, a compact random voltage and random gate generator. Even though it is a single module, it can contribute a lot to melodic patching when paired with common Eurorack building blocks like quantizers, VCOs, envelopes, VCAs, clock sources, and sequencers.

## What Rnd does musically

Rnd provides three main outputs/functions:

- **Quant Output**: stepped random voltage, changing on each clock pulse
- **Smooth Output**: continuously moving random voltage
- **Gate Output**:
  - internal clock mode: steady clock output
  - external clock mode: random gates

This makes it useful for generating:

- random melodies
- evolving pitch modulation
- rhythmic note triggering
- probabilistic variation in phrases

## Important behaviors from the manual

### 1. Internal vs External clock
The **INT/EXT switch** changes the module’s behavior:

- **Internal**
  - the module runs from its own clock
  - **Rate knob** sets internal clock speed
  - **Clock jack** becomes CV control for internal rate
  - **Gate out** sends a steady 50% duty cycle clock

- **External**
  - **Clock jack** becomes a clock input
  - **Quant output** updates on incoming clock pulses
  - **Gate out** emits random gates
  - **Rate knob** controls the probability / rate behavior of those random gates
  - **Smooth output** still changes at a speed determined by the Rate knob

### 2. Two independent random voltages
The manual states the **quantized and smooth outputs are completely independent**. That is very useful musically, because one can drive pitch while the other shapes timbre, transposition, or articulation.

### 3. Output range
Both random voltage paths have attenuators and can be adjusted from **0V to 10V**. That wide range is important, because for melodic use you will often want to reduce the range before sending it to a pitch input or quantizer.

---

# Best melodic uses

## 1. Random melody source into a quantizer
The most direct melodic patch:

**Patch**
- Rnd **Quant Output** → external **quantizer** input
- Quantizer output → VCO **1V/oct**
- Rnd **Gate Output** or another clock/gate source → envelope → VCA

**Why it works**
- The Quant Output generates a new stepped random voltage on each clock pulse
- A quantizer forces those random voltages onto a scale
- Result: random but musical notes

**Tip**
Since Rnd can output up to 10V, use the **Quant attenuator** to limit melodic range before the quantizer. Lower settings give tighter, more phrase-like melodies.

---

## 2. Use internal clock for self-running melodies
Because Rnd has its own internal clock, it can act like a self-contained melodic idea generator.

**Patch**
- Set switch to **INT**
- Rnd **Quant Output** → quantizer → oscillator pitch
- Rnd **Gate Output** → envelope trigger
- Envelope → VCA / LPG

**Musical result**
- The module clocks itself
- Every internal pulse creates a new pitch
- The gate output provides matching rhythmic triggers

This is great for:
- generative ambient lines
- aleatoric sequences
- quick self-playing patches

---

## 3. Use external clock to lock randomness to your track
For more musical control, clock it from your system master clock, trigger sequencer, or clock divider.

**Patch**
- Master clock / sequencer clock → Rnd **Clock Input**
- Set switch to **EXT**
- Rnd **Quant Output** → quantizer → VCO pitch
- Rnd **Gate Output** → envelope trigger or logic module

**Why this is useful**
- Notes now change in sync with the rest of your patch
- Random gates add variation without drifting out of time
- Great for techno, IDM, generative pop, and modular rhythm structures

---

# Melodic patch ideas

## Patch 1: Simple generative lead
**Modules needed**
- Rnd
- quantizer
- VCO
- envelope
- VCA
- filter optional

**Patch**
- Rnd Quant Out → quantizer in
- Quantizer out → VCO 1V/oct
- Rnd Gate Out → envelope gate in
- Envelope out → VCA CV
- VCO out → VCA in → mixer/output

**How to play it**
- In **INT mode**, use the **Rate knob** to choose melody speed
- Adjust **Quant attenuator** for note range
- Select a quantizer scale like minor pentatonic for always-pleasant results

**Result**
A fully autonomous random melody voice.

---

## Patch 2: Evolving melody with drifting transposition
Use both outputs together.

**Patch**
- Rnd **Quant Out** → quantizer → VCO pitch
- Rnd **Smooth Out** → attenuator/offset module → add to quantizer transpose input or oscillator FM very lightly
- Clock externally or internally

**Musical result**
- Quant Out creates note changes
- Smooth Out slowly bends or transposes the melodic center
- Feels like the melody is wandering through different tonal zones

This is one of the best uses of Rnd because the two random algorithms are independent.

---

## Patch 3: Random melody plus probabilistic rhythm
In **EXT mode**, the Gate output becomes random.

**Patch**
- Master clock → Rnd Clock In
- Rnd Quant Out → quantizer → oscillator pitch
- Rnd Gate Out → envelope trigger
- Optional: mult the master clock to another voice for comparison

**Musical result**
- Pitches update with the clock
- Notes only sound when random gates fire
- Creates rests and syncopation automatically

This is excellent for making melodies less rigid.

---

## Patch 4: Use Smooth output as a melodic source through a sample & hold or quantizer
Although Smooth is continuous, you can still make it melodic.

**Option A**
- Rnd Smooth Out → quantizer → oscillator pitch

This gives constantly shifting pitch, but may glide unpredictably depending on the quantizer behavior.

**Option B**
- Rnd Smooth Out → sample and hold input
- Clock source → sample and hold trigger
- Sample and hold out → quantizer → oscillator pitch

**Result**
- Smooth becomes a slowly evolving source from which discrete notes are sampled
- This often sounds more “composed” than pure stepped randomness

---

## Patch 5: Call-and-response with two voices
If you have two oscillators or two voices:

**Voice A**
- Rnd Quant Out → quantizer → VCO A pitch

**Voice B**
- Rnd Smooth Out → another quantizer or sample/hold/quantizer chain → VCO B pitch

**Rhythm**
- Use Rnd Gate Out for one voice
- Use a regular clock or divided clock for the other

**Result**
One voice sounds stepped and phrase-like, while the other sounds more fluid and unstable. Together they create a layered melodic texture.

---

# Practical musical strategies

## Constrain the voltage range
Because Rnd outputs **0–10V**, raw output can span a huge pitch range. For melody, that often means too many octaves.

Use the onboard attenuators to:
- keep melodies within 1–2 octaves
- reduce wild jumps
- make phrases feel intentional

This is probably the single most important technique when using Rnd melodically.

## Add a quantizer if you want tonal results
The manual calls one output “Quant,” but from the description it means **stepped random voltage**, not necessarily scale-quantized to musical notes. If you want melodies in key, use an external quantizer.

## Use external clock for arrangement-friendly melodies
If you want the random melody to sit inside a song structure:
- drive Rnd from Pamela’s, a sequencer clock, Tempi, etc.
- use clock divisions for slower pitch changes
- reset other modules around it for repeatable larger structures

## Pair smooth and stepped outputs
A very strong melodic workflow is:
- **Quant output** = note selection
- **Smooth output** = timbre, transpose, filter cutoff, wavefold amount, FM depth, or vibrato depth

That keeps the melody coherent while giving it motion.

---

# Example complete melodic system roles

## Rnd as a melody generator
- Quant Out provides note CV
- Gate Out provides note triggers
- Internal clock makes it autonomous

## Rnd as a variation generator for a sequencer
- Main sequencer handles core melody
- Rnd Smooth or Quant modulates:
  - transpose input
  - sequence direction probability
  - quantizer root note
  - VCO timbre

## Rnd as a probabilistic ornament source
- Main melody comes from a sequencer
- Rnd Gate Out in **EXT mode** creates occasional extra triggers
- Rnd Quant Out feeds a second oscillator for fills or ornament notes

---

# Strengths of Rnd for melodic patching

- Very small footprint: **2HP**
- Can operate as a self-running melody seed
- Can sync to external clocks
- Independent smooth and stepped random voltages
- Built-in gate output supports note articulation
- Wide voltage range allows both broad and tightly constrained melodic motion

# Limitations to be aware of

- It is not a full sequencer
- It does not store repeatable note patterns
- For tonal music, you will usually want an **external quantizer**
- For refined melodic phrasing, additional utilities help a lot:
  - attenuators
  - offsets
  - sample & hold
  - logic
  - sequential switches
  - clock dividers

---

# Best pairings for melodic use

Rnd works especially well with:

- **Quantizer**: turns random voltages into scales
- **VCO / voice module**: receives pitch CV
- **Envelope + VCA/LPG**: shapes notes from gate output
- **Clock divider/multiplier**: changes melodic pacing
- **Sample & hold**: turns smooth motion into stepped notes
- **Sequential switch**: alternate between random and programmed melodies
- **Mixer/offset utility**: tame voltage ranges and transpose

---

# Summary

The **2hp Rnd** is best thought of as a compact melodic unpredictability source. Its **Quant Output** is ideal for stepped note generation, its **Smooth Output** is perfect for slow melodic drift or expressive modulation, and its **Gate Output** can provide either a regular pulse or random rhythmic articulation depending on clock mode.

For melodic music, the most effective setup is:

1. **Quant Out → quantizer → oscillator pitch**
2. **Gate Out → envelope trigger**
3. **Smooth Out → timbre or transpose modulation**

That patch gives you an evolving, musical, and controllable generative voice.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)