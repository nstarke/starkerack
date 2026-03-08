# WMD SSF — DPLR

- [Manual PDF](../../manuals/DPLRmanual1.3.pdf)

---

[Manual PDF](attachment)

# WMD/SSF DPLR — using it for melodic components

The DPLR is a **dual/stereo delay** that can do much more than simple echo. From the manual, the key musical features are:

- **Delay time:** 40 ms to 700 ms
- **Two related delay outputs:** A and B
- **Spread control:** offsets B relative to A
- **Regen:** feedback amount
- **Amount:** wet level mixed with dry
- **XTALK modes:** cross-coupled feedback between A and B
- **Filter modes:** 4 low-pass flavors, from noisy/bright to darker/smoother
- **CV over delay, spread, and regen**

Because delay times fall into short rhythmic territory, DPLR is especially useful for creating **pitched rhythmic lines, canon-style repeats, ping-pong melodies, and self-generating melodic motifs**.

## What this module contributes melodically

A delay is not a pitch source by itself, but in a Eurorack patch it can become a **melody multiplier**:

- it turns one note into a **rhythmic phrase**
- it creates **call-and-response** between left/right or A/B outputs
- it can generate **interlocking note patterns**
- high feedback and short times can create **resonant pseudo-pitched material**
- modulation of delay/spread can animate a static melodic line into evolving counterpoint

## Important controls from a musical perspective

## 1. Delay Amount
Sets the base delay time for the input signal.

Musically:
- **Short settings**: tight slapback, comb-like coloration, pseudo-resonant tones
- **Medium settings**: rhythmic repeats that reinforce sequenced notes
- **Long settings**: spacious canons and staggered melodic echoes

## 2. Spread (B)
Offsets the B delay relative to A.

Musically this is huge:
- A can be your “main repeat”
- B can become an **offbeat echo**
- Different A/B timings create **polyrhythmic melodic reflections**
- In stereo, this becomes a **ping-pong phrase generator**

## 3. Regen
Sets feedback.

Musically:
- low regen = one or two supportive echoes
- medium regen = repeating motifs
- high regen = self-developing phrases and near-looping melodic cells

## 4. Amount
Wet/dry balance.

The manual notes this is **100% dry mixed with wet delay, max gain of 2**. So you can keep the original melodic line present while adding delayed harmonizing rhythm behind it.

## 5. XTALK modes
These are especially creative. XTALK determines how much of A feeds B and B feeds A in the feedback path.

Musically:
- no XTALK = two more independent delays
- some XTALK = melodic information “bleeds” between channels
- high XTALK = repeating phrases migrate between outputs, creating **countermelody**
- with stereo voices, this can feel like a melodic line is being reinterpreted each repeat

## 6. Filter modes
The four low-pass levels shape the repeats.

Musically:
- lighter filtering = brighter, more articulated melodic echoes
- heavier filtering = distant, background, dubby melodic tails
- filtering helps place repeats behind the main voice so they support melody instead of cluttering it

---

# Best melodic use cases

## 1. Turn a simple sequence into a fuller phrase
Patch a mono melodic voice into **IN**, then use:

- **OUT A** as the main delayed phrase
- **OUT B** as a second offset phrase via **SPREAD**

If your original sequence is sparse, DPLR can make it feel like a more complex composition by adding delayed “answer” notes.

### Patch idea
- Sequencer → oscillator → VCA/filter voice → DPLR IN
- Set **DELAY** to an eighth note-ish repeat by ear
- Set **SPREAD** to a dotted or slightly offset timing
- Keep **REGEN** low to medium
- Mix dry signal with OUT A and OUT B

Result:
- original note
- repeat on A
- offset repeat on B
- together these create a melodic lattice

This works especially well for:
- arpeggios
- plucked voices
- mallet/percussive synth tones
- short acid lines

---

## 2. Create stereo ping-pong melodies
The manual explicitly mentions **left/right ping-pong** via Spread.

