# Intellijel — Unity

- [Manual PDF](../../manuals/unity-mixer_manual_2020.04.15.pdf)

---

[Unity Mixer Manual (PDF)](attachment)

# Intellijel Unity Mixer — melodic use in a Eurorack system

The **Intellijel Unity Mixer** is a very simple but very useful utility for building melodic patches. It is a **dual 3:1 unity-gain mixer**, or a **single 6:1 mixer** if the top output is left unpatched.

Because it works with **CV or audio**, it can help with melody creation in two main ways:

1. **Combining pitch-related CV sources**
2. **Combining audio signals that form layered melodic voices**

---

## What the module does

### Basic structure
- **Top section:** inputs **1, 2, 3** summed to output **4**
- **Bottom section:** inputs **5, 6, 7** summed to output **8**
- If **output 4 is unpatched**, the top mix is internally sent to the bottom mixer, turning it into a **6:1 mixer** with final output at **8**

### Important behavior
- It is **unity gain**: signals are **summed but not attenuated or amplified**
- Outputs are **phase correct** (non-inverting)
- Works for **audio or CV**
- **Maximum output voltage: 10.5 V**
  - Above that, it can **clip**
- Rear jumpers can set either mixer to **-6 dB attenuation** for more headroom

---

# How it helps create melodic components

## 1. Build pitch CV from multiple sources

This is one of the most musically useful roles for a unity mixer.

In Eurorack, melodic pitch often comes from several CV layers added together:
- a **main pitch sequence**
- a **keyboard or transpose offset**
- **octave offsets**
- a **vibrato or slow pitch modulation**
- a **slewed variation**
- a **quantized random source**

The Unity Mixer lets you **add these together into one pitch stream**.

### Example patch: transposable melody
Patch:
- **IN 1:** sequencer pitch CV
- **IN 2:** keyboard/manual voltage offset or precision adder-style transpose source
- **IN 3:** slow LFO through attenuation for subtle vibrato
- **OUT 4:** to oscillator 1V/oct input

Result:
- Your melody plays from the sequencer
- The second CV transposes it
- The third adds expressive movement

### Musical note
Because this is a **plain summing mixer**, it does not quantize or scale pitch. So for precise melodic work:
- use already-scaled pitch CV
- attenuate modulation before mixing if needed
- ideally place a **quantizer after the mixer** if the sources aren’t pitch-accurate

---

## 2. Create interval stacks and harmonized lines

You can use the module to sum several fixed voltages or tuned offsets into a melodic line.

### Example patch: harmony shaping
Patch:
- **IN 1:** main pitch sequence
- **IN 2:** offset voltage representing a fixed interval
- **IN 3:** manual offset for octave switching
- **OUT 4:** to a quantizer, then oscillator

Result:
- The mixed voltage can generate melodic lines with harmonic movement
- Sending the sum into a quantizer helps “lock” the combined voltages to a scale

This works especially well for:
- transposed basslines
- modal melody shifts
- octave jumps
- adding phrase variation

---

## 3. Mix modulation sources that shape melodic phrasing

Melody is not only pitch. It also includes **expression**, **phrasing**, and **motion**.

The Unity Mixer can combine CV sources controlling:
- filter cutoff
- wavefolder amount
- FM depth
- VCA amplitude
- LPG response

### Example patch: expressive melody contour
Patch:
- **IN 5:** envelope
- **IN 6:** slow LFO
- **IN 7:** stepped random CV
- **OUT 8:** to filter cutoff of your melodic voice

Result:
- The envelope gives note articulation
- The LFO adds movement across the phrase
- The random CV creates evolving timbre per note

This makes a simple melody feel much more alive.

---

## 4. Layer oscillators into a richer melodic voice

Since the Unity Mixer also handles audio, it is useful for building a **multi-oscillator melodic sound source**.

### Example patch: layered lead
Patch:
- **IN 1:** VCO saw wave
- **IN 2:** VCO pulse wave
- **IN 3:** sub-oscillator or sine one octave below
- **OUT 4:** to filter or VCA

Result:
- A thicker, harmonically rich lead or bass tone
- Great for mono melodic lines

### Example patch: two-voice blend
Use top and bottom sections separately:
- Top mixer for one melodic voice’s oscillator blend
- Bottom mixer for another melodic layer or a parallel modulation sum

---

## 5. Use 6:1 mode for complex melodic control

If **output 4** is left empty, the top three inputs feed the bottom mixer, giving you a **6-input sum** at **output 8**.

This is very useful when you want many small melodic influences combined into one destination.

### Example patch: complex pitch ecosystem
- **IN 1:** main sequencer pitch
- **IN 2:** transpose CV
- **IN 3:** octave offset
- **IN 5:** subtle vibrato
- **IN 6:** random stepped CV
- **IN 7:** manual performance offset
- **OUT 8:** to quantizer or oscillator pitch input

Result:
- One highly composite melodic CV stream
- Excellent for generative or semi-generative melody systems

---

# Best melodic patch strategies

## Strategy 1: Put a quantizer after the Unity Mixer
This is probably the strongest melodic use.

