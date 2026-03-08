# Doepfer — A-119

- [Manual PDF](../../manuals/A119_man.pdf)

---

[Manual PDF](attachment)

# Doepfer A-119 Ext. Input / Envelope Follower — using it for melodic patching

The attached manual is for the **Doepfer A-119 External Input / Envelope Follower**.  
This module is not a pitch source by itself, but it is very useful for building **melodic components** when combined with oscillators, filters, VCAs, envelopes, slews, comparators, sequencers, quantizers, and clocking modules.

## What the A-119 does

The manual describes three main functions:

- **Preamp**
  - **Asym. In** for line-level signals
  - **Symm. In** for mic/instrument-level signals
- **Envelope follower**
  - Creates a CV proportional to input amplitude at **Env. Out**
- **Comparator / gate extractor**
  - Creates a gate at **Gate Out** when the signal exceeds the **Threshold**

It also provides:

- **Audio Out** of the amplified incoming signal
- **Overload LED**
- Envelope and gate indication LEDs

## Why this matters melodically

In a Eurorack system, melody usually needs some combination of:

- **pitch CV**
- **gates/triggers**
- **dynamic articulation**
- **timbral movement**

The A-119 directly gives you:

- **gates** from external sound events
- **dynamic CV** from external amplitude
- **amplified audio** that can enter the modular signal path

That means it can convert an external performance source into control information for melodic patches.

---

# Core melodic uses

## 1. Turn external rhythm into note triggers

The manual explains that **Gate Out** goes high whenever the input envelope exceeds the threshold.  
This is the most immediate melodic use.

### Patch idea
- Plug voice, drum loop, guitar, or percussion into **Asym. In** or **Symm. In**
- Set **Gain** so the signal is healthy but not constantly overloading
- Adjust **Threshold** so only desired events produce gates
- Send **Gate Out** to:
  - an envelope generator gate input
  - a sequencer clock/advance input
  - a sample-and-hold trigger
  - a logic module driving melodic events

### Melodic result
Each transient or phrase in the external audio can:

- trigger a note
- advance a sequence
- articulate a bassline
- create call-and-response between external performer and modular voice

This is one of the strongest ways to make melody from the A-119:  
**the external source becomes the phrasing engine**.

---

## 2. Use the envelope follower as melodic expression CV

The **Env. Out** follows the loudness contour of the input signal.  
That gives you a continuously varying CV based on how hard you sing, play, or feed audio.

### Good destinations for melody-related modulation
Patch **Env. Out** to:

- **VCO pitch FM attenuated lightly** for expressive pitch bend
- **quantizer input** for stepped melodic motion
- **filter cutoff** to shape note brightness
- **VCA CV** for dynamics
- **wavefolder amount** for intensity-linked harmonics
- **sequencer transpose input**
- **precision adder / offset + quantizer** chain for controllable note generation

### Melodic result
Your input dynamics can become:

- note accents
- melodic rises and falls
- transposition gestures
- phrase-based modulation

Because the envelope is tied to amplitude rather than pitch, it works especially well for **expression**, **contour**, and **phrase shaping**.

---

## 3. Build melodies from speech or singing contours

The A-119 does **not** track pitch.  
But the manual’s “singing synth” example shows that it works well with voice as a control/audio source.

### Practical melodic strategy
Use a microphone into **Symm. In**:

- **Gate Out** triggers an envelope or sequencer advance
- **Env. Out** modulates:
  - quantizer input
  - sequencer transpose
  - filter or VCA
- **Audio Out** can be mixed, filtered, ring modulated, or otherwise processed in parallel

### Result
Your voice controls the **shape and articulation** of a melody, even if the actual pitch is generated elsewhere.

This is ideal for:

- vocal-controlled synth lines
- talking synth patches
- phrase-synced arpeggios
- responsive lead patches

---

# Best companion modules for melodic patching

Since you asked how these modules can be used together to create melodic components, here are the most effective pairings with the A-119.

## A-119 + VCO
Use the A-119 to control when and how notes happen, while the VCO provides the actual pitch.

### Patch
- External source -> **A-119 input**
- **Gate Out** -> ADSR gate
- ADSR -> VCA CV
- VCO -> VCF/VCA -> output
- **Env. Out** -> slight pitch modulation or filter cutoff

### Melodic role
The external source becomes the articulation layer for the oscillator melody.

---

## A-119 + Quantizer
This is one of the best melodic combinations.

