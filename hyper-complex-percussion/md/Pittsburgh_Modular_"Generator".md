# Pittsburgh Modular — "Generator"

- [Manual PDF](../../manuals/Generator - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF / source](https://pittsburghmodular.com/generator)

# Pittsburgh Modular Generator for dense, hyper-complex percussion

The **Pittsburgh Modular Generator** is basically a **dual analog FM percussion voice / chaotic modulation source**. Based on the manual, it is especially strong for:

- **FM-based drum synthesis**
- **Metallic percussion**
- **Clicks, zaps, knocks, toms, woodblock-like tones**
- **Nintendo / zipper / atonal digital-ish artifacts**
- **Self-patched rhythmic modulation**
- **Layered pseudo-polyrhythmic motion** from interacting oscillator rates

It is **not a precision melodic oscillator**:
- it uses **exponential CV**
- it **does not track 1V/oct**
- it is **not temperature compensated**

That makes it less ideal for strict tonal sequencing, but **excellent for percussion, texture, unstable FM hits, and rhythmically animated drum voices**.

---

## What the module gives you for percussion

From the manual:

- **2 oscillators**
- **Oscillator 2 is internally FM’d by Generator 1 Index Out**
- **External FM input** can be routed to either oscillator
- **Shape control** continuously shifts both oscillators between triangle/square relationships
- **Index section** is effectively a **VCA on Generator 1 output**
- **Index CV** allows envelopes to dynamically control the amount of Generator 1 sent to:
  - the **Index OUT**
  - and therefore the **internal FM amount to Oscillator 2**

That means Generator is perfect for **transient-controlled FM percussion**, where the attack of an envelope changes not just loudness but **spectral violence**.

---

# Core concept for complex percussion

The key to using Generator for dense rhythm is:

1. Treat **Generator 2** as the **main struck body / resonant drum tone**
2. Treat **Generator 1** as the **modulator / transient exciter**
3. Use **Index CV** with envelopes, gates, bursts, euclidean triggers, or clock divisions to create **different FM bursts per hit**
4. Use the **External FM input** for a second modulation layer from:
   - another oscillator
   - clocked stepped CV
   - a random source
   - a trigger/gate stream
   - even Generator 2 itself

This gives you **nested rhythmic behavior**:
- amplitude contour from your VCA/envelope
- FM contour from Index CV
- waveform contour from Shape modulation
- cross-rhythm from external modulation routing

---

# Important behavior to exploit

## 1. Oscillator 2 is the “main percussion body”
Because **Generator 2 is internally FM’d by Generator 1 Index Out**, it naturally becomes the oscillator that gets the most animated timbral strikes.

Use Generator 2 for:
- main audio output
- metallic hits
- tom/drum cores
- unstable bell-ish percussion
- aggressive click-noise impacts

## 2. Generator 1 is both a sound source and FM driver
Generator 1 can do two jobs:
- be heard directly via output **1**
- act as the internal FM source via the **Index** section

This is very useful for layered percussion:
- **Out 2** = body
- **Index Out** = transient layer / brighter attack layer / second voice
- **Out 1** = pre-VCA raw modulator tone for further processing

## 3. The Index knob is inverted in function
The manual states:

- **Full left = 100% gain**
- **Full right = 0% gain**

And:
- turn **full right** to get the **full effect of CV input**
- turn **full left** to force **100% regardless of CV**

This is crucial.

### Practical meaning:
- If you want **dynamic FM per trigger**, set the **Index knob mostly right**
- Then patch an **envelope or trigger-derived CV** into **Index CV**
- That way each hit can have different FM intensity

This is one of the best features for percussion because you can make every transient uniquely sharp.

---

# Best patch roles in a rhythm system

## As a dedicated percussion voice
Use it as:
- kick-ish FM thud
- tom
- metallic snare layer
- glitch percussion
- industrial hi-hat / clang source
- zappy fill voice

## As a modulation engine for other percussion
At low or mid rates it can provide:
- asymmetric LFO-like modulation
- audio-rate FM bursts
- unstable waveform modulation
- rhythmic audio-rate CV for filter pings, LPGs, VCAs, or wavefolders

## As a dual-layer percussion generator
Because you have:
- output **1**
- output **2**
- **Index Out**

you can derive multiple related percussion layers from one module.

---

# Patch strategies for dense rhythmic music

## 1. Classic FM drum patch
This follows the spirit of the manual’s patch example.

### Patch:
- Take **Output 2** as your main audio
- Patch an **envelope** into **Index CV**
- Set **Gen 1** to **low**
- Set **Gen 2** to **mid**
- Tune fine frequency knobs by ear
- Run **Output 2** into a VCA or LPG
- Trigger the envelope from your rhythm sequencer

### Result:
- short envelope = clicky/zappy
- medium decay = tom/conga/woodblock
- higher FM amount = metallic/industrial
- lower FM amount = more drum-like

### Make it denser:
Use different trigger streams for:
- the amplitude envelope
- the Index CV envelope

For example:
- VCA envelope on a 5-step loop
- Index envelope on a 7-step loop

This creates **timbral polyrhythm**, even if the audible hits occur in a simpler meter.

---

## 2. Polyrhythmic transient vs body patch
Use separate rhythmic structures for:
- **when the sound happens**
- **when the FM spikes happen**

### Patch:
- Main audio: **Output 2**
- Envelope A to VCA: triggered every quarter-note subdivision in one meter
- Envelope B to **Index CV**: triggered by a different clock division / euclidean pattern

### Example:
- VCA opens on a 4-step repeating pattern
- Index CV fires on a 5-step euclidean pattern

### Result:
Some hits are:
- clean
- some are metallic
- some are explosive
- some are dull

This creates the feeling of **complex percussion phrasing without needing a separate voice for each variation**.

---

## 3. Audio-rate self-patched chaos percussion
The manual explicitly gives an external FM path with attenuverter and destination switch.

### Patch:
- Patch **Output 2** into **External Input**
- Set destination switch to **Generator 1**
- Listen to **Index Out** or **Output 2**
- Modulate **Index CV** with envelopes
- Adjust the external FM attenuverter around center

### Why it works:
Now Osc 2 modulates Osc 1 externally, while Osc 1 internally influences Osc 2 through the Index path.

This creates:
- recursive FM interaction
- unstable attack spectra
- pseudo-noise bursts
- very sharp mechanical percussion

### Best for:
- glitch snares
- bit-crushed-sounding zaps
- electro percussion
- IDM fills

---

## 4. Three-output layered drum architecture
Generator is unusually useful because it effectively gives you multiple related outputs.

### Use:
- **1** = raw Generator 1
- **2** = Generator 2
- **Index Out** = post-VCA Generator 1

### Patch idea:
- **Output 2** -> lowpass gate = body
- **Index Out** -> highpass/filter/VCA = click/attack
- **Output 1** -> wavefolder/distortion = noisy edge

Trigger different VCAs/envelopes for each layer with different pattern lengths.

### Result:
One module becomes a **multi-layer composite drum**:
- sub/body
- attack
- metallic tail

That is excellent for dense arrangements because one trigger can generate a very articulated hit.

---

## 5. Irregular meter patch
For complex time signatures, use Generator as a timbrally responsive voice rather than trying to force pitch sequences.

### Example rhythm structure:
- Main triggers in **11/8**
- Index accents in **7**
- Shape modulation in **5**
- External FM bursts in **3**

### Patch:
- Trigger envelope to VCA in 11-step pattern
- Trigger another envelope to **Index CV** in 7-step pattern
- Modulate **Shape** slowly with a 5-step sequencer or stepped random
- Send a clocked CV/gate source to **External Input** routed to Gen 1 or Gen 2 at a 3-step cycle

### Result:
The drum voice evolves through a long composite cycle.
Even if the hit rate is constant, the **spectral identity** of each hit keeps shifting, which is exactly what makes advanced rhythmic music feel alive.

---

# Making it punchy and percussive

## 1. Use very short envelopes into Index CV
The Index path is your friend for attack design.

Short envelope into **Index CV** gives:
- FM spike at the front of the sound
- bright attack
- percussive knock
- “stick hit” sensation

Longer envelope gives:
- metallic tail
- laser tom
- unstable sustained clang

For punch:
- keep Index envelope **fast attack**
- short to medium decay
- use VCA envelope shorter than the FM decay for hard impacts

---

## 2. Tune oscillator ranges strategically
Manual notes:
- 3-way range switch per oscillator
- left = low
- center = high
- right = mid

### Useful combinations:
- **Gen1 low / Gen2 mid** = strong percussion starting point
- **Gen1 low / Gen2 high** = sharper metallic/hat-like
- **Gen1 mid / Gen2 low** = unstable drum bass / tearing low percussion
- **Gen1 high / Gen2 high** = noisy digital chirps, tiny hits, harsh ticks

For hyper-detailed drums, don’t just think “pitch” — think:
- body oscillator range
- modulator oscillator range
- ratio instability

---

## 3. Exploit the shape knob as a percussion macro
From the manual:
- full left:
  - Gen1 = square
  - Gen2 = triangle
- full right:
  - Gen1 = triangle
  - Gen2 = square

That means one knob changes both oscillators in opposite ways.

### For percussion:
- more **triangle** = rounder, more fundamental
- more **square** = brighter, buzzier, more upper harmonics

### Technique:
Perform or sequence the **Shape** knob/CV externally if possible through recording passes or manual moves:
- left for round body with edgy modulator
- right for buzzy body with softer modulator

This is very effective for creating contrast across polyrhythms:
- one repeating phrase with one shape area
- another phrase with shape shifted
- resample multiple passes

---

## 4. Use trigger/gate signals as FM sources
The manual says external input accepts **CV and audio-rate signals**.

A trigger or gate patched into **External Input** can create abrupt frequency spikes.

### Patch:
- Clock divider or burst generator -> External Input
- Destination to Gen1 or Gen2
- Use attenuverter to control polarity/amount

### Result:
- click injection
- knock transients
- stepped pitch smears
- broken-machine accents

This is especially good for:
- compound meters
- ratchets
- tuplets
- accent systems independent of hit timing

---

## 5. Use the attenuverter for asymmetrical motion
The external FM control is an **attenuverter** and zeros at **12 o’clock**.

This is extremely useful because:
- positive FM amount gives one family of attacks
- negative/inverted FM amount gives another

So a rhythm source modulating external FM can feel totally different depending on polarity.

### Technique:
For one section:
- slight negative FM for woody, sucked-in attacks

For another:
- positive FM for more explosive metallic edges

This gives variation without repatching.

---

# How to build polyrhythms and complicated patterns with this module

Generator itself is not a trigger sequencer, so the complexity comes from **how you drive it**. The best method is to separate rhythm into layers:

## Layer 1: hit timing
Use your main trigger sequencer for when the drum sounds.

## Layer 2: timbral accents
Use a different sequencer/clock division to control:
- Index CV
- external FM input
- waveform changes
- VCA amplitude variation

## Layer 3: modulation timing
Patch unrelated clocked CV into:
- External Input
- oscillator EXP inputs
- downstream filter cutoff / wavefolder / VCA decay

This way the ear hears:
- one pattern as the hit structure
- another pattern as the spectral structure
- another as the accent structure

That is how you get **apparent hyper-complex rhythm** from one voice.

---

# Specific advanced patch recipes

## A. 5:7 metallic drum cycle
### Patch:
- Output 2 to VCA/audio out
- 5-step trigger pattern to amplitude envelope
- 7-step trigger pattern to Index CV envelope
- Gen1 low, Gen2 mid
- Shape around center-right
- Index knob mostly right for CV responsiveness

### Sound:
A repeating drum line where only some hits flare into metallic tones, making a composite 35-step phrase before full repetition.

---

## B. 4-against-3 glitch percussion
### Patch:
- Straight 16th-note pulse to VCA envelope
- Triplet clock or /3 pattern to External Input
- Route external FM to Gen1
- Patch Output 2 into External Input for partial self-mod if you want more aggression
- Listen to Index Out

### Sound:
Steady pulse with rotating glitch emphasis, useful for broken techno, IDM, or footwork-style syncopation.

---

## C. Complex snare from one module
### Patch:
- Output 2 = body
- Index Out = crack
- Output 1 = noisy ring
- Mix all three externally
- Give each its own envelope/VCA/filter if possible

### Settings:
- Gen1 high or mid
- Gen2 mid
- Index CV short decay
- Shape toward square-rich side
- Add external trigger burst to FM input

### Sound:
Snare-like composite with:
- transient crack
- metallic shell
- noisy tail

---

## D. Euclidean tom network
### Patch:
- Euclidean pattern A triggers VCA envelope for Output 2
- Euclidean pattern B triggers Index CV
- Euclidean pattern C sends stepped CV to Gen2 EXP
- Shape manually set or slowly modulated

### Sound:
Toms that seem to play independent rhythmic roles even though they come from one synthesized source.

---

## E. Broken hi-hat / digital tick voice
### Settings:
- both oscillators high
- shape toward square emphasis
- short VCA envelope
- short, sharp Index CV
- trigger/gate into external FM input

### Sound:
Harsh, alias-like, hat/tick/chirp sounds that are perfect for fast polymetric detail layers.

---

# Performance tips

## Use Output 2 and Index Out together
This is one of the best live strategies:
- **Output 2** for the stable core
- **Index Out** for aggression

Mute/unmute or crossfade them during performance to create:
- dry drum
- FM-heavy accent version
- fills
- breakdown transitions

## Ride the Index knob live
Because the Index knob changes how much Generator 1 is sent onward, it acts like a **timbral intensity macro**.

Live movement can shift a part from:
- woody percussion
- to clanging FM
- to shrieking unstable noise

## Sweep the range switches for fills
Changing oscillator range between low/mid/high can produce dramatic phrase transitions:
- low for drum fill
- mid for tom/bell
- high for glitch spray

Very effective for end-of-bar accents.

---

# Best supporting modules to pair with Generator

To get the most out of Generator for hyper-complex percussion, pair it with:

- **Trigger sequencer** with polymeter/euclidean capability
- **Burst generator**
- **Clock divider / multiplier**
- **Multiple envelopes**
- **VCAs/LPGs**
- **Filter or resonant lowpass**
- **Wavefolder/distortion**
- **Sequential switch**
- **Sample and hold / stepped random**
- **Logic module** for combining rhythms

Especially useful:
- one envelope for amplitude
- one envelope for Index CV
- one modulation source for external FM
- one VCA or LPG after the audio output

---

# Practical workflow for dense percussion tracks

## If you want “composed complexity”
Program:
- hit pattern in one meter
- Index accents in another
- external FM changes in another
- shape changes by section

This gives repeatable complexity.

## If you want “alive machine complexity”
Self-patch:
- Output 2 to External Input
- Trigger bursts to Index CV
- Slight random CV to EXP
- Shape near unstable sweet spots

This gives organic, chaotic, evolving percussion.

## If you want “punchy club percussion”
Keep it disciplined:
- short VCA envelope
- short Index envelope
- low/mid oscillator settings
- filtered Output 2 for body
- lightly mixed Index Out for click

---

# Summary

The **Pittsburgh Generator** is excellent for **dense, advanced percussion music** because it combines:

- **2 oscillators**
- **internal FM routing**
- **external FM routing**
- **a CV-controlled Index/VCA stage**
- **shared waveform morphing**

Its real strength is not conventional melody but **rhythmically controlled timbral variation**. For polyrhythms and complex time signatures, the best approach is to let one pattern decide **when the hit occurs**, and let other unrelated patterns decide:

- how much FM it gets
- which oscillator is disturbed
- how sharp the transient is
- how bright or square the waveform is

That creates the illusion of many interacting percussion voices from a single module.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)