# Doepfer — A-160-2

- [Manual PDF](../../manuals/A-160-2.pdf)

---

[Manual PDF / Product Page: Doepfer A-160-2 Clock/Trigger Divider II](https://doepfer.de/a1602.htm)

# Using the Doepfer A-160-2 to Create Melodic Components

The attached manual covers the **Doepfer A-160-2 Clock/Trigger Divider II**. This is not a pitch generator by itself, but as a Eurorack musician, I’d say it’s extremely useful for building **melodic structure**, especially when combined with sequencers, quantizers, switches, sample & hold, logic, clocked modulation, and envelope/VCA voice chains.

## What the A-160-2 does

The A-160-2 takes a clock/trigger/gate input and generates **seven divided outputs**. It offers three division sets:

- **Powers of two:** 2, 4, 8, 16, 32, 64, 128
- **Prime numbers:** 2, 3, 5, 7, 11, 13, 17
- **Integers:** 2, 3, 4, 5, 6, 7, 8

It also gives you:

- **Gate mode**
- **Trigger mode**
- **Reset input**
- Configurable:
  - clock edge behavior
  - reset behavior
  - output polarity

So musically, this is a **rhythmic structure generator** that can become a **melody organizer**.

---

## Important musical idea

A clock divider doesn’t directly output notes, but it can control:

- **when notes happen**
- **when a sequencer advances**
- **when pitch is sampled**
- **when transpositions occur**
- **when phrase resets happen**
- **when alternate voices or intervals are introduced**

That makes it very powerful for melodic composition.

---

## Best ways to use it for melody

## 1. Drive sequencers at different rates

One of the most immediate uses is to patch different divider outputs to different sequencers or sequencer functions.

### Example
- Master clock → A-160-2 clock input
- `/2` → main sequencer clock
- `/5` → transposition sequencer clock
- `/16` → reset or phrase change
- Pitch sequencer CV → quantizer → oscillator 1V/oct

### Result
Your main melody advances steadily, but the transposition layer changes more slowly and at a different cycle length. If you use the **prime division mode**, the interaction becomes less repetitive and can create long evolving melodic phrases.

### Why it works
Melody is often more interesting when:
- note steps happen at one rate
- harmonic movement happens at another
- phrase resets happen at yet another

The A-160-2 makes these timing relationships easy.

---

## 2. Create melody with sample & hold

If you have a **sample and hold** and any CV source, the divider becomes a melodic trigger source.

### Patch
- Random CV, noise, or slow modulation → S&H input
- A-160-2 output (for example `/3` or `/5`) → S&H trigger
- S&H output → quantizer → oscillator pitch

### Result
The divider determines when a new note is chosen.

### Musical advantage
Different divider outputs produce different note densities:
- `/2` = more active melodic movement
- `/7` or `/11` = sparse, phrase-like note updates
- prime-number divisions = less obvious looping

You can also use **multiple divider outputs**:
- `/2` triggers the VCA envelope
- `/5` updates the S&H pitch
- `/16` resets a modulation source

That gives repeated rhythmic notes with slower-changing melodic content.

---

## 3. Build “melody over ostinato” structures

A really musical use is separating **note articulation** from **pitch change**.

### Patch
- Fast clock → A-160-2
- `/2` → envelope trigger for every note attack
- `/8` → S&H or sequencer advance for pitch changes
- Quantized pitch CV → oscillator

### Result
You hear an ostinato rhythm where each pitch repeats several times before changing.

This is great for:
- Berlin-school sequences
- minimal techno arps
- generative tonal lines
- basslines with internal rhythmic consistency

---

## 4. Use prime divisions for long melodic cycles

The **prime number division mode** is especially musical.

Available outputs:
- 2
- 3
- 5
- 7
- 11
- 13
- 17

If you use these to control different melodic events, the full pattern takes a long time to repeat.

### Example
- `/3` → sequencer A advance
- `/5` → sequencer B advance
- `/7` → switch between two pitch sources
- `/11` → transposition event
- `/17` → reset

### Result
The melody evolves slowly and unpredictably, but still remains synchronized to the master clock.

This is one of the best uses of the module for generative melody.

---

## 5. Switch between pitch sources

If you have a **sequential switch**, **VC switch**, or **addressed switch**, the A-160-2 can choose when different pitch streams become active.

### Patch
- Sequencer 1 pitch → switch input 1
- Sequencer 2 pitch → switch input 2
- Quantized random voltage → switch input 3
- A-160-2 divided outputs → switch clock / advance / control logic

### Result
A melodic line can alternate between:
- repeated sequenced phrases
- random notes
- transposed variations

For example:
- `/4` advances the switch
- `/16` resets the switch
- `/3` clocks one sequencer
- `/5` clocks another

The melody becomes structured but non-repetitive.

---

## 6. Use trigger mode for shorter note events

The manual notes two output styles:

- **Gate mode:** acts like a normal divider
- **Trigger mode:** outputs are ANDed with the clock signal, so pulse width depends on incoming clock pulse width

### Melodic use
Trigger mode is useful when you want:
- short note articulations
- precise re-triggering
- sharper stepped melodic changes
- cleaner interaction with envelope generators

If the divided signal is used to:
- advance a sequencer
- trigger a quantized S&H
- ping an envelope

then **Trigger mode** can produce more percussive melodic patterns.

### Gate mode
Gate mode is better when you want:
- sustained notes
- longer held stages
- drones with periodic pitch changes
- tied-note phrasing

---

## 7. Use reset for phrasing

The **reset input** is a big deal musically.

Whenever reset is received, all outputs go to defined states depending on the selected mode. That lets you force phrases to restart in a controlled way.

### Patch ideas
- Bar reset from master sequencer → A-160-2 reset
- `/16` from another divider → reset
- Manual gate button → reset for live performance
- End-of-cycle from envelope or function generator → reset

### Musical result
You can make generated melodies feel intentional:
- 16-step phrases
- 8-bar cycles
- repeating motifs with internal variation
- periodic return to “home”

Without reset, generative patches can drift endlessly. With reset, they become compositional.

---

## 8. Generate transposition events

Another powerful melodic technique is using divider outputs to trigger **precision adders**, **offset changes**, or **secondary quantized voltages**.

### Example
- Main sequencer → quantizer → oscillator pitch
- `/8` → trigger S&H sampling a slow CV
- S&H output → precision adder with main pitch
- `/32` → reset transposition sequencer

### Result
The basic melody continues, but every 8 clocks it is transposed by a new interval.

This is especially effective if the sampled CV is quantized to:
- octaves
- fifths
- chord tones
- modal scale degrees

The A-160-2 becomes a phrase-level harmonic controller.

---

## 9. Make canon / counterpoint lines

Because you get several divisions simultaneously, you can create multiple melodic voices derived from one clock.

### Patch
- `/2` → sequencer 1 clock
- `/4` → sequencer 2 clock
- `/8` → sequencer 3 clock

Each sequencer controls a different oscillator, or one sequencer controls pitch while others control transposition or articulation.

### Result
You get voices moving at related but different speeds:
- lead line
- slower counterline
- very slow bass movement

This is a great way to create:
- canon-like textures
- phase music
- layered ambient melodies
- polyrhythmic tonal structures

---

## 10. Use inverted output mode creatively

The manual mentions a jumper for **output polarity**:
- positive = normal outputs
- negative = all outputs inverted

This matters if you’re using the outputs not only for triggers, but also for:
- clocking modules that react to edges
- logic combinations
- gate-controlled switches
- burst generators
- sequential routing

### Melodic application
Inverted gates can create:
- complementary phrase structures
- rests where notes previously occurred
- alternate clocking for a second voice
- anti-phase articulation between melody and harmony

For example:
- normal `/4` triggers voice 1
- inverted `/4` triggers voice 2 envelope or switch state

That can produce call-and-response motion.

---

## 11. Pair with logic for richer melodic behavior

The A-160-2 becomes much more melodic when paired with logic modules:
- AND
- OR
- XOR
- flip-flops
- comparators

### Example
- `/3` and `/5` → AND logic → trigger melodic accent note
- `/2` and `/7` → XOR → alternate phrase trigger
- `/11` → reset one sequencer
- `/13` → switch transposition source

### Result
Instead of simple repetition, you get conditional melodic events:
- occasional grace notes
- phrase accents
- long-form motif changes
- irregular but synchronized harmonic shifts

---

## 12. Clock modulation sources that affect pitch

Melody doesn’t only come from sequencers. It also comes from modulation routed into pitch.

### Patch
- A-160-2 output → clock a stepped CV source or function generator
- Modulation source → attenuator
- Attenuated CV → quantizer or pitch adder
- Main sequencer pitch + modulation → oscillator

### Result
The melodic contour shifts periodically:
- every 3 notes a small bend
- every 7 notes a new register
- every 16 notes a phrase lift

This is a subtle but expressive way to make melodies feel alive.

---

## Specific patch recipes

## Patch 1: Simple evolving melody
**Needs:** A-160-2, clock, random or looping CV, sample & hold, quantizer, oscillator, envelope, VCA

- Clock → A-160-2 clock in
- `/4` → S&H trigger
- Random CV → S&H input
- S&H out → quantizer → oscillator pitch
- `/2` → envelope trigger
- Envelope → VCA CV
- Oscillator → VCA → output

**What happens:**  
A new pitch is selected every 4 clock pulses, but notes articulate every 2 pulses. This creates repeating rhythmic notes with slower pitch movement.

---

## Patch 2: Prime-based generative tonal line
**Needs:** A-160-2, two sequencers or one sequencer + quantized random source, quantizer, precision adder

Set A-160-2 to **prime mode**.

- `/3` → main sequencer clock
- `/5` → transposition sequencer clock
- Main sequencer CV → precision adder input A
- Transposition CV → precision adder input B
- Adder output → quantizer → oscillator
- `/17` → reset both sequencers or A-160-2

**What happens:**  
The melody and its transposition evolve on different prime-length cycles, producing long non-repeating melodic structures.

---

## Patch 3: Two-voice melodic counterpoint
**Needs:** A-160-2, two voices, two pitch sources or one source plus octave shifter

- `/2` → voice 1 envelope/sequencer clock
- `/4` → voice 2 envelope/sequencer clock
- Same pitch sequence to both voices, but:
  - voice 2 transposed by 5th or octave
- `/8` → reset or switch chord tone source

**What happens:**  
Voice 1 is active and agile; voice 2 moves more slowly, creating harmonic/melodic interplay.

---

## Patch 4: Melodic switching pattern
**Needs:** A-160-2, 3 pitch sources, sequential switch, quantizer

- Pitch source A = sequencer
- Pitch source B = random stepped CV
- Pitch source C = slow LFO through quantizer
- All into switch inputs
- A-160-2 `/4` → switch advance
- A-160-2 `/16` → switch reset
- Switch out → oscillator pitch
- `/2` → note trigger

**What happens:**  
The pitch source itself changes over time, creating sections in the melody.

---

## Things to keep in mind from the manual

## 1. Pulse width matters in Trigger mode
Because Trigger mode is ANDed with the incoming clock, the incoming clock pulse width affects the output pulse width. If your source clock has extremely narrow pulses, your melodic triggers may become very short.

## 2. Reset configuration is jumper-based
Reset can be:
- level-triggered or edge-triggered
- positive or negative

That matters if your system reset source behaves unusually.

## 3. Clock edge can be selected
You can choose whether rising or falling edge drives the output changes. This is useful for timing feel:
- one edge may make the sequence feel slightly more “on the beat”
- the other can offset interaction with envelopes, switches, or sequencers

## 4. A-161 is not compatible
The manual explicitly says the **A-161 cannot be connected** to the A-160-2, because this module is conceptually different from the original A-160.

---

## Best companion modules for melodic use

The A-160-2 works especially well with:

- **Quantizers**  
  To turn sampled or modulated voltages into musical notes

- **Sample & Hold / Track & Hold**  
  For clocked pitch selection

- **CV sequencers**  
  For note patterns and transpositions

- **Sequential switches**  
  For alternating between melodic sources

- **Logic modules**  
  For more complex phrase structures

- **Precision adders / mixers**  
  For interval layering and harmonic movement

- **Envelope generators + VCAs**  
  For note articulation

- **Clock generators / master transport modules**  
  To define global tempo and resets

---

## Overall musical verdict

The **Doepfer A-160-2** is best thought of as a **melodic timing brain**, not a note source. Its strength is in organizing time relationships that create:

- repeating motifs
- polymetric melodies
- transposition cycles
- generative phrase movement
- layered counterpoint
- controlled long-form evolution

The **prime division mode** is especially valuable if you want melodies that feel organic and slow to repeat, while the **reset input** lets you keep the patch musically coherent.

If you want, I can also turn this into:
1. a **set of concrete patch diagrams**,  
2. a **“best companion modules” shopping list**, or  
3. a **genre-focused guide** for techno, ambient, Berlin school, or generative melodic patching.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)