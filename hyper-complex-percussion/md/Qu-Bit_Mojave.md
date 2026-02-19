# Qu-Bit — Mojave

- [Manual PDF](../../manuals/mojave_getting_started.pdf)

---

[Download the Qu-Bit Mojave Manual PDF](https://qubitelectronix.com/static/media/Mojave_Quickstart_v1.0.9b7ab70ae2ede6e8a8e5.pdf)

---

# Using Qu-Bit Mojave for Hyper-Complex Percussion & Dense Rhythmic Music

**Mojave** is a live granular processor, ideal for granularizing audio and creating intricate sonic textures. While it's not a traditional drum voice, its granular approach and advanced modulation options make it powerful for experimental, percussive, and rhythmically dense music.

Below are strategies and patch ideas to help you achieve hyper-complex percussion sequences, polyrhythms, and advanced patterns using Mojave:

---

## 1. **Utilize External Clock/Gate Inputs for Polyrhythms**

- **Tap/Clock Input:**  
  Use this to clock Mojave with external modular sources. Patch multiple unrelated rhythmic sources (e.g., from different sequencers, clock dividers, Euclidian generators, or random gates) to the clock and **Gen** input for layered, offset grain triggers.
- **Gen Input:**  
  Fire grains at unpredictable or offset times. Use a second sequencer or random gate pattern for further complexity.
- **Polyrhythm Patch Example:**  
  - Send a 5-step Euclidean rhythm into **Tap/Clock**.
  - Send a 7-step trigger sequence into **Gen**.
  - Result: Dense polyrhythmic showers of grains.

---

## 2. **Leverage the Distribute, Drift, and Whirl Controls**

- **Distribute (Stochastic Rhythmic Displacement):**  
  Crank this knob and/or modulate with a complex LFO or stepped random CV. This scrambles grain timing for glitchy, ratcheted, and off-grid patterns, crucial for hyper-complex timing and nested rhythms.
- **Drift (Random Audio Buffer Position):**  
  Increase for more randomness in grain selection—useful for "shuffling" percussive micro-samples.
- **Whirl (Spatial Displacement):**  
  Modulate for dynamic stereo panning, making percussive events pop across the soundstage.

---

## 3. **Complex Buffer Scrubbing and Percussive Grain Generation**

- **Zone (Audio Buffer Position) + Size (Playback Direction & Reverse):**  
  Rapidly modulate **Zone** with stepped or random CV to jump through different chunks of audio.  
  Use **Size**'s left-of-center setting for reversed grains—sharp, snappy reversed percussive hits.
- **Speed (Pitch / 1V/Oct):**  
  Sequence or modulate with a quantizer or random source to create pitched percussion and chopped, tuned bursts.

---

## 4. **Evolving, Algorithmic Patterns with Structure**

- **Structure (Algorithmic Melodic/Harmonic Displacement):**  
  Modulate or sequence for percussive arpeggios—or to "shift" grain clusters into unique tonal rhythms.

---

## 5. **Creative Freezing, Locking, and Buffer Techniques**

- **Freeze:**  
  Engage to loop and stutter grains rhythmically. Insert triggers via the Freeze input for in-time or off-grid repetition bursts.
- **Lock:**  
  "Lock" complex, evolving input audio, then sweep **Zone** and modulate **Size**/**Speed** for repeated, developable percussive patterns.

---

## 6. **Percussive Grain Design: Grain Envelope, Feedback, and Reverb**

- **Window:**  
  Select sharper grain envelopes for punchy, clicky sounds.
- **Gust (Feedback/Reverb):**  
  Feedback can make grains more aggressive, reverb adds space. Automate with CV for dynamic character.
- **Input Material:**  
  Feed Mojave with percussion samples, drum machines, FM synth hits, field recordings, or even dry clicks for source material.

---

## 7. **Dynamic CV Routing and Macro Control with Sky Modes**

- **Sky Modes:**  
  Use **Twilight** (all macro controls fully unquantized) for maximal freedom. But, for organized polyrhythms or modal constraints, use **Dusk** (chromatic) or **Dawn**/**Day** (major/minor) according to desired grid complexity.
- **Narwhal Web App:**  
  Customize macro behaviors for even more experimental rhythmic generation.

---

## 8. **Advanced: Dune Output as Algorithmic Modulator**

- Use the **Dune CV Output** as a modulation source for external percussion modules or sequencers. The output is derived from Mojave’s environmental conditions—create true feedback by patching this into pitch, decay, or timbre controls elsewhere.

---

### Example Patch Recipe

1. **Basic Patch:**
   - Input a complex drum loop or percussive sample.
   - Send steady or polyrhythmic gate to Clock input; random gates to Gen for spontaneous grains.
   - Distribute, Drift, Whirl all modulated by different LFOs or stepped random voltages.
   - Zone sequenced with a gate sequencer offset from the main Clock for buffer scrubbing.

2. **Percussive Texturizer:**
   - Sample a dry click or rimshot.
   - Set short grain size, sharp envelope (Window knob).
   - Feedback up for snap; Freeze engaged with timed triggers for complex, rhythmic echoes.

---

### Tips for Unique and Punchy Percussion

- **Use the onboard mic** to inject real-world, percussive transients and process them instantly.
- **Modulate multiple parameters** simultaneously (Distribute, Structure, Size, Speed) for evolving timbral and rhythmic density.
- **Combine multiple Mojaves** or use external granular/FX processors in series for super dense granular flurries.

---

## **References**

- [Qu-Bit Mojave Manual PDF](https://qubitelectronix.com/static/media/Mojave_Quickstart_v1.0.9b7ab70ae2ede6e8a8e5.pdf)
- [Narwhal Configurator (Qu-Bit)](https://narwhal.qubitelectronix.com/)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)