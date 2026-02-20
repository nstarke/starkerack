# Erica Synths — Compressor

- [Manual PDF](../../manuals/compressor_manual_2023.04.04.pdf)

---

[Erica Synths Stereo Compressor Manual (PDF)](https://www.ericasynths.lv/media/Stereo_Compressor_manual_2.pdf)

---

# Using the Erica Synths Stereo Compressor to Create Full Length Eurorack Songs

The **Erica Synths Stereo Compressor** is much more than just a “make-it-louder” tool for your drum bus. When leveraged creatively and paired with other essential Eurorack modules—mixers, sequencers, drums, bass voices, effects, modulation sources—it becomes a critical part of producing full-length, dynamic, and professional-sounding tracks live or in the studio.

Below you’ll find creative strategies and practical patching approaches to use this module for developing full-length modular songs with section changes, evolving energy, and impactful transitions.

---

## 1. **Song Dynamics and Section Transitions**

### **Master Bus Compression for Energy Control**
- **Patch**: Route your final stereo mix into the Stereo Compressor before outputting to your speakers/recorder.
- **Use**: The Compressor can “glue” your mix together. For chorus sections, automate the **Threshold** or **Gain** using a voltage-controlled attenuator (VCA), or have a switch/mutable control in your patch to enhance punch and perceived loudness right when you need a lift in intensity.
- **Performance Tip**: Use the **Bypass** switch for dramatic momentary drops (i.e., bypass for a stripped, dry breakdown, then re-engage for the drop/chorus).

### **Building Intros and Outros**
- **Approach**: Start with light or no compression during intro/breakdown, and gradually increase the **COMP.AMT (Ratio)** and **Gain** as the song crescendos. This can make early sections feel airy and late sections feel urgent.

---

## 2. **Sidechaining for Movement and Groove**

### **Classic Pumped Bass/Pad Animation**
- **Patch**: Use kick drum or percussion triggers into the **SIDE IN (L/R)**. Your pads/bass or other sustained voices pass through the main audio path.
- **Result**: The compressor ducks the mix every time the kick hits—this produces the classic “sidechain pumping” effect, a staple in electronic music for making the rhythm section stand out.
- **Technique**: Modulate the strength (via **Threshold**) for subtle or intense pumping at different song sections. Use mutes or sequencer logic to sidechain only during choruses or drops, or switch patterns for different sidechain effects per section.

### **Creative Sidechain Sources**
- Sidechain doesn’t have to be a kick! Try envelopes from a sequencer, gates from random rhythm generators, or a chopped vocal loop output. Use this for unique swell dynamics (for instance, have melodies duck when a vocal sample plays, or pads pump to a wonky rhythm).

---

## 3. **Parallel Processing & Wet/Dry Control**

### **Dual-Path Mixing**
- Send some sound (drums, bass) through the compressor and some (melodic, atmospheres) not, and mix together. Use crossfaders or VCA-controlled submixers.
- In different parts of the song, shift more sound *to* or *from* the compressor for distinct textural contrast between sections (tight/loose, compressed/dynamic).

---

## 4. **Automated/Evolving Stereo Imaging**

### **STEREO LINK Switch**
- The manual describes that with a very different left/right image, the compression could ‘pan’ the output undesirably. For build-ups, you could purposely disconnect STEREO LINK for a “crazy” stereo effect and re-engage LINK for sum-total equalization—using as part of your section changes.

---

## 5. **Utility: Leveling & Polishing a Modular Mix**

- The **Input Level**, **Makeup Gain**, **Threshold** and **Ratio** give you classic mixing/production moves otherwise hard to automate cleanly in modular:
    - Make diverse levels consistent across sections
    - Tame rogue peaks and fatten thin sequences
    - Shape the sustain and punch of drums for arrangement contrasts

---

## 6. **Song Structure in Modular: Practical Scenarios**

Here are a few workflow patch ideas building on the Stereo Compressor:

### **A. Dynamic Drops**
- **Verse**: No/low compression, gentle gain.
- **Chorus/Drop**: Flick up compression ratio & gain + engage sidechain from rhythm trigger.
- **Breakdown**: Hit BYPASS, kill make-up gain, or send extremely low sidechain for a “vacuum” feeling.

### **B. Morphing Groove**
- Use a sequencer or performance controller (Tetrapad, Planar, etc.) to modulate compressor parameters, so each “pattern” or song scene has its own compression feel.

### **C. Stereo Madness for Builds**
- Before a drop, pan your signals hard L/R, defeat STEREO LINK for wild imaging, then slam STEREO LINK and tight compression for the drop—super punchy and “wide-to-mono” effect.

---

## **Pairings: Recommended Module Combos**

- **Sequencers** (for song structure control): Eloquencer, NerdSeq, or Five12 Vector.
- **Switches/VCAs**: Mutate and automate sidechain input sources.
- **Modulators**: Convert LFO or envelope pressure into dynamic, evolving compressor actions.
- **Stereo Mixers & FX**: Apply compressor after your last-stage stereo output; combine with wet/dry “send” setups.
- **Performance Controllers**: Use expressive surfaces to control compression in real time as part of the song arrangement!

---

Combining the Erica Synths Stereo Compressor with routing, modulation, and performance control empowers you to create full-length, professional-sounding song structures in Eurorack—whether tightly sequenced or deeply improvisational!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)