# Erogenous Tones — VC8

- [Manual PDF](../../manuals/vc8-instructions.pdf)

---

[VC8 Manual / Product Page](https://erogenous-tones.com/erogenous-tones-vc8.html)

# Using the Erogenous Tones VC8 for melodic patching

From the attached pages, the module documented is:

- **Erogenous Tones VC8**
- **8-channel linear VCA**
- **DC-coupled**
- Per-channel:
  - **CV Level attenuator**
  - **CV Offset control**
  - LED showing effective CV amount
- Two optional **sub-mix buses**:
  - **Channels 1–3 summed into channel 4**, with channel 4 acting as the VCA for that mix
  - **Channels 5–7 summed into channel 8**, with channel 8 acting as the VCA for that mix
- Based on **LM13700 OTA**
- **18 HP**, skiff friendly
- Power: **+12/-12 V**, current **80 mA / 70 mA**

## What this module does musically

VCAs are one of the core building blocks for making melodic music in Eurorack. Even though the VC8 does not generate pitch or sound by itself, it is extremely useful for shaping and organizing the things that *do* create melody:

- note loudness
- modulation depth
- accent patterns
- voice balancing
- layered timbres
- submixing several melodic voices into playable groups
- controlling CV as well as audio, because it is **DC-coupled**

That last point matters a lot: since the VC8 is DC-coupled, it can process both:

- **audio signals** like oscillator outputs
- **control voltages** like envelopes, LFOs, sequencer rows, random voltages, and pitch-related modulation

This makes it very strong as a “melody support” module.

---

## Best melodic uses for VC8

## 1. Classic amplitude shaping for melodic voices

The most obvious use is one VCA per voice.

### Patch idea
For a 4-voice melodic patch:

- Oscillator 1 → VC8 channel 1 input
- Oscillator 2 → VC8 channel 2 input
- Oscillator 3 → VC8 channel 3 input
- Oscillator 4 → VC8 channel 4 input
- Envelope generators → each channel’s CV input
- VC8 outputs → mixer / filter / output

### Result
Each note gets proper articulation from its envelope. This is the standard use of VCAs, but with **8 channels**, you can support:

- several mono voices
- layered paraphonic patches
- oscillator + sub + noise + FM lane all independently controlled

For melody writing, this means your lines can have:
- accents
- legato vs plucky articulation
- dynamic phrasing
- voice layering

---

## 2. Control melodic modulation depth with CV VCAs

Because VC8 is DC-coupled, you can use channels to scale modulation before it reaches pitch or timbre destinations.

### Patch idea: vibrato under voltage control
- LFO → VC8 ch. 1 input
- Envelope or performance CV → ch. 1 CV input
- ch. 1 output → oscillator 1V/oct FM input or dedicated vibrato input

### Result
Vibrato appears only on selected notes or grows over time.

This is great for:
- expressive lead lines
- delayed vibrato on sustained notes
- more human-sounding melodic phrasing

You can do the same for:
- filter modulation
- wavefold amount
- FM index
- pulse width
- wavetable position

So VC8 can turn a static melodic line into a highly animated one.

---

## 3. Build accents into sequences

A sequencer may provide gates for every note, but not all notes need the same intensity.

### Patch idea
- Main envelope → VC8 ch. 2 input
- Accent CV row / gate pattern → ch. 2 CV input
- ch. 2 output → another VCA or filter cutoff CV

### Result
Only accented steps receive stronger envelope modulation.

This can create:
- stronger notes in a bassline
- more pronounced melody peaks
- pseudo-velocity in systems without dedicated velocity output

Since each channel has a **CV offset**, you can dial in a baseline amount and then use CV to add accents on top.

---

## 4. Use offset to create drones or semi-open voices

The **CV Offset** is very useful musically.

If no CV is patched, offset can open the VCA manually. That means you can:

- keep a voice partially open
- create a drone under a melody
- set a constant modulation amount
- blend in a layer without requiring another CV source

### Patch idea
- Oscillator drone → VC8 ch. 5 input
- No CV patched, or very slow CV patched
- Use CV Offset to set constant level
- Output mixed with your main melody voice

### Result
You get a sustained harmonic bed under a melodic line.

This is especially good for:
- ambient melodies
- modal patches
- techno bass + drone combinations
- generative melodic textures

---

## 5. Create layered melodic timbres

One melodic line can be made from several sound sources:
- a main oscillator
- a sub oscillator
- noise/transient
- FM sideband source

With VC8, each layer can have independent level shaping.

### Patch idea
For one melody voice:
- Saw oscillator → ch. 1
- Square sub → ch. 2
- Noise click/transient → ch. 3
- Use separate envelopes or shared envelopes with different CV Level settings
- Sum with the channel 4 submix option

### Result
Channel 4 can act as a grouped output for the first three channels, giving you a composite melodic voice.

This is one of the most powerful features in the manual.

---

## 6. Use the 1–3→4 and 5–7→8 submixes as two playable voice groups

The submix architecture makes VC8 more than “just 8 VCAs.”

According to the manual:

- **Channel 4 submix** can receive **channels 1–3** and is controlled by **VCA 4**
- **Channel 8 submix** can receive **channels 5–7** and is controlled by **VCA 8**
- Channels 1,2,3,5,6,7 still provide their regular individual outputs

### Musical meaning
You can create two multi-layered melodic instruments:

- **Voice A** = channels 1–3 mixed and shaped by channel 4
- **Voice B** = channels 5–7 mixed and shaped by channel 8

### Patch idea: two-voice melodic system
**Voice A**
- ch. 1 = oscillator A
- ch. 2 = sub oscillator
- ch. 3 = noise or second oscillator
- ch. 4 = summed voice output with overall envelope

**Voice B**
- ch. 5 = oscillator B
- ch. 6 = FM layer or detuned osc
- ch. 7 = extra harmonic source
- ch. 8 = summed voice output with overall envelope

### Result
You can build:
- lead + bass
- melody + counter-melody
- two paraphonic stacks
- call-and-response textures

This is especially useful if your case is small and you want efficient voice architecture.

---

## 7. Use VCAs for melodic CV mixing

Since the outputs can be grouped, you can use the VC8 for control-voltage combinations too.

### Patch idea: animated pitch modulation bus
- Slow LFO → ch. 1
- Random stepped CV → ch. 2
- Envelope → ch. 3
- Submix to ch. 4
- ch. 4 output → oscillator pitch modulation input (attenuated carefully)

### Result
You get a compound melodic modulation signal whose components can each be independently scaled.

This can create:
- drifting pitch ornamentation
- occasional note bends
- evolving melodic instability
- generative melodic movement

Be careful with pitch destinations, since even small voltages can produce large pitch shifts.

---

## 8. Dynamic transposition and phrase variation

A very practical melodic use of DC-coupled VCAs is controlled transposition or phrase variation.

### Patch idea
- Sequencer secondary CV row → VC8 input
- Gate pattern or envelope → VC8 CV input
- VC8 output mixed with main pitch CV elsewhere in your system

### Result
Only certain notes or sections get transposed.

This enables:
- octave jumps on selected notes
- phrase-end lifts
- alternating motif variations
- conditional harmony changes

The VC8 is not itself a precision adder, so this works best for expressive pitch modulation or coarse musical movement unless the rest of the system is carefully calibrated.

---

## 9. Rhythmic melody masking

Melodies often become more interesting when only some layers appear on certain beats.

### Patch idea
- Main melodic oscillator → one channel
- Harmony oscillator → second channel
- Counterline oscillator → third channel
- Different gate/envelope patterns control each VCA
- Submix to a grouped output

### Result
A single sequenced pitch source can sound like a much more complex arrangement because the audible layers appear and disappear rhythmically.

This is excellent for:
- Berlin-school patterns
- arpeggiated techno lines
- minimal melodic variation
- pseudo-polyphonic textures

---

## 10. Performance mixing for melodic sets

The CV Offset knobs and many channels make this useful in performance.

You can treat it like a compact voltage-controlled voice mixer:
- bring in a harmony layer
- suppress a sub oscillator
- open a drone
- alter modulation depth live
- fade between lead textures

The **knob-per-channel layout** suggests quick hands-on use, and the LEDs help you see activity.

For melodic performance, that means easier control of:
- balance
- articulation
- density
- phrase energy

---

# Practical melodic patch recipes

## Patch 1: Lead voice with expressive vibrato
- VCO audio → VC8 ch. 1
- ADSR → ch. 1 CV
- ch. 1 out → filter / output
- LFO → VC8 ch. 2 input
- delayed envelope → ch. 2 CV
- ch. 2 out → VCO FM input

**Why it works:** one channel shapes loudness, another makes vibrato bloom only on held notes.

---

## Patch 2: Bass voice with accent
- Bass oscillator → ch. 1
- Main envelope → ch. 1 CV
- ch. 1 out → filter
- Accent envelope or trigger-derived CV → ch. 2 input
- Accent gate pattern → ch. 2 CV
- ch. 2 out → filter cutoff CV input

**Why it works:** accented notes hit harder without changing the core sequence.

---

## Patch 3: Dual melodic voices using submixes
### Voice A
- Osc A → ch. 1
- Sub A → ch. 2
- Noise/transient A → ch. 3
- Shared envelope → ch. 4 CV
- ch. 4 output = full voice A

### Voice B
- Osc B → ch. 5
- Detuned osc B → ch. 6
- FM texture B → ch. 7
- Shared envelope → ch. 8 CV
- ch. 8 output = full voice B

**Why it works:** you get two compact, layered instruments from one module.

---

## Patch 4: Generative melodic movement
- Random stepped CV → ch. 1
- Slow triangle LFO → ch. 2
- Envelope from note gates → ch. 3
- Use submix to ch. 4
- ch. 4 out → small pitch modulation amount on oscillator

**Why it works:** the melody gains subtle changing contour and ornaments.

---

# Strengths of VC8 for melodic systems

## Excellent for:
- multi-voice amplitude control
- layered melodic voices
- voltage-controlled modulation depth
- drone + melody hybrids
- accent programming
- compact voice submixing
- performance-oriented balancing

## Especially valuable because:
- **8 channels** is a lot in 18 HP
- **DC coupling** lets it work with both CV and audio
- **offset controls** make it useful even without patched CV
- **submix pairs** help build complete melodic voice structures

---

# Limitations to keep in mind

Based on the manual excerpt, VC8 is a **linear VCA**. That usually means:

- very good for CV control
- clean utility behavior
- possibly less naturally “loudness-shaped” than an exponential VCA for audio amplitude

That is not a problem at all, just something to know. Linear VCAs are often preferable for modulation duties and still very useful for audio, especially in layered or precise patches.

Also, the module does **not** itself provide:
- envelopes
- oscillators
- pitch sequencing
- quantization
- filtering

So for actual melodic generation, it pairs best with:
- a sequencer or quantizer
- one or more oscillators
- envelopes
- filters
- mixers or output modules

---

# Bottom line

The **VC8** is best thought of as a **melodic infrastructure module** rather than a melody source. It helps turn simple note sequences into finished musical parts by giving you:

- articulation
- accents
- modulation control
- timbral layering
- grouped voice mixing
- performance dynamics

If you use it with oscillators, envelopes, sequencers, and filters, it can support everything from:

- tight basslines
- expressive leads
- layered pads
- generative melodies
- two-part counterpoint
- live-performed melodic texture changes

In a melodic Eurorack system, a module like this often ends up doing more real musical work than flashier modules, because it controls **how notes speak**.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)