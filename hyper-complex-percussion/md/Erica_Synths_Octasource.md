# Erica Synths — Octasource

- [Manual PDF](../../manuals/black_octasource_manual.pdf)

---

[Erica Synths Black Octasource Manual PDF](https://www.ericasynths.lv/media/Black_Octasource_manual_1.02.pdf)

---

# Using the Erica Synths Black Octasource for Hyper-Complex Rhythmic Percussion

The Erica Synths Black Octasource is not a voice or effect module; it is a **highly versatile voltage-controlled LFO with 8 phase-shifted outputs**. However, it is an *extremely powerful modulation source* when you want to create polymetric, polyrhythmic, and hyper-complex percussion and sequence modulations in your Eurorack system.

Below are advanced strategies to harness the Black Octasource for densely rhythmic, complex results:

---

## 1. **Patch Phase-Shifted LFOs to Modulate Drum Triggers/Gates**

- **Eight Outputs, Eight Rhythms:** Each of the 8 outputs delivers either a phase-shifted version of the same waveform (**SINGLE mode**) or a different waveform (**MULTI mode**).
- **Use as Envelope Generators:** Patch outputs to envelope or VCA CV inputs controlling drum voices—each output provides rhythmic, phase-shifted modulation, acting as pseudo trig/gate sources.
- **Staggered Modulation:** The 45° phase offset creates `eight cyclical but offset events`—perfect for driving polyrhythms across percussive voices or filters.

**Example Patch:**
- Output 1 CV → Kick Drum VCA
- Output 3 CV → Snare VCA
- Output 5 CV → Hi-Hat Accent Input  
Each drum will pulsate with a different, but related, rhythmic feel—a foundation for intricate grooves.

---

## 2. **External Clock Sync for Irregular Time Signatures**

- **Sync Input:** Use external sequencers or clock generators to synchronize the Octasource.
- **Complex Time Signatures:** Send odd clocks (like 5/4, 7/8, 13/16, etc) via clock dividers/multipliers. Now your LFO shapes align with non-standard meters, giving all 8 outs shifting pulses in polyrhythmic relationships.

---

## 3. **CV-Controlled Phase, Rate, and Wave Morphing**

- **Phase CV:** Patch modulation (from other random modules, chaos sources, or sequencers) to the PHASE CV input to create *nonlinear, evolving* phase relationships between outputs.
- **FM Input:** Modulate the LFO rate from audio-rate oscillators or stepped CV sources to create chaotic, stuttering rhythmic patterns.
- **Wave Select CV:** Use stepped, random, or sequencer CV to morph between waveforms for further rhythmic/tonal variation.

---

## 4. **Multi vs. Single Mode for Pattern Diversity**

- **Multi Mode:** Each output gives a different waveform. Use these as clock sources, modulation for drum tuning, or control for wavefolders or filters, adding wildly distinct rhythmic properties.
- **Single Mode:** Same waveform, each output phase-shifted—perfect for complex polyrhythmic modulation, e.g., opening and closing VCAs or filters at different times in a regular cycle.

---

## 5. **Exploiting Unipolar/Bipolar Modes**

- **Unipolar Mode for Triggers/Gates:** Switch to unipolar (0–+5V) so LFO outputs will be easier to use for triggering envelopes or drums, especially for percussive “on-off” events.
- **Bipolar Mode for Modulation:** Use -5V to +5V for controlling parameters with full-range, e.g. panning modulation or filter sweeps for “stereo percussive motion.”

---

## 6. **Freeze Function for Pattern “Glitch”**

- **Freeze Mode:** Set the RATE knob to 12 o’clock to freeze the current phase state—instantaneously creating stop/hold effects, gated stutters, or abrupt rhythmic 'freezes' in your patterns.

---

## 7. **Cross-Patching for Polymeters & Randomized Drum Patterns**

- **Self-Modulation:** Patch one output into PHASE CV, another into FM IN, or use feedback via attenuators/mixers—this creates unpredictable, evolving rhythmic cycles.
- **Layer with Sequential Switches:** Route LFO outputs through a sequential switch or logic module for even more complex polyrhythms and probability-based percussion accenting.

---

## 8. **Visual Feedback for Tight Programming**

- **Bipolar LEDs:** Use output LEDs as visual guides to precisely dial in and match phase relationships across channels—a tactile and intuitive way to “see” rhythm before you patch it out.

---

### **Bonus: For Unique, Punchy, Percussive Modulation**

- Modulate the decay and amplitude of envelope generators for your drums with *sharply rising/falling LFO waves* (e.g., saw, ramp, pulse).
- Use clock-synced stepped LFO waves (S&H) for sudden, unpredictable pattern changes on drum voice pitches or FX send levels—think glitch, IDM, or breakcore.
- Crossfade or morph between two or more LFO outputs with a CV mixer to create evolving percussion grooves not possible with fixed clock patterns.

---

## **References**

- [Erica Synths Black Octasource Manual PDF](https://www.ericasynths.lv/media/Black_Octasource_manual_1.02.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

**Ready to create hyper-complex polyrhythmic percussive grooves!**