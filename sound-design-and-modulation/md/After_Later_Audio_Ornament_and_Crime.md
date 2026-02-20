# After Later Audio — Ornament and Crime

- [Manual PDF](../../manuals/ornament and crime.pdf)

---

[Ornament & Crime v1.3 User Manual (PDF)](https://ornament-and-cri.me/user-manual-v1_3/)

---

# Eurorack Sound Design with Ornament & Crime (o_C)

Ornament & Crime is a highly polymorphic Eurorack module with a diverse array of apps. Let's dive into creative modulation strategies for designing:

- Distorted percussion  
- Crazy basslines (dubstep, DnB)  
- Haunting atmospheric pads  

Each suggestion leverages specific apps and CV modulation mappings described in the manual:

---

## 1. Distorted Percussive Sounds

### Use: **Piqued** (Quad Envelope Generator)
- **Envelope type:** Choose looping AD, ADR, or ADL2 types for sharp percussive shapes.
- **Segment shapes:** Use Ledge, Cliff, and the various "Dipper" and "Wiggle" shapes for non-standard transients.
- **Envelope Duration Modulation:** Assign CV inputs to decay, sustain, or ADR duration to make envelope times ever-changing, resulting in evolving percussive impacts.
- **Euclidean Trigger Filters:** Set up polyrhythmic, glitchy patterns via the Eucl. Length and Fill parameters. Modulate Fill and Rotation with CV for morphing rhythm structures.

### Use: **Viznutcracker, Sweet!** (Bytebeat Generator)
- **Run Bytebeat equations at audio rate** (Speed = 255).  
- Stepped, digital waveforms combine bits and clicks for industrial snares/claps.
- **Modulate Parameters:** Map CV or knob to Pitch, Parameters 0/1/2, or equation selection for morphing digital percussion timbres.
- **Step mode:** Clock it externally and use its output as raw percussive bursts, then heavily low-pass filter downstream.

### Tips
- **Cross-patch**: Envelope (from Piqued) out controls VCA amplitude for bytebeat audio.
- **Extreme Settings:** Use random envelope shapes and euclidean trigger randomness for unpredictable glitch percussion.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

### Use: **Sequins** (Step Sequencer with CV Modulation)
- **Write a sequence** of semitones to define a solid "wobble" bassline, typical of dubstep.
- **Chain sequences:** Use multiple patterns for longer riffs; combine forward, pendulum, and Brownian/random directions.
- **Aux Output:** Instead of just gates, select envelope (ADSR, ADR) for "ducking" FX.
- **Assign CV inputs** to "mult/div" for variable rhythmic sync, or to "direction"/"scale mask" for lexical morphing.

### Use: **Meta-Q / Quantermain** (Quantizer with Internal Turing, Bytebeat, Integer Sequences)
- **Set source to internal ByteB/IntSeq/LFSR**  
- Assign a Turing Machine or integer sequence as the CV source for semi-random "talking" basslines.
- **Turing Machine Probability CV:** Modulate with LFO or audio rate signals for controlled chaos.
- Apply non-octave scales (Carlos alpha/beta/gamma, Bohlen-Pierce) for "alien" tonality.

### Use: **CopierMaschine** with Modulated Buffer/Index
- Feed in wild LFOs or sample from Bytebeats.
- **Modulate buffer index** (delay) with CV or envelope.
- Freeze buffer on beats—turns sampled basslines into stuttering glitches.

### Use: **Quadraturia** (LFO)
- Audio-rate LFOs as FM for VCOs—modulate the frequency and shape of the LFO for evolving, bitcrushed modulation on your bass OSC.

---

## 3. Haunting Atmospheric Pads

### Use: **Low-rents** (Lorenz & Rössler Attractor Generator)
- Slow, self-modulating, quasi-random waveforms for evolving pads.
- Map x/y/z outputs to multiple voices/VCF cutoffs.
- Modulate "rho"/"c" parameters or LFreq via external slow LFOs.

### Use: **Quadraturia** (Quadrature LFO)
- Set very slow frequency range ("cosmological"/"geol.").
- CV-control shape spread, phase, and coupling for huge, drifting movement between layers.
- Use outputs to modulate parallel VCAs or VCFs for wide stereo fields.

### Use: **Piqued** with Long, Looping Envelopes
- ADR, ADSR with massive segment lengths (multipliers up to 8192!).
- Use Sine or Quartic shapes for slow swells and fades.
- External CV control over durations/levels for pads that "breathe" and never repeat exactly.

### Use: **Viznutcracker, Sweet!** at Slow Step Rates
- Enable Loop Mode and reduce Speed for slow-changing, stepped CV.  
- Patch to modulate effects (reverb mix, delay time) or filter cutoff for unpredictable ambiance.

---

## General Tricks

- **Extreme Randomization:** Modulate everything—masks, root, buffer index, pattern offsets—to push o_C into unpredictable territory.
- **External Feedback:** Send o_C outputs through distortion, wavefolders, or even back into its own CV inputs.
- **Non-octave Tunings:** Explore alternate tunings for unfamiliar textures, especially with random melodic/sequence sources.

---

#### For deeper reference, consult the full manual:  
[Ornament & Crime v1.3 User Manual](https://ornament-and-cri.me/user-manual-v1_3/)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
