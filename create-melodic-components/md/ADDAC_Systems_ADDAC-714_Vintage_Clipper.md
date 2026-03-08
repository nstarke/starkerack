# ADDAC Systems — ADDAC-714 Vintage Clipper

- [Manual PDF](../../manuals/ADDAC714_VintageClipper_A_0.pdf)

---

[ADDAC714 Vintage Clipper User’s Guide (PDF)](attachment)

# ADDAC714 Vintage Clipper — using it for melodic components

The attached manual covers **one module**:

- **ADDAC714 Vintage Clipper** — dual-channel soft clipper / saturator

So this isn’t a full voice by itself, but it’s very useful **with oscillators, filters, VCAs, envelopes, sequencers, and mixers** to shape melodic lines, harmonics, dynamics, and stereo character.

## What the module does

From the manual:

- **Dual channel** clipping
- **Passive diode clipping** with a fixed-knee, vintage-style response
- Built-in **3.3 kHz low-pass character filter**
- **Bypass switch per channel**
- **Gain** control sets how much clipping happens
- **Symmetry switch**:
  - **Up = symmetrical clipping**
  - **Down = unsymmetrical clipping**
- **Output gain** per channel
- **Clip LED** per channel
- **Input 1 is normalled to Input 2**
  - great for dual-processing one source in parallel

## Why this matters for melody

A clipper can help melodic parts by:

- making simple waveforms sound richer and more present
- adding harmonic content so sequences cut through a mix
- controlling peaks on plucks or basslines
- creating parallel contrast between two versions of the same melody
- emphasizing note articulation through different clipping amounts
- turning plain sine/triangle sources into more musically complex tones

Because the ADDAC714 is **dual channel** and **Input 1 normals to Input 2**, it is especially good for **parallel melodic processing**.

---

# Best ways to use ADDAC714 for melodic patches

## 1. Add harmonics to a basic VCO melody

**Patch:**

- VCO saw / triangle / sine → **Input 1**
- **Output 1** → VCA → mixer
- Sequence pitch from your sequencer as normal
- Shape amplitude with envelope + VCA

**Settings:**

- **Bypass up** = active
- Start with **Gain low to medium**
- Set **Output** to match bypassed level
- Try:
  - **Symmetry up** for more balanced harmonic enhancement
  - **Symmetry down** for more character and edge

**Result:**

- A simple melodic line gains body and attitude
- Sine and triangle waves become much more usable for leads
- Saw and pulse waves become denser and more “finished”

This is one of the easiest ways to make a melody sound more record-ready without changing the actual notes.

---

## 2. Use the two channels as parallel tone layers

Since **Input 1 is normalled to Input 2**, you can plug one melodic source into Channel 1 and automatically feed both channels.

**Patch:**

- VCO or full voice output → **Input 1**
- **Output 1** → mixer left / voice A
- **Output 2** → mixer right / voice B or second mixer channel

**Suggested settings:**

- **Channel 1**: low gain, symmetrical clipping
- **Channel 2**: higher gain, unsymmetrical clipping

**Musical use:**

- Blend the two outputs together
- Pan them slightly apart for stereo width
- Keep one side clean-ish and the other more driven

**Result:**

- One melody becomes a layered melodic texture
- Great for leads, arps, and repeating sequences
- Lets you create a “main tone + grit layer” from one source

This is probably the most musically powerful feature of this module.

---

## 3. Create a more expressive lead by clipping after a filter

**Patch:**

- VCO → VCF → **ADDAC714 Input**
- ADDAC714 output → VCA → mixer

**Why this works:**

If the filter is already moving with an envelope or modulation, the clipper reacts differently as harmonics rise and fall. That means the melodic line becomes more animated.

**Tips:**

- Use a resonant low-pass or band-pass filter before the clipper
- Push filter output into clipping moderately
- Use **Output gain** to keep level under control

**Result:**

- Acid-like or vintage solo tones
- Notes speak more aggressively
- Filter movement becomes more obvious in the melody

---

## 4. Turn a clean pluck sequence into a punchy melodic line

**Patch:**

- Oscillator → LPG or VCA with snappy envelope → **ADDAC714**
- Output → mixer

**Settings:**

- Medium clipping
- Output adjusted so transients stay lively
- Try symmetrical first

**What happens:**

