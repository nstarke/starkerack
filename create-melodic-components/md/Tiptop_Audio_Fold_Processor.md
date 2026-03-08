# Tiptop Audio — Fold Processor

- [Manual PDF](../../manuals/Tiptop_Audio_foldprocessor.pdf)

---

[Manual PDF](https://www.tiptopaudio.com)

# Tiptop Audio Fold Processor: using it for melodic parts

From the manual, this module has **two linked analog sections**:

1. **Wavefolder**  
   - Audio goes in at **IN 1 / IN 2**
   - Main controls: **FOLD** and **INJECT**
   - Both can be modulated with CV via:
     - **FOLD CV** + attenuator
     - **INJECT CV** + attenuator
   - Main folded sound comes out of **OUT**

2. **Subdivider / square & divide section**
   - Fed internally from the folded output
   - Mixed output at **SUBDIV OUT**
   - Four octave-related divisions with level knobs:
     - **÷1**
     - **÷2**
     - **÷4**
     - **÷8**

The manual specifically demonstrates pairing it with:
- a **Tiptop Z2040** self-oscillating filter as a sine source, or
- a **Z3000** sine output,
- plus optionally an **LFO**
- and even **Z-DSP** delay/feedback ideas.

So if your goal is **melodic content**, the Fold Processor is best understood as a **timbre and octave-generation voice shaper**, not a pitch source by itself.

---

## What this module contributes musically

For melody writing, the Fold Processor helps in three main ways:

### 1. It adds harmonic richness to simple pitched material
If you feed it a **sine or triangle** from a VCO, or a **self-oscillating filter sine**, the **FOLD** control adds upper harmonics while preserving the underlying pitch.

This is ideal for:
- making a plain melody line more vivid
- animating sustained notes
- creating expressive lead tones
- turning a basic bass sequence into something more vocal or metallic

This is classic wavefolding behavior: the pitch remains the same, but the overtone content becomes more complex.

---

### 2. It creates musically related sub-octaves
The **SUBDIV OUT** gives you divided versions of the already-processed signal, with four mixable divisions spaced by octaves.

That makes it useful for:
- sub-octave bass reinforcement
- adding lower octave layers under a melody
- generating organ-like stacked octave textures
- making a monophonic line feel fuller and more harmonically anchored

Because the divisions are mixed with separate gain knobs, you can dial in:
- just a single lower octave
- a thick 2-octave bass stack
- a complex pulse-rich harmonic bed underneath a lead

---

### 3. It introduces movement through CV
The manual emphasizes that **FOLD** and **INJECT** are both voltage controllable.

That means a melody can evolve over time by modulating:
- fold depth
- offset/injection amount
- the behavior of the subdivider indirectly, since it follows the folded signal

This is especially effective for:
- accents
- phrasing changes
- timbral variation per note
- dynamic bass textures
- pseudo-sequenced harmonic shifts even when pitch stays fixed

---

# Best melodic pairings from the manual

## 1. Z2040 + Fold Processor
The manual’s first patch uses the **Z2040** in self-oscillation as a natural sine source.

### Why this works melodically
A self-oscillating filter can track pitch and act like a sine oscillator. Feeding that into the Fold Processor gives you:
- a clean base tone from the Z2040
- a harmonically enriched lead/bass voice from the Fold Processor
- controllable timbre without losing clear pitch identity

### Melodic use cases
- **Lead voice**: sequence the Z2040 pitch, send its output to Fold, and animate FOLD with slow CV
- **Bassline**: use lower notes, then blend in **÷2** and **÷4** at SUBDIV OUT
- **Plucked melodic line**: use envelope-driven modulation to FOLD CV for note-by-note brightness changes

---

## 2. Z3000 sine output + Fold Processor
The manual also suggests using the **Z3000 sine output** if you don’t have the Z2040.

### Why this is strong for melody
A stable sine VCO into a wavefolder is one of the most reliable ways to build:
- articulate melodies
- FM-adjacent tones
- west-coast-style expressive voices

### Good melodic patch ideas
- **Simple lead**: Z3000 sine → Fold IN1 → OUT
- **Animated sequence**: sequence pitch on Z3000, patch LFO or envelope into FOLD CV
- **Bass melody with body**: use SUBDIV OUT and mix in **÷1 + ÷2**

---

## 3. LFO + Fold CV for evolving phrases
On page 3, the manual shows an **LFO patched to FOLD CV** while listening to **SUBDIV OUT**.

### What this does musically
This does not change the note pitch directly, but it changes the overtone profile and how the divide circuit reacts.

For melodies, this gives:
- changing articulation across sustained notes
- rhythmic animation
- “talking” or pulsing harmonic motion
- movement in octave layers

### Best applications
- sustained melodic drones
- sequenced basslines with subtle motion
- repeated arpeggios that need more life
- evolving ostinatos

---

## 4. Z-DSP after Fold Processor
The manual suggests adding **delay from the Z-DSP**, or putting Fold in the **feedback path**.

### Melodic role
This turns the Fold Processor from a simple timbre tool into a phrase-sculpting effect.

Useful for:
- melodic echoes with increasingly folded harmonics
- dubby sub-octave bass repeats
- dense lead textures
- feedback melodies that grow more unstable and expressive

---

# How to build melodic voices with this module

## Patch 1: Expressive folded lead
**Goal:** a playable or sequenced lead voice

**Patch**
- VCO or self-oscillating Z2040 sine → **Fold IN1**
- **Fold OUT** → VCA / filter / mixer / output
- Envelope or slow CV → **FOLD CV**
- Optional second modulation source → **INJECT CV**

**Result**
- clean pitch center
- harmonic complexity per note
- animated lead tone without needing multiple oscillators

**Tip**
Keep FOLD moderate for tonal melodies. High settings can become noisy or unstable.

---

## Patch 2: Melodic bass with octave reinforcement
**Goal:** a bassline that stays melodic but gains weight

**Patch**
- Sine/triangle VCO → **Fold IN1**
- Use **SUBDIV OUT**
- Bring up:
  - **÷1** for original folded core
  - **÷2** for one octave down
  - optionally **÷4** for extra depth

**Result**
- thick, organ-like or synth-bass character
- strong melodic center
- richer low-end from a single source

**Tip**
For clear bass melodies, use less folding and lower levels on the deepest divisions.

---

## Patch 3: Evolving melody from one oscillator
**Goal:** make a repetitive sequence feel harmonically alive

**Patch**
- Sequenced oscillator → **Fold IN1**
- Slow LFO → **FOLD CV**
- Different slow or offset CV → **INJECT CV**
- Monitor **OUT** or **SUBDIV OUT**

**Result**
- every repetition has slightly different harmonic behavior
- melodic phrases breathe over time
- can sound like subtle filtering, PWM, or timbral sequencing

---

## Patch 4: Call-and-response lead and sub layer
**Goal:** use both outputs in a larger patch

Since the subdivider is fed from the folded output internally, you can use:
- **OUT** as the brighter main melody
- **SUBDIV OUT** as a lower shadow voice

**Patch**
- Oscillator → Fold
- **OUT** → main melodic chain
- **SUBDIV OUT** → second VCA/mixer channel

**Result**
- top voice and low octave support from one source
- easy layered melodic phrasing
- useful for techno leads, electro basses, and cinematic monosynth lines

---

# Important musical behavior from the manual

## The sound depends heavily on the input signal
The manual says results are “heavily dependent on the type of incoming signal.”

For melodic use, that means:

### Best inputs
- sine
- triangle
- self-oscillating filter
- simple VCO waveforms

These preserve pitch clarity and produce the most controlled melodic results.

### More aggressive inputs
- samples
- drums
- already-complex waveforms

These can work, but the Fold Processor behaves more like **analog distortion** than classic melodic wavefolding.

So for melody:
- use simple waveforms when you want tonal precision
- use complex material when you want broken, gritty, industrial phrases

---

## INJECT can create “dead zones”
The manual mentions the INJECT control may create a **dead zone**, especially near edges.

Musically, this means:
- not all knob positions will respond smoothly
- some settings may seem to reduce activity
- this is normal and part of the circuit character

In performance, use this intentionally:
- dead zones can create contrast
- sweeping in and out of them can give expressive transitions
- they’re especially dramatic on the subdivider

---

## The subdivider can get “totally wild”
The manual warns that with Fold and Inject sweeps:
- octaves move in and out
- pulses get pulse-width modulated
- the sound can range from sweet to destructive

For melodic work, this means the subdivider is best used in two modes:

### Controlled mode
- modest FOLD
- modest INJECT
- one or two subdivision levels only

Good for:
- basslines
- octave doubling
- tonal accompaniment

### Wild mode
- stronger folding
- active modulation
- multiple divisions mixed

Good for:
- aggressive hooks
- experimental melodies
- broken arpeggios
- transitions and fills

---

# Practical strategies for melodic composition

## Use OUT when melody clarity matters
If the tune itself is the focus, the **OUT** jack is usually the better choice.

Use it for:
- lead lines
- melodic arps
- motif definition
- parts that must track pitch clearly

---

## Use SUBDIV OUT when harmony-by-octave matters
If you want one note to sound like a stacked instrument, use **SUBDIV OUT**.

Use it for:
- bass foundations
- octave chorusing
- drone melodies
- single-note riffs that need more size

---

## Modulate timbre, not pitch
The Fold Processor does not quantize or create scales. Its melodic role is:
- shaping harmonics
- adding octave divisions
- making one pitch line sound more musically complex

So pair it with:
- sequencers
- keyboard CV
- quantized random CV
- tuned self-oscillating filters or VCOs

That gives you a proper melodic source, while Fold adds expression and depth.

---

# A few strong “musician” patch recipes

## West-coast style melody voice
- Sine oscillator → Fold IN1
- OUT → LPG or VCA
- Envelope → amplitude
- Slow envelope/LFO → FOLD CV

Great for:
- plucks
- woody leads
- animated monosynth lines

---

## Octave bass melody
- Oscillator → Fold
- SUBDIV OUT → VCA/filter
- Raise ÷1 and ÷2, tiny bit of ÷4
- Sequence the source oscillator

Great for:
- techno bass
- electro lines
- synthwave support bass

---

## FM-adjacent melodic texture
The manual suggests patching **OUT into the FM input of a VCO**.

Try:
- VCO A sine → Fold
- Fold OUT → FM input of VCO B
- Sequence VCO B as main melody
- Use VCO A as harmonic animator

Great for:
- glassy tuned leads
- unstable melodic tones
- metallic but musical voices

---

## Melodic delay line
- Oscillator → Fold → Z-DSP delay
- Sequence oscillator
- Modulate FOLD slowly

Great for:
- ambient melodies
- dub sequences
- repeating motifs that evolve harmonically

---

# Bottom line

The **Tiptop Fold Processor** is not primarily a melody generator; it is a **melodic enhancer and octave sculptor**.

Used with modules referenced in the manual—especially a **Z2040**, **Z3000**, **LFO**, and **Z-DSP**—it can create:

- expressive folded leads
- octave-rich basslines
- animated mono melodies
- evolving arpeggios
- distorted melodic hooks
- sub-octave accompaniment from a single oscillator

For the most musical and pitch-stable results:
- feed it simple, tuned waveforms
- use **OUT** for clarity
- use **SUBDIV OUT** for octave layering
- modulate **FOLD** and **INJECT** for phrasing and movement

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)