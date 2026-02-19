# Acid Rain — Constellation

- [Manual PDF](../../manuals/Constellation_Manual_Firmware_1.1_4.7.2025.pdf)

---

[Download the Constellation Firmware V1.1 Manual (PDF)](attachment:/Constellation_Firmware_V1.1.pdf)

---

# Using Constellation for Hyper-Complex Percussive Rhythms

Constellation is not a sound generator or percussive voice, but a sophisticated, 8-channel rhythmic pattern/gate/trigger generator. It’s one of the most powerful ways to trigger drum, percussion, or modulation events in extremely rich, polyrhythmic, and non-repetitive ways. It excels at dense, complex rhythmic architectures useful for both “mathematical” rhythm and intense club-oriented percussion sequences.

Below are strategies and creative approaches for deploying Constellation to make hyper-complex, unique, and evolving percussive patterns using polyrhythms and exotic time signatures.

---

## 1. **Exploit True Polyrhythms and Polymeters**

- **Separate Clock Ratios per Channel:**  
  Use the per-channel clock **divide** and **ratchet** settings from the main clock menu (p. 18–19) to put different channels (e.g., kick, snare, hats, etc.) on unrelated clock grids.  
  - *Example:* Set Channel 1 to 5 divisions per cycle, Channel 2 to 7, Channel 3 to 13—these are relatively prime and syncopate against each other for long, evolving cycles.
- **Pattern Length Independence:**  
  Set the length and events for each pattern within a channel to different values—even prime numbers or odd/irregular lengths—to create complex, never-repeating sequences (p. 16).
- **Channel Rotation (Microtiming):**  
  Use the **rotate** function in channel clocks to nudge patterns off the grid for microtiming and shuffle.

---

## 2. **Dense, Evolving Percussion via Euclidean Layering**

- **Eight Mutable Patterns per Channel:**  
  Layer dense “core” patterns with sparse fills/bursts within each of the 8 patterns per channel. Use **mute** and **chance** (probability) to selectively bring them in and out for undeviating evolution (p. 21).
- **Ratchets & Bursts:**  
  Using high **ratchet** or **burst** values, you can get densely packed rolls/flams on selected hits—good for rimshots, hats, glitch percussion, or IDM rolls.
- **Event Rotation:**  
  Rotate patterns for offbeat “feels” or to scatter events throughout less predictable step positions.

---

## 3. **Advanced Logic for Sonic Density/Shifts**

- **Channel Logic Modes (AND, OR, XOR):**  
  With the logic section (p. 17), combine patterns using:
    - **OR:** For maximal density—any pattern produces a hit.
    - **AND:** For only intersections—rare/jointed hits for steady grooves.
    - **XOR:** For intricate, flip-flop gating, especially when multiple patterns overlap.
- **Flip-Flop Outputs:**  
  Turn on the per-channel **flop** for gate patterns (p. 10). This creates gates of variable length directly from the interaction pattern spacing, perfect for syncopations and pseudo-random groove-gates.

---

## 4. **Extreme Groove Design with Modulation and CV**

- **Freely Assignable CV (8 Inputs):**  
  Assign slow or stepped voltages, random voltages, or synced modulation (e.g., from LFOs or voltage sequencers) to pattern parameters—length, events, rotate, burst, ratchet, chance (p. 24–25).
    - *Pro move:* Modulate **chance** with a stepped or random LFO for polymorphic “fills.”
    - Assign the same CV source to multiple parameters or patterns for correlated movement.
    - Set up CV control over **mute** or **width** for dynamic channel activity or pulse length macro control.
- **Assign CV to “Load” for Generative Pattern Changes:**  
  Use gates to CV-switch between save slots for live rearrangement or algorithmic “song” mutation.
- **Quick Randomization:**  
  Use the random button for on-the-fly mutation of parameters (especially fun if assigned to input triggers for “controlled chaos”).

---

## 5. **Expanding Complexity**

- **Pattern and Channel Mutes:**  
  Use the mute menu live (or with CV assigment) to bring in/out whole patterns or layers on the fly for dramatic breakdowns/builds.
- **Saving/Recalling Structures:**  
  Design evolving “scenes” across save banks and use the live mode to instantly swap entire kits, polyrhythm layouts, or muting states—either manually or with CV.

---

## 6. **Tips for Maximum Punchy Percussion**

- **Use Tight Pulse Widths for Triggers:**  
  Set channel width narrow for punchy trigger outs; widen for creative gates.
- **Clock Swing:**  
  The internal clock has swing (p. 18); use this when you want shuffled, groove-heavy complex patterns.
- **Asymmetrical Channel Delays:**  
  Apply per-channel output delays for microtiming and inter-channel groove.

---

## **Hardware Integration and Patch Ideas**

- **Multimode Drums:**  
  Output channels to various drum modules—each voice (kick, snare, hats, percussion, digital sound) receives its own unique or layered rhythmic stream.
- **Generative Melodic/Modulation Triggers:**  
  Use as clock/gate for chaotic sequenced CV quantizers, random voltage modules, logic processors, or stepped mod sources in a generative patch.
- **Layered Physical Models:**  
  Fire multi-channel percussive voices (e.g., physical modeling, resonators) with nonaligned, bursty, evolving triggers for machine-like grooves or organic “drum circle” densities.

---

## **Summary**

Constellation is a rhythm architect's dream for Eurorack. By leveraging its pattern independence, complex logic, and intense modulation mapping, you can make dense, evolving polyrhythms and percussion lines that reach complexity unreachable with ordinary sequencers.

*Pro tip: Start simple—just two or three channels with coprime lengths and playful chance/burst/ratchet. As you gain familiarity, keep introducing more layers, CV modulations, logic, and channel delays for true rhythmic hypercomplexity.*

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)