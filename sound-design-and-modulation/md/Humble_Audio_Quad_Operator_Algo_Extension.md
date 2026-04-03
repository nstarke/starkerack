# Humble Audio — Quad Operator Algo Extension

- [Manual PDF](../../manuals/Quad Operator Manual.pdf)

---

# [Quad Operator Manual PDF](https://www.dropbox.com/paper/doc/print/JsIQoU7GbeAboEJku9ZgE?print=true)

## Humble Audio Quad Operator: modulation ideas for aggressive percussion, basslines, and pads

The **Quad Operator** is a very modulation-friendly digital FM oscillator bank. The big takeaway from the manual is:

- it has **4 operators**
- each operator can be **locked** to harmonic integer ratios or set **free** as an independent oscillator
- each operator has:
  - **ratio**
  - **detune**
  - **shape** (sine → triangle → square → saw)
  - **gain CV**
  - **mod sends to all 4 operators**, including itself
- there is also an **external AR FM input** with its own gain and modulation sends
- operator outputs are available individually
- there is a **reset input** for phase reset
- in **LFO mode**, the whole thing can become a complex, phase-locked modulation source

This means the module is best thought of as a **4-voice FM network with VCAs on each modulator**, plus an extra external modulator path. That makes it excellent for animated timbre design.

---

# First: how to think about modulation on Quad Operator

## 1. Gain CV is more important than it first appears
Per the manual, **Gain CV affects both output level and how intensely that operator modulates other operators via its sends**.

That is huge.

So if Operator 2 is modulating Operator 1, then modulating **Gain 2 CV** does two things at once:

- changes how much of Op 2 you hear at its output
- changes how hard Op 2 is FM-ing its destinations

In practice, that gives you **dynamic FM index control**, which is one of the key ingredients for:

- punchy percussion
- talking/reese bass motion
- evolving pads

If you patch envelopes, gates, stepped CV, random, or LFOs into Gain CVs, the FM network becomes alive.

## 2. Lock vs Free is the core harmonic/inharmonic switch
Use:

- **Lock mode** for stable, musical, harmonic FM
- **Free mode** for dissonance, beating, drifting, metallic chaos

A great trick is mixing both:
- keep the audible carrier in **lock**
- put one modulator in **free**
- use small amounts of free operator modulation for unstable, dirty sidebands

That often gives the sweet spot between tone and destruction.

## 3. Shape modulation is a hidden aggression control
Because the operators morph from **sine to triangle to square to saw**, modulating shape changes overtone density before FM even happens.

General rule:
- **sine** = cleaner, classic FM, glassy, more stable pitch
- **triangle** = slightly richer
- **square/saw** = more harmonics, more grit, more alias-like edge, more chaotic modulation results

If you want:
- **hard percussion**: shape modulation on modulators
- **bass brutality**: animate carrier or main modulator shape between triangle/square/saw
- **pads**: very slow shape motion, usually staying on sine/triangle side

## 4. The AR FM input is your wildcard
The AR FM input can take an external audio-rate signal and has:
- input gain
- clipping LED
- gain CV
- its own sends to all operators

This is where things can get especially unique. Feed it:
- a noise source
- a filtered oscillator
- a phase-locked copy of one Quad Operator output
- a wavefolder output
- a drum loop/transient source
- another digital oscillator

Then use the AR FM sends as a parallel external modulator layer.

The manual explicitly suggests feedback-style patching with locked operators. That means this input is ideal for:
- screaming bass feedback
- broken percussion transients
- unstable evolving drones

## 5. Reset is great for percussion and rhythmic modulation
The **Reset CV** resets all operator phases. The manual notes it is especially useful when using the module as a modulation source, but it's also very useful for sound generation.

For percussive sounds:
- send a trigger or gate to reset on each hit
- this makes transients more repeatable and punchy

For bass:
- reset on note onset for a more consistent attack

For pads:
- usually avoid hard reset every note unless you want synthetic “same-start” character

---

# Best modulation sources to pair with Quad Operator

The most effective external modulators for this module are:

- **snappy envelopes** into Gain CV
- **slow LFOs** into Shape CV
- **stepped random** into Ratio CV or modulator Gain CV
- **audio-rate oscillators** into AR FM
- **sequencer CV** into 1V/Oct and sometimes ratio CV in free mode
- **burst generators / trigger envelopes** into Reset and Gain CV for percussive attacks
- **matrix mixer or CV mixer** to combine envelope + LFO into a single Gain or Shape input

If you only use one trick, use this:
> Patch envelopes into the Gain CVs of the operators that are doing the modulation.

That gives the most musically useful results fastest.

---

# Patch strategy by sound type

# 1. Distorted percussive sounds

