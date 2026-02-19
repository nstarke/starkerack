# Intellijel — Plonk

- [Manual PDF](../../manuals/plonk_manual_v1.16_2020.11.08.pdf)

---

[Plonk Physical Modeling Percussion Synthesizer – Manual PDF](https://intellijel.com/downloads/manuals/plonk_manual_1.16.pdf)

---

## Using Intellijel Plonk for Densely Rhythmic, Hyper-Complex Percussion Sequences

As a eurorack artist, Plonk gives you powerful tools to create intricate, dynamic, and unique percussion—ideal for polyrhythms, odd time signatures, and highly detailed patterns. Below, I break down how to maximize Plonk's potential for rhythmic complexity and percussive punch, focusing on both its synthesis engine and modular patching strategies.

---

### 1. **Patch Plonk As Its Own Percussive Voice Bank**

Plonk is a voice—not an effect—meant for physical modeling percussion and tuned percussion synthesis. It excels in creating both natural and bizarre percussive sounds.

- **Duo-Voice Polyphony:** Plonk is duophonic, letting one voice decay naturally while a new strike occurs. This means overlapping hits (not just choked retriggering), which is fantastic for dense rhythmic textures.
- **128 user presets:** Set up a variety of drums, metals, woods, glitchy textures, and melodic perc. These can be stepped or morphed in real-time for evolving sequences.

---

### 2. **Sequencing for Polyrhythms and Complex Patterns**

- **Clock & Trigger Inputs:** Sequence the TRIG input from multiple rhythmic sources (Euclidean sequencer, random pulse generators, clock dividers/multipliers, etc.). 
- **Compound triggers:** Use logic modules (AND, OR, XOR) to sum or intersect various gates for emergent rhythmic patterns.
- **MOD Input as Preset Step/Select:** Assign the MOD CV input to “Preset Step” and sweep through preset kits (e.g., kicks, snares, hats) with distinct modulation voltages. The default preset is set up as a pseudo drum kit, and you can create your own articulated kits.
- **Offset Rhythms:** Feed gates from sequencers set to different divisions (e.g., 3 vs. 4, or 7 vs. 5 steps) for true polyrhythms, letting Plonk ring out notes independently.

---

### 3. **Complex Time Signatures**

- **Non-Uniform Sequencing:** Use sequencers that can handle step counts not divisible by 2, 4, or 8. Plonk's fast trigger input will respond to any odd cluster of gates—create "strange" groove cycles.
- **CV Addressing:** Use the MOD, X, or Y inputs with random/chaotic CV sources (e.g., Turing machine, LFOs with odd rates, or stepped random) to evolve Plonk parameters in time, further complicating rhythm.

---

### 4. **Make Each Hit Unique, Punchy, and Percussive**

#### A. **Manipulate Voice Characteristics**

- **Velocity (VEL) Input as Dynamics or Timbre Control:** Feed velocity-sensitive gate or random CV to the VEL input for expressive, non-static hits. Set VEL mode to “Dynamics” for realistic drum articulation.
- **Exciter Parameters:** Dial in snappy, punchy attacks (high stiffness mallet, short decay) for kicks and snares, or use Noise/exciter for claps, hats, and more abstract percussion.
- **Object (Resonator) Parameters:** Model a variety of surfaces (e.g., marimba, membrane, plate) for broad sonic territory. Inharmonicity, position, and tone settings push realism or bring out 'unreal' metallic/buzzing effects.

#### B. **Advanced Modulation**

- **Assign CV to X/Y/Mod Destinations:** Routinely change tone, decay, mix, density, or pitch envelope for complex, evolving percussion. Modulate “Noise Density” for granular, glitch hats; “Resonator Decay” for ghost notes.
- **Morph and Randomize:** Use the MOD input in “Morph” mode to sweep between substantially different preset timbres in real-time. Or, trigger “Randomize” for bursts of new percussive ideas—ideal for fills or surprises.

---

### 5. **Integration with Effects and the Rest of Your Rack**

- **Saturation & Bitcrusher:** Use onboard saturation and bitcrusher (assignable as CV destinations) for aggressive, digital, or degraded percussion. Automate these for stutter/cut-up/glitch effects during fills.
- **Choke Controls:** Use gate signals on the MOD input set to “Choke Both/Noise/Res” to instantly cut sustaining sounds—critical for realistic open-to-closed hat articulations or tight staccato grooves.

---

### 6. **Preset Management for Performance**

- **Preset Morphing and Stepping:** Rapidly step or morph between entire kits, or between “sound families,” via MOD CV—great for live sets requiring drastic changes within a sequence.
- **Preset Storage:** 128 presets = "drum machine in a module"; program full kits or mapped sounds for fast access in performance.

---

## **Summary Patch Ideas for Hyper-Complex Percussion**

- *Polymetric LFOs or Sequencers* → TRIG/VEL/MOD/X/Y for varied hit placement and articulation
- *Preset Kits* with MOD/Preset Step, selected live by voltage
- *Random Gates* on MOD (Randomize or Choke) for fills/glitch points
- *Fast CV* to Bitcrusher/Saturation for stutter/distortion ‘effects’ per hit
- *Quantized CV* on pitch for tuned percussion + evolving quantize/scale

---

For more technical information, download the full PDF manual:  
[Plonk Official Manual PDF](https://intellijel.com/downloads/manuals/plonk_manual_1.16.pdf)

---

*Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)*