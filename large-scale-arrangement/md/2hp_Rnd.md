# 2hp — Rnd

- [Manual PDF](../../manuals/2hp_Rnd.pdf)

---

[**2hp Rnd Manual PDF**](https://2hp.com/wp-content/uploads/2018/07/2hp-RND-Manual.pdf)

---

# How To Use The 2hp Rnd Module To Create Full Length Songs in Eurorack

Creating an evolving, structured full-length song in Eurorack can be challenging since the modular environment often encourages short, interesting patterns or “moments”. The 2hp Rnd module, a compact random voltage and gate source, is a powerful but flexible tool to inject variation, introduce structure, and help transform repeating patterns into dynamic compositions. Here are strategies and patch ideas for leveraging the Rnd, in combination with other modules, to move beyond loops into song form.

---

## 1. **Evolving Melodic and Harmonic Variation**

Rnd provides two independent random voltage sources — Quantized and Smooth — each with its own attenuator:

- **Quant Output**: Stepped random voltages at each clock pulse.
- **Smooth Output**: Continuously fluctuating random voltages.

**Patch Idea:**
- **Melodic Sequences:** Use the Quant output to modulate the 1V/Oct input of a quantizer or oscillator, clocked by your main rhythm or phrase clock. This will “refresh” melodies in sync with your groove, adding non-repetitive notes at each bar or measure.
- **Song Structure Variation:** Crossfade or switch between several quantizer scales (using switches or VCAs) that are selected by another random (or controlled) source to move between verse, chorus, and bridge sections.

---

## 2. **Dynamic Rhythmic Changes**

The Gate output from Rnd can be used in two ways:
- As a straight clock (50% pulse) in “Int” mode.
- As random gates in “Ext” mode, triggered at the probability set by the Rate knob.

**Patch Idea:**
- **Percussive Variations:** Use the Gate output to trigger envelopes or drum modules, introducing rhythmic “fills” or surprises that break up static beats.
- **Random Pattern Re-combination:** Route the random gate to a sequential switch, logic module, or drum trigger input. This can create generative rhythm–useful for breakdowns or bridges.

---

## 3. **Automated Modulation for Dynamic Change**

Smooth random voltages can animate filters, effects, or mix levels:
- **Slow Modulation:** Rate knob left = slow, evolving timbres for intros, ambient sections, or long builds.
- **Fast Modulation:** Rate right = FM textures, glitchy filter sweeps, or granular effects for breakdowns or drops.

**Patch Idea:**
- **Scene Transitions:** Use Smooth output to modulate send levels to reverb/delay, or the cutoff of a filter, creating swelling effects that signal changes between song sections.
- **Fade-ins, Fade-outs:** Route Smooth output through a VCA to automate volume over time for gradual intro/outros.

---

## 4. **Probability-Based Section Changes (Song Structure)**

By externally clocking the Rnd in “Ext” mode, and using the Rate knob to set the chance of high/low output, you can use the Gate out to control when major changes should happen:

- **Patching Example:** Patch the Gate out to trigger a Sample & Hold that controls a main sequencer’s reset, pattern change, or switch between melody lines.
- **Song Movement:** Combine multiple random sources (Rnd plus another S&H or noise module) to probabilistically switch between song “scenes”–for example, moving to choruses or breaks.

---

## 5. **Combinatorial Control with Other Utilities**

Rnd excels as a source for cross-patching to VCAs, logic, sequential switches, or preset morphers:

- **Use Attenuators**: The dedicated attenuators at each output allow tight control, so you can set subtle or extreme modulation depth for precise musical impact.
- **Layered Randomness:** Stack Rnd’s outputs with another LFO/random module for even more organic, less predictable structures (e.g., “Random gates only open when Rnd’s smooth output is above 5V”).

---

## **Putting it All Together: Example Song Structure Patch**

- **Intro:** Use slow Smooth output to fade in the level of pads or textures.
- **Main Beat:** Clock the Quant output with your main clock for evolving basslines/melodies.
- **Build/Breakdown:** Switch the Gate out from steady clock to random gates to trigger fills, filter sweeps, or sudden reverb swells.
- **Chorus:** Use a logic module driven by multiple gates (e.g., main clock AND Rnd gate) to switch in extra voices or layers.

By carefully integrating Rnd’s outputs into melodic, rhythmic, modulation, and structural roles, you can orchestrate non-repetitive, living song structures without tedious manual intervention, opening up the full compositional potential of modular synthesis.

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**