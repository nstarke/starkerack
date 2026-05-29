# Noise Engineering — Integra Solum

- [Manual PDF](../../manuals/Integra Solum Manual - Noise Engineering Documentation.pdf)

---

[Manual PDF / Documentation](https://manuals.noiseengineering.us/is/)

# Noise Engineering Integra Solum — Cheat Sheet

## What it is
Dual rotating clock divider / trigger generator with **2 independent sides**, each with:
- **1 Clock input**
- **1 Reset input/button**
- **1 Shift (offset) control/CV**
- **8 trigger outputs**
- **1 mode selector**

A single clock and/or reset can be used for both sides thanks to **normalled inputs**.

## Quick use
1. Patch a clock into either **Clock** input.
2. If only one clock is patched, it **normals to both sides**.
3. Choose a **Mode** on each side:
   - **/2N** = powers-of-two divisions
   - **N** = sequence of 8
   - **/2N+1** = odd-number divisions
4. Turn or CV the **Shift** control to rotate which output is “first.”
5. Patch any of the **8 outputs per side** to envelopes, drum voices, switches, sequencers, etc.
6. Use **Reset** input/button to restart the pattern alignment.

---

## Controls

### Shift knob / CV
- Rotates the output order.
- Example: **jack 2 becomes step/output 1**, then jack 3, etc.
- Lets you re-map the rhythm across the 8 outputs without changing the clock.

### Mode switch
Three standard modes per side:
- **/2N** — divide by powers of two
- **N** — sequence of eight
- **/2N+1** — divide by odd numbers

### Reset button
- While held, **all clock processing pauses**.
- When released, the divider resets on the **first clock after release**.

### Wack mode
Hidden randomized mode.

#### Enter/exit Wack mode
- **One side:** hold that side’s **Offset/Shift knob**, then press **Reset**
- **Both sides:** hold **both knobs**, then press **Reset**  
  - Works when both sides are in regular mode

#### Wack mode behavior
- **/2N:** probabilistic divide-by-2 behavior  
  - each step has a **50% chance** to generate a trigger
- **N:** one **random trigger output** per step
- **/2N+1:** all 8 outputs act independently  
  - on each rising clock, **each output has a 50% chance** of triggering

---

## Jack Reference

## Inputs

### Clock input (x2, one per side)
- Function: Advances that side’s divider/generator on a rising edge
- **Clock threshold:** responds at about **3.3 V**
- If only one clock is patched, it is **normalled to the other side**
- **Timing latency:** outputs update about **70 µs** after the clock edge

### Reset input (x2, one per side)
- Function: Resets the state of that divider section
- Inputs are also described as normalled behavior when using shared reseting across sides
- Useful for re-aligning patterns to bar starts or master transport

### Shift CV input (x2, one per side)
- Function: Rotates the output assignment/order for that side
- Manual does **not specify CV input voltage range**

---

## Outputs

### Trigger outputs (16 total; 8 per side)
- Function: Trigger streams based on selected mode and shift
- **Output voltage range:** **0 V to 5 V**
- Trigger goes high at approximately **3.4 V**
- Suitable for triggering most Eurorack gate/trigger inputs

---

## Per-side output behavior summary

### Mode: /2N
- Outputs represent divisions by powers of 2
- Best for classic clock division trees

### Mode: N
- Outputs behave as a sequence of 8 steps
- Good for stepping across 8 destinations rhythmically

### Mode: /2N+1
- Outputs represent odd-number divisions
- Good for less symmetrical polyrhythms

### Shift effect
- Reorders which physical jack corresponds to the beginning of the cycle
- Great for changing groove without repatching

---

## Voltage / Timing Summary

- **Clock input threshold:** ~**3.3 V**
- **Trigger outputs:** **0 V to 5 V**
- **Trigger high level:** ~**3.4 V**
- **Output update latency:** ~**70 µs**
- **Shift CV range:** **not specified in manual**
- **Reset input voltage range:** **not specified in manual**

---

## Physical / Power Specs
- **Type:** Rhythm Modifier
- **Width:** **8 HP**
- **Depth:** **0.8 in**
- **Power connector:** **2x5 Eurorack**
- **+12 V:** **90 mA**
- **-12 V:** **35 mA**

---

## Practical patch tips
- Use one master clock to drive both sides for related rhythms.
- Use separate clocks for independent polyrhythmic structures.
- Send resets from a master sequencer every 16 or 32 steps to keep patterns anchored.
- Use **Shift** to remix which destination gets which subdivision.
- Try one side in standard mode and the other in **Wack mode** for a stable/random layered rhythm setup.

---

## Ultra-short workflow
- **Clock in**
- **Pick mode**
- **Rotate with Shift**
- **Patch outputs**
- **Reset to re-align**
- **Enable Wack mode for randomness**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)