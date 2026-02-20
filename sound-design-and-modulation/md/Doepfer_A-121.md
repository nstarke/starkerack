# Doepfer — A-121

- [Manual PDF](../../manuals/A121_man.pdf)

---

[Doepfer A-121 VCF 2 Manual (PDF)](https://doepfer.de/a100man/A121_man.pdf)

---

# Doepfer A-121 Multimode VCF 2: Creative Modulation Techniques

As a Eurorack user, the Doepfer A-121 is an extremely versatile multimode filter, offering LP, HP, BP, and Notch outputs simultaneously along with voltage control for both cutoff and resonance. Here are targeted modulation strategies for three key sound design scenarios: **distorted percussion**, **aggressive/“crazy” basslines**, and **atmospheric pads.**

---

## 1. Distorted Percussive Sounds

### Key Approaches:
- **Overdrive the Filter Input:**  
  - Crank the **Audio Level** input so the signal begins to distort. This is explicitly mentioned in the manual:  
    > “If the filter’s output signal is distorted, turn this control down, unless the distortion is wanted as a special effect.”  
  - Use short decay envelopes (ADSR) into the **FCV 1/2** (cutoff CV inputs) for snappy, fast filter plucks.
- **Voltage-Controlled Resonance Distortion:**  
  - Patch envelopes or even audio-rate signals (like fast LFOs, other percussion, or noise) into **QCV 1** or **QCV 2** (with attenuator).  
  - High resonance can push the filter into self-oscillation, making for screaming, synthetic “kick” tails or zappy, atonal snares.
- **Resonance “Clicks”:**  
  - Patch sharp, fast envelopes (short attack and decay) to resonance, set resonance near self-oscillation for extra clicks or pops on percussion transients.

### Patch Example:
1. **Sound Source:** White Noise or VCO pulse into **Audio In**.
2. **Envelope (ADSR):** Output to **FCV 1**, adjust for snappy A/D.
3. **Audio Rate LFO or Envelope:** Output to **QCV 2**; set amount for resonance “crack”.
4. **Crank Audio Level** until you hear pleasing distortion.
5. **Output:** Use the Band Pass (**Band**) for sharper, throaty percussive sounds.

---

## 2. Crazy Basslines (Dubstep/Drum and Bass)

### Key Approaches:
- **Filter Frequency Modulation (FM):**  
  - Patch an audio-rate oscillator (or aggressive LFO) to **FCV 2**.  
  - Use the attenuator to control the intensity; this introduces nasty filter FM—perfect for vocal, squelchy, metallic basses.
- **Envelope/Sequencer Modulation:**  
  - Classic dubstep movement is made by multi-stage envelopes or sequencer CV into **FCV 1** and/or **FCV 2**.
  - Parallel motion: Route **QCV 2** CV from the same source (with different depth), so resonance/“vowel” moves with the cutoff.
- **Use Notch Output for Phasey Movement:**  
  - The Notch output, when modulated by LFO on cutoff, becomes a phaser-like effect often present in classic DnB/dubstep basslines.
- **Resonant Bass “Growl”:**  
  - Max resonance near self-oscillation, feed back a touch of the output (carefully!) into the input for extreme resonance feedback—think Zedd or Noisia style growls.

### Patch Example:
1. **VCO Sawtooth:** Into **Audio In**.
2. **Fast LFO/Audio Oscillator:** Into **FCV 2**. Set depth with attenuator.
3. **Envelope/Stepper CV:** To **FCV 1** (for rhythm/groove).
4. **Second Envelope or MIDI LFO:** Into **QCV 2** for resonant sweeps.
5. **Output:** Use **Low Pass** for weight, **Notch** for “hollow” growls, or combine via a mixer.

---

## 3. Haunting Atmospheric Pads

### Key Approaches:
- **Slow LFO or Envelope Modulation:**  
  - Slow LFO (tri/sine) to **FCV 1** or **FCV 2** makes the cutoff float smoothly.  
  - Use slow, evolving envelopes on **QCV 1** or **QCV 2** for resonance movement.
- **Multiple Outputs for Wide Stereo:**  
  - Run different outputs (e.g., LP to left, HP to right, BP to center) to create rich, evolving stereo images.  
  - Manual describes quadraphonic setup—adapt by stacking two or three outputs into a stereo field.
- **Notch Output Modulation:**  
  - Manually sweep cutoff or use simultaneous LFO and aftertouch to animate the spectral gap in ambient pads.
- **Vocal-Formant Chording:**  
  - Patch two A-121s in parallel (per manual) with different cutoffs and Q values, both gently modulated by LFOs with slightly offset periods—excellent for ghostly, evolving ambiences.

### Patch Example:
1. **Ambient VCO Chord:** Into **Audio In**.
2. **Very Slow LFO:** Into **FCV 2**, set attenuator for subtle drift.
3. **Second LFO or Envelope:** Into **QCV 2** for wandering resonance.
4. **Combine Different Outputs:** Blend LP, BP, and Notch outputs via stereo mixer.
5. **Optional:** Use MIDI controller or aftertouch to slowly alter FCV 2/QCV 2 amounts live for expressive sweeps.

---

## Advanced Tips

- **VCF self-oscillation as Oscillator:**  
  Run A-121 in self-oscillation (high Q, no input), then FM the cutoff for melodic, bell-like, or atonal drones.
- **Layering Outputs:**  
  Mix LP, HP, BP, and Notch in real time for morphing timbral textures.
- **CV Inversion:**  
  Use an inverter module (like Doepfer A-175) on one of the filter’s CV ins for “opposite” cutoff sweeps—great for vocal or formant shifting.

---

**Manual Reference**:  
- [Doepfer A-121 VCF 2 Manual (PDF)](https://doepfer.de/a100man/A121_man.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)