The Quad Operator is very good at synthetic percussion because FM excels at:
- pitch snap
- metallic overtones
- transient-rich attacks
- unstable inharmonic body tones

## A. Digital kick / tom with ripping attack

### Setup
- Set **VCO mode**
- Use **Operator 1** as your main audible output
- Set Op 1 to **lock**
- Start with:
  - Shape 1 near **sine**
  - Ratio 1 = **1**
- Set **Operator 2** to modulate Op 1
  - Ratio 2 = **2** or **3**
  - Shape 2 = sine or triangle to start
  - Mod 1 on row 2 up moderately
- Patch a **fast-decay envelope** to **Gain 2 CV**
- Patch a separate **pitch envelope** to **LF FM** for the whole module

### Result
- LF FM envelope gives the down-sweep pitch thunk
- Gain 2 envelope gives the sharp FM transient click/thwack

### To distort it harder
- move Shape 2 toward square or saw
- add a little **self-modulation** on Op 2
- push **Detune 2** slightly
- send a trigger to **Reset** for consistent punch

### Variation
For toms:
- reduce LF FM envelope depth
- lower master tuning
- use Ratio 2 = 1 or 2
- slightly detune Op 2

---

## B. Metallic snare / industrial hit

### Setup
- Op 1 = audible body
- Op 2 and Op 3 = modulators
- Set Op 1 in **lock**
- Set Op 2 in **free**
- Set Op 3 in **free**
- Op 1 shape around triangle
- Op 2 and 3 shapes toward square/saw
- Send Op 2 and Op 3 strongly to Op 1
- Patch different short envelopes to **Gain 2 CV** and **Gain 3 CV**

### Why it works
Locked carrier + free modulators = controllable metallic noise

### To get snare-like noise
- patch **noise or another oscillator** into **AR FM**
- set AR FM gain fairly hot
- send AR FM to Op 1 moderately
- modulate **Gain AR FM CV** with a very short decay envelope

That gives a burst of broadband attack layered on top of metallic FM body.

### Tips
- Use **Reset** per trigger
- Add a tiny amount of Op 1 self-mod for extra crack
- If too chaotic, move free modulators back to lock and detune slightly instead

---

## C. Broken glitch percussion

### Setup
- Use one operator as audio out, others as modulators
- Put at least one modulator in **free**
- Sequence or randomly modulate:
  - its **ratio CV**
  - its **shape CV**
  - its **gain CV**
- Clock a trigger into **Reset**
- Optionally send stepped random into **LF FM**

### Result
Each hit resets in time but the overtone content mutates, making glitchy but rhythmic percussion.

### Best modulation choices
- random stepped CV into shape
- envelope into gain
- small random voltage into detune/ratio of a free operator

---

# 2. Crazy basslines for dubstep / drum and bass

This module is excellent for bass because FM plus waveshape morphing plus gain-controlled modulation can create:

- talking basses
- neuro movement
- reese-like beating
- tearing digital growl
- sub + mid separation

A useful mindset is:
- one operator for **sub/fundamental**
- one or two operators for **moving midrange distortion**
- one operator or AR FM for **instability/texture**

---

## A. Talking FM growl bass

### Setup
- Op 1 = main audible carrier
- Op 2 = primary modulator
- Op 3 = secondary animated modulator
- All in **lock** initially
- Ratio suggestions:
  - Op 1 = 1
  - Op 2 = 2 or 3
  - Op 3 = 5 or 7
- Shapes:
  - Op 1 = triangle
  - Op 2 = sine/triangle
  - Op 3 = square/saw
- Mod sends:
  - Op 2 → Op 1 moderate/high
  - Op 3 → Op 1 low/moderate
  - optional Op 3 → Op 2 a little

### Modulation
- envelope or LFO to **Gain 2 CV**
- a different LFO to **Gain 3 CV**
- slow or tempo-synced LFO to **Shape 1 CV** or **Shape 2 CV**
- sequencer to **1V/Oct**
- gate/trigger to **Reset** on note onset

### Why it talks
Because the FM index is changing over time, and the waveshape is also moving, the spectrum forms vowel-like shifts.

### Push it further
- put Op 3 into **free**
- slightly detune it
- keep its modulation amount lower than Op 2
- now the bass gets unstable, snarling movement

---

## B. Reese / tearing DnB bass

The classic reese usually relies on detuned oscillators. On Quad Operator, do a hybrid FM version.

### Setup
- Use **Op 1 output** and **Op 2 output** as two audible voices
- Put both in **free**
- Tune them to nearly the same pitch
- Slightly detune one with its detune knob
- Set both shapes around saw/square-ish
- Use Op 3 as modulator for both
- Op 3 can be in lock or free
- Send Op 3 to both Op 1 and Op 2

