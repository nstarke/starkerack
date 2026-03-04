# Cute Lab — Mom Jeans

- [Manual PDF](../../manuals/mom-jeans-manual-rev1-1.pdf)

---

[Mom Jeans Manual PDF](sandbox:/mnt/data/Mom_Jeans_Manual_Rev1.1.pdf)

---

# Using Mom Jeans for Densely Rhythmic & Hyper-Complex Percussion in Eurorack

The **Mom Jeans** module by CuteLab is uniquely qualified for creating percussive, polymetric, and complex rhythmic material thanks to its **pulsar synthesis engine** and **granular/grain-width** controls. It’s not just a new oscillator—it's a digital percussion and rhythm generation powerhouse. Here’s how to maximize it for advanced rhythmic and polyrhythmic sequences.

## 1. **Exploit the Density Parameter for Percussive Transients**

- **Density** (Knob & CV, #3/#4):  
  Highly percussive, clicky, and stuttering effects can be achieved by setting density to extreme values. Try modulating density at audio or CV rates for rapid-fire transient creation—a key technique for glitchy or “granular drum” sounds.

- **Patch Idea**: Use a trigger sequencer or stepped random CV to the **Density input**. Each change can shift the “grain width,” creating new transient shapes and giving every attack a unique percussive character.

## 2. **Modulate Cadence and Torque for Rhythmic Complexity**

- **Cadence** (Knob & CV, #6/#11):  
  Cadence is the internal modulation LFO’s rate. Use CV to clock it in and out of sync with your master tempo for polyrhythms and shifting accents.

- **Torque** (Knob & CV, #7/#12):  
  This controls the amplitude of grain-width modulation (think: internal PWM depth). Wild swings in torque can push grains to overlap or vanish, creating silence, bursts, and complex pulses.

- **Polyrhythmic Patch**:  
  Use rhythmic CV or stepped voltage sequences into **Cadence** and/or **Torque**. Try sending different clocks or Euclidean triggers for evolving patterns.

## 3. **Engage Coupling & Quantization for Time Division Magic**

- **Coupling** (Toggle #8):  
  When active, cadence is locked to integer multiples/divisions of the oscillator frequency. This keeps rhythmic modulation “in time” with the voice pitch—great for cyclical patterns tied to tempo or note value, including odd divisions for polyrhythms.

- **Quantization** (Toggle #9):  
  Makes cadence discrete, so modulations occur as rhythmic “steps.” This is exceptional for stepping through complex patterns:
    - Cycle through rhythmic “ratchets” (2, 3, 5, 7, etc.) by automating Cadence with quantization ON for rapid time signature flips.

- **Patch Concept**:  
  Turn on **Coupling and Quantization**, then sweep the **Cadence** knob or modulate by stepped CV (sequencer or random). This creates sharply-defined, mathematically “tight” rhythmic patterns—ideal for algorithmic percussion or IDM grooves.

## 4. **Leverage the Pulsar Output for Bright, Detailed Transients**

- **Pulsar Output** (#19):  
  This output delivers the rich, harmonically complex result of all your modulation—send it to gate a VCA with an external envelope or mult into filters/further processors for evolving percussive textures.

- **Layering**:  
  Mult the **square output** (#18) into a drum module’s trigger input and the **pulsar out** into a VCA for gritty or “dirty” accents that reinforce your percussive voices.

## 5. **Complex Timing with Sync Input**

- Sync Input (#17):  
  Use gates, triggers, or audio-rate clocks to forcibly reset the pulsar engine. Try clocking it with non-4/4 clocks (triplets, 5s, 7s), for instant polymetric mayhem.

## 6. **Experimental Tips**

- **Self-Patching**:  
  Patch processed audio from the Pulsar output back into any CV input (Density, Shape, Cadence) for unpredictable, feedback-driven rhythmic complexity.

- **External Sequencer Control**:  
  Sequence pitch, density, cadence, and torque simultaneously to “play” the Mom Jeans like a percussionist, treating each step of a sequence as a new “drum hit” with variable timbre and rhythm.

- **External Modulation**:  
  Use random, Lorenz attractor, or Turing Machine outputs to any combination of modulation ins for long-evolving, pseudo-random percussion.

---

## **Polyrhythmic Patch Example**

1. Patch a stepped random or clock divider into **Cadence CV**.
2. Modulate **Density** with another clocked CV; set Density midway for both grain and gap emphasis.
3. Enable **Coupling** for rhythmic lock or disable for unpredictable timing.
4. Snap **Quantization** ON for hard-edged, stepped metric modulation.
5. Mult **Pulsar Out** and **Square Out** to various percussion VCAs or samplers.

Result: **Evolving, clock-synced, polymetric digital percussion with chaotic and algorithmic subdivisions.**

---

For further patch ideas, consult the examples in the manual’s last pages!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)