# 2hp — 3 to 1

- [Manual PDF](../../manuals/3_To_1_Manual.pdf)

---

[3:1 Module Manual PDF (2HP)](https://2hp.com/manuals/2hp-3to1-manual.pdf)

---

# Using the 2hp 3:1 for Densely Rhythmic & Hyper-Complex Percussion in Eurorack

The **2hp 3:1** is a voltage-controlled gate switch and summer, perfectly suited for creative rhythmic manipulation. Below are strategies and patches for generating dense, complex, polyrhythmic percussion using this module.

---

## 1. **Sequenced Gate Switching for Percussive Complexity**
- **Patch multiple gate/trigger sources** (e.g., clock dividers, Euclidean sequencers, random gates) into IN 1, IN 2, and IN 3.
- **MODULATE the SEL CV** input with a fast, unpredictable source (e.g., random stepped CV, sample & hold, or another sequencer). This causes the output rhythm to rapidly switch between input patterns, generating complexity.
- **Result:** The output combines or flips between different grooves/patterns, yielding a fused hyper-rhythmic sequence.

---

## 2. **Gate Summing for Polyrhythms & Time-Signature Crossings**
- Set the **MODE toggle** to the right (gate summing mode).
- Feed different rhythmic divisions or polymeter sources (e.g., 3-step and 4-step patterns, or sequencer & clock division outputs) to the three inputs.
- The output will fire **triggers when any of the inputs receive a gate** or trigger—by combining non-aligned patterns, intricate polyrhythms and time signatures such as 3:4 or even cross-rhythms are easily created.
- The output triggers are **normalized to 5 ms pulses,** great for clean, punchy percussion triggering.

---

## 3. **Voltage Controlled Rhythmic Morphing**
- Patch a **modulation source** (LFO, envelope, or stepped random CV) to **SEL CV**.
- Slowly modulate across the input selection in selective switch mode (MODE left). This "morphs" between gate/trigger sources, letting you transition abruptly or gradually between different rhythmic feels or phrases.
- **Manual SEL knob** lets you perform live, hands-on selection for expressive fills or variation.

---

## 4. **Trigger Manipulation & Cleansing**
- In **summing mode**, the 3:1 outputs 5ms triggers **regardless** of input pulsewidth. Use this as a way to "sharpen up" muddy or uneven gate lengths from DIY or old gear, or to extract crisp triggers from complex sources.
- **Chain with analog percussion voices:** these clean pulses work excellently for snappy drums and percussive synths.

---

## 5. **Complex Signal Routing for Percussive FX**
- Route the 3:1 output to multiple voices or effects using a sequential switch after the module, or feed output to audio-rate frequency dividers for chopped, stuttering textures.
- Invert, delay, or process the OUT with logic modules for even *deeper* rhythmic complexity.

---

### **Creative Tips**
- **Gate Length:** If downstream modules are sensitive to gate length, always use SUM mode for short, snappy triggers.
- **Control Input SEL with a clocked sequencer:** This can generate predictable but dense and MIDI-like polymetric structures.
- **Stack outputs:** Use stackable cables to send the OUT to multiple percussive sound sources.
- **Integrate with randomness:** Sample & Hold or Turing Machine derivatives to SEL CV create generative, never-repeating percussion.

---

> For full technical details, **consult the [official 2hp 3:1 manual here (PDF)](https://2hp.com/manuals/2hp-3to1-manual.pdf).**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