### Patch
- **Env. Out** -> attenuator/offset -> quantizer input
- quantizer output -> VCO 1V/oct
- **Gate Out** -> envelope trigger or sample-and-hold clock

### Melodic role
The amplitude contour of the external sound becomes stepped notes in a scale.

### Tips
- Use attenuation before the quantizer for musically useful note ranges
- Add offset so the melody sits in the right register
- Use slower source material for more stable notes

This turns the A-119 into a kind of **gesture-to-melody converter**.

---

## A-119 + Sample & Hold
This creates cleaner discrete melodies from complex audio.

### Patch
- **Env. Out** -> sample & hold input
- **Gate Out** -> sample & hold trigger
- sample & hold output -> quantizer -> VCO pitch

### Melodic role
Whenever the input crosses threshold, the current envelope level is sampled as a note value.

### Result
- Percussive input produces stepped melodies
- Speech produces irregular melodic phrases
- Guitar attacks can generate playable note patterns

This is one of the most musically useful ways to derive melodic material from the A-119.

---

## A-119 + Slew limiter
The manual specifically mentions using an **A-170 slew limiter** for smoothing.

### Two important melodic uses

#### A. Smoothing low-frequency envelope artifacts
The manual notes that with input frequencies below 50 Hz, extra smoothing may help.

#### B. Turning stepped CV into legato melodic movement
If you sample/hold the envelope and then slew it slightly before quantizing or after quantizing, you can get:

- portamento-like motion
- softer melodic transitions
- fewer clicks when using gate-derived articulation

---

## A-119 + Envelope generator + VCA
This is the most direct “play the modular from external sound” setup.

### Patch
- External signal -> A-119
- **Gate Out** -> ADSR gate
- ADSR -> VCA CV
- VCO -> VCF -> VCA
- **Env. Out** -> VCF cutoff or oscillator FM amount

### Melodic role
The melody source may be a sequence or keyboard, but the external signal determines **when** the notes speak and **how expressive** they are.

This is great for:
- rhythm guitar driving synth notes
- drum loop articulating a sequence
- speech opening melodic stabs

---

## A-119 + Sequencer / clocked melody source
Use gate extraction to advance notes from any sequence.

### Patch
- **Gate Out** -> sequencer clock
- sequencer CV -> VCO pitch
- A-119 **Env. Out** -> transpose / filter / accent

### Melodic role
External audio becomes the timing source for melody.

### Result
- Beatboxing can drive a bassline
- picked guitar can advance an arpeggio
- chopped vocal can clock a lead line

This produces very musical “humanized” melodies.

---

## A-119 + Ring mod / audio processor in a melodic chain
The manual gives a ring modulator example and explains using the envelope to “squelch” the ring mod output via a VCA.

### Melodic takeaway
Even though ring modulation is often timbral rather than melodic, you can use the A-119 to keep note articulation tied to the external signal.

### Patch
- External audio -> A-119
- A-119 audio out -> ring mod input
- VCO sine -> other ring mod input
- A-119 envelope or smoothed gate -> VCA controlling ring mod output

### Melodic role
The VCO can be tuned melodically while the external sound provides dynamic articulation.

This is good for:
- tuned metallic leads
- voice-controlled melodic textures
- hybrid acoustic/synth phrases

---

# Patch recipes for melodic components

## 1. External percussion to quantized melody
A very effective melodic patch.

### Patch
- Drum loop -> A-119 Asym. In
- Set threshold so kicks/snares produce clear gates
- **Env. Out** -> attenuator -> sample & hold input
- **Gate Out** -> sample & hold trigger
- sample & hold -> quantizer
- quantizer -> VCO 1V/oct
- VCO -> VCA
- **Gate Out** -> envelope -> VCA CV

### What happens
Each detected hit generates:
- a new note
- a matching articulation

### Sound
A groove-derived melody tightly connected to the source rhythm.

---

## 2. Voice-controlled lead synth
### Patch
- Mic -> **Symm. In**
- **Gate Out** -> ADSR gate
- ADSR -> VCA CV
- **Env. Out** -> attenuator -> quantizer -> VCO pitch
- VCO -> filter -> VCA
- A-119 **Audio Out** optionally into a parallel effect path

### What happens
Your singing loudness and phrasing shape the synth line.

### Sound
Organic, vocal-like melody generation.

---

