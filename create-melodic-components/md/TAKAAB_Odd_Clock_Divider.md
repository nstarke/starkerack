# TAKAAB — Odd Clock Divider

- [Manual PDF](../../manuals/TAKAAB OCD - Odd Clock Divider – Siam Modular.pdf)

---

# [Manual PDF / Product Page](https://siammodular.com/products/takaab-ocd-odd-clock-divider?srsltid=AfmBOopTsJBGyNaC6WtMfJJU3EFzdu1WvzDldMz3y6eA2c-lwQCE1iKj)

## Module identified
From the attached pages, the clearly documented module is:

- **TAKAAB OCD – Odd Clock Divider**

Related modules shown/referenced on the page:

- **TAKAAB ECD – Even Clock Divider**
- **TAKAAB OCD + ECD Clock Divider Bundle**
- **TAKAAB 2XOR – Dual 3-input Logic Exclusive OR Gate**
- **TAKAAB UXS** (mentioned as an expander/helper for bringing jumper control to the front panel)

---

## What the OCD does

The **TAKAAB OCD** is a **2HP clock divider** designed to generate less-common rhythmic divisions from an incoming clock.

### Inputs / controls
- **CLOCK IN**
  - Accepts **2.5V–10V**
  - Up to **10 kHz**
- **RESET jack**
  - Accepts **2.5V–10V**
  - Resets output clocks so they restart from pulse 1
- **RESET button**
  - Manual reset

### Outputs
It creates divided clocks at:

- **/3**
- **/5**
- **/7**
- **/9**
- **/10**

There is also a **jumper option** to change **/9** to **/6**.

### Output behavior
- Output level: **6V**
- Duty cycle: nominally **50%**, but for odd divisions it is rounded to nearest pulse:
  - /3 ≈ **1 high : 2 low**
  - /7 ≈ **3 high : 4 low**
  - /9 ≈ **4 high : 5 low**
- /6 is noted as exceptional:
  - **4 high : 2 low**

### Chaining / normalization
The page also says the board has headers to:

- normalize **RESET** between adjacent divider modules
- normalize **CLOCK IN** between adjacent **OCD** or **ECD** modules
- connect reset-button behavior to an adjacent **ECD**

That means OCD and ECD are intended to work very well as a compact clocking ecosystem.

---

## Important musical reality: this is not a pitch generator

By itself, the **OCD does not generate voltages for melody** in the usual pitch-CV sense. It generates **timing events**.

So if your goal is **melodic components**, the OCD contributes indirectly by creating:

- **rhythmic trigger structures**
- **phrase lengths**
- **reset cycles**
- **accent logic**
- **counterpoint timing**
- **non-4/4 note-entry patterns**

To make actual melodies, you pair it with one or more of:

- a **sequencer**
- a **quantizer**
- a **sample-and-hold**
- a **Turing machine / random CV source**
- an **envelope + VCA + oscillator voice**
- a **switch / sequential switch**
- logic modules such as the referenced **TAKAAB 2XOR**

---

## Best ways these modules can be used together for melodic music

## 1. Create polyrhythmic note triggers for one pitch source

### Patch idea
- Master clock → **OCD CLOCK IN**
- Use **/3** to trigger an envelope/VCA for your main voice
- Use **/5** to clock a sample-and-hold or sequencer advance
- Use **/7** to reset a short sequencer or switch

### Result
Your pitch changes and your note articulations happen at different rates.  
This creates melodies that feel:

- asymmetrical
- evolving
- less grid-locked
- “alive” without being random

### Why it works
If a sequencer advances every 5 pulses but the voice is articulated every 3 pulses, the same pitch will sometimes repeat and sometimes change before the next note. That creates emergent melodic phrasing.

---

## 2. Pair OCD with ECD to create long-form melodic cycles

The product page strongly suggests pairing **OCD + ECD**.

### Why this is powerful
Even divisions and odd divisions together create **least-common-multiple phrase lengths**. That means melodic structures take much longer to repeat.

For example:
- ECD /4 clocks a sequencer row change
- OCD /5 advances a second sequencer or transposition source
- ECD /8 resets one event
- OCD /7 resets another

### Musical effect
You get:

- long melodic forms
- repeating motifs that slowly phase
- evolving ostinatos
- pseudo-generative tonal movement

