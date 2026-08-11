# Doepfer — A-151 Quad Sequential Switch

- [Manual PDF](../../manuals/A151_man.pdf)

---

[Doepfer A-151 Quad Sequential Switch Manual (PDF)](https://doepfer.de/a100_man/a151_man.pdf)

# Doepfer A-151 Quad Sequential Switch — creative patch ideas

The **A-151** is a **4-step bidirectional sequential switch**: each trigger advances the common jack to the next of four jacks, and reset returns it to step 1. In **v2**, you also get a **2/3/4-step selector** and full **±12V** signal handling. Practically, it can behave as:

- **4 inputs → 1 output**
- **1 input → 4 outputs**
- an **audio router**
- a **CV router**
- a **rhythmic structure tool**
- a **manual-seeming form generator** when clocked and reset cleverly

Because it is so simple, it becomes powerful when paired with clocks, gates, envelopes, VCAs, mixers, sequential voltage sources, logic, and sound sources.

---

## What the manual tells us musically

Key takeaways from the manual:

- It advances on the **rising edge** of the trigger.
- **Reset** instantly forces it back to **I/O 1**.
- It is **bidirectional**, so think both “multiple sources to one destination” and “one source to multiple destinations.”
- At high trigger rates, it can create **audio-rate switching effects**, effectively generating new timbres.
- The v2 **2/3/4 step switch** is very useful for phrase lengths and polyrhythms.

That means the A-151 is not just a utility switch — it is a **structure generator**.

---

# Best companion module types

If you want the A-151 to shine, pair it with:

- **Clock / trigger sources**  
  e.g. Pamela’s New Workout, Tempi, 4ms QCD, Batumi in square mode, simple LFOs
- **Logic / trigger processing**  
  e.g. Doepfer A-166, Joranalogue Compare 2, Mutable Kinks, OR combiners
- **Sequential voltages / sequencers**  
  e.g. Doepfer A-155/A-154, Make Noise 0-CTRL, Metropolix, Pressure Points + Brains
- **Envelope generators**  
  e.g. Doepfer A-140, Intellijel Quadrax, Befaco Rampage, Maths
- **VCAs / mixers**  
  e.g. Veils, A-135, Happy Nerding 3xVCA, Mutable Blinds
- **Filters with multiple outputs**  
  e.g. Doepfer A-121, XAOC Zagrzeb, QPAS, multi-mode filters generally
- **Oscillators with multiple simultaneous outputs**  
  e.g. A-110, Dixie, STO + sub, analog VCOs with saw/pulse/triangle/sine outs
- **Effect modules**  
  delays, resonators, wavefolders, frequency shifters, granular FX
- **Sample & hold / slew / quantizers**  
  e.g. A-148, A-170, O_C, uScale, Disting

---

# Core patch concepts

## 1. Waveform animator
**What to patch**
- VCO triangle/saw/pulse/sub into **I/O 1–4**
- **O/I** to filter or VCA
- Clock the **Trig In** with LFO, gate pattern, or another VCO square

**Result**
- Slow clocks: stepped timbral changes
- Medium clocks: rhythmic waveform alternation
- Audio-rate clocks: new buzzy composite timbres, crude wavefolding-ish textures

**Make it better**
- Put slightly different processing on each waveform before the A-151:
  - one dry
  - one filtered
  - one wavefolded
  - one ring modded
- Then switch between “versions” of the same oscillator.

**Recommended partners**
- Any analog VCO
- Wavefolder like uFold / A-137
- Filter with strong character
- Fast square LFO or oscillator for triggering

---

## 2. One sequence, four destinations
**What to patch**
- Sequencer CV or modulation source into **O/I**
- Outputs **I/O 1–4** to:
  - VCO pitch
  - filter cutoff CV input
  - waveshaper amount
  - effect parameter

Clock the A-151 to rotate where the same CV goes.

**Result**
A single melodic or modulation pattern gets “thrown” around the patch, creating animated arrangements from minimal material.

**Variation**
Use different attenuators on each destination so the same source behaves differently each step.

**Great with**
- precision adders
- attenuverters
- quantizers
- modulation destinations that like stepped CV

---

## 3. Four envelopes, one voice
This is one of the manual’s examples and it’s genuinely excellent.

**What to patch**
- Four envelopes into **I/O 1–4**
- **O/I** to filter CV, VCA CV, wavefolder CV, or FM index CV
- Same clock/gate triggers all four envelopes and also clocks the A-151

**Result**
Each note uses a different envelope shape, even though the voice architecture stays the same.

**Best use**
- Different filter plucks per step
- Different VCA dynamics
- Alternating long/short accents
- Different FM index shapes for each note

**Upgrade idea**
Use:
- one AD envelope
- one slow AR envelope
- one snappy exponential envelope
- one looping envelope

Now the timbre cycles in a more performative way.

---

## 4. One envelope, four destinations
Reverse the prior idea.

**What to patch**
- A single envelope into **O/I**
- **I/O 1–4** to various CV destinations:
  - filter
  - VCA
  - oscillator PWM
  - FX send level

**Result**
On each trigger, the envelope shapes a different aspect of the patch. This can make one voice feel like a whole arrangement.

**Try**
Routing one envelope sequentially to:
1. pitch sweep
2. filter ping
3. reverb amount
4. wavefolder depth

---

## 5. Sequential effects chain selector
**What to patch**
- Voice or drum loop into **O/I**
- **I/O 1–4** each go to a separate processor input path
- Return processed outputs to mixer

Or, depending on your routing options, feed:
- four different processed versions of a sound into **I/O 1–4**
- take **O/I** as the selected result

**Example four paths**
- dry
- delay
- phaser
- distortion

**Result**
Per-step FX changes without needing a full matrix mixer.

**Best with**
- compact stereo mixer
- FX aid / Mimeophon / Magneto / Desmodus style processors
- drum voices or drones

---

## 6. Filter mode sequencer
Also suggested by the manual.

**What to patch**
- Use a multi-mode filter with several simultaneous outputs:
  - LP
  - BP
  - HP
  - notch
- Patch those to **I/O 1–4**
- **O/I** goes to VCA/output
- Advance A-151 every note or every bar

**Result**
The same source walks through different filter characters.

**Why it works**
This keeps pitch/melody stable while changing the spectral role of the sound. Very useful in techno, electro, and generative patches.

**Great companion filters**
- Doepfer A-121
- Mutable Ripples
- QPAS
- any SEM-style or multimode filter

---

## 7. Phrase-length tricks with reset
The reset input is where a lot of the musical magic lives.

**What to patch**
- Steady clock to **Trig In**
- A different rhythm or gate pattern to **Res. In**

**Result**
Instead of a boring 1-2-3-4 loop, you get asymmetrical forms:
- 1-2-1-2-3-1-2-3-4...
- 1-2-3-1-2-3...
- irregular restarts synced to another pattern

**Creative sources for reset**
- gate from sequencer end-of-cycle
- Euclidean rhythm
- manual gate button
- comparator output from slow CV
- odd clock division

**Very effective for**
- melody selection
- timbral phrase resets
- structured but non-repetitive modulation

---

## 8. 2-step / 3-step / 4-step polymeter engine
If you have **v2**, use the step selector musically.

**Patch idea**
- Run one A-151 at 3 steps
- Another sequential process elsewhere at 4 or 5 steps
- Clock both together

**Result**
Longer evolving cycles due to pattern interference.

**With one A-151**
Even just switching the module between 2, 3, and 4 steps during a performance changes perceived phrase length instantly.

**Use for**
- drum fills
- bass variation
- call/response structures
- modulation loops that never line up the same way twice

---

## 9. Sequential transposition hub
**What to patch**
- Main pitch CV sequence into **O/I**
- Outputs **I/O 1–4** to four precision adders or quantizer input chains, each with a different offset/transposition
- Or reverse it: put four different transposed versions into **I/O 1–4** and take **O/I** to the oscillator

**Result**
Same melody, different harmonic positions each step/bar.

**Examples**
- root
- +5th
- octave
- minor 3rd

**Excellent with**
- quantizer
- precision adder
- buffered multiple
- chord-capable oscillators

---

## 10. Drum voice rotation
**What to patch**
- One trigger stream into **O/I**
- Outputs **I/O 1–4** to four drum trigger inputs

Now each incoming trigger hits a different drum in sequence.

**Result**
A single pulse train becomes a pattern spread over kick/snare/hat/clap or multiple voices.

**Variation**
Send irregular triggers to the A-151 clock, and a master pulse stream through the switched path, or vice versa.

**Advanced variation**
Route accent CV instead of triggers so different drums get the same accent pattern on different steps.

---

## 11. Accent distributor
**What to patch**
- Accent gate or accent envelope into **O/I**
- **I/O 1–4** to:
  - VCA CV boost
  - filter accent
  - FM amount accent
  - delay feedback duck/accent path

**Result**
Each accent lands on a different musical parameter, which gives far more life than a static accent lane.

---

## 12. Sequential clock divider / distributor feel
The A-151 is not a divider itself, but it can behave like a **rotating clock destination**.

**What to patch**
- Master trigger into **O/I**
- **I/O 1–4** to four envelope gates, drum triggers, or sequencer advance inputs
- Clock A-151 with a slower pulse

**Result**
A repeating trigger source gets sent to different modules over time, creating changing rhythmic emphasis.

**Companion modules**
- clock dividers
- Bernoulli gates
- trigger delays
- logic modules

This is especially good in drum systems.

---

## 13. Address four modulation rates/shapes
**What to patch**
- Four modulation sources into **I/O 1–4**:
  - slow sine LFO
  - random stepped CV
  - looping envelope
  - sample & hold
- **O/I** to one destination like filter cutoff

**Result**
That one destination behaves like it has a “macro arrangement” around it, with each section animated differently.

**Best destination choices**
- filter cutoff
- wavetable position
- wavefolder depth
- stereo spread
- reverb size

---

## 14. Sequential feedback path selector
Excellent for experimental patches.

**What to patch**
- Put the A-151 in a feedback network:
  - mixer send or processor output into **O/I**
  - **I/O 1–4** go to different feedback treatments:
    - clean feedback
    - filtered feedback
    - distorted feedback
    - delayed feedback
- Selected path returns to mixer/effect input

**Result**
Feedback character changes step by step. This can create very alive dub-techno and noise textures.

**Be careful**
Levels can get intense quickly; a VCA or attenuator in the feedback loop helps a lot.

---

## 15. Sequential sample source selector for S&H
**What to patch**
- Four CV sources into **I/O 1–4**
- **O/I** to sample & hold input
- A-151 clocked slowly, S&H clocked faster or differently

**Result**
The S&H draws from a rotating set of source voltages, producing much more structured random-ish behavior.

**Example sources**
- offset voltage
- sequencer row
- noise through slew
- envelope
- slow LFO

**Great with**
- quantizer for melodies
- slew for glide
- comparator for rhythm extraction

---

## 16. Audio-rate pseudo-granular or crude wavetable stepping
**What to patch**
- Four related audio signals into **I/O 1–4**
  - same oscillator through 4 filters
  - four phase-shifted signals
  - four harmonic-rich sources
- Clock A-151 from oscillator square or another audio-rate source

**Result**
Harsh, digital-like spectral animation; metallic tones; animated drones.

**Especially good with**
- fixed filter banks
- phase shifters
- ring mod
- submixes of harmonics

---

## 17. Voice allocation / round robin
**What to patch**
- Pitch CV can be multed to several voices
- Gate into **O/I**
- **I/O 1–4** to four envelope/gate inputs for four voices

Clock the A-151 with the same keyboard gate, or a derived trigger.

**Result**
Each new note is assigned to the next voice, creating rotating pseudo-polyphony or layered variation.

**Useful with**
- multiple identical voices
- chord stacks
- per-step different timbres

---

## 18. Sequential modulation of modulation
Use the A-151 not on the final sound path, but on the control path feeding another modulator.

**What to patch**
- Four CV sources into **I/O 1–4**
- **O/I** to FM amount CV, LFO rate CV, envelope decay CV, or clock rate CV

**Result**
You’re changing the behavior of another modulator in steps, which creates deeper evolving systems.

**Example**
Route 4 voltages to your LFO rate input:
- very slow
- medium
- fast
- near audio

Now your filter modulation “changes gears” each phrase.

---

## 19. Build a 16-step sequence from 4-step parts
If you have multiple short sequencers or 4-step voltage rows:

**What to patch**
- Four 4-step sequencer rows or voltage memories into **I/O 1–4**
- **O/I** to oscillator pitch or filter CV
- Advance A-151 every 4 notes using a clock divider

**Result**
You effectively chain four short sequences into a longer form.

**Excellent modules for this**
- Pressure Points
- A-155 rows
- Voltage Block channels
- 0-CTRL rows
- simple voltage sources plus attenuators

---

## 20. Morph between four “scenes”
Create four different complete versions of a sound or control idea, then use the A-151 to move through them.

**Example scene sources**
1. dry bass
2. filtered bass
3. FM bass
4. delayed bass

or in CV terms:
1. calm modulation
2. rhythmic modulation
3. random modulation
4. extreme modulation

The A-151 gives clean scene changes with a simple clock.

---

# Particularly strong module pairings

## With Pamela’s New Workout
- Use one channel as clock
- another as reset pattern
- another as stepped random trigger density
- another as Euclidean reset

This turns the A-151 into a phrase and structure machine.

## With Maths / function generators
- Send four different envelopes or slews into the A-151
- or switch one Maths channel to four destinations
- use EOC/EOR outputs to trigger or reset the switch

Very fertile for self-running patches.

## With a quantizer
- Rotate between four CV sources before quantization
- or rotate between four quantized pitch offsets after quantization

This keeps melodies coherent while still changing.

## With logic
- Trigger from one rhythm
- reset from AND/XOR/OR-derived events

This creates “composed” irregularity.

## With a matrix mixer
Use the A-151 to select different sources or destinations, then use the matrix mixer to blend the consequences. Great for performance systems.

## With another sequential switch
Two A-151s together are much more than double the power:
- one selects pitch source
- the other selects timbre source
- different clocks/reset patterns create long cycles

Or chain them to make more than 4 stages.

---

# Performance-oriented ideas

## Manual reset as a fill button
Patch a button or gate controller to **Res. In**.  
During performance, force the cycle back to step 1 to re-anchor the phrase.

## Section changes with the step selector
On v2, move between:
- 2-step for tight alternation
- 3-step for lopsided groove
- 4-step for full phrase

It’s a simple but very effective performance gesture.

## Create “lead voice spotlighting”
Send a shared modulation or effects send sequentially to different voices. Each bar, a different voice gets the spotlight.

---

# Things to watch out for

- **Version matters**: older versions are more limited in signal range; v2 handles full **±12V**.
- Fast switching can click — but often that’s musically useful.
- If switching audio, matching levels between sources helps avoid ugly jumps unless you want them.
- Reset timing can strongly affect groove; try slightly shifted reset pulses for less rigid behavior.
- Because it’s passive in concept but active in use, attenuation and buffering around it can make patches more predictable.

---

# My favorite high-value patch recipes

## A. Four-character bassline
- One VCO to four differently processed paths
- A-151 selects path each note
- same sequencer pitch the whole time
- reset every 8 or 16 steps

You get a bassline that sounds arranged rather than looped.

## B. Modulation carousel
- 4 CV sources into A-151
- output to one important destination
- trigger every bar
- reset on phrase start

Simple, elegant macro-evolution.

## C. Rotating drum accents
- Accent envelope through A-151 to kick/snare/hat/clap accent inputs
- clocked every 2 or 4 beats

Small patch, big groove payoff.

## D. Evolving drone switcher
- 4 filtered variants of same drone
- A-151 switched at sub-audio or audio rate
- occasional resets from random gate source

Excellent for ambient, industrial, and electroacoustic work.

## E. Four-envelope sequenced filter
- the manual’s patch, but with wildly different envelope times and shapes
- use one super short pluck, one medium decay, one inverted envelope, one very slow sweep

This makes a single sequence feel alive immediately.

---

# Summary

The **Doepfer A-151** is deceptively powerful. It excels at:

- **rotating timbres**
- **distributing modulation**
- **building phrase structure with reset**
- **creating variation from minimal material**
- **audio-rate spectral switching**
- **turning one source into a multi-part arrangement**

If you treat it as a **compositional router** rather than just a utility switch, it becomes one of the most musical low-HP modules in Eurorack.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)