### Patch idea
- Put a mono melodic line into DPLR
- Send **OUT A** left and **OUT B** right
- Set a noticeable **SPREAD**
- Raise **XTALK** to moderate levels
- Set moderate **REGEN**

Result:
- notes bounce between speakers
- repeats cross-feed
- the melody sounds wider and more active without changing the source sequence

This is excellent for:
- lead lines
- sequenced plucks
- ambient bell melodies

---

## 3. Build counterpoint from one voice
Because A and B can differ in timing and feed each other, DPLR can turn one melody into **quasi-counterpoint**.

### How
- Use a melody with rests or space
- Set A for a medium repeat
- Set B slightly longer or shorter via Spread
- Add moderate XTALK
- Add some feedback

Result:
- the same note material reappears at different times
- overlapping delays create the illusion of a second and third line
- if the source melody is simple, the delayed voices can sound like composed accompaniment

This is especially effective with:
- modal sequences
- pentatonic patterns
- slow generative melodies

---

## 4. Pseudo-harmonic layering
DPLR does not shift pitch, but rhythmic offset can imply harmony if your source line moves melodically.

For example:
- play a sequence with notes changing every step
- set delay so repeats land under later notes
- the old note and new note overlap

That overlap creates:
- intervals
- suspended tones
- moving harmonic tension

This is a classic way to get richer melodic/harmonic material from a single monophonic source.

Best settings:
- moderate wet mix
- short to medium delay
- moderate spread
- low to moderate feedback

---

## 5. Karplus-adjacent resonant behavior
At shorter times and higher feedback, delays can move toward resonant/plucked territory.

While the manual gives a minimum of **40 ms**, which is longer than classic Karplus-Strong string synthesis, you can still use short delay/feedback behavior for:
- tuned rhythmic resonance
- metallic pulse thickening
- note emphasis

This is less about exact pitch and more about turning a transient melodic line into a resonant percussive melody.

Try:
- short envelope plucks into DPLR
- short delay
- higher regen
- brighter filter mode first, then darker modes

---

# CV patching ideas for melodic animation

The manual confirms CV over:
- **DLY CV**
- **SPRD CV**
- **RGN CV**

These inputs make DPLR much more than a static effect.

## Modulate delay time slowly
Patch a slow LFO, stepped random, or envelope to **DLY CV**.

Musical result:
- delayed phrases breathe and stretch
- static sequences become evolving melodic textures
- subtle modulation gives chorus-like motion
- stronger modulation gives smeared, tape-like pitch movement on repeats

Best for:
- ambient melodies
- generative minimalism
- dub techno sequences

## Modulate spread for moving stereo rhythm
Patch an LFO or clocked stepped CV to **SPRD CV**.

Musical result:
- B output changes relationship to A over time
- offbeat echoes shift around the groove
- stereo phrases become less predictable
- great for turning one ostinato into several rhythmic variants

## Modulate regen for phrase density
Patch an envelope, random CV, or sequencer lane to **RGN CV**.

Musical result:
- some notes get one repeat, others bloom into many
- accents become melodic trails
- certain steps in a sequence can become “important” by leaving longer delay tails

This is one of the best ways to make a melody feel alive.

---

# Practical melodic patch recipes

## Recipe 1: Echo harmonizer feel
Goal: make a simple melody feel harmonized

- Voice output → DPLR IN
- Dry voice to mixer center
- OUT A and OUT B to stereo mixer
- Delay around short/medium
- Spread slightly offset
- Regen low
- Amount medium
- Filter moderate

Why it works:
repeats overlap with later notes, creating intervallic interplay.

---

## Recipe 2: Canon machine
Goal: one sequence becomes a round

- Feed a sparse melody or quantized random sequence to a voice
- Voice → DPLR IN
- Delay around one beat or near-beat by ear
- Spread to a second rhythmic value
- Regen medium
- XTALK medium-high

