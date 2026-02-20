# Erogenous Tones — Levita8

- [Manual PDF](../../manuals/l8-instructions.pdf)

---

[LEVIT8 Manual PDF](http://erogenous-tones.com/assets/pdf/LEVIT8_MANUAL.pdf)

---

# Using the LEVIT8 in Eurorack for Arranging Full-Length Songs

Turning a collection of short loops or phrases into a *full song* in modular is a creative challenge. The Erogenous Tones **LEVIT8** is a highly flexible 8-channel attenuverter, mixer, and utility module that can play a crucial role in creating song structure—by enabling gradual transitions, macros, dynamic control, and scene-based programming throughout your patch. Here’s how you can employ the LEVIT8, in combination with other modules, to achieve this:

---

## 1. **Automation and Macros ― Controlling Many Things at Once**

### **Morphing Between Sections**
- **Use the gain/invert controls as "macro knobs":** Plug LFOs, envelopes, or sequenced voltages (e.g. from a voltage memory, manual controller, or sequencer track) into several LEVIT8 channels, route their outputs to key parameters (filter cutoffs, wavetable position, reverb depth, etc), and use the mix switches to group them into performance macros.
- **Scene changes:** Snap multiple controls to new values with a single move. For a chorus, push the gains up on certain effects; for a breakdown, invert or attenuate those modulations.

### **Manual Song Evolution**
- During a performance, slowly turn the physical LEVIT8 pots to fade parameters in or out, or flip the invert switch for dramatic flips (e.g. melody-to-bass inversion, filter sweeps).
  
## 2. **Building Song Sections with Mix Logic**

### **Instantly Combine or Isolate Groups**
- **Grouped Mixing:** Use the Channel 4 and Channel 8 mix switches to sum up to 4 or 8 channels at once, allowing you to quickly combine several sources (melodies, modulations, rhythms) into one output.
- Send that summed output to a VCA controlled by a manual gate, fader, or sequenced voltage to "mute" and "unmute" large sections, like verse/chorus switching.

### **Creating Transitions**
- **VCAs or Switches on the Output:** Patch individual LEVIT8 outputs through voltage-controlled switches (e.g. Doepfer, WMD SSM, or Mutable Instruments Frames), and sequence those switches to dynamically reroute modulations and audio between song sections.
- **Crossfading Sections:** Fade between two arrangement groups (A and B) by attenuating group A on channels 1-4, increasing group B on 5-8, and then sum them to main out.

## 3. **CV Processing for Dynamic Variation**

### **Live Performance Patching**
- **Attenuate & Invert Sequences or Modulations:** Put your core melody, bassline, or envelope sequences through LEVIT8 for step-by-step shaping (softening bass in verses by reducing gain, inverting for a breakdown, etc).
- **Inject DC Offset:** When a channel has nothing patched in, you can use its gain knob to create a 0-10V DC voltage. Use this as a slow manual modulation to sweep through effects, for drops or filter pulls.

### **Randomness and Generative Structure**
- **Mix random voltages with musical CV:** Sum a rhythmic sequence with some random or slowly drifting modulations for evolving patterns. Use LEVIT8 to dial in exactly how much variation, and remove randomness for more structured sections.

## 4. **Mixing Multiple Subparts for Song Layers**

### **Layer Parallel Processing**
- Split your patch into stems: melody, bass, drums, effects, etc. 
- Patch each stem to a separate LEVIT8 channel, and send mixed groups to their own FX chains, VCAs, or outputs.
- Use the module’s grouping switches to "stack" sections together—fade in additional layers or remove them for breakdowns without repatching.

---

## **Example Song Arrangement Workflow with LEVIT8**

| Section      | LEVIT8 Usage                                      | Result                                   |
|--------------|---------------------------------------------------|------------------------------------------|
| **Intro**    | Low gain/attenuation on channels 1-4 (rhythmic elements), rest off | Sparse, filtered base texture            |
| **Build-up** | Gradually increase gains on channels 5-8 (lead/melodies), invert for stutter FX | Melodic/harmonic expansion, tension rise |
| **Chorus**   | Channel 4 mix ON for parallel group mix, all gains up | Full arrangement, stacked sound          |
| **Breakdown**| Cut gains, invert envelopes, send DC offset for slow sweeps | Drops, filtered movement, empty space    |
| **Outro**    | Sequentially mute/unpatch groups, fade to silence  | Controlled fade-out                      |

---

## **Patch Tips**

- Combine with **sequencers** (e.g. Metropolix, Eloquencer), **logic modules** (OR/AND, sequential switches), or **preset scene managers** for deeper automation.
- Use **VCAs** post-LEVIT8 to impose external modulation for more controlled song automations.
- Patch modulation sources into the LEVIT8 to apply hands-on performance changes live or via external controllers (e.g. Faderbanks).

---

## **Conclusion**

The LEVIT8 turns the challenge of "static loops" into dynamic song sections. It enables macro control, mix automation, group layering, live performance morphing, DC offset scene changes, and so much more. As a central "brain" for hands-on utility mixing, it unlocks deep possibilities for evolving, structured, and full-length modular songs.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)