### Modulation
- slow LFO to **Gain 3 CV**
- slow, different LFO to **Shape 3 CV**
- small random or envelope to **Detune/Ratio 3**
- optional envelope to **LF FM** for attack movement

### Why it works
The beating between Op 1 and Op 2 makes the reese body, while Op 3 adds evolving FM tearing.

### Advanced move
Send one audible operator to the left channel and the other to the right if you record or process in stereo externally.

---

## C. Feedback-style savage bass using AR FM

This is one of the most unique things in the manual.

### Setup
- Keep Op 1 in **lock**, ratio 1 = 1
- Patch **Op 2 output** or **Op 1 output** into **AR FM**
- Start with AR FM gain low
- Send **AR FM** to Op 1 and/or Op 2
- Use **Gain AR FM CV** with an envelope or LFO

### Result
You get controllable pseudo-feedback FM behavior.

### For dubstep brutality
- shape carrier toward triangle/square
- modulate AR FM gain rhythmically
- reset on note triggers
- slightly clip the AR FM input for dirty edge

The manual notes the clipping LED indicates distortion of the input signal. Normally you'd reduce clipping, but creatively, clipping here can be useful for nastier timbres.

### Safe approach
Increase AR FM gain slowly. This patch can get extreme fast.

---

## D. Wob bass without a filter

You don't actually need a filter to make “wub” motion here.

### Setup
- build a bass patch where Op 2 heavily modulates Op 1
- send an LFO or synced envelope into **Gain 2 CV**
- send another slower LFO into **Shape 1 CV**
- optional small modulation into **Gain 3 CV** for extra formant motion

### Why this works
Instead of opening a filter, you're opening **FM intensity**, which changes spectral brightness in a very bass-music-friendly way.

### Great modulation rates
- 1/4 note wobble on Gain 2
- slower 2- or 4-bar modulation on shape
- occasional random bursts on AR FM gain for fills

---

# 3. Haunting atmospheric pads

The module can absolutely do pads, but the trick is to **avoid overdriving the modulation matrix too quickly**.

FM pads work best when:
- ratios are mostly harmonic
- detune is subtle
- shapes live in sine/triangle territory
- motion is slow and layered

---

## A. Classic eerie FM pad

### Setup
- VCO mode
- all operators in **lock**
- Ratios:
  - Op 1 = 1
  - Op 2 = 2
  - Op 3 = 3 or 4
  - Op 4 = 5
- Shapes:
  - mostly sine/triangle
- Use Op 1 as main output
- Send:
  - Op 2 → Op 1 lightly
  - Op 3 → Op 1 lightly
  - Op 4 → Op 2 lightly

### Modulation
- very slow LFO to **Gain 2 CV**
- different slow LFO to **Gain 3 CV**
- very slow LFO/random slew to **Shape 1 CV**
- subtle slow modulation to **Shape 3 CV**
- optional slow modulation to **LF FM** for ensemble-like drift

### Result
Gentle movement in FM index creates spectral breathing without obvious rhythmic pulsing.

---

## B. Haunted inharmonic drone pad

### Setup
- Op 1 and Op 2 in **lock**
- Op 3 in **free**
- Op 4 in **free**
- Op 1 = audible base
- Op 2 = harmonic support
- Op 3/4 = low-level spectral contamination

### Modulation
- very slow random or wandering CV into **Ratio 3** and/or **Ratio 4**
- slow LFO into **Gain 3 CV** and **Gain 4 CV**
- subtle shape movement on Op 3/4 toward square/saw
- tiny detune offsets on free ops

### Why it works
The locked operators keep a tonal center while the free operators add ghostly, shifting sidebands.

This is one of the best ways to get “haunting” instead of simply “pretty.”

---

## C. Pad with external texture through AR FM

### Setup
- patch external audio into **AR FM**:
  - filtered noise
  - a field recording loop from another module
  - another oscillator
  - a reverb return if your system allows feedback experimentation
- keep AR FM gain moderate
- send AR FM lightly to one or two operators
- modulate **Gain AR FM CV** slowly

### Result
The pad gets an unstable, air-filled layer that doesn't sound like standard subtractive synthesis.

### Especially effective
Use a slow random CV on Gain AR FM and a separate slow LFO on Shape 1 or 2.

---

# Specific modulation ideas that exploit the module well

## Modulate the modulators, not just the carriers
Because FM is exponential in perceived complexity, tiny motion on a modulator has a huge effect.

Best targets:
- Gain CV of modulator operators
- Shape CV of modulator operators
- Ratio CV of free-state modulators

This is often more effective than modulating the audible operator directly.

---

## Use self-modulation sparingly
The manual states each operator can modulate itself.

