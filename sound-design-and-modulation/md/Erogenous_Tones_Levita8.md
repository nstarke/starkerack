# Erogenous Tones — Levita8

- [Manual PDF](../../manuals/l8-instructions.pdf)

---

[LEVIT8 Manual PDF – Erogenous Tones](http://erogenous-tones.com/files/LEVIT8_MANUAL_v1.pdf)

---

## Creative Uses for the Erogenous Tones LEVIT8

The LEVIT8 is a powerful and flexible 8-channel attenuverter/mixer utility designed for both audio and CV processing in the Eurorack format. Here’s how you can push it into experimental, percussive, bass-heavy, and atmospheric territory using its functions creatively:

---

### **1. Distorted Percussive Sounds**

**Saturation & Distortion:**
- Each channel saturates around ±10V. Use this inherent saturation creatively: leave some channels unpatched so they normalize to 5V, then turn up the gain to drive output into saturation. Patch your drum audio signal into one input and blend in the saturated (unpatched) channels for natural wave-shaping and DC-offset distortion.
- Inverted outputs (channels with the inversion switch) further shape how positive and negative excursions of transients are clipped, providing asymmetric distortion on drum hits.

**Layering & Mixing:**
- Mix multiple percussion samples or rhythmic CVs by enabling the mixer functions (use channel 4 or 8 mix). Overlapping strong transients with DC offsets will result in distortion and combative mixing, delivering punchy, sometimes unstable percussive layers that jump out in a mix.

**Gate ‘Pulse Bending’:**
- Run gate signals through LEVIT8, attenuate or invert them, and overdrive them into the output mix. This bends the shape of the gate, which can trigger envelopes or pitch randomization in downstream modules, leading to glitchy, granular percussive elements when clocked fast.

---

### **2. Crazy Dubstep/Drum & Bass Basslines**

**Basserator: Massive Signal Twisting**
- Take your VCO's raw waveform (triangle, saw, or square) and route through a LEVIT8 channel. Use the gain control to push the amplitude into saturation.
- Add another unpatched channel (with the normalization active) and use its control to introduce a DC offset. By automating this offset (via hands or CV via an external VCA/attenuator) you can shift and "wobble" the bass tone, especially when paired with the inversion switch for pseudo-paraphonic effects.

**Multi-Channel Parallel Processing:**
- Split your bass signal into two paths:
  1. Dry or slightly overdriven in one channel.
  2. Inverted or heavily saturated in another channel.
- Use the mix function to combine the two for a composite, aggressive bass sound with broken symmetry (classic for crazy dubstep "talking" basses).

**FM/AM Effects:**
- Route an audio-rate oscillator into one LEVIT8 input (as carrier), and modulate its gain knob with a slow LFO or envelope, creating amplitude modulation (AM) effects.
- Use an LFO in another channel, invert and mix it with the main bass to achieve evolving filter-like modulation without a filter.

---

### **3. Haunting Atmospheric Pads**

**Stack & Blend CV**
- Set up multiple unpatched channels, normalize to 5V, and slightly adjust the gain on each to output different offsets.
- Mix in subtle audio-rate signals (like a slow triangle wave) on other channels, gently overdriven.
- Use the mix switches to create a giant, evolving DC-shifted pad signal. The summed output becomes a drone with continuously evolving harmonic character.

**CV Animation:**
- Use the LEVIT8 to blend several slow LFOs (or S&H noise sources) for a complex positive or negative voltage shape. Use the output to modulate filters, VCAs, or oscillators in your synth, resulting in ghostly, undulating modulations.

**Signal Bleed & Crossfading:**
- With the inversion switches, you can create phase-cancellation effects: Blend an inverted and non-inverted channel driven by similar signals—minute tweaks to each knob create subtle, haunting movement and amplitude modulation, especially when run into delay or reverb modules downstream.

---

### **Bonus Tips**

- **Visual Feedback:** Use the bicolored LEDs to dial in the exact amount of distortion or DC offset. If colors suddenly shift or ‘sit’ at max, you’re well into signal break-up territory—a sweet spot for harsh percussion or nasty bass.
- **Live Performance:** Quickly 'mute' a signal by turning a gain to zero rather than unplugging, keeping DC offset out of your mixes.
- **Voltage Mixing:** Turn the LEVIT8 into a live performance macro controller—use empty channels as performance CV faders to modulate many things at once with expressive manual control.

---

### **Further Resources**

- [LEVIT8 Manual PDF – Erogenous Tones](http://erogenous-tones.com/files/LEVIT8_MANUAL_v1.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)