The clipper rounds and compresses the loudest part of each pluck while adding upper harmonics. This can make short melodic patterns sound more solid and percussive.

**Best for:**

- plucks
- bass arps
- sequenced ostinatos
- techno and electro melodies

---

## 5. Use unsymmetrical clipping for more character in melodies

The manual notes:

- **Symmetrical clipping**: odd and even harmonics
- **Unsymmetrical clipping**: odd harmonics only

Even if the exact harmonic description may feel a bit unconventional compared with some distortion theory discussions, the practical point is simple:

- **Symmetrical** sounds more balanced and stable
- **Unsymmetrical** sounds more skewed, characterful, and “vintage”

**For melodic use:**

- Use **symmetrical** for basslines that need solidity
- Use **unsymmetrical** for expressive leads or quirky sequences
- Compare both positions while the sequence is running

Some melodies suddenly “speak” better with one symmetry mode than the other.

---

## 6. Use one channel for the lead, one for the bass

Because it is dual-channel, the module can process **two independent melodic parts**.

**Patch:**

- Bass oscillator/submix → **Input 1**
- Lead oscillator/submix → **Input 2**
- Outputs to separate VCAs or mixer channels

**Use case:**

- Bass: lower gain, symmetrical clipping
- Lead: higher gain, unsymmetrical clipping

**Result:**

- Shared tonal family across both parts
- Bass stays firm
- Lead gets bite and presence

This is great if you want a track’s melodic content to feel sonically related.

---

## 7. Use it after a wavefolder or FM source to tame and focus melodies

If your melodic source is already complex:

- FM voice
- wavefolder output
- additive voice
- resonator voice

the ADDAC714 can act as a **finishing saturator**.

**Patch:**

- Complex voice → **ADDAC714**
- Output → mixer / delay / reverb

**Why useful:**

The built-in clipping plus low-pass shaping can smooth out excessive peaks and make bright tones sit better in a track.

**Result:**

- More controlled upper harmonics
- Better note consistency
- Complex melodies sound more intentional, less spiky

---

## 8. Create pseudo-stereo melodic distortion from one mono voice

Because one input can feed both channels:

**Patch:**

- Mono melodic voice → **Input 1**
- Ch1 output → left mixer channel
- Ch2 output → right mixer channel

**Settings:**

- Different Gain settings on each side
- Different Symmetry settings
- Similar output levels

**Optional:**

- Send each side to different delays or reverbs

**Result:**

- Wide stereo lead from a mono source
- Nice for ambient melodies, arps, and drones with pitch content

---

## 9. Use clipping to keep melodies audible at lower mix levels

A saturated signal often reads as louder and clearer in a mix even when actual level is not much higher.

**Practical use:**

If your melody is getting buried:

- Add moderate clipping
- Bring output level down so peak level stays controlled
- Compare in context with drums and bass

This often helps melodic parts sit in front without simply turning them up.

---

# Patch ideas

## Patch 1: Vintage lead voice

**Modules needed:**

- Sequencer
- VCO
- VCF
- Envelope
- VCA
- ADDAC714
- Delay/Reverb optional

**Patch flow:**

- Sequencer pitch → VCO 1V/oct
- Gate → envelope
- VCO → VCF
- VCF → ADDAC714 Input 1
- ADDAC714 Output 1 → VCA
- Envelope → VCA CV
- VCA → mixer

**ADDAC714 settings:**

- Bypass active
- Gain around 10–1 o’clock
- Symmetry down for character
- Output to unity or slightly boosted

**Sound:**

- expressive mono lead
- warm grit
- classic saturated melodic line

---

## Patch 2: Parallel clipped arp

**Modules needed:**

- Arp/sequencer
- Oscillator
- VCA
- Envelope
- Mixer
- ADDAC714

**Patch flow:**

- Oscillator → ADDAC714 Input 1
- Output 1 → mixer ch1
- Output 2 → mixer ch2
- If needed, VCA after each output or one VCA before the clipper depending on your system

**Settings:**

- Ch1: low gain, symmetrical
- Ch2: high gain, unsymmetrical
- Pan channels left/right

**Sound:**

- animated stereo arp
- one clean-ish layer + one dirty layer
- very effective with repeating melodic patterns

---

## Patch 3: Bassline enhancer

**Patch flow:**

- Bass VCO → filter → VCA → ADDAC714 → mixer

or

