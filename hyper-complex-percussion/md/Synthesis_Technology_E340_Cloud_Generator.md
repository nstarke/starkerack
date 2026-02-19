# Synthesis Technology — E340 Cloud Generator

- [Manual PDF](../../manuals/E340_manual.pdf)

---

[Download E340 Cloud Generator Manual (PDF)](http://www.synthtech.com/docs/E340_manual.pdf)

---

## Using the Synthesis Technology E340 Cloud Generator for Densely Rhythmic, Hyper-Complex Percussion

The **E340 Cloud Generator** is a powerful "swarming" VCO rather than a drum module, but with creative patching, you can coax unique, polyrhythmic, and percussive textures ideal for advanced rhythmic music. Here’s how you can exploit its capabilities for the complex percussion and sequencing styles you want:

---

### 1. **Percussive Sound Design with Voice Architecture**

- **Pinged Sine Bursts:**  
  Ping (trigger) the *SYNC* input with gates/triggers from rhythm generators or sequencers. At extreme *SPREAD* and *CHAOS* settings, the SYNC jack will rhythmically reset all VCOs, making tight, snappy "plucks" and percussive sine hits—especially with sharp decay VCAs.
- **Super-Saw Claps/Snares:**  
  With *SAW OUT*, high *SPREAD*, and *CHAOS* (plus CV control for animated movement), short triggered envelopes through a VCA can carve the resulting wall of detuned saws into clap/snare-like textures.
- **FM Percussion:**  
  Patch velocity-sensitive, stepped, or rhythmic modulation into the *FM CV* input for pitched toms, congas, or metallic percussion. Envelope or LFO-driven FM can add tip-top punch and complexity to each "hit."

### 2. **Creating Hyper-Complex Patterns & Polyrhythms**

- **Polyrhythmic Sequencing:**  
  Use multiple, interlaced clock/triggers to the *SYNC* jack, or rhythmically modulate *SPREAD* and *CHAOS* with different polyrhythmic envelopes, LFOs or sequencer rows. Each VCO responds uniquely to spread and chaos, creating layered micro-timing within the cloud.
- **Multiple Modulations:**  
  Assign independent rhythm sources to the *SPREAD CV*, *CHAOS CV*, and *CHAOS BW CV* for evolving, irregular spectral glitches and “swarming” accents. Use logic modules or clock dividers/multipliers to achieve meta-rhythms.
- **Density Variation for Dynamic Texture:**  
  Switch between 2/4/8 VCOs live as part of the rhythm sequence (using manual or CV switches via external means). Fewer VCOs for crisp, loud hits; more VCOs for lush, clustered “clouds.”

### 3. **Patch Example for Unique Percussive Patterns**

```markdown
1. Main rhythmic clock pulse to SYNC for "strike" events.
2. Envelope generator (with variable decay) into FM CV,
    clocked polyrhythmically against the SYNC clock.
3. Chaotic stepped random or a Euclidean LFO modulates SPREAD CV for micro-timing and pitch spray per hit.
4. CHAOS CV is modulated by a slow, off-time LFO or evolving stepped CV source to animate timbre over bars.
5. Output (SAW or SINE) into a VCA controlled by short envelopes—use one per output or blend for multi-stack drum timbres.
6. Routings can also include parallel ring-mod or wavefolder modules for metallic percussion textures.
```

### 4. **Patch Strategy Tips for Percussive Use**
- Keep *SPREAD* and *CHAOS* in motion—even subtle modulations add complex, organic "imperfections" essential for dynamic percussion.
- Use external VCAs with fast attack and variable decay envelopes to sculpt attack shapes from the raw waveforms.
- Try random or algorithmic sequencers (like *Pam’s New Workout, Marbles, or Zularic Repetitor*) to drive the CV ins for non-repetitive, unexpected results.
- Clock-modulate *CHAOS BW* for “granular” variations in attack transients.

---

### 5. **Additional Processing for Punch & Character**
- Run the E340’s outs through highpass filters or transient shaping modules post-VCA to emphasize click and reduce low droning.
- Further saturate or wavefold the output for metallic or noise-based percussion.
- Layer with other sound sources for composite percussion, using the E340 primarily for airy/lush/fizzing or detuned impact layers.

---

## Conclusion

The E340, while not a drum module per se, is a powerful textural and spectral oscillator for animated and complex polyphonic percussion layers, especially when sequenced and modulated with polyrhythmic patterns. CV control is your key to rhythmic density.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)