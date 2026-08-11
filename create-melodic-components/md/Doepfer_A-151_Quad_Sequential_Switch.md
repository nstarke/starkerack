# Doepfer — A-151 Quad Sequential Switch

- [Manual PDF](../../manuals/A151_man.pdf)

---

[Doepfer A-151 Quad Sequential Switch Manual (PDF)](https://doepfer.de/a100_man/A151_man.pdf)

# Using the Doepfer A-151 to Create Melodic Material

The attached manual is for the **Doepfer A-151 Quad Sequential Switch**, a very simple but extremely musical utility. Even though it does not generate pitch by itself, it becomes a strong **melody-creation module** when combined with oscillators, sequencers, envelopes, clocks, LFOs, quantizers, mixers, and filters.

## What the A-151 does

The A-151 is basically a **4-step sequential signal router**:

- One **common jack**: `O/I`
- Four switched jacks: `I/O 1–4`
- A **Trigger In** input advances the switch by one step
- A **Reset In** input returns it to step 1
- LEDs show the active step
- Version 2 adds a **2 / 3 / 4 step selector**

It is **bidirectional**, which is the key to musical use:

- **4 inputs → 1 output**
- or **1 input → 4 outputs**

That means it can be used to:
- rotate through **different pitch CV sources**
- distribute one pitch sequence to **different destinations**
- rotate through **different rhythmic gates / envelopes / timbral states**
- create repeating phrase structures with reset control

## Important practical notes from the manual

- Triggering happens on the **rising edge**
- Reset immediately returns the switch to **I/O 1**
- Older versions handle about **-8V to +8V**
- Version 2 handles **-12V to +12V**
- Fast switching can enter **audio-rate territory**, which can create new timbral results

For melodic patching, this means it is ideal for **control voltage sequencing**, phrase switching, and step-based variation.

---

# Best melodic uses of the A-151

## 1. Switching between multiple pitch sources

This is the most direct melodic application.

### Patch idea
Send four different melodic CV sources into `I/O 1–4`, and take `O/I` to your oscillator’s 1V/oct input, ideally through a quantizer if needed.

Example sources:
- `I/O 1`: a slow 8-step sequencer
- `I/O 2`: a transposed copy of that sequencer
- `I/O 3`: random stepped CV
- `I/O 4`: a fixed voltage or keyboard CV

Then:
- clock the A-151 from a divided trigger
- send `O/I` → quantizer → VCO 1V/oct

### Result
Each trigger to the A-151 changes which melodic source is currently controlling pitch. This gives:
- phrase changes
- verse/chorus-style movement
- call-and-response lines
- evolving melodic patterns

### Musical benefit
Instead of writing one sequence, you can write **four related pitch behaviors** and let the A-151 structure them into a larger melody.

---

## 2. Creating 2-, 3-, or 4-bar melodic phrases

If your A-151 is version 2, the **step count switch** is very useful musically.

### Patch idea
Use the A-151 to cycle through:
- 2 phrase variants
- 3 phrase variants
- 4 phrase variants

For example:
- `I/O 1`: root melody
- `I/O 2`: variation
- `I/O 3`: higher-register variation
- `I/O 4`: tension phrase

Clock the switch once per bar.

### Result
- In **2-step mode**, you get ABAB...
- In **3-step mode**, you get ABCABC...
- In **4-step mode**, you get ABCD...

This is excellent for melodies that feel composed rather than merely looped.

---

## 3. Reset-controlled melodic form

The reset input is one of the most useful musical features.

### Patch idea
Advance the A-151 with a regular clock, but send a reset pulse from:
- a manual gate button
- a clock divider
- an end-of-cycle trigger
- a sequencer reset output

### Result
You can force the melodic structure back to phrase 1 at predictable moments.

Examples:
- reset every 4 bars for a repeating song form
- reset irregularly for non-looping phrasing
- reset from a keyboard gate so every new played note starts from phrase 1

### Why this matters
Without reset, sequential switching can drift against the rest of your patch. With reset, it becomes a **musically aligned phrase sequencer**.

---

## 4. Routing one sequencer to different pitch destinations

Because the A-151 is bidirectional, you can also use it as **1 input → 4 outputs**.

### Patch idea
Send one melodic CV sequence into `O/I`, and use `I/O 1–4` as switched outputs to different destinations:
- `I/O 1`: VCO 1 pitch
- `I/O 2`: VCO 2 pitch
- `I/O 3`: filter cutoff CV input
- `I/O 4`: wavefolder or FM index CV

Trigger the A-151 every note or every few notes.

### Result
A single sequence is distributed to different parts of the patch over time. This creates:
- alternating lead and bass motion
- melody-to-timbre interaction
- pseudo-counterpoint
- dynamic phrase orchestration

This is especially effective if different destinations are attenuated differently.

---

## 5. Switching between transpositions

A very powerful melodic use is to patch **the same sequence processed four different ways**.

### Patch idea
Start with one pitch sequence. Mult it and process the copies differently:
- `I/O 1`: original
- `I/O 2`: +7 semitones
- `I/O 3`: +12 semitones
- `I/O 4`: -5 semitones

Then send `O/I` to your oscillator pitch input through a quantizer.

### Result
The A-151 turns a simple sequence into a **harmonically shifting melody generator**.

This can sound like:
- chord changes implied by a monophonic line
- modal movement
- octave jumps
- recurring refrain structures

This is one of the most musical uses of a sequential switch.

---

## 6. Switching gate patterns that drive pitch events

Melody is not just pitch; it is also **when notes happen**. The A-151 can shape note rhythm by switching which gate stream is active.

### Patch idea
Patch four rhythmic gate sources into `I/O 1–4`:
- straight 8ths
- syncopated rhythm
- sparse accents
- bursty pattern

Take `O/I` to:
- envelope trigger
- sequencer advance
- sample-and-hold clock
- quantizer trigger input

### Result
The pitch material may stay the same, but the **articulation and note timing** changes every time the A-151 steps.

This creates much more expressive melodies from simple CV material.

---

## 7. Stepping through different envelopes for melodic articulation

The manual itself gives a related example with switching between envelopes. This is very musical.

### Patch idea
Have one pitch sequence running, but send four different envelope shapes into `I/O 1–4`, and route `O/I` to filter CV or VCA CV destination.

For example:
- `I/O 1`: short pluck
- `I/O 2`: long swell
- `I/O 3`: medium decay
- `I/O 4`: snappy accent

Clock the A-151 with the same rhythm as the melody or a slower subdivision.

### Result
Each note or phrase has a different articulation, making the melody feel more “played.”

This is especially useful for:
- acid-style phrasing
- animated arpeggios
- evolving pads
- repeated motifs that need variation

---

## 8. Switching between different filter outputs for melodic timbre changes

The manual specifically mentions using the A-151 with a multimode filter such as the A-121.

### Patch idea
Send different filter outputs into the four switched jacks:
- lowpass
- bandpass
- highpass
- notch

Take `O/I` to the VCA or mixer.

Advance the switch with each note or each bar.

### Result
The melody keeps the same pitch, but its **spectral identity changes step by step**. This is musically powerful because timbre can imply phrasing just as strongly as pitch.

This works beautifully for:
- repeating basslines
- techno riffs
- generative melodies
- motif development

---

## 9. Building larger melodies from small cells

The A-151 excels at **form**. Think of each input as one “melodic cell.”

### Patch structure
- Cell A: 3-note motif
- Cell B: answer phrase
- Cell C: transposed fragment
- Cell D: rest / drone / held note

Clock the A-151 once every few beats or once per completed mini-pattern.

### Result
Instead of one long programmed melody, you get a melody built from interchangeable phrase fragments. This feels more modular and more alive.

This is one of the best ways to create:
- evolving Berlin-school sequences
- generative ambient lines
- modular “composition by recombination”

---

## 10. Using audio-rate switching for pitched timbral melodies

The manual notes that very fast triggering can produce **audio-frequency modulation**.

### Patch idea
Feed different waveforms from a VCO into `I/O 1–4`:
- sine
- triangle
- saw
- pulse

Take `O/I` to filter or VCA, and trigger the A-151 at audio or near-audio rates from:
- a fast LFO
- another VCO square wave

### Result
You get a composite waveform with a distinct timbre. If the switching rate or source relationships are tuned musically, this can create tones with melodic identity.

This is less about note sequencing and more about **melody-through-timbre**, but it is very effective in experimental patches.

---

# Strong patch combinations for melodic music

## A. Sequential phrase selector
**Modules to combine:**
- pitch sequencer
- precision adder or offset source
- quantizer
- A-151
- VCO
- envelope + VCA

**Idea:**
Use the A-151 to switch between four versions of a melody:
1. original
2. transposed up a fifth
3. octave up
4. sparse alternate line

This gives instant melodic arrangement.

---

## B. Four articulation melody engine
**Modules to combine:**
- one sequencer
- one VCO
- VCF
- four envelopes
- A-151
- clock / trigger source

**Idea:**
Pitch stays constant, but the A-151 rotates through four envelopes going to the filter.  
This creates a melody with changing accent, contour, and emotional feel.

---

## C. Generative melody selector
**Modules to combine:**
- random stepped CV
- sequencer
- keyboard CV
- fixed offset
- quantizer
- A-151
- clock divider
- reset source

**Idea:**
Put four types of pitch source into the A-151 and use reset to define formal boundaries.  
This gives structured unpredictability: random, but still phrased.

---

## D. Note-by-note timbre melody
**Modules to combine:**
- VCO
- multimode filter
- A-151
- gate source from keyboard or sequencer
- envelope + VCA

**Idea:**
Every new note advances the A-151 through different filter outputs.  
The melody becomes orchestrated step-by-step without changing the pitch line.

---

# Musical strategies

## Use the A-151 at different clock divisions
Try advancing it:
- every note
- every 2 notes
- every bar
- every 4 bars

This changes whether it behaves like:
- a step sequencer
- a phrase selector
- an arrangement tool

## Pair it with a quantizer
The A-151 itself does not constrain pitch. If you are switching voltages intended as melody, a quantizer will keep results harmonically useful.

## Use reset for structure
Reset is what turns “cycling” into “composition.”  
A reset every 4 or 8 bars keeps melodic changes aligned with your piece.

## Switch both pitch and timbre in parallel
For richer melody, use one A-151 for pitch-source switching and another for envelope or filter-output switching. Even if you only have one A-151, you can still create this feel by switching one domain at a slower rate than another part of the patch.

## Exploit 3-step mode
Three-step phrase cycling over 4/4 rhythms creates beautiful asymmetry.  
A 3-phrase melodic cycle against a 4-beat bar can feel much less repetitive.

---

# Best roles for the A-151 in melodic patching

The A-151 is especially good as a:

- **phrase selector**
- **melodic variation router**
- **transposition cycler**
- **articulation switcher**
- **timbral melody animator**
- **structural resettable form generator**

It is less a melody generator on its own and more a **melody organizer**. In a modular system, that is often even more valuable.

---

# Example melodic patch recipes

## Patch 1: Four melodic phrases
- Four CV phrase outputs into `I/O 1–4`
- `O/I` to quantizer, then VCO 1V/oct
- Trigger A-151 once per bar
- Reset every 4 bars

**Result:** a looping 4-part melodic form.

## Patch 2: Same melody, four transpositions
- One sequence multed four ways
- Add different offsets to each copy
- Send to `I/O 1–4`
- `O/I` to quantizer and oscillator

**Result:** chord-implying monophonic melody.

## Patch 3: One pitch line, rotating articulations
- Sequence to VCO
- Four envelopes into `I/O 1–4`
- `O/I` to filter CV input
- Trigger switch every note

**Result:** expressive melodic variation.

## Patch 4: One note source, four destinations
- Pitch CV into `O/I`
- `I/O 1–4` to VCO1, VCO2, filter, FM amount
- Advance at phrase intervals

**Result:** the melody moves around your patch and creates evolving roles.

---

# Conclusion

The **Doepfer A-151** is a deceptively simple module that becomes highly musical when used for **melodic routing and phrase structure**. Its real strength is not just switching signals, but switching **musical roles**:

- which pitch source is active
- which transposition is heard
- which articulation shapes the note
- which timbre carries the melody
- when a phrase restarts

If you build your patch so that each of the four positions represents a different but related musical idea, the A-151 becomes a compact **melody form generator** for Eurorack.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)