Self-mod gives:
- edge
- buzz
- instability
- more complex digital grit

Use cases:
- percussion transient crack
- bass rasp
- drone corrosion

But:
- too much self-mod easily becomes noise

Start tiny.

---

## Use different envelopes on different operators
Instead of one global modulation source, try:
- Op 2 gain envelope = fast decay
- Op 3 gain envelope = medium decay
- AR FM gain envelope = ultra-short click

This creates layered timbral evolution like acoustic attack/body/resonance, but synthetic and brutal.

---

## Animate the shape of only one operator at a time
If everything is moving at once, the sound can smear.

Try:
- static carrier shape
- moving modulator shape

or:
- moving carrier shape
- static FM index

This makes the patch more intelligible and easier to tune musically.

---

## Use free-state operators as “controlled chaos injectors”
A free operator with:
- low gain
- non-integer pitch
- slowly moving shape
- modest send level

can add beautiful dirt without overwhelming the tone.

This is especially useful for:
- neuro bass
- eerie pads
- industrial percussion

---

## Use reset for transient discipline
Even on chaotic patches, **Reset** can keep them playable.

Use it:
- on every drum trigger
- on every bass note
- every few beats for rhythmic consistency in drones

Without reset, some FM attacks may vary depending on phase relationships. Sometimes that's good; sometimes it weakens the impact.

---

# Concrete patch recipes

## Patch 1: Distorted FM kick
- VCO mode
- Op 1 lock ratio 1, shape sine
- Op 2 lock ratio 2, shape triangle
- Op 2 → Op 1 medium
- envelope to Gain 2 CV
- pitch envelope to LF FM
- trigger to Reset
- optional AR FM with noise burst to Op 1 for click

---

## Patch 2: Metallic industrial snare
- Op 1 lock, ratio 1
- Op 2 free, higher pitch
- Op 3 free, different pitch
- Op 2 → Op 1 medium/high
- Op 3 → Op 1 medium
- short envelopes to Gain 2 and Gain 3
- AR FM noise burst to Op 1
- trigger Reset each hit

---

## Patch 3: Neuro growl bass
- Op 1 lock ratio 1, shape triangle
- Op 2 lock ratio 2 or 3, shape triangle
- Op 3 free, shape saw
- Op 2 → Op 1 high
- Op 3 → Op 1 low/mod
- envelope/LFO to Gain 2
- different LFO to Gain 3
- slow LFO to Shape 1
- sequencer to 1V/Oct
- gate to Reset

---

## Patch 4: Feedback destroyer bass
- Op 1 lock ratio 1
- patch Op 1 or Op 2 output to AR FM
- AR FM send to Op 1
- envelope or synced LFO to Gain AR FM CV
- slight clipping on AR FM allowed for aggression
- small self-mod on Op 1 for added bite

---

## Patch 5: Ghost pad
- all in lock except Op 4 free
- Op 1 = carrier
- Op 2 → Op 1 light
- Op 3 → Op 1 light
- Op 4 → Op 2 very light
- slow LFOs to Gain 2 and Gain 3
- very slow random to Ratio 4
- shapes mostly sine/triangle
- no hard reset, or only occasional reset

---

# Best practices from the manual, translated into musical use

The manual warns that the module can quickly become noisy and dissonant. That's true. The musical way to work is:

## For harmonic results
Start with:
- VCO mode
- all operators locked
- all detunes centered
- shapes at sine
- all modulation sends down

Then add one thing at a time:
1. one modulator send
2. one envelope to that modulator’s Gain CV
3. one shape movement
4. one free operator or AR FM layer

That keeps patches intentional rather than random.

## For extreme results
Break the “safe” rules by:
- moving modulators toward square/saw
- adding self-modulation
- using free-state modulators
- clipping AR FM
- animating gain CV aggressively
- layering multiple modulators into one carrier

---

# My strongest recommendations for the sounds you asked for

## For distorted percussion
Prioritize:
- **Reset**
- **envelopes into Gain CV**
- **free-state modulators**
- **AR FM noise/audio bursts**
- **short pitch envelopes into LF FM**

## For dubstep / DnB bass
Prioritize:
- **one stable carrier + one animated main modulator**
- **Gain CV motion as your “wobble”**
- **shape modulation for vocal movement**
- **AR FM feedback patches**
- **free operator at low level for grit**

## For haunting pads
Prioritize:
- **lock mode with subtle ratios**
- **slow Gain CV modulation**
- **very slow shape modulation**
- **one or two low-level free operators**
- **light AR FM texturing**

---

If you want, I can also turn this into:
1. a **set of exact knob-position starter patches**, or  
2. a **“what to patch from common Eurorack modules” guide** using envelopes, LFOs, random, filters, and VCAs.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)