- Bass VCO → filter → ADDAC714 → VCA → mixer

Try both.

**Why order matters:**

- **Clipper before VCA**: distortion remains part of the voice before amplitude shaping
- **Clipper after VCA**: envelope dynamics hit the clipper more dramatically

**Recommended settings:**

- Symmetry up
- Gain moderate
- Watch clip LED and tune by ear

**Sound:**

- thicker bass melody
- more harmonics on small speakers
- tighter note consistency

---

## Patch 4: Two melodic voices, one module

**Patch flow:**

- Voice A → Input 1
- Voice B → Input 2
- Output 1 and Output 2 to separate mixer channels

**Use:**

- Voice A = bass sequence
- Voice B = upper counter-melody

**Benefit:**

You can give both melodic lines a similar saturation aesthetic while tailoring the clipping independently.

---

# Performance tips

## Use the Gain control like a tone threshold

The manual says Gain mostly works like a **threshold control for how much clipping is applied**.

That means:

- lower settings = mostly clean
- middle settings = harmonic enhancement
- high settings = obvious distortion/compression

For melody, the sweet spot is often **just before it sounds “too distorted.”**

## Use Output to level-match while auditioning

Because clipping changes apparent loudness, use the **Output** knob to match bypassed and active levels. This helps you judge whether the tone is truly better, not just louder.

## Watch the Clip LED, but trust your ears

The LED monitors output clipping, but musical clipping may sound good before or after the LED behavior suggests caution. For synth melodies, a little excess is often the point.

## Symmetry is a performance switch

Flip the symmetry switch while a sequence is running:

- one position may suit sustained notes
- the other may suit short staccato phrases

It can act like a quick “lead mode” or “bass mode” change.

---

# Where it works best in a melodic signal chain

## Great placements

- **After oscillator, before filter**
  - adds harmonics for the filter to shape
- **After filter**
  - turns filtered sweeps into more aggressive tones
- **After VCA**
  - emphasizes envelope-driven dynamics
- **On a submix of multiple oscillators**
  - glues a melodic stack together

## Less obvious but useful

- **Before delay**
  - repeats inherit the saturation
- **Before reverb**
  - richer harmonic tails
- **On a send/return path**
  - blend clipped melody in parallel with dry melody

---

# Strengths of the ADDAC714 for melodic use

- Dual channel = process two melodic parts or make parallel layers
- Normalled input = instant split from one voice
- Simple controls = fast live performance use
- Built-in tonal shaping from the passive low-pass behavior
- Good for turning clean tones into musically rich ones

# Limitations

This module is **not**:

- a sound source
- a pitch generator
- a VCA
- a filter with CV control
- a wavefolder with voltage control

So for melody creation, it depends on pairing with other modules. Its role is **voicing, enhancement, saturation, and layering**.

---

# Best “used together” recommendations

Since only this manual was attached, “used together” mainly means using the two channels together, or using the module with a standard melodic voice chain.

## Most useful combinations

1. **Oscillator + envelope + VCA + ADDAC714**
   - basic lead or bass enhancement

2. **Oscillator + filter + ADDAC714**
   - richer subtractive melodies

3. **One oscillator into both channels of ADDAC714**
   - parallel melodic coloration

4. **Bass voice on Ch1, lead voice on Ch2**
   - unified track character

5. **ADDAC714 into delay/reverb**
   - saturated melodic ambience

---

# Quick recipe cheatsheet

## For bass melody
- Symmetry: **Up**
- Gain: **Low-medium**
- Output: match level
- Goal: thickness and presence

## For lead melody
- Symmetry: **Down**
- Gain: **Medium-high**
- Output: slightly backed off
- Goal: bite and expressiveness

## For arp
- Ch1 low gain, Ch2 higher gain
- Pan apart
- Goal: width and motion

## For plucks
- Medium clipping
- Output conservative
- Goal: punch and note definition

---

# Summary

The **ADDAC714 Vintage Clipper** is best understood as a **melodic tone-shaping and parallel saturation tool**. It won’t generate melodies by itself, but in a Eurorack patch it can make melodic material:

- richer
- louder-feeling
- more harmonically dense
- more characterful
- more mix-ready
- wider through dual-channel parallel processing

Its strongest melodic trick is feeding **one voice into Input 1** and using **both channels differently** to create layered lead, bass, or arp textures.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)