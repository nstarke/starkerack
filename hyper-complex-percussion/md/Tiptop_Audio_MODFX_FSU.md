# Tiptop Audio — MODFX FSU

- [Manual PDF](../../manuals/Tiptop_Audio_fx_manual_MODFX_FSU.pdf)

---

[Tiptop Audio MODFX & FSU Manual PDF](https://tiptopaudio.com/manuals/FSU-MODFX-Manual.pdf)

---

# Using Tiptop Audio MODFX & FSU for Hyper-Complex Percussive Rhythms

## Overview

Tiptop Audio’s **MODFX** and **FSU** are multi-algorithm stereo effects modules designed for deep creative manipulation of audio signals. While not sound sources themselves, their real-time modulation, dynamic CV control, and unique effect algorithms are **extremely powerful tools** to intensify, skew, and generative-complexify percussion and rhythm sources in your eurorack system.

Let’s break down approaches to use both modules to accomplish your goal: **densely rhythmic, hyper-complex, polyrhythmic percussion sequences.**

---

## Core Strategies

### 1. **Clock & CV as Rhythmic Modulators**
- **Clock Inputs**: Both modules allow for **analog clocking of DSP**. Patch rhythmic clock/LFO/gate sources (especially ones generating polymetric or non-standard patterns) to the clock or CV inputs to sync effect parameters to your percussion’s groove.
- **CV Control**: Patch highly rhythmic CV (from sequencers, Euclidean/Burst generators, or random stepped sources) to the DSP parameters (Rate, Depth, Filter/Feedback) to drive **modulation rates, effect sweep depths, and filter feedback** in time with your polyrhythms.

### 2. **MODFX for Dynamic Percussion Processing**
Choose programs that accentuate movement, spatialization, and spectral animation. Manipulate these in a rhythmic and percussive context:

#### *CHORUS/FLANGER/PHASER for Animated Rhythm*
- **Tri Stereo Chorus/Random Chorus 4 Voice**: Apply to percussive loops for swirling, moving width. Modulate Rate/Depth with rhythm to create constantly shifting texture, emphasizing downbeats/offbeats as the stereo movement ‘swings’.
- **Dual Vibrato/Diffuse Chorus**: Use extreme Depth, then rapidly modulate Rate with stepped/triggered CV for wild tape-flutter or granular effects on drums.
- **Tape Filter/Many 1 Pole**: Drive the cutoff with stepped sequences or polyrhythmic envelopes to create stuttering, wah-like sweeps over the high frequencies of percussion.

#### *FLANGER as Percussive Resonator*
- **Short Karplus/Chord Resonator**: Patch short/noisy percussion hits as input. Use CV to trigger changes in Filter/Depth (feedback and tuning), turning each hit into a different metallic/resonant timbre. Sequence parameter changes to lock to odd meters or pulse divisions.
- **Thru Zero Flanger**: Set effect 100% wet, then “play” the Rate with triggers—instant tape-flange-drum stabs.

### 3. **FSU for Glitch, Granular, and Destructive Percussion**
The FSU’s banks (Distort, Glitch/Warp, Sound on Sound) radically re-interpret audio. Here’s how to wrangle them into rhythmic intensity:

#### *Glitch/Warp for Timbral Polyrhythms*
- **Glitch Pitch/Varispeed Grains/Random Grain**: Patch percussion through these, and tempo-sync the Rate/Gain to polyrhythmic triggers or stepped random outputs. Use Depth to make granules jump further, causing unpredictable, rhythmically mangled stutters and clips.
- **Many Head Pitch Feedback**: This creates rhythmically complex delays with shifting pitches—great for percussive echoes that never quite repeat. Modulate tap fade Rate/Depth with Euclidean or polyrhythmic clocks.

#### *Distort for Percussive Bite*
- **Ring Mod, Rectifier, Bit Crusher**: Gate or rhythmically CV-modulate the Drive/Depth controls with complex sequences, so the effect intensity hits only on select beats, odd-numbered steps, or tuplet divisions in your pattern.
- **Dual Frequency Shifter**: Patch the output of two complementary drum parts (e.g., kick and snare) through the Left and Right inputs, and automate the shift parameters with clocked or manually played CV wriggles for evolving metallic rhythm tones.

#### *Sound on Sound for Live Rhythmic Loops*
- **Dual Head/Dual Pitch/Panning Heads**: Use envelopes or rhythmic gates to record micro-percussive hits into the buffer. Play back with different head rates/positions, modulated (via sequencers or LFOs) to create chopped, offset polyrhythm loops. The buffer-degrade options let you decay layers for constantly evolving glitch textures.

---

## Example Patch Concepts

### **A. Kinetic Polyrhythmic Drum Loop Enhancer**
- Patch **drum mix** into MODFX set to 'Quad Bandpass LFO'.
- Sequence Rate and Depth with two unsynced (or polyrhythmically related) CV LFOs or clock dividers.
- Modulate the filter Q with a third stepped or random sequence.
- Result: Constantly morphing, notch/pulse-modulated percussion—never the same pulse twice.

### **B. Hyper-Destructive glitch beat**
- Drum input → FSU ‘Glitch Pitch’ or ‘Random Grain’.
- Use a trigger sequencer with weird divisions (like 7, 11, 13-step patterns) to control the Rate/Depth CVs.
- Output is rhythmically shattered, with abrupt pitch jumps/slips—ideal for experimental genres.

### **C. Resonant Metal Percussion**
- Pulse or noise bursts → MODFX 'Chord Resonator'.
- Modulate Rate/Depth with fast step CV to ‘strike’ different chord intervals and resonance amounts per drum hit.

### **D. Live Looping Time-Stretch Polyrhythm**
- Percussion → FSU 'Dual Pitch' looper.
- Record short sequences using an envelope on Gain (from drum triggers).
- Sequence Filter/Depth with two slow LFOs at different, non-matching divisions for “beat-cycling” time stretches.

---

## General Percussive Enhancement Tips

- **Hard CV modulation:** Use stepped voltages, random sources, or gate+S&H CV to change parameters sharply in time with percussion hits—this creates punchy, per-step variation.
- **Dynamic Mix:** Sometimes keep wet/dry at 50/50 so original hits cut through but are joined by complex effect tails/percussive ambience.
- **CV Multing:** Split your main clock or accent triggers to both your drum sequencer and MODFX/FSU’s CV ins for tempo-locked effect changes.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)