### Example patch
- Master clock → normalized to **ECD + OCD**
- **ECD /2** → trigger bass envelope
- **OCD /3** → trigger melody envelope
- **ECD /4** → advance 4-step sequencer
- **OCD /5** → transpose sequencer via precision adder input or switch
- **OCD /7** → reset melody every 7 pulses
- **ECD /8** → reset bass every 8 pulses

This creates a melody that loops against a different harmonic cycle.

---

## 3. Use odd divisions to define phrase boundaries

The **RESET** input is especially important musically.

### Patch idea
- Main clock → OCD
- **/10** output → reset a melodic sequencer
- **/3** output → trigger the sequencer to advance
- **/5** output → trigger an accent envelope or open a secondary VCA

### Result
A sequence might be stepped at /3 but forced back to step 1 every /10.

That means:
- the pattern does not simply run linearly
- phrase starts occur at a different interval than note events
- your melody acquires a recognizable but unusual structure

This is excellent for:
- minimalist melodies
- Berlin-school style pattern mutations
- modular techno phrases
- nonstandard arpeggios

---

## 4. Generate melodic syncopation with odd trigger streams

If you already have a quantized CV melody, the OCD can shape **when notes are heard**.

### Patch idea
- Quantizer CV → oscillator 1V/oct
- Envelope trigger from **OCD /3**
- Accent or filter envelope from **OCD /5**
- A second layer or sub voice from **OCD /7**

### Result
One pitch line becomes multiple interacting note layers:
- some notes are short
- some are accented
- some appear only every 5 or 7 base pulses

This turns a plain melody into a more composed line.

---

## 5. Use OCD + 2XOR for melodic gate logic

The related product list includes **TAKAAB 2XOR**, which is very useful here.

### What XOR adds
XOR outputs are high when inputs differ. With divided clocks, XOR produces new composite rhythms.

### Example patch
- OCD **/3** and **/5** → XOR input pair
- XOR output → trigger sequencer advance
- OCD **/7** → trigger envelope
- ECD **/4** → reset

### Musical result
The sequencer advances only on the changing relationship between /3 and /5. This creates:
- irregular note placements
- emergent motifs
- structured unpredictability

If the sequencer is quantized, these irregular advances become melodic phrases rather than just rhythmic noise.

### Another strong use
- XOR two divisions to create a trigger stream
- use that trigger stream to clock a **sample-and-hold**
- sample a slow CV or random source
- quantize the result

That gives you melodies whose note changes are mathematically patterned instead of purely random.

---

## 6. Use /6 jumper option for more conventional melodic support

The manual text says **/9 can be changed to /6** via jumper.

### Why this matters
/9 is musically unusual and great for long cycles, but /6 is often easier to integrate with:
- 3-based grooves
- 6/8 feels
- triplet-adjacent structures
- phrase balancing against /3

### Example
- /3 = note trigger
- /6 = accent reset or transposition event
- /5 = alternate melodic voice trigger

This gives a melody that feels semi-structured rather than fully “off-grid.”

If you want accessible but still interesting melodic motion, using **/6 instead of /9** may be preferable.

---

## 7. Build counterpoint from one master clock

A very modular-musician way to use OCD/ECD is to derive multiple “players” from one pulse train.

### Example 3-voice melodic patch
- Master clock → OCD + ECD
- **ECD /2** → bass trigger
- **OCD /3** → mid voice trigger
- **OCD /5** → high voice trigger
- one shared quantized CV source goes to a switch or S&H system
- **ECD /4** changes the bass pitch source
- **OCD /7** changes the high voice pitch source
- **/10** resets everything

### Result
You get independent note entrances from one timing network.  
Even with simple pitch material, the differing trigger rates imply counterpoint.

This is one of the best uses of clock dividers in melodic patching:  
**timing independence creates the illusion of compositional complexity.**

---

## 8. Use OCD as a melodic “form” generator, not just rhythm generator

Many people first think of clock dividers as drum tools, but odd dividers are especially good for **formal structure**.

### They can control:
- when a sequencer advances
- when a sequencer resets
- when a transposition occurs
- when a switch changes source
- when a random voltage is sampled
- when a second harmony line appears
- when a melodic motif is muted/unmuted

### Example form patch
- /3 → melody gate
- /5 → transposition change
- /7 → switch between two stored CV rows
- /10 → reset the row sequencer

This gives you melody, variation, and phrase recurrence from one 2HP utility.

---

## 9. Excellent use with sequential switches

If you have a switch module, OCD becomes much more melodic.

