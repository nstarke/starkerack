# Mutable Instruments — Ripples

- [Manual PDF](../../manuals/Manual - Mutable Instruments Documentation.pdf)

---

[**Mutable Instruments Ripples Manual (PDF)**](https://mutable-instruments.net/modules/ripples/manual.pdf)

---

# Using Mutable Instruments Ripples to Arrange Full-Length Songs in Eurorack

Mutable Instruments Ripples is a high-quality voltage-controlled multimode filter with voltage-controlled resonance and VCA that excels in classic subtractive synthesis. While it’s easy to use Ripples as a solid filter or simple VCA for patches, using it as a tool for full-length songs in a Eurorack format requires thinking beyond the loop. Here are practical ways to leverage Ripples in song structuring:

---

## 1. **Dynamic Filtering for Structure and Movement**

**Technique:**  
Utilize Ripples’ voltage-controlled cutoff and resonance to gradually evolve a patch over time, creating traditional song sections (intro, verse, breakdown, etc).

**How:**  
- **Automation:** Use an external sequencer or function generator (like Mutable Instruments Stages or Make Noise Maths) to slowly modulate the cutoff frequency, opening up the filter to reveal new harmonics and energy as the song transitions.  
- **Scene Changes:** Use a random or step-sequencer voltage to shift the filter from a deeper, darker sound (closed filter) to a brighter, more open timbre (open filter) for choruses or climaxes.
- **Resonant Sweeps:** Assign a slow envelope with varying curves to the resonance CV, bringing in accentuated peaks at key musical moments.

---

## 2. **Voltage Controllable VCA for Transitions and Automation**

**Technique:**  
Leverage the built-in VCA on the LP output to fade parts in and out without needing a separate VCA module, making song structure cleaner and more automated.

**How:**  
- **Main Voice Automation:** Connect an LFO, envelope, or automation track to the VCA CV input to bring filtered sounds in and out at specific points (like drops or transitions).
- **Individual Scene Fades:** Patch sequencing lanes from modules like Intellijel Metropolis, Malekko Voltage Block, or Mutable Instruments Marbles to automate when certain voices (processed by Ripples) are faded in or out for arrangement.

---

## 3. **Multimode Output for Textural Variation**

**Technique:**  
Use all three outputs (HP, BP, LP) creatively to introduce variety and evolution to recurring musical elements.

**How:**  
- **Parallel Processing:** Route different outputs to different effects or even to different mixers or panning positions. For example, send the HP out to a delay for airy top-end textures, the BP for midrange motion, and LP for punchy bass.
- **Song Section Swapping:** Switch which output you use for your main element between sections (for example, verse on LP, chorus on BP), or fade between them with a crossfader module for new timbres as the arrangement progresses.

---

## 4. **Live Jamming and Performance Macros**

**Technique:**  
Use the 2-pole/4-pole slope switch and manual controls (cutoff, resonance, input level) as hands-on performance tools to keep a jam evolving or to introduce decisive, song-level gestures.

**How:**  
- **Slope as a Macro Control:** Flip between 2-pole and 4-pole slopes during a breakdown or fill to create obvious timbral change.
- **Performance Improv:** Ride the resonance and input drive like a DJ to induce drops, sweeps, tension, and excitement that define clear song sections.

---

## 5. **Precision Bass and Percussion Shaping**

- Process kicks, basslines, or percussion through Ripples, using CV to dynamically shift cutoff at specific song moments (for breakdowns, outros, or evolving intros).
- Use envelope followers or dedicated function generators to sculpt elements with precision, making each section unique.

---

## **General Patch Suggestions for Full-Length Songs:**

1. **Create a Master Modulation Lane:**  
   Use sequencers or clocked modulation sources to develop large-scale movements in filter cutoff and VCA gain synced to your song sections.

2. **Layer Outputs:**  
   Record multiple passes using different Ripples outputs for different song sections and blend in production.

3. **Utilize CV Control for Macro Changes:**  
   Stack slow-moving LFOs or S&H signals to modulate slope, cutoff, and resonance, automating large-scale section transitions.

---

## **Helpful Example Patch:**
- **Voice Source (VCO) → Ripples IN1**
- **Ripples LP → Output Mixer (Main Bass/Lead)**
- **Ripples BP → Effect Chain (Chorus/Outro Section)**
- **CV Sequencer (e.g., Stages/Metropolis) → Ripples Cutoff + VCA**
- **Performance Macro (manual or external switch) → Slope Switch**

By patching this way, your synth lines can morph and move across the scope of an entire song, making it possible to keep the modular jam engaging and dynamic.

---

**Remember:**  
The key to full-length song creation in eurorack is **macro control** and **timbral variation** over time—Ripples is a powerful module for both, especially when used with external CV modulation, sequencers, and careful planning for song structure!

---

Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)