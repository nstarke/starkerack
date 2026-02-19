# Doepfer — A-119

- [Manual PDF](../../manuals/A119_man.pdf)

---

[Doepfer A-119 Ext. Input / Envelope Follower Manual (PDF)](https://doepfer.de/a100man/A119_man.pdf)

---

# Using the Doepfer A-119 for Hyper-Complex, Densely Rhythmic Percussion in Modular Synthesis

The Doepfer A-119 Ext. Input / Envelope Follower is not a voice or effect in itself, but is a crucial utility module for extracting rhythmic, amplitude-following control voltages and gate signals from external audio. Mastering this module opens creative doors for inserting polyrhythmic, complex, and percussive patterns into your modular system by making external sources or even internal signals interact rhythmically with your patch.

## Core Functions for Rhythm Complexity

### 1. Envelope Follower as Rhythmic CV Source
- **What it does:** Converts the amplitude envelope of external audio (like drum machines, loops, or live percussion/mic signals) into a proportional control voltage.
- **Applications:**
  - **Triggering Modulators:** Use this output to control parameters on VCAs, filters, quantizers, or even sequencer clocks. If your external audio has a complex rhythm (e.g., an odd-meter drum loop), any A-100 parameter you attach the envelope out to inherits that rhythm.
  - **Dynamic Modulation:** Route the envelope out to modulate decay/release times, filter cutoff, or waveshaper parameters on percussion voices for evolving, organic patterns.

### 2. Gate Extraction for Complex Triggering
- **What it does:** Produces a gate whenever the input signal exceeds the manual threshold (set via “Thres.”).
- **Applications:**
  - **Triggering Envelopes:** Sync envelope triggers to transient events in external material, even if they’re irregular or polyrhythmic.
  - **Patch Polyrhythms:** Feed different rhythmic loops or live input to several A-119s to extract gates from each, and trigger different percussion voices in your rack. Layering odd/subdivided loops creates inherently polyrhythmic trigger patterns.
  - **Complicated Clocking:** Use multiple A-119s’ gate outs as asynchronous clocks for sequencers, Turing Machines, or logic modules.

## Patch Techniques for Dense Rhythmic and Percussive Results

### A. Polyrhythmic Percussive Gating
1. **Setup:**
    - Send two separate external audio sources with different meters or rhythmic feels to two A-119s.
    - Use each Gate Out to trigger different drum voices or envelope generators.
2. **Result:** Your percussion voices will be triggered in complex, always-changing relationship to each other, producing polyrhythms.

### B. Rhythmic CV Layering
1. **Setup:**
    - Patch Envelope Out of the A-119 to a VCA controlling a percussive sound.
    - Patch the same Envelope Out to modulate filter cutoff or waveshaper—the contour of incoming audio directly sculpts the percussive sound’s timbre.
2. **Result:** Percussive timbres that are dynamically shaped by the input’s rhythm—perfect for unpredictable, evolving rhythms and textures.

### C. Beat Extraction From Chaos
- Feed in non-musical sources (spoken word, field recordings, analog noise textures) and use the Envelope Follower and Gate for glitchy, irregular percussion triggers. Invert or process these CV signals (with Slew, logic, or random generators) for even stranger results.

### D. Advanced Ducking Groove
- Use the Envelope Out to sidechain-compress or modulate other mix elements, ducking ambient or melodic elements whenever the percussive source is active—tightening the groove and creating syncopated “pump” effects.

### E. Microdynamic Percussion Accent Generator
- Set threshold low and gain high on the A-119, send in heavily syncopated material, and use the Envelope Out for fast, sharp CV curves to modulate multiple percussion or noise voices.

---

## Making the Percussive Result Unique, Punchy, and Complex

- **Shape the Envelope:** Add a Slew Limiter (like Doepfer A-170) to add lag and further sculpt complexity, making gates “softer” or deliberately offset.
- **Mix and Layer:** Combine several A-119-modulated percussion voices for dense layers.
- **Invert/Process CV:** Use attenuverters, comparators, logic, or CV delays to add unpredictable elements, offsetting or randomizing rhythmic accents.
- **Threshold Tricks:** Ride the “Thres.” control live or automate it with CV (patch through a VCA or voltage processor) for evolving gate sensitivity.

---

## Tips for Densely Rhythmic, Polyrhythmic Modular Percussion

- **Extract rhythm from anything:** Any source—from modular drums to DAW breakbeats, acoustic instruments, or found sound—can be a clock or accent with the A-119.
- **Multiple A-119s:** Consider using several in parallel for ultimate polycomplexity.
- **Live Manipulation:** Twist gain/threshold knobs in real time to shift which signals are accentuated or gated—real time feel!
- **Creative Sidechain:** Use envelope or gate to control other elements’ volume, pitch, or effects for tightly woven rhythmic interplay.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)