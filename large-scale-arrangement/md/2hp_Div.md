# 2hp — Div

- [Manual PDF](../../manuals/Div_Manual.pdf)

---

[2hp Div Manual (PDF)](https://2hp.com/docs/div_manual.pdf)

---

# Creating Full-Length Songs with 2hp Div in Eurorack

One of the biggest hurdles in modular synthesis is transforming captivating modular jams into structured, evolving full-length songs. The **2hp Div** is a compact but powerful clock divider/multiplier that, when combined with other modules, is ideal not only for complex rhythms but also for bringing compositional structure and variation to your patches.

## What 2hp Div Does (Key Capabilities)

- Two independent clock division/multiplication channels (per channel: divide or multiply by 1, 2, 3, 4, 5, 6, 7, 8, or 16).
- CV control over clock rate allows for external modulation/sequencing of divisions/multiplications.
- Allows you to extract or generate multiple rhythmic layers from a single clock for different parts of your patch.

---

## Strategies to Structure a Full Song

### 1. **Multi-Part Song Sections with Clock Manipulation**
Use Div to create different rhythmic clocks that you can switch or morph between over time to simulate "arrangements" or "sections" in a song.
- **Patch Example:**  
  - Master clock → Div IN.  
  - OUT 1 (e.g. divided by 4) → Trigger drums.  
  - OUT 2 (e.g. multiplied by 3) → Trigger envelope for arpeggios or melodic sequencer.
- **How to Transition:**  
  - Modulate RATE knob or send CV from a sequencer or voltage recorder (like Befaco VC ADSR, Voltage Block, or Planar Joystick) to smoothly morph between divisions/multiplications over the course of the track.  
  - Use precision adders or sequenced voltage sources to automate when Div switches clock divisions (e.g., more open "chorus," tighter "verse," breakdowns at /16 or *16).

### 2. **Polyrhythms and Evolving Grooves**
Polyrhythmic shifting is a classic trick to create tension and release, move into breakdowns, or make pattern changes.
- **Patch Example:**  
  - OUT 1 provides a straight clock for hi-hats or percussion.  
  - OUT 2 set to an odd division (e.g., /5, /7 or *3) clocks another percussion voice or a sequencer, creating evolving rhythmic interplay that can change under voltage control.
- **Automation:**  
  - Send stepped or smooth CV to RATE CV to automate these polyrhythmic progressions, aligning with song structure cues.

### 3. **Controlling Song Progression with Logic or Switching**
Use Div outputs together with logic modules and sequencers to gate different voices or events at specific times.
- **Patch Example:**  
  - OUT 1 and OUT 2 feed different sequential switches, logic gates (AND/OR/XOR), or clock randomizers.
  - Select which voices are enabled/triggered in sections ("verse" vs "chorus") by routing those gates to VCAs, muting, or clocking envelope/trigger sequencers.

### 4. **Dynamic Fill Sections and Transitions**
Automate sudden tempo shifts or clock muting for fills, breakdowns, or build-ups.
- **Patch Example:**  
  - Use a trigger, manual gate, or sequencer to send sudden CV jumps to the RATE CV, quickly shifting OUT 1 or 2 for tempo-doubling, triplets, or massive slowdowns.
  - Perfect for automated drum fills or re-triggering melodic patterns for dramatic effect.

### 5. **Phrase Sequencing & Macrostructure**
If you have a phrase sequencer or voltage memory/recorder (like Ornament & Crime, 1010 Toolbox, or similar):
- Sequence phrases or song sections with stored voltages that recall different Div clock settings for various channels, syncing all sections to a master timebase.
- Use with samplers or melodic parts for classic "song" structure (intro, verse, chorus, bridge, outro).

---

## Typical Companion Modules for Song Structuring

- **Sequencers:** Malekko Voltage Block, Make Noise Rene, Tiptop Z8000, or Erica Black Sequencer.
- **Switches/Logic:** Doepfer A-151, WMD Sequential Switch, 4ms Rotating Clock Divider, Intellijel Plog.
- **Envelope Generators:** Intellijel Quadrax, Maths.
- **Random/Chaos Generators:** Mutable Marbles, Wogglebug.
- **Utilities:** Precision Adder, Attenuators, Sample & Hold.
- **Performance Controllers:** Pressure Points, Planar 2, or CV recorders.

---

## Sample Patch Workflow for a Song

1. **MASTER CLOCK** into **Div IN**.
2. **OUT 1** divided by 4 (kicks, start of track), **OUT 2** divided by 7 (snares, hats—polyrhythm).
3. A **sequencer** or **CV storage module** modulates **RATE 1/2 CV** over time to change rhythm/composition.
4. Use **logic modules** to gate when each rhythmic clock controls other modules—so only certain patterns/voices are playing at certain times.
5. Use a **sequential switch** to switch between different Div outputs, providing instant "scene/cue" style changes.
6. For breakdowns/drops, automate Div to go to extreme divisions/multiplications or stop (for silence or effects).

---

By thinking of rhythmic clock sources as "sections" and automating division, multiplication, and routing, the **2hp Div** becomes a central tool in providing the macrostructure and movement needed to turn modular jams into full, evolving tracks.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)