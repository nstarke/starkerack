# Doepfer — A-160-2

- [Manual PDF](../../manuals/A-160-2.pdf)

---

[**A-160-2 Clock/Trigger Divider II Manual (via Doepfer)**](https://doepfer.de/a1602.htm)

---

## Creative Uses for the Doepfer A-160-2 Clock/Trigger Divider II

The Doepfer A-160-2 Clock/Trigger Divider II is a highly flexible clock utility, capable of generating a broad variety of rhythmic divisions. Its versatility allows it to serve a range of functions in any Eurorack system beyond simple drum clocking. Here are some creative patching ideas:

---

### 1. **Complex Rhythms and Polyrhythms**

**How:**  
Use the prime number division mode (2, 3, 5, 7, 11, 13, 17) to create evolving polyrhythms.  
**Combine With:**  
- Multiple drum modules (e.g., **ALM Akemie's Taiko**, **Tiptop Audio ONE**)  
- Sequential switches or analog switches (e.g., **Doepfer A-151 Sequential Switch**)  
**Idea:**  
Patch different divider outputs to individual drum triggers. Using non-binary divisions, you get non-repeating rhythmic patterns. Pass some of these triggers to a sequential switch to rotate the destinations for even less predictability.

---

### 2. **Generative and Evolving Sequences**

**How:**  
Send divided clocks into random generators or sequential switches for generative melody/rhythm.  
**Combine With:**  
- Random or sample & hold (e.g., **Mutable Instruments Turing Machine**, **Doepfer A-184-1**)  
- Quantizers (**Intellijel Scales**, **Doepfer A-156**)  
**Idea:**  
Feed the A-160-2’s divided outputs to trigger random voltage generators, then quantize those voltages to create musical pitches. The varying length of divided clocks introduces organic timing into your generative process.

---

### 3. **Clocked Modulation/Gates**

**How:**  
Use gate or trigger outputs to cycle modulation sources in sync with your master clock.  
**Combine With:**  
- Envelope generators (**Intellijel Quadra**, **Make Noise Maths**)  
- LFOs  
**Idea:**  
Trigger envelopes or reset LFOs with different divisions for evolving modulation that stays rhythmically relevant to your sequence.

---

### 4. **DIY Euclidean Patterns**

**How:**  
Patch divisions from the "integer" output set (2, 3, 4, 5, 6, 7, 8) to gate the steps of a sequencer/reset logic, mimicking Euclidean rhythms.  
**Combine With:**  
- Simple step sequencer (**Doepfer A-155**, **Erica Synths Sequencer**)  
- Logic modules (AND/OR, e.g., **Doepfer A-166**)  
**Idea:**  
AND-gate together different divider outputs for DIY Euclidean patterns or to create rests/accents in drum parts.

---

### 5. **Clocked Effects & Synchronized Modulation**

**How:**  
Synchronize effects like delays, filters, or audio processing with sub-divided clock signals.  
**Combine With:**  
- Synchronized effects processors (**Make Noise Mimeophon**, **Erica Synths Pico DSP**)  
- VCAs or LPGs  
**Idea:**  
Use a divided clock output to ping a filter resonance, open a VCA/LPG, or modulate effect send levels, all perfectly in sync but at musically related sub-divisions.

---

### 6. **Performance/Improvisation Tools**

**How:**  
Switch divisions and modes live for spontaneous variation.  
**Combine With:**  
- Manual gate or switch modules (**Mutable Instruments Shades**, **Doepfer A-150**)  
**Idea:**  
Flip the divider set switch mid-performance for instant rhythm changes, or engage/reset the module on the fly to reorganize the patterns.

---

### 7. **Syncing Analog and Digital Worlds**

**How:**  
Take a MIDI clock or a DAW sync signal (via a MIDI-to-CV interface) and use the A-160-2 to produce complementary clocks for analog sequencers, drum machines, or S&H modules.  
**Combine With:**  
- MIDI-to-CV interface (**Doepfer A-190-series**, **Expert Sleepers FH-2**)  
- Clock distributors/multiples (**Intellijel Buff Mult**, **Mutable Instruments Links**)  
**Idea:**  
Let your DAW run at one tempo, while different synth voices or modulation lines run on intricate, clocked subdivisions for intricate interplay.

---

## Additional Creative Nuggets

- **Inverted Outputs:** With the output polarity jumper, you can get negative-polarity clocks for specialized logic patches.
- **Trigger Mode AND Clock Pulsewidth:** Use the trigger mode with clock sources that have variable pulsewidth to create variable-duration triggers—handy for driving percussion modules with dynamic amplitude or accent response.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)