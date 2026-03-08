# Itijik — Toggle

- [Manual PDF](../../manuals/toggle.pdf)

---

[Manual PDF](#)

# Itijik Toggle — creative patch ideas and combo suggestions

This module is a **quad flip-flop with a normalized inverter per channel**. In practice, that makes it a compact bank of:

- **4 gate toggles / state memories**
- **4 manual-free logic inverters** via the `VERT` outputs
- **4 simple clock dividers by 2** when hit with regular clocks
- **4 gate conditioners / event routers**
- **4 places to derive complementary rhythms** from one source

The key trick is this:

- `CLK` toggles `OUT`
- `SET` forces `OUT` high
- `RST` forces `OUT` low
- `VERT` is normally the inverse of `OUT`
- plugging something into `IN` breaks that normalization, so `VERT` becomes an inverter for whatever you patch into `IN`

That means each section can be either:

1. a **flip-flop with complementary outputs**, or  
2. a **standalone logic inverter**

That’s extremely useful in a patch.

---

## What Toggle is especially good at

Before getting into combinations, here are the main musical jobs it excels at:

- **Turning pulses into alternating on/off states**
- **Creating complementary gate streams**
- **Remembering events**
- **Switching between two structural states**
- **Deriving “anti-rhythms” from a rhythm**
- **Converting trigger streams into longer-held gates**
- **Building patch logic without a dedicated logic module**
- **Driving mutes, resets, fill states, and performance macros**

---

# Best module pairings

## 1. With clock sources / trigger sequencers
**Examples:** Pamela’s Pro Workout, Tempi, 4ms QCD, Noise Engineering Horologic Solum, trigger lanes from Metropolix, Eloquencer, Circadian Rhythms

This is probably the most obvious and powerful pairing.

### Ideas
- Send a steady clock to `CLK` for one channel: `OUT` becomes a **divide-by-2 square gate**
- Use `OUT` and `VERT` to create **alternating rhythmic layers**
- Feed irregular trigger patterns into `CLK` to get **stateful rhythms** that depend on event history instead of simple multiplication/division

### Patch example: alternating drum voices
- Clock source → `CLK`
- `OUT` → kick trigger input
- `VERT` → closed hat trigger input

Now kick and hat alternate every pulse.  
Run those through VCAs or logic afterward for more dynamic behavior.

### Patch example: fills every other bar
- Bar clock / phrase pulse → `CLK`
- `OUT` → open a VCA for fill triggers
- `VERT` → open the “normal groove” lane

This gives you a simple A/B phrase alternation.

---

## 2. With sequential switches
**Examples:** Doepfer A-151, Joranalogue Switch 4, Boss Bow Two, Erica Sequential Switch, Verbos Sequence Selector

Flip-flops and switches are fantastic together.

### Why it works
Use Toggle to decide **when a switch changes role** or **which structural layer is active**.

### Patch example: melody every other phrase
- Phrase clock → Toggle `CLK`
- Toggle `OUT` → A-151 advance or reset logic
- Toggle `VERT` → gate a second voice or route a second CV lane

### Patch example: A/B/A/B modulation routing
- LFO bank into switch inputs
- Toggle channel controls whether the switch is addressed or reset
- Complementary `OUT`/`VERT` can drive two switch control inputs or VCAs for cross-routed modulation

This makes long-form structure from simple clocks.

---

## 3. With logic modules
**Examples:** Joranalogue Compare 2, Doepfer A-166, Klavis Logica XT, Intellijel Plog, Bastl Little Nerd, Vice Virga, Mystic Circuits Ana/XOR

Toggle gets much more interesting when mixed with Boolean logic.

### Ideas
- Use `OUT` and `VERT` as complementary logic sources into **AND/OR/XOR**
- Combine a trigger stream with a latched state for **conditional rhythms**
- Use `SET` and `RST` from different event sources to create a patch that “remembers” which event happened last

### Patch example: last-event-wins rhythm memory
- Euclidean rhythm A → `SET`
- Euclidean rhythm B → `RST`
- `OUT` = “A currently dominates”
- `VERT` = “B currently dominates”

Then use those outputs to enable different voices or modulation buses.

### Patch example: XOR accents
- Toggle `OUT` + another trigger sequence into XOR
- Use result for accent or ratchet triggers

This can create more complex rhythmic behavior than simple divisions.

---

## 4. With VCAs
**Examples:** Veils, Quad VCA, ALM Tangle Quartet, Intellijel Quad VCA, Happy Nerding 3xVCA

VCAs turn Toggle from “logic utility” into a **patch structure controller**.

### Patch example: alternating modulation destinations
- LFO → mult to two VCAs
- Toggle `OUT` opens VCA 1
- Toggle `VERT` opens VCA 2
- VCA 1 → filter FM
- VCA 2 → wavefolder CV

One clock pulse now flips where the modulation goes.

### Patch example: pseudo mute groups
- Drum triggers through VCAs or logic-controlled VCAs
- `OUT` opens one rhythmic lane
- `VERT` opens another

You get performance-friendly contrast with a single clocked toggle.

---

## 5. With envelope generators and function generators
**Examples:** Maths, Function, Contour 1, Zadar, Quadrax, Delta-V, Pip Slope

This is great for turning trigger sequences into alternating articulation states.

### Patch example: alternating envelope shapes
- One trigger source goes to two envelopes
- Toggle `OUT` triggers envelope A
- Toggle `VERT` triggers envelope B
- Envelope A = short pluck
- Envelope B = long decay

Now a single rhythm alternates between two articulations.

### Patch example: attack/release mode changes
Use Toggle outputs to gate which envelope reaches a VCA or LPG. This creates phrasing that feels intentional and arranged.

---

## 6. With drum modules / percussion voices
**Examples:** Basimilus Iteritas Alter, WMD Crucible, Tiptop drum voices, SSF Entity, Noise Engineering drum modules, sample players

Toggle is excellent for percussion structure.

### Patch ideas
- Alternate two drum voices from one trigger stream
- Use `SET`/`RST` for fills and break states
- Invert accent patterns using `VERT`

### Patch example: breakbeat mutator
- Main trigger clock → `CLK`
- `OUT` → snare lane enable
- `VERT` → percussion lane enable
- Manual or sequenced pulse to `SET` at phrase start
- Different pulse to `RST` at phrase end

This lets you force known states at structural boundaries.

---

## 7. With sample & hold / random modules
**Examples:** Mutable Marbles, Wogglebug, SSF Ultra-Random, Turing Machine, Sapèl, Orbit 3, Ochd + S&H, Nano Rand

This pairing is very musical because Toggle can impose **binary order** on random material.

### Patch example: random only every other beat
- Random trigger source → `CLK`
- `OUT` opens a VCA carrying random CV to pitch
- `VERT` opens a slewed or quantized alternative source

Result: random and stable phrases alternate.

### Patch example: controlled chaos gate
- Random pulse source → `SET`
- Master reset pulse → `RST`
- Use `OUT` to indicate “chaos mode active”

That state can control feedback amount, modulation depth, sample rate reduction, etc.

---

## 8. With quantizers and melodic sequencers
**Examples:** uScale, Scales, O_C, Bard Quartet, Metropolix, René, Pressure Points + quantizer

Toggle is not a pitch module, but it’s excellent for **phrase logic**.

### Patch example: two-sequence alternator
- Sequencer A and B each go through separate VCAs or switches
- Toggle `OUT` selects sequence A
- Toggle `VERT` selects sequence B
- Clock Toggle from bar or phrase pulse

You get instant verse/chorus melodic alternation.

### Patch example: melodic answer phrases
- Main melody trigger → `CLK`
- `OUT` opens quantized melody lane
- `VERT` opens transposed response lane

This creates call-and-response behavior.

---

## 9. With burst generators / ratchets
**Examples:** Quadrax burst mode, Pamela’s ratchets, Noise Engineering Integra Solum / related trigger tools, 4ms PEG, Befaco Burst

### Patch example: ratchets every other hit
- Trigger stream → `CLK`
- `OUT` → ratchet trigger enable
- `VERT` → straight trigger lane

Now only alternating hits ratchet.

### Patch example: phrase-end drama
- End-of-bar pulse → `SET`
- Next downbeat → `RST`
- While `OUT` is high, burst generator is active

This creates a fill window during the final part of a phrase.

---

## 10. With comparators / gate extractors
**Examples:** Joranalogue Compare 2, Doepfer comparator utilities, envelope followers, threshold extractors

These combinations let Toggle respond to **analog events**.

### Patch example: dynamics-driven state switching
- Envelope follower from drum loop or external input → comparator
- Comparator pulse → `CLK` or `SET`
- Toggle state then controls another layer

So the patch changes state when the source material crosses a threshold.

### Patch example: sidechain-controlled alternation
- Kick envelope threshold crossing → `CLK`
- `OUT` and `VERT` then alternate modulation destinations or voice access

---

## 11. With manual gate controllers / touch controllers
**Examples:** Pressure Points, 0-CTRL gate outs, manual buttons, gate keyboards, Tetrapad, controllers with trigger outputs

### Patch example: playable latching performance state
- Button/touch gate → `CLK`
- `OUT` = “section A active”
- `VERT` = “section B active”

Or use dedicated buttons:
- button 1 → `SET`
- button 2 → `RST`

This gives you a super immediate performance control layer for mutes, transpositions, modulation buses, effect sends, etc.

---

## 12. With effects and feedback systems
**Examples:** Mimeophon, Magneto, Data Bender, FX Aid, feedback mixers, filters, wavefolders

Toggle is very useful for controlling **when feedback or effect routing is active**.

### Patch example: alternating dry/wet phrases
- Audio path split to dry and FX return VCAs
- Toggle `OUT` opens dry emphasis
- Toggle `VERT` opens wet emphasis

### Patch example: controlled feedback danger
- `OUT` opens feedback path
- `RST` receives a safety reset pulse every bar

You can flirt with unstable feedback but force the system back to safe territory periodically.

---

# Clever uses of the `IN` jack and `VERT` output

The normalization is a big deal and easy to overlook.

## 1. Free inverter bank
When you patch something into `IN`, `VERT` becomes the inversion of that signal instead of the inversion of `OUT`.

That means Toggle can act as:
- **four logic inverters**
- **four complementary gate generators**
- **a way to derive opposite mute logic**

### Example
- Trigger sequence into `IN`
- `VERT` → another voice

Now one voice gets the original sequence, and another can get the opposite logic behavior downstream.

This is especially useful if another module wants “not this gate”.

---

## 2. Dual-purpose channel
A single channel can be used as either:
- a flip-flop state source, or
- an inverter

So in one patch:
- channels 1–2 = state machines
- channels 3–4 = logic inversion for clocks, mutes, accents, reset conditioning

That makes it a very space-efficient “boring but magic” module.

---

# Patch ideas by musical goal

## For techno
- Use one channel as divide-by-2 for kick variations
- Another to alternate closed/open hats
- Another for fill activation every 8 or 16 beats
- Another as an inverter for accent logic into percussion FM depth

Good pairing:
- Pamela’s Pro Workout
- Basimilus Iteritas Alter
- Quad VCA
- A-151
- Compare 2 / logic module

---

## For generative ambient
- Use slow clocks into `CLK`
- Use `OUT`/`VERT` to alternate between two slow modulation ecosystems
- `SET` and `RST` come from random comparators or thresholded CV events
- Send outputs to VCAs controlling reverb send, filter opening, chord source selection, or delay feedback

Good pairing:
- Marbles / Turing Machine
- Ochd / Batumi
- Quad VCA
- Sequential switch
- Quantizer
- long-envelope generators

---

## For IDM / broken rhythm
- Clock channels from non-uniform trigger streams
- Cross-patch `OUT` of one channel to `SET` or `RST` of another
- Use `VERT` outputs as anti-rhythms into XOR/AND logic
- Route results into burst generators and sample players

Good pairing:
- logic module
- burst generator
- random trigger source
- clock manipulator
- switch
- drum sampler

---

## For live performance systems
- Use channels as persistent mute/scene states
- Manual triggers to `SET`/`RST`
- `OUT` and `VERT` drive two halves of your system
- Phrase clocks periodically reset things to known states

Good pairing:
- manual gate controller
- VCAs
- mutes/switches
- clock source
- sequencer with gate outs

---

# Advanced patch concepts

## 1. Cross-coupled state network
Use multiple channels to affect each other.

### Example
- Ch1 `OUT` → Ch2 `SET`
- Ch2 `OUT` → Ch3 `RST`
- Ch3 `VERT` → Ch1 `CLK`

Now the system has memory and can evolve in semi-unpredictable ways depending on initial conditions and incoming clocks.

This gets especially good when the driving clocks are not simple divisions.

---

## 2. State-based arrangement engine
Think of each channel as one “arrangement bit”.

- Ch1 = drums on/off state
- Ch2 = bass active/inactive
- Ch3 = FX send active/inactive
- Ch4 = fill mode active/inactive

Drive `SET`/`RST` from sequencer gates, manual buttons, or end-of-cycle signals.  
Then use the outputs to open VCAs, enable switches, or trigger logic.

You’ve basically built a mini patch-state controller.

---

## 3. Event memory from two competing sources
Because `SET` and `RST` force state, you can encode “which thing happened most recently.”

### Example
- Envelope threshold from voice A → `SET`
- Envelope threshold from voice B → `RST`

`OUT` now represents whether A or B was the last dominant event.  
That can drive panning, ducking, modulation focus, or voice allocation.

---

## 4. Alternating probability lanes
Pair Toggle with probabilistic triggers.

- Probabilistic trigger stream → `CLK`
- `OUT` enables sparse sequence
- `VERT` enables dense sequence

Because the trigger arrivals themselves are probabilistic, the alternation feels less mechanical than a straight divider.

---

# Specific module recommendations

## Excellent specific pairings
- **ALM Pamela’s Pro Workout** — clocks, odd divisions, logic-like gating, phrase control
- **Doepfer A-151** — simple but powerful routing partner
- **Joranalogue Compare 2** — thresholds, logic, comparators; very strong with Toggle
- **Intellijel Quad VCA / Mutable Veils** — convert logic states into audible structure
- **Xaoc Batumi / Instruō Øchd** — modulation sources to route or alternate
- **Mutable Marbles / Turing Machine** — random with binary structure
- **Noise Engineering Numeric Repetitor / trigger sequencers** — lots of pattern material to condition
- **Doepfer A-166 or Klavis Logica XT** — make the most of complementary outputs
- **Quadrax / Maths** — alternating envelopes and burst/fill logic
- **Boss Bow Two / switched routing modules** — patch-state changes become very performable

## Generic module types that pair well
- clock generator
- trigger sequencer
- logic module
- sequential switch
- VCAs
- envelope generator
- burst generator
- random source
- comparator
- quantizer
- drum voices
- manual gate controller
- effect send/return mixer

---

# A few simple “instant win” patches

## Instant patch 1: alternating hats
- steady 16th clock → `CLK`
- `OUT` → closed hat
- `VERT` → open hat

## Instant patch 2: every-other-bar bass variation
- bar pulse → `CLK`
- `OUT` opens primary bass modulation
- `VERT` opens alternate modulation or transposition

## Instant patch 3: fill latch
- fill button → `SET`
- next phrase start → `RST`
- `OUT` enables ratchets, bursts, or delay feedback

## Instant patch 4: free inverter utility
- trigger pattern → `IN`
- `VERT` → complementary logic for another lane

## Instant patch 5: memory of competing generators
- random trigger A → `SET`
- random trigger B → `RST`
- `OUT` and `VERT` control two different voices

---

# Bottom line

Itijik Toggle is deceptively simple, but it’s one of those modules that can make a whole system feel more intentional. It excels at:

- **alternation**
- **state memory**
- **complementary gate creation**
- **arrangement logic**
- **converting raw triggers into structure**

It becomes especially powerful when paired with:

- **clocks**
- **logic**
- **VCAs**
- **switches**
- **random sources**
- **manual performance controls**

If you want, I can also give you:
1. **10 concrete patch recipes** using specific popular Eurorack modules, or  
2. **a small “system design” plan** showing what kind of case pairs best with Toggle.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)