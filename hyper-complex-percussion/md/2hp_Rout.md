# 2hp — Rout

- [Manual PDF](../../manuals/Rout_Manual.pdf)

---

[2hp Rout Manual PDF](https://2hp.com/wp-content/uploads/2019/05/2hp-Rout-Manual.pdf)

---

## Using 2hp Rout for Hyper-Complex Percussion and Rhythmic Patterns

**2hp Rout** is a voltage-controlled gate/trigger switch that routes one input to one of four outputs, under manual or CV control. While simple in concept, it is *highly* potent for generative, polymetric, and polyrhythmic architectures.

Below are advanced, musical strategies for leveraging Rout to build dense, intricate percussion and rhythm:

---

### 1. **Polyrhythmic Trigger Distribution**

- **Clock Dividers/Multipliers:** Inject a high-speed master clock or polymetric trigger train from a sequencer or clock module (like Pamela’s NEW Workout or Tempi) into Rout’s INPUT. Use several independent clock divisions (e.g., /3, /5, /7) as modulation sources patched to **SEL CV**.
- **Outcome:** Rout dynamically re-routes a single, fast fluid rhythm into four destination voices or percussion modules, according to the interplay of several unrelated rhythms, creating emergent polyrhythms.

---

### 2. **Complex Time Signature Sequencing**

- **Step Sequence the Rout Selection:** Use a voltage sequencer (e.g., Make Noise Pressure Points, Malekko Voltage Block) clocked in a complex time signature (e.g., 7/8, 5/4, or Euclidean patterns) to supply changing voltages to **SEL CV**.
- **Result:** The switching logic splits a main sequence, reassigning individual trigger/gate steps to different percussion voices, allowing you to cycle through “odd” patterns across a four-voice drum kit.

---

### 3. **Algorithmic or Generative Drumming**

- **Randomized/Probabilistic Routing:** Patch a stepped random voltage (e.g., Wogglebug, Pamela’s Random, or Sapèl) to **SEL CV**. The random CV causes Rout to bounce the same trigger to various destinations unpredictably—fantastic for glitch, IDM, breakcore, or evolving machine music.
- **CV Quantization:** Use a CV quantizer on **SEL CV** to keep output switching snappy and rhythmically aligned.

---

### 4. **Pattern Variation & Fills**

- Use a manual offset voltage as a “fill” or “break” selector—add an offset from a fader, joystick, or a footswitch to force Rout to select a particular output (e.g., a snare fill or rim hit).
- Employ logic modules or comparators to toggle Rout’s selection on-the-fly, injecting burst energy during particular sections.

---

### 5. **Multi-Voice Percussion Engine**

- Send a single dynamically evolving gate/trigger pattern into Rout’s INPUT.
- Route outputs to four distinct percussive modules (kick, snare, hi-hat, and percussion voice).
- By modulating **SEL CV** rapidly, you can "jump-cut" different percussion modules’ hits from a single rhythm, building stuttered, fractured, and intricate beat structures.

---

### 6. **Creative Effects Routing (if patched with effect units)**

- **Live FX Chopper:** You can gate on/off effects by sending gates or audio pulses through Rout, switching between four different FX chains or parallel processing paths in sync with the rhythm.

---

#### ***Quick Tip***:
- **Envelope Synchronicity:** Use Rout to send triggers to envelope generators that control percussive synth voices with different decay, wavefolding, or filter characteristics per channel for extremely varied and punchy output.

#### ***Perceptual Punch***:
- Exploit Rout’s abrupt switching for “machine gun” fills or polymetered gate overlaps—combine with analog processing (VCAs, filters, wavefolders) downstream for even greater punch and timbral variety.

---

## Patch Example

1. **Input:** High-paced Euclidean or binary trigger from a clock/module.
2. **SEL CV:** Complex voltage pattern from a sequencer or random stepped voltage.
3. **Outputs 1-4:** Trigger four distinct percussive voices or drum modules.
4. **(Optional):** Route CVable parameters (timbre, decay, pitch) of your drum modules to dynamic gates for wild sonic movement.

---

By cleverly sequencing and CV-modulating the output selector, **Rout** becomes a backbone for hyper-rhythmic, unpredictable, and intricate musical systems that are always evolving.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)