Why:
- multiple CV sources summed together often drift off exact semitone values
- a quantizer after the mix turns those combined voltages into scale-aware notes

### Patch flow
`Sequencer + transpose + random + vibrato -> Unity Mixer -> Quantizer -> VCO 1V/oct`

This gives:
- controlled pitch additions
- musically stable results
- evolving but tonal melodies

---

## Strategy 2: Use it before a precision-sensitive destination only with care
Because the Unity Mixer is not specifically described as a **precision adder**, I would not rely on it as a perfect replacement for one in highly exact pitch applications over wide ranges.

It is still very useful musically for:
- short-range melodic transposition
- adding expressive CV
- summing already modest pitch offsets

Best practice:
- keep pitch modulation subtle unless quantized afterward
- test tuning if using it directly into 1V/oct

---

## Strategy 3: Use the attenuation jumpers for hot audio sources
If you are mixing several oscillators for a melodic voice, the summed level can exceed the module’s **10.5 V max output** and clip.

The manual notes:
- each half has its own **-6 dB attenuation jumper**
- useful for **high amplitude sources such as raw VCO outputs**

That means if you are building:
- supersaw-style leads
- stacked bass oscillators
- thick drones with melodic articulation

then enabling attenuation can preserve headroom and keep the tone cleaner.

---

# Patching ideas for melodic music

## 1. Transposing sequence mixer
Use the top mixer for pitch:
- sequencer
- offset row from another sequencer
- keyboard transpose

Send to:
- quantizer
- oscillator

Good for:
- basslines
- arpeggios
- lead motifs

---

## 2. Melody + ornament CV mixer
Use the top mixer to combine:
- main pitch
- short envelope into pitch for attack “pluck”
- tiny random CV

Send to oscillator pitch.

Good for:
- acid-style lines
- animated plucks
- pseudo-acoustic articulation

---

## 3. Audio voice stacker
Use the top mixer for:
- oscillator A
- oscillator B detuned
- sub oscillator

Then send to:
- filter
- VCA

Use bottom mixer for:
- second voice
- noise + tone blend
- parallel melody layer

Good for:
- lead voices
- basses
- unison melodic sounds

---

## 4. CV phrase shaper
Use the bottom mixer for:
- envelope
- LFO
- manual offset

Send to:
- wavefolder
- filter FM
- VCA CV input

Good for:
- adding expression to repeating melodies

---

## 5. Generative melodic bus in 6:1 mode
Combine:
- sequence
- random source
- clocked offset
- slow drift
- manual transpose
- octave offset

Then quantize the result.

Good for:
- ambient
- Berlin-school style evolving lines
- generative techno melodies

---

# Pairing with Intellijel Triatt or Quadratt

The manual specifically mentions that Unity Mixer pairs well with **Triatt** and **Quadratt**.

This is especially important for melodic patching because those modules provide the control that Unity Mixer lacks:
- attenuation
- offset
- manual level control

### Strong combo
- Use **Triatt/Quadratt** to scale pitch modulation or audio levels
- Send their outputs into **Unity Mixer**
- Use Unity Mixer to create the final combined melodic CV or audio voice

### Example
As the manual suggests:
- patch 3 Quadratt outputs into Unity Mixer’s top inputs
- patch Unity Mixer output back into the 4th Quadratt channel

This gives:
- a **3:1 mix**
- plus a **master level control**

For melodic work, that means:
- 3 oscillators into Unity Mixer
- summed output back to Quadratt
- Quadratt channel 4 becomes your lead voice volume/tone control path

Very practical for performance.

---

# Practical limitations to keep in mind

## No knobs, no mute switches, no level controls
This is not a performance mixer. It is a **set-and-forget utility mixer**.

So for melodic patching, it works best when:
- sources are already at the right level
- you want compact routing
- you don’t need live balancing on the module itself

## Output clipping at 10.5 V
Important for:
- stacked audio oscillators
- summed positive CV

If your melodic patch behaves oddly or sounds harsh, clipping may be the reason.

## Not a dedicated precision adder
For exact pitch summing across many octaves, a dedicated precision adder is usually safer. But for many musical uses—especially with quantizers or moderate offsets—this module is still very handy.

---

# Best overall melodic roles for the Unity Mixer

The most useful melodic applications are:

- **Combining pitch CV sources**
- **Creating transposition buses**
- **Mixing multiple modulation sources for phrasing**
- **Layering oscillators into richer melodic voices**
- **Building complex generative melody control signals**
- **Submixing audio or CV in very little rack space**

In a melodic Eurorack system, this is less of a “feature module” and more of a **glue module**. It helps separate melodic ideas become one playable signal.

---

# Technical summary
- **Width:** 2 hp
- **Depth:** 39 mm
- **Current draw:** 11 mA @ +12V, 14 mA @ -12V
- **Modes:** dual 3:1 or single 6:1
- **Signal type:** audio or CV
- **Max output:** 10.5 V
- **Optional attenuation:** -6 dB per section via rear jumpers

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)