### Patch
- 3 or 4 different CV sources into a sequential switch
- OCD **/5** advances the switch
- OCD **/3** triggers the envelope
- ECD **/4** or OCD **/10** resets the switch
- switched CV goes through a quantizer to oscillator pitch

### Result
The pitch source changes on a different cycle than the note triggers.  
That yields:
- recurring motifs
- broken arpeggios
- phrase mutation
- musically coherent “generative” melody

---

## 10. Best use with sample-and-hold for generative melody

A classic patch:

- Noise or slow chaotic CV → Sample & Hold input
- OCD **/7** → S&H trigger
- S&H output → Quantizer
- Quantizer → oscillator pitch
- OCD **/3** → envelope trigger
- ECD **/8** or OCD **/10** → reset related clocking/sequencer logic

### Why this works
The note selection changes slowly at /7, while the actual played notes articulate at /3.  
So each sampled pitch may repeat a few times before changing, producing recognizable melodic cells.

This is far more musical than triggering random pitch on every note.

---

## Strengths of the OCD for melody-making

### 1. Odd divisions create non-obvious phrase structures
/3, /5, /7, /9 are great for:
- polymeter
- additive-feel melody
- pattern drift
- non-repeating ostinatos

### 2. Reset makes the complexity controllable
Without reset, odd clocks can drift indefinitely.  
With reset, you can define phrase lengths and keep the music intelligible.

### 3. Compact size
At **2HP**, it’s ideal as a support module in a melody-focused system.

### 4. Chainable architecture
The onboard normalization with adjacent ECD/OCD modules makes it easy to create a compact clock network for:
- melody
- bass
- transposition
- accents
- structural resets

---

## Limitations to understand

For melodic use, the OCD is **support infrastructure**, not a full melodic source.

You will still want at least one of:
- quantizer
- sequencer
- S&H
- logic
- precision adder
- switch

Also note:
- fixed divisions only
- no CV control over division
- no swing or shuffle mentioned
- no built-in pattern memory or pitch generation

So think of it as the **skeleton of melodic timing**, not the melody itself.

---

## Best musical pairings

## OCD + ECD
Best for:
- long non-repeating phrases
- bass vs melody timing separation
- phrase resets
- polymetric sequencing

## OCD + 2XOR
Best for:
- derived trigger logic
- irregular sequencer clocks
- more “composed” generative patterns
- accent and articulation streams

## OCD + quantizer + S&H
Best for:
- generative melodies
- slowly changing tonal lines
- ambient and experimental sequencing

## OCD + switch / sequencer
Best for:
- melodic variation
- phrase mutation
- transposition events
- arpeggio restructuring

---

## Practical patch recipes

## Recipe 1: Minimal melodic generator
- Master clock → OCD
- /5 → Sample & Hold trigger
- Random or slow CV → S&H in
- S&H out → Quantizer → VCO pitch
- /3 → Envelope trigger → VCA
- /10 → Reset sequencer or related clock tool

**Sound:** evolving melody with repeating sub-phrases

---

## Recipe 2: Bass + lead polymeter
- Master clock → ECD + OCD
- ECD /2 → bass trigger
- ECD /4 → bass sequencer advance
- OCD /3 → lead trigger
- OCD /5 → lead sequencer advance
- OCD /7 → lead reset
- ECD /8 → bass reset

**Sound:** stable bass with drifting lead phrase

---

## Recipe 3: Logic melody clock
- OCD /3 + /5 → 2XOR
- XOR out → sequencer clock
- OCD /7 → envelope trigger
- Sequencer CV → quantizer → VCO
- /10 → reset

**Sound:** irregular but structured melodic line

---

## Recipe 4: Two-row melodic switching
- Row A CV and Row B CV into switch
- OCD /5 → switch advance/toggle
- OCD /3 → gate envelope
- ECD /4 → sequencer advance
- /10 reset

**Sound:** melody that alternates between two harmonic identities

---

## Bottom line

The **TAKAAB OCD** is best used for melody as a **rhythmic and structural control module**. On its own, it does not output pitch, but when paired with modules like the **ECD**, **2XOR**, sequencers, quantizers, sample-and-hold, and switches, it becomes a very effective tool for:

- generating nonstandard melodic rhythms
- creating long-form evolving phrases
- introducing controlled asymmetry
- building polymetric bass/lead relationships
- resetting and shaping melodic form

If you use it like a **phrase engine** rather than just a divider, it becomes surprisingly powerful for melodic composition in Eurorack.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)