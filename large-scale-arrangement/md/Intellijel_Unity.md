# Intellijel — Unity

- [Manual PDF](../../manuals/unity-mixer_manual_2020.04.15.pdf)

---

[Download the Unity Mixer Manual (PDF)](https://cdn.intellijel.com/manuals/unity_mixer_manual_2020.04.15.pdf)

---

# Using the Intellijel Unity Mixer to Build Full-Length Eurorack Songs

The [Intellijel Unity Mixer](https://intellijel.com/shop/eurorack/unity-mixer/) is a deceptively powerful dual 3:1 or single 6:1 unity gain mixer for both audio and CV. While it may not have "performance" controls or modulation onboard, it is a key building block in the kind of dynamic patching that lets you transform loops and ideas into cohesive, evolving, full-length tracks.

Below are strategies and Eurorack patching tips for using the Unity Mixer to structure, transition, and perform full-length songs.

---

## 1. Song Structure With Selective Mixing

### **Scene/Section Routing**
- Use the Unity Mixer to combine different sources for each section of your song (e.g., verse, chorus, breakdown).
- Place sequenced audio or CV sources (melodic, bass, drum voices, etc.) on the Unity Mixer's inputs.
- Use mute switches, sequential switches, or voltage-controlled switches upstream of the Unity Mixer to select which elements reach the final sum (i.e., only certain voices play per section).

**Patch Example:**  
- Input 1: Drum sequence 1  
- Input 2: Alternate hi-hat pattern  
- Input 3: Melodic sequence A  
- Output to mixer/master: Use a switch (like a Doepfer A-150 or similar) to rout in/out alternating patterns for each song section.

---

## 2. Layering and Seamless Transitions

### **Dynamic Layering**
- Use the dual 3:1 mixer capability to sum several sources: layer percussion, blend wavetable oscillators, or overlay different sampled textures.
- For transitions, crossfade or switch between summed mixes (using external VCAs, manual switches, or CV-addressed muters).
- Use both mixers independently for layer control, or chain them to build up/thin out arrangements for verse/chorus/buildup structures.

### **Blending Variations**
- Send two different pattern variations (e.g., two basslines) into the Unity Mixer.  
- Mix their outputs selectively into the master using VCA mutes, allowing for instant swaps or smooth blends during your track.

---

## 3. Dynamic CV Routing for Macro Song Control

### **Macro CV Scenes**
- Sum multiple modulation sources (envelopes, LFOs, random, automation CV from a sequencer like Hermod or NerdSEQ) into key parameter destinations.
- For example, combine an envelope, an LFO, and random voltage into a filter cutoff. Change the modulation flavor by patching different sources, thereby evolving the arrangement over time.
- Use a sequential switch to change between “modulation scenes” (e.g., animated vs subdued/ambient sections) on the fly without repatching.

---

## 4. Creating Performance Tools and FX Sends

### **FX and Performance Routing**
- Use the Unity Mixer as a summing stage for FX sends—from multiple sound sources, sum sends into a delay or reverb input.
- With dual sections, create parallel FX chains; e.g., send wet/dry blends or parallel signals (dry, reverb, delay channels) to allow spontaneous juggling of FX states throughout your song.

---

## 5. Multi-Part Track Creation with Flexible Resampling

### **Live Looping and Resampling Routes**
- Route outputs from Unity Mixer to a sampler/looper (e.g., 1010music Bitbox, Morphagene, Lubadh).
- Quickly swap what gets captured/looped by the sampler via patching different sources to each input throughout the set, building up the track piece by piece and then reintroducing them as new sections ("drop," breakdown, fills) unfold.
- This allows hands-on, non-linear building of a long-form arrangement.

---

## 6. Example Patching: Full Song Architecture

1. **Drum Machine Section:**  
   - Drum sequencer outs → Unity Mixer (inputs 1-3) → VCA/FX send → Main Mixer
2. **Bassline/Lead Section:**  
   - Two melodic voices → Unity Mixer (inputs 5-6) → Chorus/Delay → Main Mixer
3. **Structural Changes:**  
   - Use an external switch (Doepfer A-151, Erica Pico SEQS, etc.) or manual patching to move parts in and out.
4. **Transitions/Evolution:**  
   - Repatch, mute, or switch Unity Mixer inputs between sections for arrangement building—no need for multitudes of dedicated mixers.
5. **Global FX:**  
   - Unity Mixer acts as a submixer for all reverb/delay returns, instantly muting or blending FX levels.

---

## Key Takeaways

- The **Unity Mixer** serves as a backbone for patch rearrangement, signal blending, and evolving song structure, even though it has no controls of its own.
- Pair with muting modules, sequential switches, and VCAs for live arrangement manipulation.
- Essential for creating movement, dynamic layers, and macro-structural transitions in a live or studio Eurorack environment.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)