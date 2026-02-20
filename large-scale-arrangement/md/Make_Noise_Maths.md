# Make Noise — Maths

- [Manual PDF](../../manuals/MATHSmanual2013.pdf)

---

[Download the Make Noise MATHS Manual (PDF)](https://makenoisemusic.com/content/manuals/MathsManual2020.pdf)

---

# Using Make Noise MATHS To Build Full Length Eurorack Songs

Many modular musicians face the challenge of moving beyond killer loops and short textures to develop evolving, structured, full-length tracks. The Make Noise MATHS, thanks to its flexibility as an analog function generator and control voltage (CV) processor, can serve as a central device in overcoming this challenge by creating modulation, events, clocking structures, and dynamic variations across your system. Here’s an in-depth look at how you can leverage MATHS—alongside other modules—to achieve song-length evolution and structure in your Eurorack compositions.

---

## Key Eurorack Songwriting Strategies Using MATHS

### 1. **Create Dynamic Song Structure with Self-Patching and Clocking**
Using MATHS’ cycling functions, you can generate slow LFOs or stepped envelopes lasting anywhere from a second to over 25 minutes. These slow modulations can control filters, sequencer stages, or effects, producing the macro-evolution typically needed for verse, bridge, and breakdown transitions.

**Technique Example:**  
- Set Channel 1 or 4 to self-cycle at a very slow rate (for example, a 3–5 minute period).
- Use the Unity or Variable Out to modulate the cutoff of a filter used on your main melodic or pad voice, creating evolving timbre shifts across the duration of the song.
- Alternatively, patch a slow cycling envelope to voltage control the sequence length or step address input on a sequencer, shifting the sequence or pattern over time without hard cuts.

### 2. **Automatic Drops, Builds, and Transitions with End-of-Rise/Cycle Logic**
MATHS provides End-of-Rise (EOR) and End-of-Cycle (EOC) gate outputs, which make it possible to generate triggers at precise, programmable moments. Chain these to events like drum fills, variation triggers, or clock-divided breakdowns.

**Technique Example:**
- Use EOC from a long envelope as a reset for a pattern sequencer or clock divider, causing fills or changes at regular musical intervals.
- EOR can trigger effects or transitions, such as opening a VCA for a riser sound or launching a new scene of modulation.

### 3. **Scene Changes and Macro-CV Control**
Patch complex modulation mixtures using MATHS’ sum/invert/offset features. By changing offset voltages, attenuverters, or mod sources, you can create 'scenes' where many parameters subtly shift together, imitating traditional song sections.

**Technique Example:**
- Use a Channel 2 or 3 offset to simultaneously move multiple parameters (e.g., filter cutoff, oscillator wave shape, reverb amount) by sending the summed output to several destinations using stackables or a multiple.
- Combine with voltage-controlled switches (e.g., Doepfer A-150, WMD SSM) to move to new routing topologies at specific moments.

### 4. **Gate Extraction, Envelope Following, and Sidechain Triggers**
MATHS can act as a gate extractor or envelope follower by patching audio or CV into a channel and taking EOR/EOC outputs. This enables dynamic interaction between different song elements—e.g., ducking, gating, or triggering new voices based on existing material.

**Technique Example:**
- Extract a gate from a drum track to generate synchronized modulations or sidechain ducking effects elsewhere.
- Use envelope following to make ambient pads swell in response to percussion intensity, creating organic, song-length interactions.

### 5. **Advanced Clocking, Division, and Polyrhythms**
By programming Rise/Fall times sharp and triggering channels with clocks, MATHS can divide, delay, or multiply clock signals. This enables pattern changes, fills, swing, and evolving rhythm, essential for full song development.

**Technique Example:**
- Use MATHS as a programmable clock divider to generate varying rhythmic subdivisions over the course of a track.
- Cross-patch EOR/EOC outputs between two channels for evolving polyrhythms and unpredictable minimal techno-inspired grooves.

---

## Practical Example: Structuring a Song with MATHS and Friends

### **Goal:**  
Develop an evolving Eurorack track where song sections gradually emerge, drums drop in and out, melodic elements drift in timbre and sequence, and energy grows and releases—without touching the system mid-recording.

### **Suggested Module Pairings:**  
- **Sequencer**: (e.g., Make Noise Rene, Intellijel Metropolix, or simple gate sequencers)
- **VCAs/VCF**: For dynamic amplitude/tone shaping
- **Random/Noise Source**: (e.g., Wogglebug, Turing Machine)
- **Drum Voices**: (e.g., Tiptop 808/909 modules, Mutable Instruments Peaks)
- **Effect Modules**: (e.g., reverb, delay, distortion)

### **Patch Overview:**  

1. **Master Song LFO:**  
    - CH1 set to slow cycle (e.g., Rise and Fall full CW).
    - Unity Out to modulate filter cutoff on pads/bass for slow, evolving movement.
    - Variable Out also sent to a VC switch or sequential switch to periodically swap audio routings or send gates to drum voice modules for mutes/unmutes or fills.

2. **Section Transition Trigger:**  
    - CH4 set as an even slower envelope (6-8 minutes Rise+Fall, Linear).
    - EOC used to trigger a dramatic scene change—reset sequencer, activate fill pattern, or flip a switch to new voices.

3. **Complex Rhythm Shifts:**
    - Route your master clock to CH1 Trigger input.
    - Adjust Rise/Fall for desired division—take EOR as a downbeat accent or fill trig every X bars.

4. **Accent or Fill Generator:**  
    - Program a fast cycling envelope on CH2, attenuate and sum with CH3 offset, patch to VCA controlling percussion or melody to introduce rhythmic variation within sections.

5. **Performing Macro Modulation:**
    - As the initial slow modulation reaches a peak, perform manual adjustments to attenuverters, switching scene offsets, or bring in additional MATHS modulation via Unity Out.
    - Alternatively, feed in a burst of random CV to modulate MATHS Rise/Fall using another module for surprise/performance "automation".

6. **Envelope Follower Dynamics:**
    - Patch audio from a main drum track into CH1, set Rise short and Fall slightly longer—use output to gate a sidechained VCA, ducking pads during kick, or to trigger effects like reverbs at hits/transitions.

---

## Additional Tips

- Self-patch MATHS for complex shapes—feedback Variable Out to Rise or Fall, or cross-modulate channels for evolving contours.
- Use unused channels for offsets or intentional muting in SUM/OR bus to keep the patch environment clean and manageable.
- Record and overdub modulation through a performance, using attenuverter knobs as live performance controls for macro-changes (e.g., moving between verse, chorus, breakdown).

---

## Conclusion

By leveraging the utility, modulation, and temporal control that MATHS offers, along with thoughtful clocking, section/event automation, and creative patching, you can move from great four-bar loops to living, breathing, fully structured compositions. Make MATHS your songbrain, and let other modules be the voice, rhythm, and character!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)