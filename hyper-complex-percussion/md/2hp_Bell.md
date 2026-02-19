# 2hp — Bell

- [Manual PDF](../../manuals/2hp_Bell.pdf)

---

[2hp Bell Manual PDF](https://2hp.com/wp-content/uploads/2hp-bell-manual.pdf)

---

# Using the 2hp Bell for Complex, Densely Rhythmic, and Hyper-Complex Percussion in Eurorack

The 2hp Bell is a **polyphonic melodic percussion generator** based on modal synthesis, best suited as a *voice* module in your Eurorack setup. Its strengths for the creation of intricate percussion lie in its wide model selection, CV-controllable parameters, and ability to sharply articulate or drastically dampen metallic sounds. Here’s how you can leverage it for advanced, rhythmically dense music making:

---

## Strategies for Generating Dense, Complex Percussion

### 1. **Exploit Polyphony & Fast Retriggering**
- **6-Voice Polyphony** lets you layer overlapping rhythms—send multiple triggers in fast succession (using clock dividers/multipliers or burst generators) to saturate the sound with metallic, bell-like percussion to create textural “clouds.”
- Pair with eurorack sequencers or trigger modules (like Euclidean sequencers, or Varigate) programmed with polyrhythms (e.g., 5 against 4, 7 against 3) for wildly complex results.

### 2. **Create Polyrhythms and Complex Patterns**
- Patch several out-of-phase trigger generators (e.g., Pamela’s New Workout, Zularic Repetitor, or logic gates combining triggers from different clocks) into the **TRIG** input.
- Use probability or conditional triggers for evolving patterns; let the Bell’s voices “overlap” at odd intervals for density.

### 3. **Use Model CV for Rapid Timbre Shift**
- Patch stepped random, sequenced, or rhythmic CV into **MODEL** to “flip” between physical models (vibraphone, marimba, bowl, etc.) in sync or off-sync with your rhythm, keeping timbre in motion as your patterns evolve.
- Bipolar CV (-5V to +5V) allows tight or wild sweeps—use slow modulation for gradual evolution or audio-rate for pseudo-FM metallic clangs.

### 4. **Modulate Damp for Percussive Variation**
- Assign envelopes, random, or stepped modulation to **DAMP**. A tight envelope means crisp, short hits; a slow one gives hanging, resonant decays.
- Change decay characteristics per trigger for dynamic groove and mutating tail lengths—essential in complex, humanized percussion.

### 5. **Sequence Pitch and V/Oct for Melodic Percussion**
- Drive **PITCH** and **V/OCT** with a sequencer to create tuned percussion arpeggios. 
- For pitch slides, use slewed CV or LFOs; combine quantized melody lines with unquantized microtonal variance for complexity.
- Interleave melodic sequences with rhythmic triggers for tone clusters and bell-chords in odd rhythms.

### 6. **Further Processing for Punch and Character**
- Multi-patch Bell outputs to wavefolders or distortion modules for harsher, more aggressive hits.
- Route through dynamic processors (VCAs/envelopes) or rhythmic effects (delays set to non-standard clock divisions) for additional pattern complexity.
- Layer Bell with traditional drums for punch, using its timbral sharpness to accentuate or contrast other percussive layers.

---

## Example Patch for Complex Hyperpolyrhythm

**Modules:**
- Pamela’s New Workout or Temps Utile (polyrhythmic triggers)
- Turing Machine or random CV source (for unpredictability)
- Quantizer (for V/Oct sequences)

**Patch idea:**
1. Patch several independent clock divisions/multiplications to Bell’s **TRIG**.
2. Sequence **MODEL** with random CV and quantize to force model changes on every 3rd/5th/7th hit.
3. Use envelope with random length or a burst from a logic gate to **DAMP** for evolving decay.
4. Generate melody for **V/Oct** using a rotating quantized sequence, clocked at a prime division relative to the main rhythm.
5. Feed Bell output to a VCA controlled by another envelope or dynamic processor for punch.
6. Patch output through a wavefolder or distortion for metallic aggression.

---

## Manipulating for Unique, Punchy, and Percussive Sounds
- **Short Damp, Sharp Envelope:** For in-the-pocket high-clarity percussion, combine very short decay with punchy envelopes downstream.
- **Switch/Randomized Models:** Use sample & hold or random CV to force the Bell through different metallic objects in sequence or at unpredictable moments.
- **Fast Retrigger:** Overlap triggers <50ms apart for granular metallic shimmer.
- **Audio-rate Modulation:** Modulate **MODEL** or **DAMP** at audio rates for unnatural, digital clangs and “cyborg” chimes.
- **VC Mixer:** Mix Bell with other percussive modules and stereo pan/ring modulate for further density/complementation.

---

For deep, unpredictable, and richly layered techno, breakcore, IDM, or generative percussion, the Bell’s combination of **polyphony, modulation destinations, and physical modeling** makes it a miniature powerhouse.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)