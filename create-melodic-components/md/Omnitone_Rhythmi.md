# Omnitone — Rhythmi

- [Manual PDF](../../manuals/Rhythmi_Information_Package.pdf)

---

[Manual PDF](attachment)

# Using Rhythmi to Create Melodic Components

Rhythmi is primarily a **drum sequencer**, but it has a few features that make it useful for building **melodic and quasi-melodic material**, especially when paired with other Eurorack modules.

## What in Rhythmi is melodic?

The key melodic feature is:

- **TOM CV output**
  - Outputs tom pitch
  - Tracks **1V/oct**
  - Quantized to a **minor pentatonic scale**

This means Rhythmi is not only generating triggers for percussion, but also a usable pitch control signal. That makes it possible to treat the tom lane as a kind of melodic sequencer.

## Core patch concept

Use Rhythmi as:

- a **rhythmic brain**
- a **trigger source**
- a **pitched CV source** via the TOM CV output

Then patch it into:

- an oscillator
- a percussive voice with pitch input
- a low pass gate
- a sampler
- a resonant filter ping setup
- a quantized melodic voice

## Best ways to extract melody from Rhythmi

### 1. Tom lane as a melodic sequencer

Patch:

- **TOM trigger out** → envelope or trigger input of a voice
- **TOM CV out** → 1V/oct input of an oscillator or synth voice

This turns the tom pattern into a melodic line. Since the TOM CV is quantized to minor pentatonic, it will usually sound musical immediately.

Why this works well:

- The tom rhythm is already pattern-based
- The **Energy** control tends to create tom activity near the end of the loop, so you naturally get melodic fills
- The manual says tom pitch is biased toward a **descending pattern near the end of the loop**, which is excellent for fill-like melodic phrases

This is one of the strongest hidden musical uses of the module.

---

### 2. Use the hi-hat gate output to articulate a melodic voice

The **HI-HAT output** produces:

- short triggers for closed hat
- longer gates for open hat

You can repurpose that as **articulation** for a melodic patch:

- **HI-HAT out** → envelope gate input / LPG strike input
- **TOM CV out** → pitch input of oscillator

This gives different note lengths depending on whether the pattern generates open or closed hats. So the hat lane can become a kind of phrasing generator for a melody.

This is especially nice for:

- plucky voices
- noise-plus-filter melodic textures
- LPG-based “bongo melody” patches

## Interaction of the major controls for melodic use

### Energy

Energy is extremely useful musically.

From the manual:

- It increases kick, snare, and tom density
- It introduces more variation
- It creates fills, especially with toms
- At higher levels, crash triggers at loop starts

For melodic use, this means:

- low Energy = sparse melodic notes
- medium Energy = more active riffs
- high Energy = dense fills and transitions

You can think of Energy as a **macro for melodic intensity**.

A great use:
- Send a slow CV or manually ride Energy during a performance
- Let the tom melody bloom during transitions

### Evolve

Evolve is the most compositionally interesting parameter.

It creates related rhythm variations that persist until changed. For melody, that means:

- the TOM trigger pattern changes in related ways
- the melodic contour can feel like variations on a theme
- you can move back to the root rhythm by reducing Evolve

Musically, Evolve behaves like:
- phrase mutation
- controlled recomposition
- branching variations

Patch idea:
- Keep TOM CV patched to an oscillator
- Use Evolve manually or via CV
- Generate new branches with the encoder press
- Return to zero Evolve to come back to the “home phrase”

That gives you a very playable melodic variation system without traditional step editing.

### Swing

Swing affects every second clock pulse and can push hits late, even beyond following syncopated hits.

For melodic material this is powerful because it can create:

- lazy or shuffled riffs
- displaced pentatonic motifs
- off-grid melodic fills

If the tom lane is driving a melodic voice, swing can make it feel much more human and animated.

### Length

Loop length ranges from **2 to 32 clock pulses**.

For melody:

- short lengths create repeating motifs
- longer lengths create evolving phrases

Especially useful trick:
- Set one melodic voice from TOM CV with a long loop
- Use shorter rhythmic phrases on other outputs
- This creates polymetric-feeling interplay even though it all comes from one sequencer

## Base patterns matter for melody

The manual explains that there are **5 base patterns**, and these determine the order in which hits appear as density increases.

This is very important for melodic use because the base pattern is effectively a **phrase skeleton**.

Changing base pattern changes:

- where notes first appear
- how the melody fills in as density rises
- whether the phrase feels backbeat-heavy, anticipatory, or more circular

So for melodic patching, base patterns are not just drum feel—they are also **note-order personality**.

