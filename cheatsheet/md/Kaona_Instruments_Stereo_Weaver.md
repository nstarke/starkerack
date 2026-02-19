# Kaona Instruments — Stereo Weaver

- [Manual PDF](../../manuals/stereoweaver.pdf)

---

[Download the Official Manual (PDF)](attachment:/STEREOWEAVER_MANUAL.pdf)

---

# **Stereoweaver Eurorack Module – Cheat Sheet**

## **Module Overview**
- **Type:** Mono-to-Stereo Spatial FX
- **Width:** 10 HP
- **Depth:** 28 mm
- **Power:** +12 V: 140 mA, –12 V: 20 mA, +5 V: 0 mA
- **Function:** Turn mono signals into musically useful stereo images using psychoacoustic tricks, phase, movement, and delays.
---

## **Front Panel Controls & Jacks Reference**

### **Inputs**
- **IN MONO (Jack)**: Mono signal input (Eurorack level)
- **CV Inputs (Jacks):**
  - **depth** *(±5V)* — Modulates Depth knob
  - **phase** *(±5V)* — Modulates Phase knob
  - **motion** *(±5V)* — Modulates Motion knob
  - **haas** *(±5V)* — Modulates Haas knob
  - **width** *(±5V)* — Modulates Width/Move knob

### **Outputs**
- **OUT L (Jack)**: Left channel
- **OUT R (Jack)**: Right channel

---

### **Knobs and Switches**

- **Depth**  
  - _Controls:_ Amount/Intensity of spatial effects and interactions
  - _Range:_ Low = direct, front; High = organic, deep stage; Max = adds micro-chorus/phasing
  - _CV:_ Yes (depth input, ±5V)

- **Phase**  
  - _Controls:_ Phase relationship (0–180º) between L/R
  - _Effect:_ Impacts stereo stability, diffusion, and strangeness
  - _CV:_ Yes (phase input, ±5V)

- **Motion (with rotary toggle)**  
  - _Controls:_ Movement/modulation of stereo image
    - *Slow* = subtle, organic "living" stereo  
    - *Fast* = obvious spatial movement  
    - *Rotary* = Leslie-style rotating effect
  - _CV:_ Yes (motion input, ±5V)

- **Haas**  
  - _Controls:_ Inter-channel micro delay (Haas effect)
    - *Moderate* = natural stereo presence  
    - *High* = pronounced, characterful effect
  - _CV:_ Yes (haas input, ±5V)

- **Width (with 'move' mode)**  
  - _Controls:_ Stereo field widen/narrow, hollows center; Move introduces dynamic width/panning
  - _Move Position:_ Channels crossfade, speed set by Motion, width by Phase. At max: chaotic L/R displacement.
  - _CV:_ Yes (width input, ±5V)

- **Input Level**  
  - _Controls:_ Gain for mono in; set to avoid or induce (artiﬁcial/coloring) distortion  
  - _Clip LED:_ Reduces to avoid distortion unless wanted

- **Left/Right Output Levels**  
  - _Controls:_ Adjusts L/R levels for precise stereo balance/output matching

---

## **Typical Use**
1. **Input**: Plug your mono source to IN MONO. Set input gain watching the clip LED.
2. **Depth/Phase/Motion/Haas/Width**: Adjust creatively for desired stereo effect. Use Motion (rotary) for animated/Leslie-style FX.
3. **Outputs**: Connect OUT L / OUT R to stereo mixer or further processing.
4. **CV Control**: Patch modulation sources (LFOs, envelopes, random, etc.) into CV inputs to animate spatial parameters. All CVs respond to ±5V.

---

## **Manual Voltage Ranges**

- **CV Inputs**: All CV jacks accept ±5 V, they sum with the knob position and allow bipolar modulation.

---

## **Visual Aids**

- *LEDs visualize clipping, motion, Haas effect, and width interaction in real time.*

---

## **Quick Tips**

- For subtle stereo, use low Depth, moderate Haas, slow Motion.
- For dramatic FX, crank Depth/Phase, use Motion (Rotary) and Move mode on Width.
- Animate CVs for ever-changing or rhythmic spatial movement.
- Deliberate clipping can add harmonics/character.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
