# Humble Audio — Quad Operator

- [Manual PDF](../../manuals/Quad Operator Manual.pdf)

---

[Quad Operator Manual PDF](https://www.dropbox.com/paper/doc/print/JsIQoU7GbeAboEJku9ZgE?print=true)

# Humble Audio Quad Operator: modulation ideas for aggressive percussion, basslines, and haunted pads

The **Quad Operator** is a 4-operator digital linear FM voice with a very flexible **modulation matrix**, variable operator **waveshapes** (sine → triangle → square → saw), per-operator **gain CV**, **self-modulation**, **cross-modulation**, **independent outputs**, and an **external audio-rate FM input**. That combination makes it much more open-ended than a fixed-algorithm FM synth.

The key to getting great sounds out of it is understanding a few things from the manual:

- In **lock state**, operators stay in **integer ratios** relative to the master pitch. This is where the most useful **harmonic FM** lives.
- In **free state**, each operator becomes an **independent oscillator** with its own tuning. This is where the module gets more unstable, clangorous, inharmonic, and wild.
- **Gain CV** is very important: it changes both:
  - the operator’s **audio output level**
  - and how strongly that operator modulates other operators through the matrix  
- The **AR FM input** lets you inject an **external audio-rate modulator** and route it to any/all operators with its own modulation sends.
- The module supports **self-FM**, which is excellent for grit, edge, tearing basses, and impact transients.
- The **Reset** input can force phase restart, which is especially useful for repeatable percussion and tempo-synced modulation shapes.

---

# First: the best mindset for patching this module

Think of each operator as simultaneously being:

1. **a sound source**
2. **a modulator**
3. **a VCA-controlled modulation source**

That means the most interesting patches usually come from modulating:

- **operator gain CV**
- **shape CV**
- **ratio CV**
- **external AR FM gain + send amounts**
- and switching between **lock/free use-cases**

If you only modulate pitch, you’ll get some movement.  
If you modulate the **amount of FM itself**, the module becomes much more animated and “alive.”

---

# General modulation strategies that work especially well on Quad Operator

## 1. Animate FM depth with envelopes, not just static knobs
Since **Gain CV** controls both output amplitude and modulation intensity, patching envelopes there creates very organic FM timbre motion.

This is one of the strongest features on the module.

### Try:
- Put one operator mostly as a **carrier** (the one you listen to)
- Use another as a **modulator**
- Send a **fast decay envelope** to the modulator’s **Gain CV**
- Set the modulation send from that modulator to the carrier

Result:
- The note starts bright/noisy/aggressive
- Then decays into a cleaner tone

That gives:
- punchy kicks
- snares
- plucks
- bass attacks
- evolving pad strikes

This is classic FM behavior, but here it’s especially intuitive.

---

## 2. Modulate shape slowly for spectral drift
Each operator can morph continuously through:
**sine → triangle → square → saw**

This is huge. In standard FM, changing the waveform of the modulator dramatically changes the sideband structure.

### Good uses:
- Slow random or triangle LFO into **Shape CV** for atmospheric textures
- Envelope into **Shape CV** for a bass that starts rounded and becomes buzzy
- Audio-rate modulation into **Shape CV** for unstable digital tearing textures

### Important note:
The manual warns that overtone-rich shapes plus FM can quickly become noisy/aliased.  
That’s not always bad — for distorted percussion and bass, that’s often exactly the point.

---

## 3. Use lock state for “designed” tone, free state for chaos
A very effective technique is:

- Start in **lock state** for harmonic, musically stable structure
- Introduce a single operator in **free state** as a destabilizer

This gives you the best of both worlds:
- fundamental pitch remains readable
- a rogue operator adds nasty, inharmonic edge

This is especially strong for:
- reese-like basses
- metallic attacks
- haunted drone pads
- industrial percussion

---

## 4. Self-modulation is your distortion engine
Because each operator can modulate itself, you can treat self-FM like a kind of internal waveshaping/distortion.

### Low self-mod:
- slight sharpening
- brighter harmonics
- more bite

### High self-mod:
- tearing digital distortion
- unstable transients
- noisy bass aggression
- broken percussion

For best results:
- modulate the operator’s **Gain CV** or the overall modulation source dynamically
- pair self-mod with **square/saw** shape for brutal textures
- pair self-mod with **sine/triangle** for more controllable growl

---

## 5. Use AR FM input as a fifth chaos source
The **AR FM input** is one of the coolest parts of the module.

You can patch in:
- another oscillator
- filtered noise
- a resampled drum loop
- a wavefolder output
- even one of Quad Operator’s own outputs for externalized feedback-style behavior

Then route that external source via **Mod 1–4** on the AR section.

### Excellent sources for AR FM:
- noise burst for snare texture
- a synced saw VCO for bass tearing
- a sub oscillator for wobble complexity
- another operator output for pseudo-feedback
- a harsh digital oscillator for screaming sidebands

Watch the **clipping LED** and use the AR gain control intentionally:
- moderate clipping = useful grit
- heavy clipping = crushed, broken, industrial tone

---

## 6. Use Reset for repeatable attacks and percussion
The **Reset CV** resets all operator phases.

For percussion and tight bass attacks, this matters a lot. Without phase reset, transients can vary from hit to hit. With reset:

- kicks hit more consistently
- FM toms sound more focused
- bass stabs feel tighter
- modulation can lock better to clocked events

Patch a trigger from your sequencer to **Reset** for percussion patches.

---

# Patch design ideas by sound category

---

# 1. Distorted percussive sounds

The Quad Operator should be very good for:
- kicks
- metallic toms
- snares
- rimshots
- digital hats
- broken industrial hits

The trick is to use **short envelopes on pitch and FM amount**.

## A. FM kick drum
### Setup
- Put all operators in **lock**
- Start with **sine shapes**
- Choose one operator as carrier, say **Op 1**
- Use **Op 2** to modulate **Op 1**
- Set Op 2 ratio to something simple like **2**, **3**, or **4**
- Send **Op 2 → Mod 1**
- Monitor **Op 1 out**

### Modulation
- Send a **fast pitch envelope** to **LF FM**
- Send a **very fast decay envelope** to **Gain CV of Op 2**

### Result
- Initial pitch snap from LF FM
- Initial click/thump brightness from FM burst
- Body settles into low sine-heavy tone

### To distort it
- Add slight **self-mod on Op 1**
- Move Op 2 shape toward **triangle or square**
- Increase Op 2 ratio for more smack/click
- Patch **Reset** from the trigger source

### For harder techno/industrial kicks
- Add **AR FM** with a short noise burst or clipped oscillator
- Route AR FM lightly to Op 1
- Let it just dirty the transient

---

## B. Snare / clap-like digital percussion
### Setup
- Carrier: **Op 1**
- Modulators: **Op 2 and Op 3**
- Op 2 ratio around **6–8**
- Op 3 ratio around **1 or 2**, or set one free for inharmonicity
- Use more angular shapes: **triangle/square/saw**

### Modulation
- Envelope to **Op 2 Gain CV** with short decay
- Envelope to **Op 3 Gain CV** with slightly longer decay
- Optional envelope to **Shape CV** of Op 1 or Op 2
- Use a noise source into **AR FM**
- Route AR FM mainly to Op 1 and maybe Op 2

### Result
- Body from lower modulator
- Rattle/noise from higher modulator + AR FM noise
- Shape CV creates “snap opens into sizzle”

### Make it more broken
- Put Op 3 in **free state**
- Slight self-mod on Op 1
- Push AR FM gain until clipping LED flickers

---

## C. Metallic percussion / FM toms / industrial hits
This module should excel here.

### Setup
- Carrier: Op 1
- Modulators: Op 2, Op 3
- Put at least one modulator in **free state**
- Tune by ear to non-integer relationships
- Use triangle or sine first, then push to square

### Modulation
- Very short decay envelopes to modulator gain CVs
- Trigger **Reset**
- Optional slow random to one modulator’s **shape CV**

### Result
- Bell/tom/metal strike with unstable overtone bloom

### For really mangled hits
- Add **self-FM** on a modulator
- Route **Op 4** back conceptually as extra modulator to Op 1
- Or use **Op 4 out → external processing → AR FM**

That creates semi-feedback percussion textures.

---

## D. Hi-hats and noisy ticks
### Setup
- Use several high-ratio or free operators
- Listen to one output, or mix multiple outputs externally
- Shapes more toward **square/saw**
- Lots of inharmonic modulation

### Modulation
- Fast decay envelopes to gains
- Noise or digital oscillator into AR FM
- Trigger Reset

### Great trick
Use multiple operator outputs as separate hat layers:
- one for body
- one for sizzle
- one for metallic tail

Then externally mix and process.

---

# 2. Crazy basslines for dubstep / drum and bass

This module is very capable of modern bass design because it gives you:
- FM tone shaping
- internal VCA-style modulation of FM amount
- waveform morphing
- self-FM
- external audio-rate modulation
- multiple outputs to layer externally

For dubstep and DnB, the best patches usually combine:
- a stable low fundamental
- aggressive moving harmonics
- modulation of FM amount, not just filter cutoff
- multiple layers

---

## A. Basic neuro / growl bass core
### Setup
- Keep **Op 1** in **lock**, ratio **1**, shape near **sine/triangle**
- Monitor **Op 1 out**
- Use **Op 2** in lock, ratio **2 or 3**, as main modulator
- Use **Op 3** as secondary modulator, ratio **5, 7, or 8**
- Optional mild **Op 1 self-mod**

### Modulation
- LFO or envelope follower into **Op 2 Gain CV**
- Different LFO/envelope into **Op 3 Gain CV**
- Slow CV into **Shape CV** for one or more modulators
- Small movement on **Detune** for one modulator
- Optional stepped random into shape or ratio CV, attenuated

### Result
- fundamental stays present
- harmonic profile shifts over time
- bass sounds like it’s “talking” or “chewing”

### Make it more dubstep
- Use synced LFOs into gain CVs for rhythmic wobble
- Use different modulation rates for nested movement
- Push one modulator shape toward square during stronger moments

---

## B. Reese-like bass using free-state destabilization
Classic reese is detuned saws, but here you can get a related vibe through FM instability and layering.

### Setup
- Op 1 = main carrier in lock
- Op 2 = lock ratio 1 or 2, slight detune
- Op 3 = **free state**, tuned close but not harmonically exact
- Use Op 3 to modulate Op 1 lightly
- Optionally monitor Op 1 + Op 3 mixed externally

### Modulation
- Slow LFO to **Op 3 Ratio CV** in free mode
- Slow LFO to **Op 3 Shape CV**
- Envelope or LFO to **Op 3 Gain CV**
- Small self-FM on Op 1 or Op 3

### Result
- unstable stereo-like movement even in mono
- shadowy beating and tearing edge
- excellent for dark DnB

If you have external processing:
- distort after mixing
- then bandpass/filter
- then compress

This will get very “record-ready.”

---

## C. Talking bass / vowel-ish FM movement
This module doesn’t have a filter built in, so “vowel” movement has to come from **changing sideband structure**.

### Setup
- Op 1 as carrier
- Op 2 and Op 3 as modulators
- Keep harmonic ratios at first: 2, 3, 4, 5
- Start from sine/triangle

### Modulation ideas
- Put a slow triangle LFO into **Op 2 Gain CV**
- Put a different phase-offset LFO into **Op 3 Gain CV**
- Put a third LFO or envelope into **Shape CV** of Op 2 or Op 3
- Sequence different FM depths with CV into gain inputs

### Result
- the harmonic emphasis shifts in a mouth-like way
- more animated than simple filter sweeps
- especially strong when later run through a lowpass or bandpass externally

---

## D. Bass stab with violent transient
### Setup
- Op 1 carrier ratio 1
- Op 2 ratio 4–8 for high transient bite
- Op 3 ratio 2 or 3 for body
- Add light self-mod on Op 1

### Modulation
- Sharp envelope to **Op 2 Gain CV**
- Longer envelope to **Op 3 Gain CV**
- Very fast pitch envelope to **LF FM**
- Trigger **Reset**

### Result
- click/snap from high-ratio short FM
- punch/body from lower-ratio FM
- stable low pitch with lots of impact

This is ideal for:
- one-shot bass hits
- staccato DnB sequences
- machine-like dubstep punctuation

---

## E. External audio-rate FM for monstrous bass
### Setup
- Build a decent FM bass internally first
- Patch another oscillator or processed signal into **AR FM**
- Route AR FM lightly to Op 1 and/or Op 2

### Good external sources
- hard-synced VCO
- wavefolder output
- noisy digital oscillator
- distorted sub octave
- one of the Quad Operator outputs itself via external effect

### Modulation
- Modulate **Gain AR FM CV** rhythmically
- Alternate between no external FM and bursts of it
- Use clipping intentionally

### Result
- bass tone suddenly opens into violent tearing layers
- very effective for fills, transitions, and drop moments

---

# 3. Haunting atmospheric pads and drones

The Quad Operator can absolutely do pads, but the patching approach is different:
- keep modulation comparatively restrained
- use mostly **lock mode** for harmonic coherence
- animate **gain CV** and **shape CV** slowly
- use multiple outputs layered externally
- use LFO mode if you want internal phase-locked modulators

The manual specifically notes LFO mode can generate **phase-locked complex modulation signals**. That can be extremely useful.

---

## A. Evolving FM pad
### Setup
- Keep all operators in **lock**
- Ratios: start simple, like **1, 2, 3, 4**
- Shapes near **sine/triangle**
- Monitor multiple outputs externally, not just one

### Modulation
- Very slow LFO to **Op 2 Gain CV**
- Different very slow LFO to **Op 3 Gain CV**
- Slow random or triangle to **Shape CV** on one or two operators
- Subtle detune on one operator
- Very small LF FM vibrato overall

### Result
- gently shifting overtone architecture
- chorused, spectral movement without obvious filter sweeps
- ghostly harmonic bloom

### Best practice
Use the individual outputs as layers:
- one output for the body
- one for shimmer
- one for unstable upper haze

Then mix with reverb and delay externally.

---

## B. Frozen-glass pad with free-state contamination
### Setup
- Most operators in lock
- One operator in **free state**
- Keep that free operator fairly low in modulation amount
- Use sine or triangle first

### Modulation
- Very slow CV into the free operator’s ratio CV
- Slow envelope/LFO into its gain CV
- Maybe a touch of shape modulation

### Result
- stable musical core with eerie drifting inharmonic halo
- ideal for dark ambient and horror-adjacent textures

---

## C. LFO-mode internal animation patch
Because VCO/LFO switch changes the base frequency range globally, you can use the module as a modulation network too.

### Idea
Use the Quad Operator in **LFO mode** to generate phase-locked complex modulation, then use its outputs to animate other modules — or self-patch in creative ways if you’re repatching between voices.

### Example
- Set operators to simple harmonic relationships in lock mode
- Use internal modulation matrix among them
- Take one or more outputs as CV/audio-rate hybrid modulation sources
- Use Reset to sync movement

This can create:
- repeating spectral swells
- pseudo-organic tremolo
- cyclic but non-obvious animation for pads elsewhere in your rack

---

## D. AR FM with field recordings / texture layers
For haunted atmospheres, the AR FM input is excellent.

### Patch
- Send a filtered noise source, radio noise, contact mic texture, or granular source into **AR FM**
- Set low/moderate gain
- Route subtly to one or two operators only

### Modulation
- Slowly modulate **Gain AR FM CV**
- Slowly modulate operator gain CVs too

### Result
- organic contamination of the pad
- whispering, breathy, haunted upper detail
- much more unique than ordinary oscillator + reverb patches

---

# Specific modulation tips by control

## Ratio CV
### In lock mode
Best for:
- changing harmonic relationships in stepped or semi-stepped ways
- shifting from mellow to bright intervals
- creating sequence-dependent timbre changes

Use:
- stepped CV
- sequencer rows
- sample & hold with attenuation

### In free mode
Best for:
- independent oscillator pitch movement
- drifting dissonance
- unstable bass tearing
- metallic percussion

Use:
- slow random
- pitch envelopes
- audio-rate sources for chaos

---

## Detune
The manual notes ±6 semitones per operator.

Best uses:
- tiny amounts for animated beating
- moderate amounts for unstable bass complexity
- larger amounts for bells, metal, broken percussion

For pads:
- use tiny detune offsets

For bass:
- automate or manually sweep one detuned operator while keeping carrier stable

---

## Shape CV
One of the best sound-design controls on the module.

### Use it for:
- transient aggression
- brightening during note onset
- slow spectral drift
- moving between clean FM and abrasive digital tone

### Especially good pairings:
- envelope to modulator shape CV for punchy attacks
- LFO to carrier shape CV for bass growl articulation
- random CV to secondary modulator shape for haunted pad drift

---

## Gain CV
Probably the most important modulation input on the entire module.

Because it affects both:
- modulation depth
- output amplitude

It is the natural place to patch:
- ADSR/decay envelopes
- VCAs controlling modulation amount
- LFOs for wobble
- random for evolving textures

If you only explore one thing deeply on this module, explore **Gain CV modulation**.

---

## LF FM
Per manual: good for vibrato, bends, pitch envelopes.

### Best uses:
- kick pitch drops
- bass attack pitch snap
- subtle vibrato on pads
- coordinated global movement across locked operators

Because it affects all operators in lock state, it is especially useful when you want the whole sound to move together.

---

## AR FM + Gain AR FM CV
This is where external chaos enters.

Use it for:
- dirtying transients
- adding external sidebands
- pseudo-feedback
- introducing non-matching tone sources into the FM network

The gain CV here is perfect for:
- burst modulation
- drop accents
- rhythmically opening the external FM only on selected steps

---

# Three full patch recipes

---

## Patch 1: Distorted industrial kick/snare hybrid
### Goal
A hard, broken drum voice with body plus digital crack.

### Setup
- Op 1 = carrier, lock, ratio 1, sine/triangle
- Op 2 = lock, ratio 2 or 3, modulates Op 1
- Op 3 = free, tuned high-ish, modulates Op 1 lightly
- Op 4 optional self-mod or extra attack component
- Noise into AR FM
- Monitor Op 1

### Modulation
- Trigger to Reset
- Fast decay envelope to LF FM
- Fast decay envelope to Op 2 Gain CV
- Very short envelope to AR FM gain CV
- Slight slower decay to Op 3 Gain CV

### Tune by ear
- Increase Op 3 inharmonicity until it sounds metallic/broken
- Raise AR FM until crack appears
- Add slight Op 1 self-mod for crunch

### Outcome
A drum hit that can sit between kick, snare, and machine impact.

---

## Patch 2: Dubstep talking growl
### Goal
A rhythmic, vocalized bass with evolving aggression.

### Setup
- Op 1 carrier, lock ratio 1
- Op 2 modulator, lock ratio 2
- Op 3 modulator, lock ratio 5
- Op 4 free or lock ratio 7 for extra complexity
- Monitor Op 1 and maybe Op 4 mixed externally

### Modulation
- Tempo LFO to Op 2 Gain CV
- Offset LFO or envelope sequencer to Op 3 Gain CV
- Slow triangle to Op 2 Shape CV
- Subtle random to Op 4 Ratio CV if free
- AR FM from another oscillator, brought in only on accents via Gain AR FM CV

### Outcome
Chewing, morphing bass movement with lots of variation across the bar.

### Improve further
Run the result through:
- distortion
- multimode filter
- phaser/flanger
- compression

---

## Patch 3: Haunted glass pad
### Goal
Slow-moving dark ambient harmonic texture.

### Setup
- Op 1, 2, 3 in lock, simple ratios
- Op 4 in free state, tuned by ear for slight dissonance
- Shapes mostly sine/triangle
- Monitor multiple outputs and mix externally

### Modulation
- Slow sine LFO to Op 2 Gain CV
- Different slow LFO to Op 3 Gain CV
- Very slow random to Op 4 Ratio CV
- Very slow CV to one shape input
- Subtle vibrato to LF FM
- Textural source into AR FM very quietly

### Outcome
A pad that feels harmonic but fragile, dusty, and haunted.

---

# Best practices for avoiding “just noise” when you want control

The manual is honest: this module can easily become dissonant/noisy. To stay musical while still getting interesting sounds:

## For harmonic tones
- Use **VCO mode**
- Keep operators in **lock**
- Set **detune to noon**
- Start with **sine waves**
- Start with **all modulation sends down**
- Add only one modulation path at a time

## Then introduce instability gradually
- one operator to free
- one shape toward square/saw
- one self-mod path
- one external AR FM source
- one moving gain envelope

That staged approach gives much better results than turning up everything.

---

# Advanced creative ideas

## 1. Use independent outputs as multiband layers
Each operator has its own output. Even if one operator is mainly acting as a modulator, its output may still sound great on its own.

Try:
- Op 1 = low body
- Op 2 = mid growl
- Op 3 = high grit
- Op 4 = unstable fizz

Process them separately:
- lowpass the body
- distort the mids
- bandpass the grit
- reverb the fizz

This is a huge advantage over closed FM synths.

---

## 2. Feedback-style patching with AR FM
The manual specifically suggests trying feedback patches with a phase-locked operator.

Try:
- patch one operator output out of the module
- process it through distortion, filtering, delay, wavefolder, or VCA
- return it to **AR FM**
- route it back into one or more operators

This gives controllable external feedback networks.

Excellent for:
- screaming basses
- unstable drones
- tearing percussion

---

## 3. Use one operator as a transient designer
Instead of thinking of all operators as “tones,” treat one as purely attack content.

### Example
- Op 1 = bass body
- Op 2 = body modulator
- Op 3 = very short bright attack FM burst
- Op 4 = noisy or inharmonic click layer

Then shape each with separate envelopes via gain CV.  
This is a great way to make complex bass hits and drum impacts.

---

## 4. Sequence timbre, not just notes
Because the FM matrix is open-ended, a sequencer lane can control:
- operator gain CVs
- shape CVs
- AR FM gain CV
- ratio CVs

This means one pitch sequence can become far more alive if another sequencer row changes timbre per-step.

Excellent per-step controls:
- Op 2 gain amount
- Op 3 shape
- AR FM amount
- one free operator pitch offset

---

# My strongest recommendations for your target sounds

## For distorted percussion
Prioritize:
- **Reset**
- **fast envelopes to Gain CV**
- **short LF FM pitch envelope**
- **self-FM**
- **AR FM with noise or clipped oscillator**
- **free-state modulator for metallic edge**

## For dubstep / DnB bass
Prioritize:
- **lock-state carrier**
- **one or two moving modulators**
- **Gain CV wobble**
- **Shape CV animation**
- **light self-FM**
- **AR FM bursts**
- **independent output layering**

## For haunting pads
Prioritize:
- **mostly lock-state operators**
- **very slow Gain CV motion**
- **subtle Shape CV drift**
- **one free operator very low in mix**
- **tiny detune**
- **quiet AR FM texture source**
- **external reverb/delay**

---

# Bottom line

The Quad Operator is most interesting when you stop treating it like a fixed FM synth voice and start treating it like a **small modulation ecosystem**. The most unique sounds will usually come from:

- modulating **Gain CV** constantly
- mixing **harmonic lock-state structure** with **one unstable free-state operator**
- using **self-FM** as distortion
- using **AR FM** as external contamination/feedback
- layering the **independent outputs**

If you want, I can also give you:

1. **10 concrete patch recipes with knob-by-knob starting positions**, or  
2. **a “best modulation sources for Quad Operator” guide** using envelopes, random, sequencers, and VCAs.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)