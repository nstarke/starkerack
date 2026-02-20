# Rebel Technology — Stoicheia

- [Manual PDF](../../manuals/Stoicheia – Rebel Technology.pdf)

---

[Stoicheia Manual PDF](https://raw.github.com/pingdynasty/EuclideanSequencer/master/EuclideanSequencerSchematic.png)

---

# Using the Rebel Technology Stoicheia to Build Full-Length Eurorack Songs

As an experienced Eurorack musician, you know that modular rigs let you patch up endless grooves, melodies, and textures, but turning those short loops and patterns into enticing, evolving, song-length pieces is another art form entirely. The **Stoicheia** dual Euclidean sequencer (see [full manual above](https://raw.github.com/pingdynasty/EuclideanSequencer/master/EuclideanSequencerSchematic.png)) is a powerful tool for rhythmic organization and transformation—let’s break down practical strategies to use it for full-length arrangement and performance.

---

## Key Stoicheia Features

- **Dual independent Euclidean sequencers**
- **Variable sequence length** (1–16 steps per sequencer)
- **Variable number of fills/hits** (1–length)
- **Sequence rotation (start step shift)**
- **Modes:** Trigger, Alternating, Chained
- **Reset input for re-synchronization or pattern changes

---

## Songwriting and Arrangement Approaches

### 1. **Multiple Sections with Parameter Modulation**

**Patch Idea:**  
- Use one channel for drums (e.g., kick), the other for hats or claps.
- Vary _length_ and _fills_ (manually, with CV if using external utilities, or with an external controller).
- Use _rotation_ control for subtle groove changes—especially effective for fills or breaking monotony.

**Song Programming:**  
- Use a sequencer or automation module (like **Planar2**, **Tetrapad**, or **Pamela's New Workout** expander) to change Stoicheia parameters at pre-planned moments.
- Program “sections” (e.g., A/B/C/Break) by reconfiguring the fills, length, or rotating the patterns.
- Send timed reset triggers from another sequencer, clock divider/multiplier (like **Pamela's New Workout** or **Clock Divider**), or even a DAW-clocked impulse, to synchronize scene changes.

### 2. **Chained Mode for Extended Patterns**

**Patch Idea:**  
- Set Chained Mode to combine the two internal sequencers into longer, non-repeating patterns.
- Example: First channel 12 steps, second 4 steps = 16-step cycle, but with shifting downbeats over time.
- Use this for polyrhythmic interest, intro/outro sections, or “verse/chorus” contrast.

**Practical Use:**  
- Dynamically switch into Chained Mode during a performance to introduce a new section or to grow rhythmic complexity.
- Reset at phrase boundaries for tight transitions.

### 3. **Layering and Complex Grooves**

**Patch Idea:**  
- Use both channels for percussive voices: kick/snare, tom/clap, etc.
- Cross-patch the two outputs to trigger different drum modules, envelope generators, or clock other event-sequencing tools (e.g., **Mutable Instruments Branches**, **Rene**, **Pressure Points**).
- Use a sequential switch or matrix mixer (e.g., **Doepfer A-151**, **Livestock Electronics Maze**) to alternate or layer Stoicheia’s outputs throughout your song.

**Song Programming:**  
- Vary which percussion instruments are triggered by using mute switches or sequential switches, allowing arrangement evolution over time.

### 4. **Breaking Out of Loops with External Control**

**Patch Idea:**  
- Use external reset triggers (from a performance controller, random gate, or even your DAW) to unsync periodicity, creating intentional glitches or reset points—great for breakdowns, fills, or transitions.

**Integrating Melody/Bass:**
- Use Stoicheia patterns to trigger note events in a pitch sequencer (e.g., **Voltage Block**, **Metropolis**, **O_C**, or **Arturia Keystep**) to drive melodies/bass lines in rhythmically evolving ways.
- Alternate between Euclidean pulses and regular straight clocks to the same sequencer for “verse/chorus” transitions.

### 5. **Transitions and Arrangement Techniques**

- **Manual Tweaking:** Turn length and fills in real time to build/strip down arrangements—e.g., start minimal, then increase fills for a “drop,” decrease for a “breakdown.”
- **Automated Scenes:** If you have a programmable switch or macro CV controller, script parameter changes to create a song’s flow hands-free.
- **Layered Resets:** Use synced or offset resets to bring different musical elements (Stoicheia, pitch sequencer, modulation sources) into or out of phase, adding tension/release points.

---

## Example Song Structure with Stoicheia

| Section    | Pattern Length | Fills | Mode         | Other Actions                        |
|------------|---------------|-------|--------------|--------------------------------------|
| Intro      | 8             | 1-2   | Trigger      | Minimal percussion                   |
| Build      | 8             | 3-5   | Trigger      | Add hats, more fills over time       |
| Drop       | 8 or Chained  | 6-8   | Chained      | Upshift fills/length, layer outputs  |
| Break      | 16            | 2-4   | Alternating  | Trigger melody, rotate patterns      |
| Outro      | 4-8           | 1-2   | Trigger      | Reduce to minimal, then full stop    |

**Throughout:** Use reset inputs, switch modes, and rotate patterns for bridges/fills.

---

## Advanced Tips

- **VCAs & Modulation:** Patch Stoicheia outputs to modulate VCAs for chopping audio, or to trigger random CV generators for probabilistic melodies.
- **Open Hardware/Firmware:** Modify or reflash the firmware (see [GitHub](https://github.com/pingdynasty/EuclideanSequencer)) for customized behavior, or hack in CV control over length/fills.
- **Combining Multiple Euclidean Modules:** Layer Stoicheia with other Euclidean, random, or traditional sequencers for deep generative potential—keep transitions manual or automate them for live performance.

---

## Final Thoughts

With careful use of Stoicheia’s parameter changes, chaining, and sync/reset, you can morph static loops into full-length, expressive modular songs. Pair it with scene control, manual or automated modulation, and clever cross-patching for truly dynamic modular compositions.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)