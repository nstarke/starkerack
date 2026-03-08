# 2hp — Unity

- [Manual PDF](../../manuals/2hp_Unity.pdf)

---

[Manual PDF](#)

# Unity — melodic patch ideas and how to use it musically

Based on the attached manual, **Unity** is a **dual 3-input unity/averaging mixer** with smart output normalling, so it can behave as:

- **two 3-to-1 mixers**, or
- **one 6-to-1 mixer** if **Out 1 is left unpatched**

It has three gain modes:

- **Averaging mode**: each input at **1/3 gain**
- **Unity mode**: each input at **1x gain**
- **Split mode**:
  - top mixer = **unity gain**
  - bottom mixer = **1/3 gain**

Because it mixes either audio or CV, this is very useful for **melodic generation**, especially when combining sequencers, quantizers, envelopes, LFOs, offsets, and transposition voltages.

---

## What Unity does well in a melodic system

Unity is not itself a pitch source, oscillator, or quantizer. Its role is to **combine voltages**. In melodic patching, that means it is ideal for:

- **adding transposition to a sequence**
- **blending multiple modulation sources into pitch movement**
- **creating stepped melodic variation from several CVs**
- **mixing related audio voices into a single melodic line**
- **building a larger 6-source modulation mix**
- **combining “main melody + ornament + drift”**

In practice, Unity becomes a **pitch-control hub**.

---

## Key behaviors that matter musically

## 1. Unity Mode for pitch and melodic CV

In **Unity Mode**, each input is passed at full level. This is the most important setting for melodic CV, because pitch voltages generally need to preserve their original scale relationships.

Use this when combining:

- a sequencer pitch CV
- a keyboard CV
- a slow transpose voltage
- a vibrato LFO
- a random stepped voltage
- an envelope adding pitch bend

### Example
If you patch:

- Input 1: main sequence
- Input 2: slow offset/transposition CV
- Input 3: small LFO

Then **Out 1** becomes:

**sequence + transpose + vibrato**

That output can go to a **quantizer** or directly to a **1V/oct input**, depending on how controlled you want the melody to be.

---

## 2. Averaging Mode for combining related CVs more gently

In **Averaging Mode**, each input is attenuated to **1/3**. This is described in the manual as ideal for audio because it preserves relative loudness, but it can also be musically useful for CV when you want to **blend sources without large pitch jumps**.

This is especially good for:

- mixing several LFOs into a subtle pitch contour
- combining random voltages into a softer melodic movement
- layering several transposition sources without overdriving pitch range

### Example
Patch into the top mixer:

- stepped random
- triangle LFO
- envelope

In averaging mode, the sum is smoother and smaller than in unity mode. Send that to a quantizer and you get a **coherent melody generator** from simple sources.

---

## 3. Split Mode for simultaneous pitch CV and audio mixing

In **Split Mode**:

- top mixer runs at **unity gain**
- bottom mixer runs at **1/3 gain**

This is a very practical live-patching mode.

### Why this matters
You can use:

- **top section** for **melodic CV**
- **bottom section** for **audio voice summing**

That means one Unity can support a complete melodic lane:

- top: combine pitch-related CV
- bottom: combine audio from oscillators, sub-oscillators, or parallel sound sources

### Example melodic voice chain
**Top mixer**
- sequencer CV
- keyboard transpose CV
- vibrato LFO  
→ **Out 1 to oscillator 1V/oct or quantizer input**

**Bottom mixer**
- oscillator saw
- sub oscillator
- FM side tone  
→ **Out 2 to VCA/filter/audio path**

This makes Unity useful as a compact “control + tone” support module.

---

## 4. Cascading / normalling for 6-source melodic control

The manual notes:

- **If Out 1 is not patched**, the top mix is internally sent to the second mixer.
- Then **Out 2** contains the bottom three inputs **plus** the top three inputs.

So Unity can become a **6-input summing mixer**.

This is extremely useful for melodic CV construction.

### 6-way melodic control example
Patch all six inputs with:

1. main sequencer
2. octave transpose CV
3. slow random voltage
4. envelope pitch bend
5. sine LFO vibrato
6. manual offset or second sequencer

Leave **Out 1 unpatched** and take the result from **Out 2**.

Now you have a single “meta melody CV” made from six elements.

Best use cases:

- feeding a **quantizer**
- feeding a **precision adder downstream**
- feeding a voice for experimental melodies

Because Unity is not a precision adder, it’s best thought of as a **creative CV combiner**, especially before quantization.

---

# Melodic patch recipes

## 1. Sequence + transpose + vibrato

**Goal:** a stable melody with motion

**Patch**
- Unity in **Unity Mode**
- Input 1: sequencer pitch CV
- Input 2: offset or keyboard CV for transpose
- Input 3: slow sine LFO
- Out 1: to quantizer or oscillator pitch input

**Result**
A sequence that can be transposed and gently animated.

**Tip**
If the vibrato is too wide, attenuate it before Unity.

---

## 2. Random melody generator

**Goal:** evolving melodic phrases

**Patch**
- Unity in **Averaging Mode**
- Input 1: stepped random CV
- Input 2: slow triangle LFO
- Input 3: envelope or decay CV
- Out 1: to quantizer
- Quantizer out: to oscillator 1V/oct

**Result**
The quantizer turns the mixed CV into notes. Averaging mode keeps it from becoming too wild.

---

## 3. Call-and-response melody mix

**Goal:** merge two melodic sources

**Patch**
- Unity in **Unity Mode**
- Input 1: sequencer A
- Input 2: sequencer B
- Input 3: gate-derived accent envelope to nudge pitch
- Out 1: quantizer

**Result**
A more complex composite melody. If one sequencer is slower, it acts like a transposition contour over the other.

---

## 4. Ornamenting a bassline

**Goal:** add small melodic detail to a stable line

**Patch**
- Input 1: bass sequence
- Input 2: very small fast envelope
- Input 3: subtle LFO
- Unity Mode or Averaging Mode depending on intensity
- Out 1: oscillator 1V/oct or quantizer

**Result**
Your bassline gains slides, pushes, and micro-ornaments.

---

## 5. Six-source generative melody

**Goal:** one dense melodic control signal

**Patch**
Leave **Out 1 unpatched**.

Top inputs:
- sequencer
- random stepped voltage
- slow envelope

Bottom inputs:
- transpose CV
- LFO
- manual offset

Take **Out 2** to a quantizer.

**Result**
A deep, evolving melodic CV made from six sources.

---

## 6. One side CV, one side audio

**Goal:** build one complete melodic voice with a single module

Use **Split Mode**.

### Top section for pitch
- sequence CV
- transpose CV
- vibrato

→ Out 1 to oscillator pitch

### Bottom section for audio
- oscillator waveform 1
- oscillator waveform 2
- noise/sub layer

→ Out 2 to filter or VCA

**Result**
One half shapes the notes, the other half shapes the timbre/body of the melodic voice.

---

# Best companions for Unity in melodic patching

Unity becomes most musical when paired with other module types:

## Sequencers
Use Unity to combine:
- main pitch line
- secondary sequence for transposition
- accent-derived pitch movement

## Quantizers
This is one of the best pairings.
Since Unity sums voltages freely, a quantizer after it turns mixed CV into usable scales and melodies.

## LFOs and function generators
These add:
- vibrato
- pitch drift
- bends
- phrase contour

## Random / sample-and-hold modules
These create:
- generative melodies
- note variation
- pseudo-counterpoint

## Keyboards, pressure, or manual CV sources
Great for:
- live transposition
- expressive pitch changes
- performance interaction

## Oscillators and voice chains
Bottom section can sum audio sources while top section sums pitch CV in split mode.

---

# Practical musical advice

## Use Unity Mode for pitch accuracy
If you are mixing a sequencer with transposition CV, **Unity Mode** is usually the right choice.

## Use Averaging Mode before a quantizer
If the mix gets too extreme, average the sources and let the quantizer impose note structure.

## Use Split Mode in compact systems
This is probably the most performance-friendly setup:
- top = CV
- bottom = audio

## Watch pitch range
Three full-strength CVs summed together can create very large voltage swings. If that causes melodies to jump too far:
- attenuate inputs before Unity, or
- send the result to a quantizer

## Remember the output normalling
Leaving **Out 1 empty** turns Unity into a 6-input mixer. This is one of the module’s most powerful melodic uses.

---

# Summary

**Unity** is a compact but very useful melodic utility. It helps create melody not by generating notes itself, but by **combining the voltages that define melody**.

Its strongest melodic roles are:

- **adding transposition to sequences**
- **mixing vibrato and pitch modulation**
- **combining random and structured CV**
- **feeding quantizers with richer composite voltages**
- **supporting a full voice by handling CV on one side and audio on the other**
- **building 6-source generative pitch mixtures via output normalling**

In a Eurorack system, this makes Unity a small but powerful **melody-shaping tool**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)