Why it works:
the same phrase returns in staggered time, almost like multiple players entering one after another.

---

## Recipe 3: Generative ambient melody cloud
Goal: evolving melodic wash from minimal material

- Use a slow random or 4–8 step melody
- Send to a soft voice: sine/triangle/FM bell/pluck
- Voice → DPLR
- Set longer delay
- Spread moderate
- Regen medium-high
- Filter darker
- Slowly modulate DLY CV and SPRD CV with separate slow sources

Why it works:
repeats smear into a melodic environment while preserving enough note definition to still feel tonal.

---

## Recipe 4: Ping-pong lead enhancement
Goal: widen a lead without losing the main melody

- Main lead voice → DPLR
- Delay set fairly short
- Spread clearly audible
- Regen low-medium
- XTALK low-medium
- Dry voice louder than wet

Why it works:
you keep the lead upfront while echoes create stereo motion and melodic reinforcement.

---

# How XTALK changes melodic behavior

This is the most distinctive feature on DPLR.

The manual says XTALK affects the **source of the regen signal**, moving from:
- **RED** = A→A and B→B
toward more crossfed feedback:
- more of A feeds B
- more of B feeds A

For melody, this means:

## Low XTALK
- cleaner repeats
- predictable A/B timing
- good for precise rhythmic accompaniment

## Medium XTALK
- notes begin to migrate across outputs
- more interlocking pattern behavior
- good for stereo melodies and counterpoint

## High XTALK
- feedback paths become more entangled
- phrases become less linear and more emergent
- good for generative and dubby melodic systems

If you want “composed” sounding echoes, stay lower.
If you want “self-creating” melodic interplay, raise XTALK.

---

# Filter choices for melody

The filter modes matter because delays can easily crowd a melodic patch.

Use:
- **lighter filtering** for crisp rhythmic repeats, arps, and plucks
- **heavier filtering** for supportive background echoes behind a main melody

A good rule:
- bright source + busy sequence = use more filtering
- simple sparse melody = use less filtering

---

# Best companion modules for melodic use

If you’re asking how this module can be used together with others for melodic work, DPLR pairs especially well with:

## Sequencers
Any step sequencer or quantized random source
- creates note material for DPLR to elaborate

## Quantizers
Useful if your melodic source is random or semi-random
- DPLR then turns quantized notes into richer phrases

## Function generators / envelopes
- strike plucks
- modulate regen for accents
- sweep delay time subtly

## VCAs and mixers
Essential for controlling dry/wet relationship and stereo placement.

## Filters / LPGs
Excellent before DPLR
- short filtered plucks create very clear delayed melodic structures

## Stereo output modules
To fully enjoy the A/B spatial behavior.

---

# Musical strategies

## Use sparse source material
DPLR shines when the input melody has room. Too many notes can blur into clutter.

## Let repeats land between notes
Tune delay and spread by ear so echoes fill gaps instead of landing exactly on every new note.

## Use feedback selectively
Too much feedback can overwhelm tonal clarity. For melodic work, moderate settings often feel most musical.

## Use darker filtering for accompaniment
If the delay is meant to support rather than dominate, darker repeats sit better.

## Modulate one parameter at a time
- delay for temporal drift
- spread for stereo rhythm
- regen for phrase emphasis

This keeps the melodic result intelligible.

---

# Summary

The **WMD/SSF DPLR** is best understood as a **melodic phrase expander** rather than just an effect. It can:

- turn a single melodic line into layered rhythmic counterpoint
- create stereo ping-pong note patterns
- overlap notes into implied harmony
- produce canon/round-like structures
- evolve a simple sequence into a generative melodic texture

Its most musically distinctive feature is the combination of:
- **A/B delay structure**
- **Spread**
- **XTALK cross-coupled feedback**
- **CV control over delay, spread, and regen**

That makes it especially strong for:
- ambient melody design
- dubby sequenced leads
- plucked arpeggios
- self-evolving generative music

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)