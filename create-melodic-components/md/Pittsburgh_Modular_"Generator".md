# Pittsburgh Modular — "Generator"

- [Manual PDF](../../manuals/Generator - Pittsburgh Modular Synthesizers.pdf)

---

[Manual PDF](https://pittsburghmodular.com/discontinued-products/generator)

# Pittsburgh Modular Generator — melodic use analysis

The **Pittsburgh Modular Generator** is a discontinued **dual analog oscillator / FM source** designed more for wild FM, percussion, and texture than precision tonal work. But it can still be used very effectively for **melodic components** if you treat it as a **character oscillator pair**, a **complex voice core**, or a **melodic modulation source** rather than a strict 1V/oct VCO.

## What the module is, musically

From the manual:

- **2 oscillators** built around triangle cores
- Wide frequency range
- **Internal FM routing**: Oscillator 1, via the **Index** section, internally FM-modulates Oscillator 2
- **External FM input** routable to either oscillator
- **Variable shape control** shared across both oscillators
- Outputs:
  - **1** = Generator 1 pre-Index VCA output
  - **2** = Generator 2 output
  - **OUT** = Generator 1 post-Index VCA output
- Not designed for accurate pitch tracking:
  - **Exponential CV**
  - **Does not track 1V/oct**
  - **Not temperature compensated**

That last point is the main limitation for conventional melody writing. Still, that does **not** make it unusable melodically. It just means:

- it is better for **short melodic figures**, drones, hooks, and layered tonal material
- it works best when **tuned by ear**
- it excels at **relative pitch relationships**, FM color, and animated harmonic lines
- pairing it with a quantizer, tuner, or a stable companion oscillator helps

---

## Important controls for melodic patching

## Oscillator 1 / GEN1

- **EXP input**: pitch/frequency CV input
- **3-way range switch**:
  - Left = **Low**
  - Center = **High**
  - Right = **Mid**
- **Range pot**: fine tuning

## Oscillator 2 / GEN2

Same basic controls, but with a key difference:

- **Oscillator 2 is internally FM’d by Generator 1 Index Out**
- The **Index pot** and **Index CV** determine the amount of internal FM sent from Oscillator 1 to Oscillator 2

This makes Oscillator 2 the main destination for classic internal two-operator-style FM tones.

## External FM section

- **External input**
- **Attenuverter**
  - 12 o’clock = 0
  - one side positive, the other inverted
- **Destination switch**
  - Up = modulate **GEN1**
  - Down = modulate **GEN2**

This is very useful for adding **vibrato, envelopes, audio-rate FM, or sequenced pitch motion**.

## Shape section

One shared **SHAPE** knob affects both oscillators inversely:

- Full left:
  - GEN1 = **square**
  - GEN2 = **triangle**
- Full right:
  - GEN1 = **triangle**
  - GEN2 = **square**

This is important melodically because:
- triangle gives smoother, purer, more fundamental-heavy tones
- square gives brighter, hollow, more overtone-rich tones
- changing shape alters perceived pitch clarity and articulation

## Index section

- **CV input** for Oscillator 1 VCA / FM amount control
- **OUT** = post-VCA Oscillator 1 output
- **Index pot**
  - Full left = **100% gain**
  - Full right = **0% gain**

That’s slightly counterintuitive. For stronger internal FM from Oscillator 1 into Oscillator 2, you generally want the **Index pot toward the left**, unless you’re using CV to dynamically control the amount.

---

# How to use Generator melodically

## 1. As a dirty dual-oscillator melodic voice

The simplest melodic use is to treat it like a two-oscillator voice source.

### Patch idea

- Send your pitch CV to:
  - **GEN1 EXP**
  - **GEN2 EXP**
- Set both oscillators to similar range settings, usually **Mid**
- Tune them by ear with the **Range pots**
- Take:
  - **Output 2** for the main tone, or
  - **Output 1 / OUT** for Oscillator 1
- Patch to a filter/VCA/envelope chain

### Musical result

- Slightly unstable but lively melodic lines
- Excellent for:
  - synth leads
  - basses
  - game-like hooks
  - raw twin-oscillator riffs

### Tip

Tune the oscillators to:
- unison for thickening
- octave for bass/lead reinforcement
- fifth for harmonically rich melodic drones
- slight detune for chorusing

Because it doesn’t track perfectly, intervals may drift a bit across the keyboard range, but this can sound beautiful in small melodic ranges.

---

## 2. As an FM melodic voice

This is where the module really shines.

Oscillator 1 internally FM-modulates Oscillator 2. So you can use:

- **GEN2** as the audible carrier
- **GEN1** as the modulator
- **Index** to control FM amount

### Patch idea: playable FM lead

- Pitch CV to **GEN2 EXP**
- Optionally mult same pitch CV to **GEN1 EXP**
- Set both to **Mid**
- Tune GEN1 relative to GEN2:
  - same pitch for denser tone
  - octave above for brighter FM
  - fifth above for more clangorous harmonic color
- Listen from **Output 2**
- Use **Index pot** to set FM depth
- Patch envelope to **Index CV** for transient brightness

### Musical result

- expressive FM plucks
- metallic melodic lines
- electric piano-ish tones
- bell-like sequences
- animated basses

### Why this works well

Even though the module is not precision-tracking, FM timbre often benefits from slight instability. If your melodic line stays within a moderate register, you can get very musical results.

---

## 3. Envelope-controlled FM for articulated notes

A particularly strong melodic use is applying an envelope to **Index CV**.

Because Index controls how much Oscillator 1 contributes to the internal FM path, you can create notes that start bright and become pure over time.

### Patch idea: FM pluck

- Sequencer pitch CV to **GEN2 EXP**
- Tune GEN1 above GEN2
- Envelope to **Index CV**
- Audio out from **2**
- Filter/VCA as usual

### Musical result

- percussive melodic notes
- marimba-like tones
- glassy plucks
- synthetic mallet sounds

### Best settings

- low-to-medium Index amount
- fast attack
- short decay
- triangle-leaning waveform for cleaner pitch center

This is probably one of the strongest “melodic component” patches for this module.

---

## 4. Using Oscillator 1 as audio and modulation at once

Generator’s architecture allows Oscillator 1 to serve two roles:

- audible tone source
- internal FM source for Oscillator 2

Since **Output 1** is pre-Index VCA and **OUT** is post-Index VCA, you can derive multiple related melodic signals.

### Patch idea

- Use **2** as your main melodic FM voice
- Use **OUT** or **1** as a second audio layer
- Tune both via shared or related pitch CV
- Pan them apart or process separately

### Musical result

- stereo melodic voices
- carrier/modulator dual-line textures
- layered harmonics from one compact module

For example:
- **2** into lowpass filter for body
- **OUT** into wavefolder or delay for sparkle

Because both oscillators are tightly related, the result feels coherent even when complex.

---

## 5. Cross-patched melodic instability

The manual includes a patch where **Generator 2 output** is sent into the **External CV input** to modulate Generator 1. That idea can be repurposed for melodies.

### Patch idea

- Patch **2** into **External Input**
- Set destination switch to **GEN1**
- Sequencer CV into both EXP inputs
- Tune by ear
- Use the external attenuverter carefully
- Take melodic audio from **OUT** or **2**

### Musical result

- aggressive, unstable FM leads
- tearing bass tones
- animated melodic phrases with lots of movement

This is less “clean melody” and more “musical chaos under pitch control.” Great for IDM, industrial, experimental electro, and game soundtrack sounds.

---

## 6. Use the shape control to make melodies read better in a mix

The **SHAPE** knob changes both oscillators in opposite directions, which is very musical.

### Practical melodic use

If your melody is too:
- **muddy or indistinct**: move toward more square content
- **harsh or overly buzzy**: move toward more triangle content

### Tonal behavior

- **Triangle-heavy settings**
  - better note definition
  - softer FM
  - more pitch-stable perception
  - good for bass and melodic sequences
- **Square-heavy settings**
  - more edge
  - better for leads
  - more pronounced upper harmonics
  - stronger retro/game-like tone

This single knob is excellent for shaping where your melodic part sits in the arrangement.

---

## 7. As a melodic modulation source for other modules

Even if you don’t use Generator as the main voice, it can be crucial in building melodic parts elsewhere.

Because it provides two related oscillators, it can create:

- audio-rate FM for another VCO
- LFO-rate vibrato if set low
- animated filter FM
- timbral modulation locked to the pitch contour of your sequence

### Patch idea: Generator modulates a stable oscillator

If you have a precise VCO elsewhere:

- Sequencer pitch CV to your stable VCO
- Same or related CV to **GEN1** or **GEN2**
- Use **1**, **OUT**, or **2** to FM that stable oscillator, filter, or wavefolder
- Listen to the stable oscillator as main audio

### Musical result

- melodic line remains in tune
- Generator adds animated harmonic personality
- best of both worlds: pitch stability + FM chaos

This is arguably the most practical “melodic” role in a larger system.

---

# Best melodic roles for each output

## Output 1
**Generator 1 pre-Index VCA**

Use when you want:
- a direct Oscillator 1 tone
- a raw modulator signal
- a second oscillator layer unaffected by Index VCA behavior

Best for:
- supporting melodic lines
- additional drone
- modulation duties

## Output 2
**Generator 2 output**

This is usually the best main melodic output because:
- it receives the internal FM action from Oscillator 1
- it tends to be the more interesting “complex oscillator” output

Best for:
- leads
- basses
- plucks
- metallic tonal sequences

## OUT
**Oscillator 1 post-Index VCA**

Use when you want:
- a dynamically shaped version of Oscillator 1
- amplitude linked to the Index section
- CV-controlled articulation

Best for:
- companion melodic layer
- FM-linked rhythmic audio
- dynamic sublayer under Output 2

---

# Melodic patch recipes

## 1. Simple bassline voice

- Pitch CV to **GEN2 EXP**
- GEN2 range = **Mid**
- GEN1 range = **Low** or **Mid**
- Tune GEN1 to unison or octave below/above
- Output from **2**
- SHAPE toward triangle
- Low Index amount

**Result:** warm but gritty bass with subtle FM body.

---

## 2. Metallic lead

- Pitch CV multed to **GEN1 EXP** and **GEN2 EXP**
- Both in **Mid**
- Tune GEN1 slightly above GEN2
- Envelope to **Index CV**
- Output from **2**
- SHAPE toward brighter side
- Optional filter after

**Result:** animated lead with metallic attack and evolving sustain.

---

## 3. Bell sequence

- Pitch CV to **GEN2 EXP**
- Tune GEN1 at a higher interval
- Index moderate to high
- Fast-decay envelope to **Index CV**
- Use **2** out
- Add reverb/delay

**Result:** chiming, bell-like melodic notes.

---

## 4. Retro game melody

- Pitch CV to both oscillators
- Keep FM low
- Use SHAPE so one oscillator is square-heavy
- Mix **1** and **2** externally if possible
- Add slight detune

**Result:** strong chip-ish hook with analog instability.

---

## 5. Dual-line harmonic melody

- Same sequence to both EXP inputs
- Tune GEN1 a fifth above GEN2
- Use **1** and **2** as separate voices
- Send to separate VCAs or filters

**Result:** one module creates an interval-based melodic stack.

---

# Strengths for melodic music

## 1. Rich timbre from minimal patching
Internal FM routing gives immediate complexity without needing multiple extra modules.

## 2. Great transient tone design
Index CV makes it easy to shape note attacks, which is very important for melodic articulation.

## 3. Strong interval-based tuning by ear
Even without exact tracking, it is excellent for fixed melodic relationships like:
- octaves
- fifths
- detuned unison
- upper partial emphasis

## 4. Characterful pitch drift
For many styles, slight instability feels alive rather than flawed.

---

# Limitations for melodic use

## 1. Not true 1V/oct
This is the biggest limitation for conventional keyboard-style playing over large ranges.

## 2. FM can obscure pitch center
At high Index settings the tone may become clangorous or noisy, reducing melodic clarity.

## 3. Shared shape control
You cannot independently shape the two oscillators, so balancing harmonic content takes compromise.

---

# Best companions for melodic use

This module becomes much more effective in melodic systems when paired with:

- **Quantizer**
  - helps keep CV moves musically constrained
- **Tuner**
  - useful for manual calibration by ear and eye
- **Filter**
  - taming harsh FM for more note-focused lines
- **Envelope + VCA**
  - essential for note articulation
- **Stable oscillator**
  - for layering or external FM targets
- **Mixer**
  - to combine outputs 1, 2, and OUT into composite melodic tones
- **Wavefolder / LPG / delay / reverb**
  - especially good for plucks and bells

---

# Overall melodic verdict

The **Pittsburgh Modular Generator** is not a conventional precision melody oscillator, but it is very useful for **melodic sound design**.

It works best as:

- a **character lead/bass source**
- a **2-operator-style analog FM voice**
- a **bell/pluck/percussion melodic generator**
- a **dual oscillator for interval tuning**
- a **chaotic modulation partner** for a more stable tonal voice

If you want **clean tonal sequencing across many octaves**, this is not ideal by itself.  
If you want **expressive, aggressive, animated melodic components with analog FM personality**, it is excellent.

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)