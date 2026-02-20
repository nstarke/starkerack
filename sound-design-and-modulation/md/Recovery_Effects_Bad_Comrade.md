# Recovery Effects — Bad Comrade

- [Manual PDF](../../manuals/Bad_Comrade_V3_Eurorack_module_manual_Recovery_Effects.pdf)

---

[Download the Bad Comrade V3 Manual (PDF)](https://recoveryeffects.com/cdn/shop/files/BadComradeV3_WEB.pdf)  
---  

# Modulation Tips for Bad Comrade V3  
*(Recovery Effects Eurorack Module)*

Based on the manual, the **Bad Comrade V3** is a compact 4hp module combining glitch, delay, and chaotic distortion with CV inputs for *mix* and *delay time*. Here's how you can push it beyond the ordinary for different sound design goals in your eurorack setup:

---

## 1. Distorted Percussive Sounds

**Approach:** Feed short transients (drum triggers, gate pulses, or chopped samples) into the Bad Comrade V3 to turn any percussive sound into a mangled, noisy hit.

- **Mix Modulation:** Patch an envelope (preferably fast-attack and fast-decay) into the *Mix CV* input. This will make the percussive hit start dry and quickly get drenched in chaos.
- **Time Modulation:** Use another envelope, LFO, or random stepped source into *Delay Time CV*—this shifts the delay buffer in real time, creating stuttering, machine-like artifacts at the tail of each hit.
- **Glitch:** Set the Glitch knob higher for aggressive, crushed transients, or lower if you want more bits to sneak through.
- **Freeze Button:** For truly experimental shots, trigger *Freeze* with a gate or manual press during the attack for “slammed” noise slices.

*Patch example:*  
- Drum hit → Bad Comrade IN  
- Envelope (from drum trigger) → Mix CV  
- Stepped random CV / Clocked LFO → Delay Time CV  
- Output → Mixer/Effects

---

## 2. Crazy Dubstep/Drum & Bass Basslines

**Approach:** Inject a bassline or synth voice and let Bad Comrade V3 mangle it for digital filth.

- **Delay Time Wobble:** Use a synced LFO or envelope follower (from your kick or snare) into *Delay Time CV* to create pitch-varying, glitched bass growls.
- **Mix Automation:** Slow LFO or sequence controlling *Mix CV* to make the distortion surge and dip along your bassline progression.
- **Glitch “Clipping”:** Dial Glitch near the edge—let it clip the waveform for gritty, gated tones.
- **Freeze as Fill/Hits:** Smash *Freeze* (or sequence it) mid-sequence for those abrupt, chopped fills and bass “edits”.

*Patch example:*  
- Bass oscillator/synth → Bad Comrade IN  
- Triangle/Square LFO (mod rate) → Delay Time CV  
- Slow LFO or step-sequencer CV → Mix CV  
- Optional: Clock/gate → Freeze  
- Output → VCA or FX

---

## 3. Haunting Atmospheric Pads

**Approach:** Sweep pads, strings, or textures into the module, then slowly morph parameters with modulation for ghostly, broken-ambient effects.

- **Mix CV:** Use a slow random (sample & hold) or gradual envelope tied to note changes/chords for gentle washes between clean and chaos.
- **Delay Time Mod:** Another slow LFO (especially with lots of unevenness, like a wobbly sine or pseudo-random) into *Delay Time CV* to create drifting, cloudy echoes and spectral jumps.
- **Glitch:** Set low for lo-fi shimmer, higher for grainy, foamy pad 'damage'.
- **Freeze:** Tap or clock *Freeze* sparsely for repeating fragments—almost like granular playback.

*Patch example:*  
- Ambient pad output → Bad Comrade IN  
- S&H random CV or slow LFO → Mix CV  
- Slow, wonky LFO → Delay Time CV  
- Tap Freeze in time with chord changes  
- Output → Long reverb (optional)

---

## Bonus: Power-On "Wide Open" Tip
Remember to power up the Bad Comrade V3 with the *Glitch* and *Time* knobs fully clockwise for best results!

---

### CV Source Suggestions
- Function generator/envelope (Maths, Zadar, or Intellijel Quadrax)
- LFO (Batumi, Pam's New Workout, or any modulation source)
- Stepped random/S&H (Wogglebug, Turing Machine)
- Sequencer with CV tracks (Metropolis, Rene)

---

For more creative tips and patch sharing, visit:  
**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**