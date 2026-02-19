# Tiptop Audio — Z4000

- [Manual PDF](../../manuals/Tiptop_Audio_z4000.pdf)

---

[Z4000 Voltage Controlled Envelope Generator – User Manual (PDF)](http://tiptopaudio.com/manuals/z4000_manual.pdf)

---

# Creative Patch Ideas: Tiptop Audio Z4000 VC-EG

The Tiptop Audio Z4000 is a highly flexible, CV-controllable envelope generator designed with integrated signal processing for advanced voltage control. Here’s how you can creatively patch the Z4000 with other Eurorack modules to build expressive, musical, and experimental patches:

---

## 1. Dynamic Percussion Designer  
**Combine With:** Drum modules (e.g., Tiptop BD808, HiHats, or Mutable Instruments Peaks)  
- Use the Z4000’s fast transient control to create punchy envelopes for percussion hits.
- Patch the envelope OUT directly into a drum module’s CV input (e.g., decay or pitch).
- Voltage control the Attack/Decay segments via a sequencer to morph between snappy and soft drum sounds.

---

## 2. Animated Filter Sweeps  
**Combine With:** Analog filter (e.g., Tiptop Z2040, Doepfer A-120, or Mutable Ripples)  
- Patch Z4000 OUT into the filter’s cutoff CV input.
- Use the Deviater to offset the envelope positively or negatively, pushing the filter into “sweet spots” or resonance regions.
- Insert an LFO into the Deviater’s VC input to make the offset itself dynamic, giving the filter sweep “waves” or pulsing character.

---

## 3. Complex Modulation with Self-Feedback  
**Combine With:** Multiple Z4000s or Attenuator/Polarizer (Mutable Instruments Shades, Happy Nerding 3xMIA)  
- Patch the Z4000 OUT back into its own segment CV inputs (e.g., modulating Release by its own output).
- This feedback creates evolving, non-linear envelopes ideal for experimental sound design or generative music.
- Process feedback with a secondary attenuverter/polarizer for further control.

---

## 4. Audio-Rate Envelope Modulation  
**Combine With:** Audio-rate oscillator (Tiptop Z3000, Intellijel Dixie II+)  
- Drive the Z4000’s Deviater VC input with an audio oscillator or noise source.
- The result is the “ring modulation” of the envelope, producing AM/FM-like effects when sent through a VCA or filter.
- Try patching a sample & hold output into a segment CV input for randomizing envelope times in rhythmic ways.

---

## 5. Morphing Envelope Generator for VCAs  
**Combine With:** VCA bank (Intellijel Quad VCA, Doepfer A-132-4)  
- Patch the Z4000 OUT into multiple VCAs controlling different sound sources (oscillators, samples, FX returns).
- Use segment CV inputs for “morphing” between different amplitude contours, dynamically changing the intensity and shape of layers.

---

## 6. Envelope Mirroring & Inversion  
**Combine With:** Dual destination patching (VCF + VCA or VCA + effect wet/dry)  
- Set Attenuverter left of 50% for negative envelopes: modulate cutoff inversely as amp increases.
- Create ducking effects: as one source gets louder, another is simultaneously attenuated, great for sidechain-style patches.

---

## 7. Rhythmic or Melodic Retriggering  
**Combine With:** Clock divider or gate sequencer (4ms RCD, Pamela’s Pro Workout)  
- Patch a rhythmic gate or random pulses into the Z4000 Retrig input.
- Envelopes retrigger at unpredictable moments, giving evolving texture to static drones or rhythmically complex melodic material.

---

## 8. Creative Layering through CV Processing  
**Combine With:** CV mixer/processor (ALM O/A/x2, Befaco A*B+C)  
- Use the Deviater for voltage summing or mirroring alongside another CV source (e.g., another envelope, LFO).
- Patch the combined signal to modulate pitch, filter, or effect parameters for constantly shifting, morphing modulation.

---

## More Tips  
- **Use Sustain with a footswitch:** Performance technique for on-the-fly sound shaping.
- **Log/Exp Switch:** Switch often to hear subtle but important changes, especially with long attack times.

---

**Experimentation is key:**  
The Z4000 shines when its segment CVs, Attenuverter, and Deviater are actively patched and modulated. It can go from percussive snappiness to fluid, long gestures — and even analog computation for unusual, composite control voltages.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)