Practical approach:
1. Set Evolve and Energy low
2. Dial in tom density/synco
3. Change base pattern by long pressing encoder
4. Listen for which one gives the most musical phrase shape
5. Then add Evolve and Energy

## Syncopation as melodic placement

Rhythmi’s **Synco** control for a piece sets the approximate ratio of on-grid vs off-grid hits.

For the tom lane, this means the melody can be:

- more anchored
- more syncopated
- more conversational against the beat

A melodic line with:
- low synco = stable, grounded riff
- high synco = offbeat hook or fill language

This is especially effective when the melodic voice is plucky or percussive.

## Strong melodic patch examples

## Patch 1: Pentatonic tom lead

- **TOM CV out** → oscillator 1V/oct
- **TOM out** → envelope trigger
- Envelope → VCA
- Oscillator → filter → VCA
- **Clock out** from Rhythmi → modulation reset or synced delay clock

Use:
- low tom density for sparse motifs
- medium Evolve for phrase variation
- higher Energy for fills

Result:
- an automatically varying minor pentatonic lead or riff

## Patch 2: LPG melodic percussion

- **TOM CV out** → tuned oscillator or resonator pitch
- **TOM out** → LPG strike
- Optional: mult **SNARE** or **HI-HAT** out to extra strikes
- Add reverb

Result:
- mallet-like melodic percussion
- naturally fill-oriented phrasing
- very good for ambient, dub techno, or generative grooves

## Patch 3: Hi-hat articulation with tom pitch

- **TOM CV out** → oscillator pitch
- **HI-HAT out** → envelope gate input
- Oscillator → VCA/LPG

Result:
- note lengths vary with open/closed hat behavior
- more expressive melodic articulation
- less obviously “tom-based”

## Patch 4: Crash as melodic phrase reset marker

At high Energy, the **CRASH output** triggers at the beginning of each loop.

Use it to:
- reset an LFO modulating oscillator timbre
- retrigger an envelope affecting filter cutoff
- clock a sequential switch for phrase changes

This lets the melody feel structured in larger phrases, not just note-by-note.

## Patch 5: Rhythmic sequencer for sampled melodic slices

- **TOM out** or **HI-HAT out** → sample trigger
- **TOM CV out** → sample pitch input or playback rate CV
- Use Evolve to mutate phrase rhythm

Result:
- chopped melodic fragments
- pseudo-sequenced vocal/sample riffs
- excellent for experimental or breakbeat-oriented music

## Using Rhythmi with another melodic module

Even though Rhythmi is not a traditional note sequencer, it pairs well with:

- analog oscillator voices
- quantizers
- sample players
- resonator voices
- physical modeling percussion
- LPG-based west coast voices

Especially good pairings would be modules that accept:

- trigger/gate
- 1V/oct
- accent/timbre CV

Then Rhythmi can provide:
- timing
- density
- groove
- phrase variation
- some pitch data

## Musical strengths of Rhythmi for melody

Rhythmi is best at melody when you want:

- **groove-first melodic writing**
- **generative fills**
- **variation without step programming**
- **pentatonic, percussive, phrase-based lines**
- **drum/melody hybrid behavior**

It is not ideal if you need:
- exact note entry
- harmonic chord sequencing
- precise scale selection beyond the built-in tom behavior

But it is excellent for:
- melodic percussion
- auxiliary riffs
- generative lead fragments
- call-and-response lines with drums
- evolving pentatonic hooks

## Best performance strategy

A good live workflow for melodic use:

1. Start with low **Energy** and low **Evolve**
2. Dial in tom **Density** and **Synco**
3. Choose a good **base pattern**
4. Patch **TOM CV** to a melodic voice
5. Add **Swing** for feel
6. Increase **Evolve** to explore phrase variations
7. Raise **Energy** to generate fills and transitions
8. Use **Crash** output as a macro phrase marker elsewhere in the patch

This makes Rhythmi function like a **groove-driven melodic variation instrument**, not just a drum sequencer.

## Bottom line

Rhythmi can create melodic components mainly through its **TOM CV output**, especially when paired with the **TOM trigger**, **HI-HAT gate behavior**, **Energy**, **Evolve**, and **base pattern** system. Its strength is in producing **organic, groove-locked, pentatonic melodic phrases and fills** rather than programmed note sequences.

So if you use it as the rhythmic and phrase-generation center of a patch, it can drive:

- melodic tom lines
- pentatonic leads
- tuned percussion
- generative fills
- articulated riffs
- phrase-synced modulation for larger melodic structure

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)