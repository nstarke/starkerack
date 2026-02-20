# Shakmat — Time Wizard

- [Manual PDF](../../manuals/TW-User_Manual.pdf)

---

[Download the Shakmat Time Wizard Manual (PDF)](https://shakmat.com/manuals/time_wizard_manual.pdf)

---

# Creative Sound Design With the Shakmat Time Wizard

As a Eurorack modular synthesist, the **Shakmat Time Wizard** can become a potent generative clock modulator in your rack, especially for percussive distortion, bass movement, and haunting pads. Here’s how you can creatively modulate it for those sound palettes:

---

## 1. Distorted Percussive Sounds

### **Random Ratcheting & Poly-Rhythms**
- Use the _Multiply A switch_ (A) to set A1, A2, or A3 to unusual divisions/multiplications (like x3, x4, or 3/7). This will “decompose” your main clock signal into odd patterns, perfect for unpredictable, jagged hats and glitchy percussion.
- Deploy two or more outputs to trigger drum modules (kicks, snares, hats), then patch a divider output (e.g., A2 or B3) through a distortion or wavefolder module downstream.
- Flip the _Clock B switch_ (B) so B5/B6 runs at independent clocks—a great way to have a snare on a totally different groove.

### **Half-Period Gates for Drum Accents**
- Enable the **half period gates jumper** (see manual), so B5 & B6 outputs deliver longer gates rather than triggers. Use this to fire envelope followers that control VCAs, saturators, or bitcrushers for thick, distorted drums.

---

## 2. Crazy, Syncopated Basslines (Dubstep/DnB)

### **Clock-Move Basslines**
- Clock a sequencer running your bass voice from one of the divided or weirdly-multiplied outputs (like A3 set to 7, or only firing on “OR” combinations from the _Logic A2 switch_ (C)). This lets basslines break free of simple 4/4 sync and introduces non-linear groove shifts.
- Mult your main clock, but apply different divide/multi scalings to A and B columns; then, on every reset, the pattern will “shift” forward, creating rolling, evolving bass line syncopation.

### **Rhythmic Bass Modulation**
- Use the _Logic A2 switch_ to combine clock signals—set to “A2 and B5” or “A2 or A3”—and patch its output into the clock/reset of an envelope generator, or modulate a filter/LFO. Each time a logical AND/OR is true, your modulation cycle triggers, resulting in unexpected, complex bass movement.

---

## 3. Haunting Atmospheric Pads

### **Slow, Evolving Gates**
- Use the highest division factors (e.g., set A1, B2, and B3 to high values: 16, 32, etc.) and combine multiple gate outputs to open LPGs or long-attack EGs on drone and pad oscillators. The _Reset B6_ (D) switch lets you periodically reset or re-sync everything, causing lush, phasing pad events.

### **Intermittent Layer Triggering**
- Patch several divider outputs to various melodic/ambient events (sample players, granular engines, long reverb tails). Each divider can be set to a mathematically distinct pattern so the pad layers phase in and out of each other, creating a meditative or “haunted” feel.
- Use the _half period gate mode_ for dividers B5 and B6 to open reverb/delay sends during select stretches of your generative pad textures.

### **Haunted, Glitchy Clocked FX**
- Use the _Multiply A_ and _Logic A2_ switches to drive random S&H circuits or clocked modulation of effects—so your reverb shimmer, pitch delay, or granular freeze only happen on specially “magicked” clock events.

---

## **Patch Tips & Further Modulation**

- Cross-modulate clocks: Use other sequencers/LFOs/arpeggiators into the Time Wizard’s _Clock or Reset inputs_ for evolving mayhem.
- Self-patch logic outs into reset inputs for self-generating patterns.
- Stack outputs (using OR combiners) for chained rhythmic events.
- Pair with a distortion, waveshaper, or LPG downstream for maximal impact.

---

**Experiment with switch settings and divider factors live—every combination yields a unique rhythmic landscape!**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)