## 3. Guitar attack drives arpeggio
### Patch
- Guitar -> **Symm. In**
- **Gate Out** -> clock input of sequencer/arpeggiator
- sequencer CV -> oscillator pitch
- **Env. Out** -> transpose amount or filter cutoff
- oscillator -> VCA
- **Gate Out** -> envelope -> VCA

### What happens
Each picked note steps the sequence forward.

### Sound
The guitar “plays” the synth melody rhythmically.

---

## 4. Ducking-based counter-melody
The manual includes a ducking example. You can adapt it melodically.

### Patch
- External audio -> A-119
- Internal melodic voice through VCA
- **Env. Out** -> inverter -> VCA CV for internal melody

### What happens
When the external signal is present, the internal melody ducks.

### Musical use
This creates:
- responsive call-and-response
- space for live voice/instrument
- dynamic interaction between melodic layers

---

## 5. Singing synth / subharmonic melody
The manual’s “singing synth” patch uses the voice with a divider/sub-octave path.

### Melodic extension
Instead of only using the source as raw audio:
- mic -> A-119
- **Gate Out** -> envelope
- **Env. Out** -> filter movement or quantized transpose
- A-115/suboctave or oscillator stack -> VCA/filter chain

### Sound
A vocal-driven melodic synth with strong tracking of phrasing, not pitch.

---

# Important operational details from the manual

## Input choice matters
- **Asym. In**: line-level/unbalanced
- **Symm. In**: mic/instrument-level/balanced, much more gain available

The manual notes the gain ranges:
- unbalanced input: about **0–20**
- balanced input: about **0–500**

So for melody extraction from:
- drum machines / mixers / line outputs: use **Asym. In**
- mic / guitar: use **Symm. In**

## Use only one input at a time
The manual explicitly warns there is only one gain control for both inputs.  
If both are used, they are mixed in a **1:25 ratio**.

For predictable melodic control, use just one source at a time.

## Watch the overload LED
If the preamp overloads, your envelope and gate behavior can become less controllable.

For melodic patches, stable tracking is important:
- increase gain until response is strong
- back off if overload is constant
- then set threshold carefully

## Threshold is the key to musicality
The **Threshold** control determines what counts as an event.

This affects whether your melody is:
- dense
- sparse
- stable
- noisy
- rhythmically locked

In practice:
- low threshold = more triggers, more chaotic note generation
- high threshold = fewer, more deliberate notes

---

# Limitations to understand

## It is not a pitch tracker
The A-119 does not extract 1V/oct pitch from incoming audio.  
So it will not turn singing directly into correctly tracked note CV.

Instead, it gives:
- **amplitude-following CV**
- **gate extraction**
- **audio amplification**

To get stronger melodic behavior, pair it with:
- quantizer
- sample & hold
- sequencer
- precision adder
- slew
- envelope/VCA chain

## Envelope output is better for contour than exact notes
By itself, **Env. Out** is not musically scaled. It is a raw control voltage.  
To use it melodically, shape it with:
- attenuation
- offset
- quantization
- sampling
- inversion

That is where the real melodic patching comes from.

---

# Most musical combinations, ranked

## Best for immediate melody
1. **A-119 + Sample & Hold + Quantizer + VCO**
2. **A-119 + Sequencer clock input + VCO**
3. **A-119 + ADSR/VCA + existing pitch source**
4. **A-119 + Ring mod + VCA for tuned textures**
5. **A-119 + Inverter/VCA for ducking and counterpoint**

---

# Practical performance tips

## For tighter melodic triggers
Use percussive or clearly articulated input.

## For smoother melodic CV
Use slower, sustained sources like:
- voice
- bowed strings
- pads
- legato guitar

## For controlled note ranges
Always attenuate **Env. Out** before it reaches a quantizer or pitch input.

## For expressive phrasing
Use:
- **Gate Out** for note onset
- **Env. Out** for accent, timbre, or transpose

That combination gives the most natural musical behavior.

---

# Conclusion

The **Doepfer A-119** is best thought of as a **bridge from external sound into melodic control**.  
It does not generate pitch on its own, but it is excellent for:

- extracting gates from live or recorded audio
- deriving expressive CV from dynamics
- bringing external sound up to modular level
- making external performance drive melodic sequencing and articulation

If you combine it with standard melodic modules like a **VCO, quantizer, sample & hold, sequencer, ADSR, VCA, and slew limiter**, it becomes a very powerful tool for:

- voice-controlled synth lines
- rhythm-driven melodies
- guitar-triggered sequences
- dynamic transposition
- expressive hybrid acoustic/modular patches

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)