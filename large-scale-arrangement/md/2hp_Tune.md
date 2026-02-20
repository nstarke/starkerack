# 2hp — Tune

- [Manual PDF](../../manuals/Tune_Manual_2023.pdf)

---

[2hp Tune Module Manual (PDF)](https://cdn.shopify.com/s/files/1/0585/4070/5019/files/Tune.pdf)

---

# Using the 2hp Tune to Create Full Length Eurorack Songs

The **2hp Tune** is a voltage quantizer for Eurorack synthesizer systems, turning incoming CV into quantized pitches within a selectable musical scale. While quantization is a basic tool, this module can be used for sophisticated musical arrangement across full-length compositions when paired with appropriate patching strategies and other modules.

Below is an analysis of how to incorporate the 2hp Tune into song-length structures in your modular setup.

---

## Core Capabilities of the 2hp Tune

- **CV Quantization**: Locks incoming voltages to musical notes within a scale.
- **Scale Selection**: 11 music scales including major, minor, pentatonic, whole tone, octatonic, and more, selectable by knob or CV.
- **Bias Control**: Shifts the quantized output across the scale diatonically, allowing transpositions and modal movement.
- **LED Feedback**: Visually abled scale and control status for performance confidence.
- **Output**: Clean 1V/oct quantized pitch for oscillators and synth voices.

---

## Strategies for Creating Full Length Songs

### 1. **Melodic Variation & Transposition**
- **Cycling Melodies:** Use a sequencer or random CV generator (like Turing Machine, Ornament & Crime, or a simple sample & hold) into 2hp Tune’s Input. The output will always stay in scale, even as the sequence changes or is randomized.
- **Transposing Sections:** Use the **Bias CV input** to shift the root note of the melody over time—route a slow LFO, stepped CV (from sequencer, or scene recall from modules like Voltage Block), or manually modulate the Bias knob live to move between different "song sections" or keys.

### 2. **Changing Scales for Song Sections**
- Assign different scales to correlate with song structure: major for verses, minor for chorus, diminished or whole tone for bridges. You can automate this with a sequencer sending CV to the **Scale CV input** (you'll need a module that outputs precise voltages or triggers—like a programmable CV source).
- The Scale LEDs give immediate feedback for live performance or improvisation.

### 3. **Automated Melodic & Harmonic Progressions**
- Use two or more 2hp Tune modules: Route different CVs into each—one for bass, one for melody/harmonies. Change their scales independently (or together via multed Scale CV) for complex, evolving harmonic structures.
- Create chord progressions: Use quantized outputs to drive oscillators or poly-oscillator modules. With a clever gate/CV sequencing and multing, you could even mimic chord changes and arpeggios.

### 4. **Integration with Rhythm and Structure**
- **Tidy up Basslines:** Patch random or sequenced CV into Tune for your bass voice, guaranteeing every note is ‘in key’—pairs well with algorithmic drum/rhythm generation.
- **Song Phrasing:** Chain CV from a voltage-addressed sequencer or scene-based performance module to both Tune’s Scale and Bias inputs. This creates distinct verse/chorus/bridge/intro sections via scale and pitch movement.
- **Automation & Transitions:** Change scales or bias at specific moments using gate-to-triggered CV, synced to your master clock or performance gestures.

### 5. **Performance and Live Jamming**
- **Manual Scale/Bias Changes:** The front-panel knobs are performance-friendly; transition between sections, create tension with bias shifts, or “lift” the energy with a sudden mode change.
- **Visual Cues:** The bright scale LEDs give quick feedback during improvisation for tight, confident live sets.

### 6. **Advanced: Algorithmic & Generative Song Structures**
- Combine with logic, switch, and clock divider modules to algorithmically change the mode, bias, and even which sequencer drives Tune—resulting in generative song forms that evolve over time but remain harmonically coherent.
- Use tuners, comparators or precision adders to fine-tune how the CV morphs and transitions over a long performance.

---

## Example Patch for Evolving Song Structure

**Modules Suggested:**
- Sequencer (e.g., Pamela’s New Workout, Rene, SQ-1)
- Random/Noise CV Source
- Slow LFO
- Precision Adder or Attenuverter (for voltage control)
- VCO(s)
- Envelope and VCA
- Drums/percussion modules

**Workflow:**
1. Sequencer or random source → 2hp Tune CV Input.
2. 2hp Tune Output → VCO 1V/oct input (melody or bass OSC).
3. Multi-stage CV (from voltage block, LFO, or scene-based sequencer) → Bias CV (to switch “root note”/scale degrees at specific moments).
4. Step CV or gate pattern → Scale CV input for automatic scale changes (verse/chorus).
5. All rhythm and melodic triggers/gates clocked in sync for tight song structure.

This lets you create dynamic, changing melodies and song parts with scale and root shifts, enabling full length song performance and arrangement directly in-the-rack.

---

## Conclusion

While the 2hp Tune is a small quantizer, its full-scale and bias control unlocks powerful musical possibilities across a whole composition, especially when combined with scene, sequence, and modulation sources. Its utility for both generative and tightly-sequenced music makes it invaluable for creating organized, engaging full-length songs in modular environments.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)