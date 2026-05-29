# Pittsburgh Modular — Synthesizer Box

- [Manual PDF](../../manuals/Synthesizer Box - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF / Product Page](https://pittsburghmodular.com/synthesizer-box)

# Pittsburgh Modular Synthesizer Box for Dense Rhythmic / Hyper-Complex Percussion

The **Pittsburgh Modular Synthesizer Box** is an unusually strong module for percussion design because it gives you a **complete analog voice** with multiple places to interrupt or repurpose the normal signal flow:

- **Complex oscillator** with triangle / saw-or-blade / square / sub
- **Lopass gate** with **MOD** and **PING** behavior
- **ADSR envelope**
- **Wide-range LFO** that can run slowly or into audio-rate
- **VCA**
- **Glide**
- Normalized internal routings that can be broken with patching

That means it can act as:

- a **kick / tom / blip / click / bass percussion voice**
- a **metallic pseudo-snare / hat source**
- a **modulated percussion layer**
- a **self-contained “one-voice drum machine lane”**
- a **chaotic accent voice** inside a larger patch

---

## What in the manual makes it good for percussion?

A few especially important details from the manual:

1. **LPG has a Ping mode**  
   This is gold for percussion. The manual says in **PING mode**, incoming modulation is converted to a short trigger that “pings” or “strikes” the lopass gate, creating **organic percussive sounds with natural decay**.

2. **LPG has 3 modes**
   - **VCA**
   - **LPG**
   - **LOPASS**
   
   So the same sound source can be made:
   - tighter and cleaner with **VCA**
   - woody / natural / bongo-like with **LPG**
   - filtered and resonant with **LOPASS**

3. **Oscillator has waveform modulation + FM**
   - **FM CV IN** can be exponential or linear
   - **MOD CV** changes square pulse width and blade waveshape
   - **Blade** is a special complex saw-like waveform
   
   This is ideal for making one drum lane constantly mutate.

4. **LFO can go wide range, including audio rate**
   So it can be:
   - a clocked-ish modulation source
   - a pseudo-second oscillator
   - an FM source for clangorous percussion

5. **Internal normalizations are performance-friendly**
   Without patching, the module already behaves like a voice. With patching, you can override:
   - LFO → oscillator FM / MOD
   - envelope → LPG CV
   - envelope → VCA CV
   - mixer → LPG IN
   - LPG OUT → VCA IN

This makes it easy to move between **stable rhythm voice** and **patch-programmed percussion machine**.

---

# Best roles for this module in rhythm-heavy music

For your goal—**densely rhythmic, hyper-complex percussion sequences with polyrhythms and unusual meters**—this module is best used as one or more of the following:

## 1. Primary analog percussion voice
Use it as a drum lane that receives:
- triggers/gates from a sequencer
- separate clocks/divisions
- logic-derived accents
- burst triggers
- Euclidean patterns

Because the module has **ENV IN**, **LPG CV IN**, **VCA CV IN**, **1V/O IN**, **FM CV IN**, and **MOD CV IN**, you can make every strike differ in:
- pitch
- brightness
- decay feel
- transient shape
- harmonic density

## 2. Accent / ghost-note percussion lane
It excels at:
- muted taps
- woody pings
- tuned ticks
- synth conga / tom-like voices
- laser zaps between main hits

This is especially effective when your main drums are elsewhere and the Synthesizer Box handles the **off-grid complexity**.

## 3. Polyrhythmic modulation destination
Even if it only plays one audio voice at a time, you can inject many independent rhythmic layers into different parameters:
- one rhythm to **ENV IN**
- another to **LPG CV IN**
- another to **FM CV IN**
- another to **MOD CV IN**
- stepped CV to **1V/O IN**

That creates the illusion of several intertwined percussion parts coming from a single voice.

---

# Core percussion patch strategies

## Patch 1: LPG ping percussion
This is the most direct “drum synthesis” use.

### Patch
- Use oscillator **MIX OUT** into the normal signal chain, or patch **MIX OUT → LPG IN**
- Set LPG to **PING**
- Send triggers/gates from a sequencer into **LPG CV IN**
- Take audio from **LPG OUT** or through the normal VCA chain to **VCA OUT**

### Result
Each trigger “strikes” the LPG, producing a natural decaying hit. This is excellent for:
- bongos
- toms
- woodblock-like synth hits
- plucks
- short kick-like sounds
- muted percussive bass

### How to shape it
- **Triangle-heavy mix** = rounder, more drum-like
- **Square/blade-heavy mix** = sharper, more aggressive
- **Low frequency setting** = tom / kick territory
- **Higher frequency setting** = claves / bleeps / rim-click zones
- **LPG mode center (LPG)** = organic
- **LOPASS mode** = more resonant synthetic percussion
- **VCA mode** = cleaner transient, less “acoustic” character

---

## Patch 2: Envelope-controlled drum voice
Use the ADSR for more explicit shape control.

### Patch
- Trigger sequencer/gate source → **ENV IN**
- **ENV OUT** is already internally routed to VCA CV and LPG CV, but you can break/reassign as needed
- Audio out from **VCA OUT**

### Why this is useful
This gives you more traditional synthesized drum behavior:
- fast attack
- short decay
- little/no sustain
- controlled release

### Good settings
- **Attack**: very low
- **Decay**: short to medium
- **Sustain**: low or off
- **Release**: short

### Use this for
- punchy synth kicks
- zaps
- snappy bass percussion
- resonant blips
- machine-like low drums

---

## Patch 3: Layered trigger logic illusion
Use different rhythmic sources on different inputs.

### Example
- Pattern A → **ENV IN**
- Pattern B → **LPG CV IN**
- Pattern C → **FM CV IN**
- Pattern D → **MOD CV IN**
- Quantized/stored CV sequence → **1V/O IN**

Now one module behaves like a whole percussion ecosystem:
- one rhythm decides **when a hit happens**
- another decides **when it gets brighter**
- another decides **when pitch splashes or bends**
- another decides **when the overtone profile changes**

This is one of the best ways to get **polyrhythmic density** from a single semi-modular voice.

---

# How to make it punchy and percussive

## 1. Exploit very fast attacks
The module’s percussion strength depends on **sharp transients**.

For punch:
- Set **Attack** near minimum
- Use short **Decay/Release**
- Keep **Sustain** low for drum behavior
- Favor **VCA mode** for the hardest hits
- Favor **PING/LPG mode** for more woody / natural hits

## 2. Use pitch envelopes externally if possible
The manual doesn’t describe an internal pitch envelope, but you can create one by patching an envelope or fast CV source into:
- **FM CV IN** for pitch thwack
- or stepped pitch into **1V/O IN**

A tiny downward pitch sweep on attack gives:
- kicks more impact
- toms more realism
- zaps more aggression

## 3. Use the blade waveform for unusual attacks
The **BLADE** waveform is one of the module’s secret weapons. Because it responds to **MOD CV** and **BLADE IN**, it can make each hit feel more articulated and less generic than standard saw/square percussion.

Great use:
- Put switch on **BLADE**
- Send rhythmic CV to **MOD CV IN**
- Optionally send additional modulation to **BLADE IN**
- Keep decay short

This gives a changing top-end snap that works well for:
- synthetic hats
- metallic ticks
- glitch percussion
- evolving tom attacks

## 4. Use audio-rate LFO FM for metallic percussion
The LFO can run at high range, including **audio rate**.

Try:
- LFO high range
- LFO **TRI OUT** or **SQR OUT** patched to **FM CV IN**
- Use small FM amount first
- Trigger the voice with short envelope or LPG ping

This creates:
- clangs
- metallic pings
- dirty snares
- industrial clicks
- brittle hats

## 5. Keep the sub oscillator for body, not always for every hit
The **sub oscillator** can add huge low-end, but too much makes dense patterns muddy.

Use sub:
- on downbeats
- on accent hits
- on longer cycle resets
- sparingly in polyrhythmic contexts

Very effective for:
- accent toms
- low knock layers
- pseudo-kicks

---

# Building complex rhythms with this module

The Synthesizer Box itself is not a sequencer, so the complexity comes from **how you drive it**. The key is to distribute different rhythmic functions to different destinations.

## A. Use separate clock divisions/multiplications for each destination

Example:
- /5 clock → **ENV IN**
- /7 clock → **LPG CV IN**
- x3 burst trigger stream → **MOD CV IN**
- /4 accent gate → **FM CV IN**
- 8-step pitch CV sequence of irregular length → **1V/O IN**

Because these streams are different lengths, the combined result cycles over a long span and feels highly complex.

---

## B. Use odd step lengths against each other

Excellent pattern structure:
- pitch sequence: **11 steps**
- hit gate pattern: **7 steps**
- FM accents: **5 steps**
- waveform modulation pattern: **9 steps**

This creates long-form non-repeating percussion behavior even from one voice.

---

## C. Use different time signatures per modulation lane

For example:
- Main trigger pattern implies **4/4**
- Pitch accents imply **5/8**
- Brightness modulation implies **7/8**
- FM bursts imply **3 over 4**

The ear hears one voice, but the parameter changes imply multiple overlapping meters.

---

## D. Feed logic or probability to PING mode
Since the LPG can behave like a struck resonant element, it responds well to:
- logic AND/OR/XOR trigger combinations
- random trigger skips
- Bernoulli gates
- burst generators
- ratchets

This is one of the best paths to **complicated percussion patterns** that still sound musical rather than merely chaotic.

---

# Practical patch recipes for specific percussion voices

## 1. Analog kick / low tom
### Setup
- Oscillator tuned low
- Favor **triangle** and maybe a little **sub**
- LPG in **VCA** or **LPG** mode
- Fast envelope
- Short decay/release

### To improve impact
- Add a brief external CV to **FM CV IN** for pitch drop
- Slight resonance only if using filter mode carefully
- Keep waveform simple for weight

### Best rhythmic use
- anchor voice in polymetric patch
- low accent every 5th or 7th beat
- rotating kick pattern

---

## 2. Bongo / conga / wood drum
### Setup
- Oscillator mid-low tuning
- Triangle + a little blade
- LPG in **PING**
- Moderate frequency setting
- Short trigger pulses into **LPG CV IN**

### Variation
- Send slow or stepped CV to **1V/O IN** to move between drum “sizes”
- Use different trigger lengths or amplitudes externally if available

### Best rhythmic use
- 3:2 and 5:4 interlocking hand-drum patterns
- ghost notes against rigid kick grid

---

## 3. Metallic snare-ish hit
### Setup
- Use **square + blade**
- Add audio-rate LFO to **FM CV IN**
- Trigger envelope with short attack/decay
- Use **LOPASS** mode for tone shaping

### Extra trick
- Send a second rhythm to **MOD CV IN** so some hits are more splattered/metallic than others

### Best rhythmic use
- offbeat accents
- 7-step snare cycle against 16-step foundation
- industrial / IDM percussion

---

## 4. Hats / ticks / digital-feeling top percussion
### Setup
- Tune oscillator high
- Emphasize **square** and/or **blade**
- Very short envelope or LPG ping
- Little or no sub
- Light FM or rapid MOD CV

### To make it more alive
- Alternate between saw and blade
- Modulate pulse width via **MOD CV**
- Use irregular triggers and bursts

### Best rhythmic use
- ratchets
- Euclidean hat streams
- 11-against-4 top layer

---

## 5. Glitch blips / zaps / laser percussion
### Setup
- Mid-high tuning
- Blade waveform
- More aggressive FM
- Short envelope
- Optional glide for sliding multi-hit phrases

### Why glide matters
The glide is hardwired between **1V/O IN** and oscillator. If you sequence rapid pitch changes with some glide, each strike smears into the next in a very synth-percussion way.

### Best rhythmic use
- fills
- transition bursts
- asymmetrical phrase endings
- “reply” hits to the main groove

---

# Making one voice feel like many voices

Since this is a monophonic voice, dense music requires intelligent reuse.

## Technique 1: Alternate timbre by alternating destinations
Send one trigger stream to **ENV IN**, another to **LPG CV IN**. Some hits become:
- full voice hits
- others become struck LPG hits
- others become modulated variants

The ear hears multiple instruments.

## Technique 2: Use pitch zones as “drum identities”
Program different voltages into **1V/O IN** such as:
- very low = kick
- medium-low = tom
- medium = bongo
- high = click/hat

Now one sequencer line creates a family of drums.

## Technique 3: Use modulation accents instead of only velocity accents
Instead of just louder hits, accent by:
- more **FM**
- more **MOD CV**
- more **resonance** in filter mode
- switching **saw/blade**
- changing LPG mode between sections manually

This makes patterns feel much more compositional.

## Technique 4: Reserve sub oscillator for structural accents
Don’t leave sub constantly on at full volume in dense music. Use it conceptually:
- phrase start
- cycle reset
- every 8th, 10th, or 15th hit
- only on one branch of a polymeter

---

# Polyrhythm and odd-meter patch examples

## Example 1: 4 against 5 against 7
- 4-step gate loop → **ENV IN**
- 5-step trigger loop → **LPG CV IN**
- 7-step CV loop → **MOD CV IN**
- static or slow-changing pitch on **1V/O IN**

This produces repeating hit locations with non-repeating brightness articulations.

---

## Example 2: 11-step percussion organism
- 11-step sequencer sends pitch to **1V/O IN**
- triggers on steps 1, 2, 5, 7, 10 → **ENV IN**
- separate 8-step accent loop → **FM CV IN**
- random skip gate → **LPG CV IN**

The voice keeps changing identity over a long phrase before repeating.

---

## Example 3: Compound meter percussion
For a **7/8** track:
- Main hit pattern follows **2+2+3**
- MOD accents follow **3+2+2**
- FM accents every 5 pulses
- sub oscillator only emphasized on the first pulse of each bar

This creates motion without crowding the grid.

---

# Section-by-section performance strategies

## Oscillator
Use the oscillator not just as “a note source,” but as your percussion tone designer.

### Percussive strengths
- **Triangle** = body, thump, soft mallet
- **Saw** = direct, classic synth edge
- **Blade** = complex, animated, strange
- **Square** = hollow, nasal, snappy
- **Sub** = mass and weight

### Good practice
For dense rhythm, keep only 1–2 dominant waveforms at a time. Too many full-level layers can blur the attack.

---

## Mixer
The mixer is crucial because it determines what kind of transient excites the LPG / VCA.

### Useful pairings
- **Triangle + sub** = kick/tom
- **Triangle + blade** = woody organic strike
- **Square + blade** = hats, clicks, aggressive snare layer
- **Saw + square** = direct electro percussion

### Performance idea
Change the mixer settings every few bars rather than every hit. Let the sequencer handle micro-complexity while the panel sets macro-identity.

---

## LPG
This is your best percussion character shaper.

### Mode guide
- **VCA**: tight, modern, hard-edged
- **LPG**: natural, plucky, rounded
- **LOPASS**: resonant, synthetic, filter-drum territory
- **PING**: percussion magic

### Best use in dense music
Use **LPG mode** or **PING mode** for voices that need to remain vivid even in packed mixes. They often sit better than a plain VCA contour.

---

## Envelope
The ADSR is simple but enough for drum articulation.

### Suggested drum settings
- Attack: minimum
- Decay: short
- Sustain: low
- Release: short or medium-short

### Suggested evolving percussion settings
- Attack: still low
- Decay: medium
- Sustain: medium-low
- Release: medium

This can create hybrid percussive-bass lines in odd meters.

---

## LFO
Think of the LFO as a rhythm complication tool, not just a slow modulation source.

### Uses
- Slow triangle to **MOD CV IN** for gradual timbral motion across a polyrhythm
- Square to **FM CV IN** for stepped aggression
- Audio-rate into **FM CV IN** for metallic attacks
- Audio-rate into **MOD CV IN** for harsher texture shifts

### Trick
Because the oscillator FM and MOD inputs are internally patched to the LFO triangle unless overridden, the module already wants to move. In dense rhythm patches, deliberately decide whether to:
- keep that built-in motion
- or replace it with clocked external modulation

---

## VCA
The VCA is linear and clean. That makes it useful when you want rhythmic precision after the more characterful LPG.

### Two good workflows
1. **Oscillator → LPG → VCA**  
   Best for shaped, controllable percussion.

2. **External signal → VCA IN**  
   Use the VCA alone as a clean rhythmic chopper if desired.

### Percussion tip
If the LPG gives too much softness, let it shape tone while the **VCA** handles stricter amplitude articulation.

---

# Recommended external module pairings

To reach your stated goal most effectively, pair the Synthesizer Box with:

- **clock divider / multiplier**
- **trigger sequencer**
- **Euclidean sequencer**
- **logic module**
- **burst generator / ratcheter**
- **sample & hold / stepped random**
- **sequential switch**
- **attenuverters / VCAs for modulation depth**
- **precision adder / quantizer** if using pitched percussion

This module becomes much more powerful for hyper-complex rhythm when different timing systems are distributed to its different CV inputs.

---

# A few high-value patch concepts

## “One module drum battery”
- low pitches for kick/tom
- high pitches for click/hat
- pattern-dependent FM for snare-like hits
- PING mode for hand-drum realism

Sequence pitch and trigger differently so one line produces many drum identities.

## “Polymetric metallic lane”
- audio-rate LFO to FM
- blade waveform active
- odd-length trigger sequence to ENV
- separate odd-length modulation to MOD CV

Great for IDM, industrial, and abstract techno percussion.

## “Organic counter-rhythm”
- main groove elsewhere
- Synthesizer Box in LPG ping mode
- sparse but irregular triggers
- small pitch changes on each bar
- occasional sub accents

This gives a living hand-played-feeling layer over rigid grids.

---

# Bottom line

The **Synthesizer Box** is very well suited to **dense rhythmic and hyper-complex percussion music**, especially because of:

- the **pingable LPG**
- the **complex waveform oscillator**
- **FM and waveform modulation inputs**
- the ability to **separate trigger, timbre, and pitch rhythms**
- normalized routing that makes it easy to go from simple voice to highly patched percussion engine

If you want the best results for **polyrhythms, complex time signatures, and complicated patterns**, treat it less like a “lead synth” and more like a **single-voice modular drum organism** where:

- **ENV IN** controls event timing
- **1V/O IN** controls drum identity
- **LPG CV IN** controls strike/brightness behavior
- **FM CV IN** controls aggression/metal
- **MOD CV IN** controls articulation/timbre complexity

That division of labor is what lets one analog voice produce surprisingly intricate percussion music.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)