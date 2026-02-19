# Make Noise — Maths

- [Manual PDF](../../manuals/MATHSmanual2013.pdf)

---

[Make Noise Maths Manual PDF](https://makenoisemusic.com/content/manuals/Maths2020Manual.pdf)

---

# Using Make Noise Maths for Densely Rhythmic, Hyper-Complex Percussion

The **Make Noise Maths** module, while not a sound source per se, is a flexible function generator, envelope, logic, LFO, CV processor, and clock/trigger manipulator ideal for generating intricate rhythmic patterns and evolving percussive complexity in a eurorack system. Below are strategies and patch ideas for using Maths to craft polyrhythms, strange time signatures, complex clock divisions, and unique percussive manipulations.

---

## 1. **Mathematics as a Rhythmic Brain: Clocks, Dividers & Gate Manipulation**

### **A. Polyrhythmic Clocking with EOR/EOC**
- Use Maths’ **Channel 1 and 4** in cycling mode, straight or modulated, as clocks with different cycle lengths/times.
    - EOR (End of Rise) and EOC (End of Cycle) outputs give gate/pulse signals at function phase boundaries.
- Set Channel 1 for a 5-step pattern, Channel 4 for a 7-step pattern (for instance) by adjusting Rise/Fall and using external modulation.
    - Patch both EOR/EOC outs to trigger drum modules or envelopes for polyrhythms.

### **B. Generating Odd Time Signatures**
- Use *Trigger Input* to sync Channel 1 or 4 to a master clock, but set Rise or Fall to an “unnatural” division.
    - The slopes act as clock dividers; e.g., a long Rise ignores several repeated triggers, only passing every 3rd/4th/5th.
- Chain EOR/EOC and Trigger/Cycle inputs for cross-patterned triggers. 
    - Example: EOR from Channel 1 triggers Channel 4, EOC from Channel 4 back to Channel 1.

---

## 2. **Evolving Rhythmic Complexity through Self-Modulation & Feedback**

### **A. Feedback for Irregular/LFO-Driven Patterns**
- Take a Variable Output and patch it to the Rise/Fall/Both CV input of the same or another channel.
    - Attenuverter controls turn simple LFOs into bouncing, mutating rhythmic CVs.
- Mult complex outputs into clock dividers, logic modules, or further Maths channels for procedural rhythms.

### **B. Logic & Comparator Processing**
- Use the **OR output** to combine multiple triggers/gates, generating composite clocks for off-beat/irregular hits.
- Patch a steady pulse and a Variable Output (ramped slope) into separate channels, take the OR output as a trigger “mask” or gate-extractor with rhythmic swing or gate delay.

---

## 3. **Maths as a Percussive Modulation Source**

While Maths doesn't directly output audio, it processes control voltages:
- **Envelope Follower/Transient Generator:** Patch percussion audio into a channel's Signal Input, use EOR/EOC or the Variable Output as rhythmic triggers for other voices, compression, or synced CV.
- **Voltage-Controlled Pulse Delays** allow “flam” or ratcheted percussive effects—use EOR outputs with varied Rise/Fall for swung/offset hits.
- **Bouncing Ball** and trilling patches (from the manual) create irregular, dynamic envelope shapes; use for unique hats, rimshots, or FM timbre tweaks on percussion voices.

---

## 4. **Voice & Effect Manipulation for Percussive, Punchy Results**

If you use Maths to control VCFs, VCAs, or even as an audio-rate oscillator:

- **Ping Maths at Audio Rate:** Patch a fast LFO (cycling channel as audio osc) through a low pass gate or filter for metallic, pseudo-physical drum sounds.
- **Complex Envelope Percussion:** Use both Channel 1/4 for layered attack/decay; combine envelopes in the SUM/OR bus for one-shot punchy transients or compound percussion (stacked drums).
- **Voltage Mirror/Pseudo-VCA Patches:** Achieve hard, clipped modulation—great for unusual transient snap or accent envelopes.

---

## 5. **Patch Examples from the Manual Adapted for Rhythmic Complexity**

- **Clock/Divider Patch**: Send master clock to Channel 1 Trigger. Use Rise parameter to set division, EOR out triggers percussive voices on divided clock.
- **Flam/Offset Beats**: Use Pulse Delay (EOR out with varied Rise/Fall) to introduce microtiming between sequential drum triggers.
- **281 Mode**: Interlocking cyclic channels create overlapping and displaced rhythmic contours—each can modulate a different drum sound or effect.
- **Chaotic LFOs**: Create morphing patterns by feedback patching Variable Outputs into Rise/Fall/Both of other channels.

---

## 6. **General Tips**

- **Modulate everything**: Use slow, cycling envelopes on Rise/Fall of fast triggers for controlled drift and non-repetitive rhythms.
- **Explore SUM/OR**: Blend triggers/gates/offsets for evolving, dynamic rhythmic sources and CV for percussion modulation (decay, pitch, filter).
- **Latch and Reset**: Use BOTH input as a reset/gate width for further temporal manipulation.

---

## 7. **Inspirational Patch Starters**

- Use *EOR* to clock a sequencer, *EOC* to clock off-beat percussion.
- Patch envelope or LFO from Maths to VCA controlling drum body, another to VCA controlling “noise” or “FM ring”.
- Use the *OR bus* as a pulse generator modulating a sample’s start point or a drum synth’s pitch parameter.

---

For more detailed reference, you can find all official patch ideas and detailed operation:

[Make Noise Maths Manual (PDF)](https://makenoisemusic.com/content/manuals/Maths2020Manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)