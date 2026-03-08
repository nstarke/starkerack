# Erica Synths — Graphic VCO

- [Manual PDF](../../manuals/graphic_vco_manual_web.pdf)

---

[Erica Synths Graphic VCO Manual (PDF)](https://www.ericasynths.lv/media/Graphic_VCO_manual_v2.pdf)

# Erica Synths Graphic VCO: using it for melodic parts

This manual is for a single module: **Erica Synths Graphic VCO**.  
So rather than explaining how *multiple modules in the PDF* work together, I’ll explain how this **VCO can work with the rest of a Eurorack system** to build strong melodic components: leads, basses, arps, plucks, evolving hooks, and harmonic layers.

## What this module is, musically

The Graphic VCO is not just a basic oscillator. It gives you:

- custom waveform drawing
- morphing between two waves
- wavetable playback
- wavetable matrix scanning
- onboard wave shaping FX:
  - FM
  - ring modulation
  - phase distortion
  - wavefold
  - wavewrap
  - bitcrush / sample-rate reduction
  - overdrive
- a configurable **suboscillator output** on **OUT2**
- snapshot recall for fast sound changes

That means it can be the **main voice source** for melodic material, especially if you pair it with:

- a sequencer
- envelope generator
- VCA
- filter
- modulation source(s)
- quantized CV or keyboard controller

## Main patch role in a melodic voice

A standard melodic chain would be:

**Pitch sequencer/keyboard → 1V/OCT input**  
**Graphic VCO OUT1 → filter or VCA → mixer/output**  
**Envelope → VCA CV**  
Optional:
- LFO or envelope → MORPH CV
- modulation source → FX CV
- CV source → FX AMT CV

The module accepts:

- **1V/OCT:** 0V to +8V
- **FX AMT CV:** unipolar 0 to +10V
- **FX CV:** bipolar -10V to +10V
- **MORPH CV:** bipolar -10V to +10V

This is important because it tells you what kinds of modulation are best:
- envelopes are great for **FX AMT**
- LFOs, random, and bipolar envelopes are great for **MORPH CV** and **FX CV**

---

# Best melodic uses

## 1. Expressive lead voice

Use **Wave Design mode** with two contrasting waves, A and B.

For example:
- Wave A = smoother sine/triangle-derived custom shape
- Wave B = brighter saw/pulse-like custom shape

Then:
- sequence pitch into **1V/OCT**
- use **MORPH knob** or **MORPH CV** to move between the two waves
- send **OUT1** through a VCA and maybe a lowpass filter

### Why it works
Morphing creates a lead sound that breathes with the melody. You can keep the pitch sequence simple and get movement from timbre instead of note density.

### Great modulation ideas
- slow LFO → MORPH CV for evolving sustained lines
- envelope → MORPH CV for pluck attacks that brighten then settle
- velocity CV or accent CV → FX AMT CV for more expressive phrasing

---

## 2. Bassline oscillator with sub reinforcement

The module has two outputs:

- **OUT1** = main output
- **OUT2** = configurable suboscillator/mix output

In the **Suboscillator Configuration menu**, you can set:

- pitch offset up to **24 semitones down**
- detune ±50 cents
- wave for the sub
- dry/wet mix between main and sub at OUT2

### Bass patch
- pitch sequencer → 1V/OCT
- **OUT2** → VCA/filter chain
- set sub offset to **-12 semitones** or **-24 semitones**
- set a square-ish or simple sub waveform
- keep main wave moderately bright, sub solid and stable

### Why it works
This gives you a bass voice with:
- harmonic articulation from the main oscillator
- fundamental weight from the sub

It’s especially useful for:
- monosynth bass
- acid-adjacent lines
- electro sequences
- techno hooks

If you want extra presence, use **OUT1 and OUT2 as separate layers**:
- OUT1 → brighter filtered path
- OUT2 → cleaner low-passed path

That effectively turns one oscillator into a layered melodic bass instrument.

---

## 3. Wavetable melody scanning

In **Wavetable mode**, you load a bank of **16 waves** and scan through them with:
- the **MORPH knob**
- or **MORPH CV**

### Musical use
Instead of treating morphing as subtle animation, treat it as a compositional parameter:
- one note pattern
- changing wave position across each step or phrase

### Patch ideas
- sequence pitch normally
- stepped CV from a sequencer row → MORPH CV
- envelope or accent → FX AMT CV
- OUT1 → LPG or VCA for plucky lines

### Result
Each note can have a different harmonic identity while staying in tune.  
That’s excellent for:
- melodic techno riffs
- chiptune-ish sequences
- evolving arpeggios
- “single oscillator but sounds like many notes are articulated differently” lines

---

## 4. Matrix scanning for animated melodies

The **Wavetable Matrix mode** is one of the most powerful melodic features.

You get a 2D field:
- one axis = wavetable selection
- one axis = wave selection within those tables

On the panel in this mode:
- **FX knob / FX CV input** scan one direction
- **MORPH knob / MORPH CV input** scan the other direction

### Musical advantage
This lets you move through a large organized timbral map while pitch remains stable.

### Best use cases
- long evolving melodies
- generative melodic patches
- note repeats where the timbre changes per step
- phrase-based modulation, where one CV controls “brightness family” and another controls “internal wave position”

### Patch example
- quantized melody sequencer → 1V/OCT
- slow random or sequencer row → MORPH CV
- another CV lane or LFO → FX CV
- gate envelope → VCA

Now the melody has:
- note content from pitch CV
- timbral phrasing from X/Y scanning

This is one of the best ways to make a simple 8-step melody sound like a composed line.

---

# Using the onboard FX for melody

The FX are applied to the main resulting wave before output.  
Per the manual, **FXes except FM are not applied to the suboscillator**.

That means you can keep the sub stable while making the main tone animated.

## 5. FM for tuned melodic brightness

The FM section uses:
- selectable modulation waveform
- sync on/off
- ratio or free frequency
- depth control

### Best melodic use
Use **small to medium FM depth** with a synced ratio.

Good starting points:
- sine modulator
- sync ON
- simple ratios
- low/moderate depth

### Result
- bell-like leads
- glassy plucks
- metallic but still tonal basses
- expressive sequence accents

If the ratio is synced, melodic intervals remain musically coherent.

### Great patching
- sequencer accent row or envelope → FX AMT CV
- keep base timbre clean, add FM only on accented notes

That gives you articulate melodic phrasing without changing pitch sequence.

---

## 6. Phase distortion for sharper plucks and digital leads

This is especially useful for melodic content because phase distortion often keeps the pitch center clear while changing the edge and attack character.

### Musical use
- manual POT mode for live tweaking
- envelope to FX CV for per-note transient shaping
- subtle amount for animated leads
- stronger amount for aggressive bass sequences

This is excellent when you want:
- Casio-like digital edge
- sharper attacks
- more note definition in busy arrangements

---

## 7. Ring mod for tuned dissonant melodies

Ring modulation can get wild, but for melodic use:
- keep modulation amount low
- use synced internal oscillator
- try sine or triangle modulators

### Best application
Use it sparingly as:
- an accent layer
- a transition sound
- a second phrase variation recalled via snapshots

It’s less “main bassline all night” and more “special color” in melodic composition.

---

## 8. Wavefold / wrap for dynamic articulation

Wavefolding is great for melodic lines because it responds well to envelopes.

### Patch
- choose FOLD or WRAP
- use **POT** or external CV
- envelope → FX CV or FX AMT
- sequence into 1V/OCT

### Result
Each note opens with harmonic intensity, almost like a filter envelope but at the oscillator level.

This is one of the best ways to make:
- West-coast flavored plucks
- animated sequences
- aggressive modern lead lines

---

## 9. Bitcrush / sample-rate reduction for melodic texture

For melody, bitcrush works best when controlled, not maxed out.

### Good uses
- lo-fi arps
- video-game style hooks
- broken-digital melodic layers
- occasional phrase variation

Try:
- fixed melody
- slight morph movement
- moderate crush amount
- high resonance filter after the oscillator

This gives a very characterful line without losing note identity.

---

## 10. Overdrive for lead presence

Overdrive is simple but useful:
- makes a lead sit forward
- adds harmonics to bass
- can make simple custom waves more musically dense

It works especially well if your wave design starts smooth and you use drive to introduce harmonic urgency.

---

# Strong system pairings for melodic patches

## With a sequencer
This is the most obvious pairing.

Use a sequencer to send:
- pitch to **1V/OCT**
- gates to envelope/VCA
- extra CV lane to **MORPH CV**
- accent lane to **FX AMT CV**

This turns a basic sequencer into a much more expressive melodic engine.

### Great strategy
One lane controls note pitch, another lane controls **timbre per step**.  
That’s where the Graphic VCO really shines.

---

## With a quantizer
If you feed random CV or a slow function generator into a quantizer and then to **1V/OCT**, the Graphic VCO becomes a very strong generative melody voice.

Then use different slow CVs for:
- MORPH CV
- FX CV
- FX AMT CV

Now:
- pitch evolves in scale
- timbre evolves independently

That creates musical ambient lines, generative hooks, and self-moving motifs.

---

## With an envelope and VCA
This is essential if you want discrete notes rather than a drone.

Use:
- gate sequencer → envelope
- envelope → VCA CV
- Graphic VCO → VCA audio in

For more expression:
- mult the envelope to **MORPH CV** or **FX AMT CV**

That makes every note change shape, not just amplitude.

---

## With a filter
Even though the VCO can do lots of internal shaping, a filter still adds huge value.

### Why
The oscillator can provide very complex harmonic movement, while the filter:
- controls spectral focus
- adds contour
- turns static timbral changes into more “synth-voice” phrasing

### Great combinations
- bright wavetable scan → lowpass filter for classic subtractive melody
- wavefolded tone → bandpass filter for nasal lead
- FM tone → lowpass gate or VCA for plucky digital percussion-melody hybrids

---

## With LFOs and function generators
This is where the module becomes truly alive.

Use modulation for:
- slow morphing between waves
- rhythmic FX parameter shifts
- phrase-level timbral modulation
- subtle vibrato via pitch source upstream if desired

Since the module has dedicated CV control over morph and FX, it rewards having **at least two modulation sources** available.

---

# Practical melodic patch recipes

## Patch 1: Evolving lead
- Sequencer pitch → 1V/OCT
- Gate → envelope → VCA
- OUT1 → VCA → delay/reverb
- Slow triangle LFO → MORPH CV
- Envelope attenuated → FX AMT CV
- FX = phase distortion or mild FM

**Sound:** expressive, singing lead with evolving harmonic shape.

---

## Patch 2: Solid techno bass
- Sequencer pitch → 1V/OCT
- OUT2 → lowpass filter → VCA
- Sub offset = -1 or -2 octaves
- Mix% favors sub, with some main tone
- FX on main voice = overdrive or mild wavefold
- Short decay envelope to VCA/filter

**Sound:** punchy, harmonically rich bass with strong low end.

---

## Patch 3: Animated arp
- Arp/sequencer → 1V/OCT
- Clocked stepped CV → MORPH CV
- Slow LFO → FX CV
- FX = bitcrush lightly or phase distortion
- OUT1 → stereo effects

**Sound:** each note has a different timbral edge, making the arp feel composed and lively.

---

## Patch 4: Generative melodic texture
- Random CV → quantizer → 1V/OCT
- Random gates → envelope → VCA
- Slow random CV → MORPH CV
- Another slow random CV → FX CV
- Wavetable Matrix mode active
- OUT1 → filter → reverb

**Sound:** evolving tonal textures with melodic coherence.

---

## Patch 5: Dual-layer mono voice from one oscillator
- OUT1 → brighter filter/VCA path
- OUT2 → lowpassed support path
- Same pitch source to 1V/OCT
- Main output carries animated wave/FX
- Sub output provides body

**Sound:** one VCO behaving like a layered synth voice, ideal for hooks and lead-bass hybrids.

---

# Best workflow features for songwriting

## Snapshots
You can save a snapshot of:
- wave settings
- wavetable state
- suboscillator config
- FX settings
- related sound design choices

This is very useful for melodic composition because you can build:
- verse lead
- chorus lead
- breakdown texture
- alternate bass tone

…and switch quickly between them.

### Performance benefit
You can write several related melodic timbres and recall them during arrangement or live play.

---

## Custom wave drawing
This matters musically because you can design waves with a specific melodic role:
- smoother waves for foreground melody
- hollow waves for counter-melody
- nasal waves for cutting through a mix
- asymmetric waves for punchy bass

Rather than picking from generic oscillator shapes, you can build a wave that supports the exact line you want.

---

## Harmonic editing
The spectral/harmonic editing mode is especially useful if you think in arrangement terms.

For example:
- strong fundamental + low harmonics = bass
- richer upper harmonics = lead
- odd harmonic emphasis = hollow/reedy line
- sparse harmonics = cleaner melody that leaves room for pads/drums

---

# Most useful melodic strategies

## Keep pitch simple, vary timbre
This module excels when the melody is not overly complex but the timbre is changing.

A 4-step or 8-step sequence can feel very rich if:
- morph shifts per note
- FX amount changes with accents
- wavetable position evolves over time

## Use suboscillator for weight, not complexity
For melodic lines, the sub is best used to support pitch perception and groove.  
Let the main output carry the interesting motion.

## Use FM and ring mod carefully
They’re powerful, but for melodic writing:
- start subtle
- prefer synced ratios
- use them as articulation, not constant chaos

## Save snapshots as arranged sections
Treat snapshots like:
- intro
- verse
- chorus
- fill
- bridge variants

That makes the module very effective in live melodic performance.

---

# Limitations to keep in mind

From the manual, this is fundamentally an **oscillator**, not a full voice.  
To make complete melodic parts, you typically still want:

- a sequencer or keyboard
- an envelope
- a VCA
- often a filter
- possibly effects downstream

Also note:
- non-FM FX do **not** affect the suboscillator
- in snapshot recall, knobs won’t affect parameters until they reach the saved position
- the most musical results usually come from intentional CV attenuation rather than full-range modulation

---

# Bottom line

The **Graphic VCO** is excellent for melodic work because it combines:

- stable pitch tracking
- custom waveform design
- wavetable scanning
- 2D matrix morphing
- internal digital waveshaping
- a useful sub layer
- snapshot recall

In a Eurorack system, it works best as the **core tone generator** for:

- expressive leads
- animated arps
- rich mono basses
- generative melodies
- layered digital/analog hybrid hooks

If I were building melodic patches around it, I’d prioritize pairing it with:

1. a strong pitch sequencer  
2. at least one envelope + VCA  
3. a filter  
4. one or two CV sources for morph and FX control  

That combination turns the Graphic VCO from “interesting oscillator” into a **full melodic instrument**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)