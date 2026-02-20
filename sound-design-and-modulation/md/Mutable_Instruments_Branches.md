# Mutable Instruments — Branches

- [Manual PDF](../../manuals/branches_quickstart.pdf)

---

[Branches Dual Bernoulli Gate – Official Manual PDF](https://mutable-instruments.net/modules/branches/manual)

---

# Creative Modulation Strategies for Mutable Instruments Branches

As a Eurorack musician focused on percussive, bass-heavy, and atmospheric sound design, Mutable Instruments Branches offers a unique utility for injecting controlled randomness and dynamic switch-based motion into your patch. Here are some ways to leverage its features for maximum creative impact:

---

## Overview of Modulation Options

Branches is a **dual Bernoulli gate**—it takes a trigger/gate signal and probabilistically routes it to one of two outputs. Key features for modulation:
- **Probability knob (and CV input)**: Sets/randomizes the odds of where each trigger lands.
- **Toggle Mode**: Remembers previous state, sending triggers in toggling sequence.
- **Latch Mode**: Output stays at +5V until another output is triggered.

---

## Applications

### 1. **Distorted Percussive Sounds**

- **Patch model:** Branches splits/distracts rhythm sources (**kick/snare triggers**, Euclidean patterns, more).
- **How to modulate:**  
    - **CV Modulate the probability input** with fast LFOs, random S&H voltages, envelopes from your percussion voices for instantaneously shifting rhythms.
    - Use **Toggle or Latch mode** to create varied, choking, or gated triggers for drum modules, making grooves unpredictable and heavily syncopated.
    - Feed Branches output(s) to a **distortion or wavefolder** after a drum module – rapid, random switching creates ‘glitchy’, tearing percussive effects.

#### Example Patch:
- **Kick trigger to Branches IN.**  
- **Set probability to 50%.**  
- **CV in from an envelope or random module.**  
- **Outputs to two different percussion modules or one drum sound and a noise source.**  
- Run final audio to a distortion unit for harsh, broken-up percussion.

---

### 2. **Crazy Basslines (Dubstep/Drum & Bass)**

- **Patch model:** Use Branches to randomly or periodically switch **between bassline patterns, wavetables, filter modulations, or envelopes.**
- **How to modulate:**  
    - Use a popcorn LFO or rhythmic random CV to the **probability CV input** to switch between classic reese bass and growl patches, or dual filter/folder chains.  
    - In **toggle mode**, use a repeating gate/clock so the bassline alternates between two different modulation destinations (such as two synced complex oscillators or filter cutoff voltages).
- **Trigger re-triggers, sample holds, or envelope re-firings** for weird syncopated movement.

#### Example Patch:
- **Sequencer triggers to Branches IN.**
- **Outputs control two different bass voices (i.e., clean and dirty).**  
- **Random or clocked CV to probability input.**  
- **Modulate ‘which bass’ with envelope followers from your main drum hits.**  

---

### 3. **Haunting Atmospheric Pads**

- **Patch model:** Branches provides semi-random gates to activate/dampen modulations or send CV to effects, filters, or VCA chains for pads.
- **How to modulate:**  
    - Use very slow LFO or gentle, attenuated random voltage on probability CV in: produces shifting, unpredictable movement between outputs.
    - In **Latch mode**, create sustained, droning gate states that change only with new triggers—drives slow fade-ins/outs on reverb, delay, or granular parameters.
    - Gate pads’ modulations **between two reverbs or FX sends**, randomly accenting different portions of the stereo field or wet/dry amount.

#### Example Patch:
- **Slow clock or enveloped pad gate to Branches IN.**  
- **Outputs to two VCA/FX send paths:** one dry, one through intense reverb/lush chorus.
- **CV input from slow LFO.**
- **Latch mode ON:** one reverb washes in, another fades out, pads morph unpredictably for organic/ghostly ambience.

---

## Tips for Further Exploration

- **Stack multiple Branches modules** to create multi-layered decision trees for incredibly complex, probabilistic patches.
- **Volatile Performances**: Use manual toggle/latch switching in live performance to warp between order and chaos.
- **Non-audio signals**: Branches is not just for gates—use to steer modulation sources (clock, random, LFO triggers) for maximum surprise.

---

## Useful Links

- [Branches Dual Bernoulli Gate – Official Manual PDF](https://mutable-instruments.net/modules/branches/manual)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---