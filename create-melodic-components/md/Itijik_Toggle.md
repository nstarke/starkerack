# Itijik — Toggle

- [Manual PDF](../../manuals/toggle.pdf)

---

[Manual PDF](#)

## itijik Toggle — melodic use in a Eurorack patch

The **itijik Toggle** is a **quad flip-flop / logic inverter** module. On its own, it does not generate pitch CV directly, but it is very useful for building **melodic structures** by creating:

- stepped rhythmic logic
- divided/toggled gate streams
- alternating note triggers
- simple binary patterns
- complementary gate lines for harmony and call/response

Because there are **4 identical sections**, you can create several related gate patterns at once and use those to drive sequencers, quantizers, envelope generators, switches, or sample-and-holds that *do* produce melodic voltages.

## What the module does musically

Each section has:

- **SET**: forces OUT high
- **RST**: forces OUT low
- **CLK**: toggles OUT on each pulse
- **IN**: external logic input to the inverter side
- **OUT**: main flip-flop output
- **VERT**: inverted logic output

Important behavior:

- If **IN is unpatched**, **VERT is the inverse of OUT**
- If **IN is patched**, that normalization breaks, and **VERT becomes the inversion of the signal at IN**

So each channel can act as:

1. a **toggle latch**
2. a **gate alternator**
3. a **binary pattern source**
4. a **logic inverter**

## Best ways to use Toggle for melody

### 1. Alternating notes from one clock
Patch a steady clock into **CLK** of one section.

Result:

- **OUT** goes high, low, high, low...
- **VERT** does the opposite

Use these two outputs to trigger two different melodic events:

- **OUT** → envelope for voice A
- **VERT** → envelope for voice B

Then send different pitch CVs to the two voices, or use one voice with two different timbral states. This gives a simple **back-and-forth melody**.

### 2. Drive a sequential switch for pitch alternation
Use **OUT** from one Toggle section to advance or control a switch module.

Patch idea:

- Clock → Toggle **CLK**
- Toggle **OUT** / **VERT** → switch control or trigger
- Two different pitch CV sources → switch inputs
- Switch output → oscillator 1V/oct

This creates a melody that alternates between two pitch sources every clock pulse.

### 3. Create binary melodic patterns
Since each section toggles state, multiple sections can be clocked at different rates or reset at different times to create longer patterns.

Example:

- Master clock to section 1 **CLK**
- Section 1 **OUT** clocks section 2
- Section 2 **OUT** clocks section 3

Now you have chained logic states that behave like a simple binary counter. Use these gates to:

- open different VCAs for different pitch rows
- select between quantized voltages
- trigger sample-and-hold events at different moments

This is great for **pseudo-sequencing** and **algorithmic melodies**.

### 4. Trigger sample-and-hold for stepped melodies
If you have a random or slowly changing CV source:

- random CV / LFO / noise → sample-and-hold input
- Toggle **OUT** or **VERT** → sample-and-hold trigger
- sample-and-hold output → quantizer → oscillator pitch

Because Toggle produces alternating gates, you can control **when notes are sampled**, making melodies more structured than plain random.

Use one section for the main trigger and another for occasional resets or alternate sampling moments.

### 5. Generate call-and-response phrases
Because **OUT** and **VERT** are complementary, they naturally split a rhythm into two opposite halves.

Patch:

- **OUT** → trigger melodic phrase A
- **VERT** → trigger melodic phrase B

Phrase A and B could be:

- two sequencers
- two rows of a sequencer
- two quantizer channels
- one voice transposed differently

This creates a very musical **question/answer** structure.

### 6. Force phrase starts with SET and RST
The **SET** and **RST** inputs make the module useful for controlled musical form.

For example:

- send a bar-reset pulse to **RST**
- clock into **CLK**

Now the alternating pattern always starts in a known phase at the beginning of the bar. This is very useful when using Toggle to control melody switching, because it keeps phrases aligned.

Use **SET** instead if you want the pattern to begin on the opposite state.

### 7. Invert gate logic for rests and accents
Patch a gate pattern into **IN** and use **VERT** as its inversion.

This is useful for melody generation because you can derive:

- note triggers from the original gate
- rests, accents, or alternate note lanes from the inverse

Example:

- sequencer gate pattern → **IN**
- **VERT** → trigger a second envelope or another pitch event only when the first pattern is silent

This can create interlocking melodies.

## Practical melodic patch ideas

## Patch 1: Simple two-note alternating melody
You need:

- clock
- Toggle
- two pitch voltages or a sequencer with two rows
- VCO
- envelope/VCA
- optional quantizer

Patch:

- Clock → Toggle channel 1 **CLK**
- Toggle **OUT** → trigger envelope A
- Toggle **VERT** → trigger envelope B or switch trigger
- Pitch source A and B → switch or mixer logic
- Final pitch CV → oscillator 1V/oct

Musical result:

- every other beat plays a different note source
- easy to make bassline + reply note patterns

## Patch 2: Four-stage logic melody selector
Use all four sections to build a more complex gate network.

Patch:

- Master clock → channel 1 **CLK**
- Channel 1 **OUT** → channel 2 **CLK**
- Channel 2 **OUT** → channel 3 **CLK**
- Channel 3 **OUT** → channel 4 **CLK**

Then use the outputs to control:

- 4 VCAs containing different fixed voltages
- or 4 switch inputs
- summed result → quantizer → oscillator pitch

Musical result:

- an evolving stepped voltage pattern
- simple binary melody generation
- especially good for minimal, Berlin-school, and generative patches

## Patch 3: Structured random melody
You need:

- random CV source
- sample and hold
- quantizer
- Toggle
- oscillator

Patch:

- Random CV → sample-and-hold input
- Clock → Toggle **CLK**
- Toggle **OUT** → sample-and-hold trigger
- Sample-and-hold out → quantizer → oscillator pitch
- Toggle **VERT** → envelope trigger for a second voice or accent lane

Musical result:

- notes are sampled in a repeating alternating structure
- randomness sounds more intentional and phrase-based

## Patch 4: Melody and harmony split
Patch one sequencer pitch line to two voices, but use Toggle to alternate which voice sounds.

- Clock → Toggle **CLK**
- **OUT** → envelope/VCA for voice 1
- **VERT** → envelope/VCA for voice 2
- Same pitch CV to both oscillators
- Offset or transpose voice 2

Musical result:

- one sequence becomes a **melody + harmony answer**
- especially effective if voice 2 is a fifth or octave above

## Patch 5: Resettable melodic phrases
Patch:

- Main clock → **CLK**
- Bar reset pulse → **RST**
- **OUT** → trigger sequencer A advance
- **VERT** → trigger sequencer B advance

Musical result:

- alternating phrase structure that always starts correctly at the top of the bar
- useful live, since resets keep your melodic logic predictable

## How Toggle works best with other modules

Toggle is most melodic when paired with:

- **quantizers** — to turn stepped or sampled voltages into scales
- **sample-and-hold modules** — to create notes from changing CV
- **sequential switches** — to alternate between pitch sources
- **clock dividers/multipliers** — for phrase timing
- **sequencers** — to gate different rows or channels
- **logic modules** — to combine Toggle states into more complex note patterns
- **fixed voltage sources / precision adders** — to create interval-based pitch changes

## Musical strengths of this module

For melody work, Toggle is especially good at:

- creating **alternation**
- producing **complementary gate streams**
- making **resettable phrase logic**
- deriving **binary and semi-generative structures**
- splitting one rhythm into two musical parts

It is less about directly writing a melody, and more about creating the **decision logic** that makes melodies evolve.

## Summary

The **itijik Toggle** is a logic utility that becomes a melodic tool when used to control:

- when notes happen
- which pitch source is heard
- which voice responds
- how phrases alternate and reset

Its strongest musical application is building **structured, rhythmic melody logic** from simple clocks and gates. If you pair it with a quantizer, switch, sequencer, or sample-and-hold, it can become the backbone of very musical generative patches.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)