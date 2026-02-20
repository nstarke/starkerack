# Doepfer — A-160-2

- [Manual PDF](../../manuals/A-160-2.pdf)

---

[Doepfer A-160-2 Clock/Trigger Divider II Manual (PDF)](https://doepfer.de/A1602_jumper.pdf)

---

# Creative Modulation Techniques for the Doepfer A-160-2

The **A-160-2 Clock/Trigger Divider II** is far more than just a utilitarian clock divider; its combination of unique division sets, output modes, and various onboard configuration jumpers make it a deep tool for sculpting complex and unique rhythms, pulses, and modulation shapes. Below are some tailored techniques geared to stylistic exploration: harsh drum timbres, bassline animation, and eerie pads.

---

## 1. Distorted Percussive Sounds

**Goal:** Use odd or shifting clock divisions to ‘glitch’ drum triggers, shuffle gates for bit-crushed snares or kicks, and inject chaos into percussive chains.

### Techniques

- **Prime Division Glitches:**  
  Set the division switch to “prime” (divisions: 2, 3, 5, 7, 11, 13, 17). Patch a square LFO or clock from a sequencer to the Clock In. Use the non-binary outputs (7, 11, 13, etc.) to clock drum modules, creating unpredictable, “off-grid” hits and fills.  
  *Tip*: Layer two percussion voices triggered by outputs with nearby-by divisions (e.g., 5 and 7) for rapidly phase-shifting polyrhythmic hits.

- **Trigger Mode Slicing:**  
  The trigger mode ANDs output with the incoming clock pulse width. Drive the Clock In with a narrow pulse for ultra-short, clicky triggers or with wide pulses for more sustained “gatted” percussive elements. Modulate the width of the clock signal (via a variable clock source or PWM LFO) for extreme, dynamically-changing transient shapes.

- **Output Polarity Inversion:**  
  On the board, set the polarity jumper to negative. Now, the division outputs become ‘reverse gates’ – modulating amplified white noise or VCA CVs with these, you get sharp stuttering, reverse flams, or “splattered” hats.

---

## 2. Crazy Dubstep/Drum & Bass Basslines

**Goal:** Inject stepped, re-triggered, or otherwise animated modulation into bass oscillators or filter cutoff frequencies, creating the motion and unpredictability typical of modern heavy bass music.

### Techniques

- **Integer Division Arpeggiation:**  
  Use the “integer” division set (2,3,4,5,6,7,8). Send a gate pattern (from a sequencer or hand-played source) into the Clock In, and use different outputs to retrigger envelopes on your bass voice.  
  *Tip*: Stack several envelope generators, each retriggered by a different division, and mix their CVs to modulate a VCF or VCA for complex evolving wobble patterns.

- **Clock-Edge Micro-Syncopation:**  
  Move the onboard jumper to select falling clock edge triggering. Now, incoming short (eighth/triplet) pulse clocks re-synchronize your bass modulations on the “offbeat” relative to the rest of your system for real swung or syncopated feel.

- **Reset Mayhem:**  
  Use a random gate source or a sequencer reset as the A-160-2's Reset. This will “shuffle the phase” of all outputs unpredictably. Patch this into bass mod envelope triggers, or clocked step sequencers, causing abrupt, mangled bass movement at every reset.

---

## 3. Haunting Atmospheric Pads

**Goal:** Generate time-varying gate/trigger patterns that can be used for subtly altering textures, evolving drones, or slowly shifting modulations.

### Techniques

- **Super-Slow Modulation Cycles:**  
  Patch an ultra-slow LFO to the Clock In, and use the highest division outputs (e.g., divide by 64 or 128 in “power of two” mode) to gate long envelopes or step a quantizer, causing pad layers to drift and evolve over long periods (e.g., minutes).

- **Gated Effects Automation:**  
  Use multiple divider outputs to drive VCA CVs, reverb send levels, or wavefolder depths on sustained drone sources. The outputs' complex, interleaved patterns gently gate or animate effects, resulting in a spectral, haunted “breath” across your pads.

- **Pulse-Width Modulated Gate Clouds:**  
  In trigger mode, run a PWM LFO or stepped random pulse into the Clock In so that output pulsewidths are ever-changing. These can gate crossfades between multiple pad tones/samples, creating spectral phase-shifting, flickering atmospheres as layers weave in and out.

---

## Additional Tips

- **No A-161 Support:**  
  Remember, the A-160-2 cannot directly interface with the A-161 like the classic A-160 does—exploit that difference for more “standalone” clock-altering roles.

- **Custom Mode Potential:**  
  The “Cst” switch mode is currently unimplemented (as of the manual revision), but keep an eye on future firmware for new division options, possibly inverted or custom division sets for further creative mayhem.

- **Manual for Jumpers:**  
  [Direct PDF Link: A160_2_jumpers.pdf](https://doepfer.de/A1602_jumper.pdf) — Use this to locate jumpers for clock edge, reset behavior, and polarity.

---

*[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)*