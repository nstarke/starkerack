# TAKAAB — Odd Clock Divider

- [Manual PDF](../../manuals/TAKAAB OCD - Odd Clock Divider – Siam Modular.pdf)

---

[TAKAAB OCD Odd Clock Divider – Siam Modular Manual (PDF Link)](https://siammodular.com/products/takaab-ocd-odd-clock-divider?srsltid=AfmBOopTsJBGyNaC6WtMfJJU3EFzdu1WvzDldMz3y6eA2c-lwQCE1iKj)

---

# Creative Eurorack Patch Ideas with the TAKAAB OCD - Odd Clock Divider

The TAKAAB OCD is a compact 2HP module specializing in generating **odd** clock divisions from an incoming clock, trigger, or gate. With outputs for 1/3, 1/5, 1/7, 1/9 (or 1/6 via jumper change), and 1/10 divisions, it can drive sequences and modulations well beyond regular 2/4/8 patterns—especially when paired with drum modules, oscillators, or external effects.

Below you will find experimental patch ideas aimed at achieving:

- Distorted percussive sounds
- Crazy modulated basslines for dubstep/drum & bass
- Atmospheric, haunting pads

---

## 1. **Distorted Percussive Sounds**

### Patch Idea
- **Clock Source:** Plug a fast LFO, trigger, or sequencer clock into the OCD’s clock input.
- **Odd Outputs:** Patch *multiple* divisions (e.g., 1/3 & 1/7) into the trigger/gate inputs of drum modules (kick, snare, or metallic percussion).
- **Distorted Percussion:**  
  - Mult the 1/3 output and process through a wavefolder or distortion module before hitting a drum synth or physical modeling percussive voice.  
  - Combine two or more OCD outputs with a logic/OR gate (like Takaab 2XOR) before sending to a percussion envelope or sample player to create glitchy, unpredictable rhythms.
- **Bonus:** Use the OCD’s RESET button or jack to abruptly re-sync the rhythms for glitch fills.

### Why this works:
- **Odd divisions** skip the usual grid, creating offbeat, syncopated, and “wrong-feeling” timings—a hallmark of experimental percussive music.
- Processing with **distortion or wavefolding** on pulse signals creates digital “crush” tones and brutal artifacts.

---

## 2. **Crazy Basslines for Dubstep/Drum & Bass**

### Patch Idea
- **Oscillator Sync:** Patch a division (e.g., 1/5 or 1/7) into the sync input of an analog VCO.  
- **Modulation:** Patch another division into a VCA’s CV input controlling amplitude of the bass voice, or use it to trigger an envelope for the filter’s cutoff.
- **Bass Movement:** Use RESET input from a manual or sequencer gate to resync the groove—now every time you hit RESET, your wobbles and bass modulations start tight on cue.
- **Glitch:** Use the 1/9/1/6 output (especially with the non-1:1 duty cycle) to trigger short filter sweeps or waveshaper modulation for extra grittiness.

### Why this works:
- **Odd divisions** throw the bass out of predictable sync, creating weird stutters and polyrhythms.
- **Syncing the VCO** to an odd clock pulses result in gnarly, wobbling, or burbling sounds typical of hard genres.
- **Split odd clock** between amplitude and filter to get complex *compounded modulation*.

---

## 3. **Haunting Atmospheric Pads**

### Patch Idea
- **Layered Pads:** Take the outputs from divisions like 1/5, 1/7, and 1/10 and use them to trigger long, evolving envelopes for multiple oscillators/wavetables/pad voices.
- **Textural Modulation:** Use an odd division to slowly modulate the amount of reverb, delay feedback, or granular FX mix.
- **Pad Swells:** Assign one output to the reset input on a looping function generator (Slow LFO or envelope), ensuring slowly shifting, unrepeatable cycles form part of the pads.
- **Layered Complexity:** Reset two synchronized OCD modules (via the normalization jumpers & Dupont cable) from a single pulse to orchestrate chaos that periodically aligns.

### Why this works:
- **Pads** feel alive when their harmonic content or effects modulation is driven by *non-repetitive clocks*.  
- Using **RESET** ensures “resonant resets”—think of ghostly textures that occasionally unify in time.

---

## General Modulation Tips

- **Jumper setting:** Experiment with changing 1/9 output to 1/6—use this to introduce a more major, musical ratio into your polyrhythms.
- **Duty Cycle:** Take advantage of 1/7, 1/9 and others with 'rounded down' HIGH:LOW. For instance, patch divisions with asymmetric ratios into slew limiters to get sliding envelopes or differing mod depths.
- **Clock Chaining:** Chain the OCD to other dividers (e.g., Takaab ECD) for multi-layered polyrhythms.
- **Dupont Normalization:** Use the supplied cable to chain RESETs for instant, complex, interlocked resets and grooves.

---

For more creative patching resources:

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)