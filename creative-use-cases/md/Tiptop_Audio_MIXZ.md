# Tiptop Audio — MIXZ

- [Manual PDF](../../manuals/Tiptop_Audio_mixz.pdf)

---

[Tiptop Audio MIXZ Manual (PDF)](https://tiptopaudio.com/manuals/MIXZ_Manual.pdf)

---

# Creative Uses for Tiptop Audio MIXZ in Your Eurorack System

The Tiptop Audio MIXZ is far more than just a straightforward utility mixer; its unique design, dual-mixer structure, and Tiptop Bus Mix integration make it an especially flexible and creative tool for your modular system. Below are some creative ways to use MIXZ in combination with other modules and a variety of patching scenarios.

---

## **1. Parallel Processing: Wet/Dry Mixes and FX**

**Patch Example:**  
- **Mixer A:** Patch your dry signal (e.g., oscillator through a filter) into Mixer A and take OUT A.
- **Mixer B:** Send the OUT A (dry signal) into effect modules (e.g., reverb, delay, distortion), route the effected outputs into Mixer B's inputs.  
- **Mix:** Use Mixer B to blend the processed (wet) signals plus keep OUT A for the dry signal. Excellent for instant wet/dry parallel mixing.

**Recommended Modules:**  
- FX modules: **Make Noise Mimeophon**, **Happy Nerding FX Aid**, **Tiptop Z-DSP**
- VCFs: **Mutable Instruments Ripples**, **MA SARA VCF**

---

## **2. Mixing Drum Voices with the Bus Mix**

If you’re running several Tiptop drum modules (e.g., **HATS909**, **BD909**, **SD808**, **CP909**, **ONE**), enable their Bus Mix headers so all their outputs are summed internally via the_bus_board_ into Mixer B. This allows for a super clean front panel—no patch cables needed for main drum mix.

**Patch Example:**  
- Enable the Bus Mix headers on the modules you want mixed.
- Use Mixer B to control drum mix amplitude.
- Use the Bus On/OFF switch to instantly mute/unmute drum set—great for live performance drops!

**Creative Tip:**  
Route Mixer B OUT to a stereo processor or delay and automate the Bus Mix switch for glitch/stutter effects on the entire drum submix.

---

## **3. Mixing Audio & CV/Gate for Performance Control**

Both Mixer A and B can mix audio, CV, and gates _with linearity_:
- Combine LFOs, random voltages, envelopes, and manual controls into a summed modulation source for a single parameter (e.g., a filter's cutoff or wavefolder's symmetry).
- Use Mixer A as a performance mixer for hands-on level control over several modulation sources.
- Send Mixer A OUT to a filter's FM input or VCAs for animated effects.

**Recommended Modules:**  
- **LFOs/Function Generators:** **ALM Pamela’s PRO Workout**, **Make Noise Maths**
- **Random Voltage Sources:** **Mutable Instruments Marbles**, **Noise Engineering Mimetic Digitalis**

---

## **4. On-the-fly Subgroup Mixing**

Since Mixer A is normalized into Mixer B, this enables traditional “subgroup” mixing:
- Use Mixer A for one group of voices (e.g., bass and leads), output summed signal to Mixer B.
- Use Mixer B for overall drum summing (via Bus Mix + dedicated in).
- Fade or mute subgroups instantly using Mixer B's master gain or the physical out patches.

**Patch Example:**  
- Patch all synth voices to Mixer A; patch OUT A to Mixer B.
- Bus Mix drums to Mixer B; now have total control over full mix.

---

## **5. Utility Mixer for Performance Transitions**

- Use the panel Mixers for effects return, submixes, or as an “audio crossfader”—send Mixer A’s OUT into a VCA or crossfade module, give hands-on transitions for performance or DJ-style sets.

**Recommended Modules:**  
- **VC-Fader/Crossfade:** **Intellijel Planar2**, **Doepfer A-134-1 VC Panning/Crossfader**

---

## **6. Summing Gates and Triggers for Algorithmic Rhythms**

Since MIXZ can handle gates with ease and low crosstalk:
- Patch rhythmic gate sources (sequencer, Euclidean trigger modules, burst generators) to Mixer A. The summed output can create composite rhythms by overlapping logic signals.
- Output the summed gate to percussion modules or clock dividers for complex groove patterns.

**Recommended Modules:**  
- **Trigger Sequencers:** **ALM Gatestorm**, **Euclidean Circles**
- **Logic Modules:** **Doepfer A-166 Dual Logic Module**

---

## **7. Integration With Non-Tiptop Gear**

Use Mixer A or B as an interface for external gear, or as a level stage for signals that need attenuation or boosting (e.g., integrating desktop synth outputs, Korg Volcas, etc.)

**Recommended Modules:**  
- **Input/Output Modules:** **ALM S.B.G.**, **Intellijel Audio I/O**

---

## **Noise & Signal Quality Note**

For the cleanest possible results, use the front-panel Mixer A or B for critical audio signals. Use Bus Mix for drums/trigger-heavy sources where a slight noise floor isn’t a problem.

---

## **Final Thoughts**

The MIXZ is a compact, high-headroom utility that rewards creative patching—especially when combined with modular submixes, CV assemblies, and drum workflows. Its internal routing means you can change your system architecture on the fly without a spaghetti mess of cables—particularly valuable in live and improvisational settings.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
