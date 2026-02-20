# ADDAC Systems — ADDAC-506 SignalFlow

- [Manual PDF](../../manuals/ADDAC506_SignalFlow.pdf)

---

[ADDAC506 VC Stochastic Function Generator & Expansion Manual PDF](https://media.addacsystem.com/files/ADDAC506_Manual.pdf)

---

# Creative Modulation Techniques with the ADDAC506 VC Stochastic Function Generator

The ADDAC506 is an extremely flexible and deep function generator and envelope source, capable of generating randomized, evolving modulation across four channels. With a wealth of CV control, randomization options, and unique architecture, it’s possible to coax everything from wild, distorted percussion to gnarly basslines and eerie pad textures from your modular setup. Below are targeted tips for using its features to unlock these sonic possibilities.

---

## Quick Overview of Key Features for Modulation

- **Four independent envelope channels (Envelope 1–4)**, each with:
  - Randomizable rise and fall times (including external triggers for randomization mid-cycle)
  - Linear/logarithmic curve morphing
  - Attenuvertable amplitude and offset (-10V to +10V)
  - Voltage-controlled min/max rise/fall
  - Speed range (Low/Medium/High)
  - Loop/One-shot modes
  - Slew and Trigger modes
  - Individual EOR (End of Rise) and EOF (End of Fall) outputs for rhythm creation

- **Sum and averaging mix outputs** for morphing multiple envelopes together

- **Expansion randomization triggers and outputs** for deeper algorithmic control

---

## 1. **Distorted Percussive Sounds**

To achieve aggressive, modulated, and sometimes distorted percussion (kicks, snares, metallic hits):

### Settings & Patching Tips

- **Activate One-shot Mode:** Use Trigger mode to fire percussive shapes, with each new trigger producing a fresh, randomized envelope.
- **Randomize Rise and Fall Times:** Set RISE MIN/MAX and FALL MIN/MAX to short and mid values, with moderate randomness (external random triggers for extra variation).
- **Sharp Curves:** Twist the CURVE knob towards LOG to get exponential punch (fast attack, snappy decay).
- **Amplitude & Offset:** Use large amplitude, possibly with a positive offset for upward-moving CV, driving a VCA or wavefolder for clipping/distortion.
- **Speed Range:** Use MED or HIGH for snappy envelopes.
- **Patch Ideas:**
  - Run the envelope outputs (1–4) directly into a VCA or LPG that shapes a drum sample or oscillator.
  - Modulate the amplitude of a distortion module with an envelope channel for gated, overdriven hits.
  - Use EOR/EOF gates to trigger aggressive FM or sync events on other oscillators.
- **Wild Mixing:** Route SUM or AVG outputs into effects like ring mods, wavefolders, or direct into audio paths for noisy, atonal hits.

### Example Patch:
1. **Output 1** → VCA CV IN (controlling percussion oscillator).
2. **AVG MIX OUTPUT** → Feedback CV of a distortion unit for pseudo-dynamic drive.
3. **Random Trigger IN (Expansion)** → Envelope 2, to vary timbre for each hit.

---

## 2. **Crazy Basslines (Dubstep/Drum & Bass Style)**

For modulated, moving basslines with unpredictable contours:

### Settings & Patching Tips

- **Loop Mode:** Set envelope(s) to self-loop for LFO-style modulation.
- **Randomization:** Use RISE/FALL min/max to define a playable range for wubs and growls.
- **Curve Morphing:** Use LIN for precise timing, LOG toward more organic growl/boom.
- **Amplitude Automation:** Patch envelope CV outs to a filter cutoff, wavefolder, or drive, and sweep amplitude ranges (-10V to +10V).
- **CV Over Everything:** Patch sequencer lanes or other LFOs into the min/max CV inputs to create stepped/randomized modulation patterns for riser/faller times.
- **Slew Mode:** Use SLEW instead of TRIGGER to have the channel follow crazy, wobbly CV shapes for bass movement. Input unpredictable, stepped CV for the SLEW to process.
- **Sum/Average Output:** Route the AVG OUT or SUM OUT to deeper bass effect chains to glue the envelopes into a 'super modulator'.

### Example Patch:
1. **Envelope 3 (looped, randomized) output** → Low-pass filter cutoff on a bass voice.
2. **Random CV OUT (Expansion, set to RISE)** → FM depth input of the bass oscillator.
3. **EOR/EOF OUT (set to gate)** → Clock divider/reset to poke sequencer timing off-kilter.

---

## 3. **Haunting Atmospheric Pads**

For evolving, eerie, or haunting pads and textures:

### Settings & Patching Tips

- **Long Rise/Fall Times:** Set RISE and FALL min/max to high/long values, allowing envelopes to drift and swell.
- **Random Variation:** Enable random triggers (manually or via external source) to make pad animation unpredictable.
- **Lock/Unlock Channels:** Work on one channel at a time, lock when satisfied for evolving but controlled complexity.
- **Morph Curves:** Sweep from LIN to LOG/EXP for swelling, organic shapes.
- **Amplitude & Offset:** Use positive/negative offset to keep envelopes in desired modulation region.
- **Mixing Magic:** SUM or AVG OUT to modulate the navel of your reverb or phaser for swirling clouds.
- **Complex Modulation:** Feed slow-moving envelopes to spectral processors, filterbanks, or pitch shifters for time-warping effects.

### Example Patch:
1. **Envelope 1 OUT** → Reverb wet/dry CV input on a pad chain.
2. **Envelope 2 OUT (different random time)** → Modulate a phaser, chorus, or granular window shape.
3. **SUM OUT** → Control feedback of delay, or amount of shimmer/harmonizer.
4. **Random TRIG Input** → Occasionally re-randomize the movement for non-repetitive swells.

---

## Advanced Tricks

- **EOR/EOF as Triggers:** Use these to sequence or randomize events elsewhere—clocking shift registers, switching audio paths, etc.
- **Cross-Modulate Rise/Fall Times:** Use the output of one channel (or SUM/AVG) into the min/max CV in of another channel for chained, non-linear rhythms.
- **In the Audio Path:** For extreme digital distortion, try running the envelope or sum output directly into a wavefolder, FM input, or audio VCA.

---

## Further Reading

For reference, download the full [ADDAC506 VC Stochastic Function Generator & Expansion Manual PDF](https://media.addacsystem.com/files/ADDAC506_Manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)