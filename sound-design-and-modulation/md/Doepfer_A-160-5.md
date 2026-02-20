# Doepfer — A-160-5

- [Manual PDF](../../manuals/A-160-5.pdf)

---

[Doepfer A-160-5 Voltage Controlled Clock Multiplier / Ratcheting Controller Manual (HTML)](https://doepfer.de/a1605.htm)

---

## Creative Modulation Tips for Doepfer A-160-5

The Doepfer A-160-5 is a voltage-controlled clock multiplier designed to take a clock input and output a multiplied, rhythmically complex version, with the multiplying factor selectable via CV and a mode switch. By modulating its clock multiplication factor with control voltage (CV), you can inject rhythmic variation, glitches, and intensity into all sorts of modular patches. Below are some detailed patch ideas and techniques targeted at:

- Distorted percussion
- Crazy dubstep/drum & bass basslines
- Haunting atmospheric pads

---

### 1. Distorted Percussive Sounds

**Patch Idea: Glitchy Perc I/O**

- **Clock In:** Use a snappy clock source like a drum machine trigger out, or a fast LFO square wave.
- **Clock Out:** Send to a percussion module trigger/gate input (e.g., drum module, LPG, or noise burst envelope).
- **CV In:** FM the multiplication factor with an audio-rate oscillator (for audio-rate clock multiplication), or with a very fast LFO cycling through the 2–5 V range.
- **Mode:** Try middle (powers of two) or right (hybrid) for unpredictable rhythmic bursts.
- **Manual Knob:** Use in combination with attenuated CV for finer, real-time glitch control.
- **Result:** This will create unpredictable rapid-fire “ratcheting” triggers at audio or control rates, producing anything from rapid rolls to very harsh, tearing distortion (especially with audio-rate modulation), especially effective when passed through a distortion or wavefolder after the percussion module.

**Bonus Tip:** Stack multiple triggers via a mixer to overdrive drum modules, and use the A-160-5 to make the overdrive rhythms unpredictable.

---

### 2. Crazy Basslines (Dubstep / Drum & Bass)

**Patch Idea: Wobble & Glitch Bass Rhythms**

- **Clock In:** Feed the output from a steady sequencer clock or tap LFO.
- **Clock Out:** Use to clock a sample & hold, envelope, or sequencer dealing with note pitch/cutoff/gate.
- **CV In:** Envelope follower from your bass oscillator fed into the A-160-5’s CV In. As your bass synth gets louder, it speeds up the clock, producing wild gating and rhythmic shifts that “follow” bass amplitude.
    - Alternatively, route modulation sources (LFOs, looping envelopes, random generators) to the A-160-5 for stepped, randomized, or evolving multiplication.
    - Assign sequencer CV lanes to the A-160-5 for “ratcheting” runs on specific notes.
- **Mode:** Sweep through modes to find the most aggressive syncopation—middle mode does classic DnB fast hats, right mode gives glitchy fills.
- **Result:** The CV-controlled multiplication injects classic “rolling,” tearing rhythms, hyper-fast gates, or unpredictable syncopations—ideal for modern neuro/dubstep/jungle sounds.

**Extra:** Use the A-160-5’s output to gate FX like distortion, comb filtering, or amplitude modulation. As the clock rapidly multiplies/decreases, effects will chop, slice, and mutate in wild, musical rhythms rather than just plain on/off.

---

### 3. Haunting Atmospheric Pads

**Patch Idea: Stretched Time & Ratcheted Textures**

- **Clock In:** Very slow LFO, random clock, or manually triggered gate.
- **Clock Out:** Send to granular modules, looping envelopes, the freeze function of delays/reverbs, or any CV-able effect needing rhythmic gates.
- **CV In:** Try slowly evolving modulation: a voltage sequencer, the output of a random source into a slew limiter for smooth drift, or the “wobble” from a joystick or aftertouch strip.
- **Manual Knob:** Morph through rhythmic textures live—beautiful for ambient performances.
- **Mode:** Use left or right mode for access to longer, polyrhythmic cycles, then sweep CV in small amounts—multiplication subtly varies, adding organic, ghostly drift to your textures.
- **Result:** Clouds of evolving, shifting rhythmic accents or filter sweeps, ideal for pads that seem “alive” and always in motion. If patched creatively to modulate aux FX (e.g., granular grain trigger, shimmer reverb freeze), you can generate distant, shimmering echoes, swirling pads with ever-shifting presence.

**Atmospheric Bonus:** Pair with random or audio-rate clock for instant horror soundtracks—chaotic clusters, jittery swells, or static-riddled fade-in textures.

---

## General Pro Tips

- **Layering:** Use multiple A-160-5 outputs (via comparator, logic, or clock divider after multiplication) to build complex polytempic rhythms or layered texture.
- **Clock Feedback:** Patch Clock Out to trigger parameter changes (e.g. sample select/envelope time) for ultra-tight rhythmic modulation, especially at high multiplication rates.
- **Audio-Rate Modulation:** For extreme effects, clock the A-160-5 with audio signals and mult the output back into CV pathways—this can turn CV pathways into pseudo-ring modulators or harsh digital FM effects.

---

For further patch ideas and technical details, visit the [Doepfer A-160-5 Manual](https://doepfer.de/a1605.htm).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)