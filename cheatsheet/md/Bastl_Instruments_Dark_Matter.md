# Bastl Instruments — Dark Matter

- [Manual PDF](../../manuals/manual-dark-matter.pdf)

---

Certainly! Here is a concise cheat sheet for the **Bastl Instruments Dark Matter Feedback Observatory** Eurorack module based on your screenshots.

---
**[View the official Dark Matter Manual (PDF)](https://bastl-instruments.com/content/manuals/darkmatter_manual.pdf)**

---

# Dark Matter: Cheat Sheet

## **Overview**
- **Type:** Feedback/Distortion/EQ with dynamic shaping
- **Role:** Feedback processing, unique textures, aggressive FX, creative distortion

---

## **Panel Reference**

### **Inputs**
- **Input**: Main audio signal input (**±5V** typical).
- **Drive CV**: CV control for drive/gain (**0–5V**).
- **Dynamics CV**: CV for envelope's effect on drive/gain (**0–5V**).
- **Tone CV**: CV control for EQ (**±5V**).
- **FBK CV**: CV control for feedback loop's VCA (**0–5V**).
- **X-Fade CV**: CV for crossfade between dry & feedback (**0–5V**).
- **EXT FBK IN**: External feedback loop input (audio).

### **Outputs**
- **X-Fade Out**: Main output, post crossfade section (audio).
- **Dynamics Out**: Envelope follower output (**0–5V**).

---

## **Knobs, Sliders, Switches**

**DRIVE**
- **Knob**: Sets gain/saturation of input VCA.
- **Switch ("Drive/Drive+")**: Hyperdrive mode for hard clipping & distortion.

**DYNAMICS**
- **Knob**: Envelope intensity amount (how much envelope affects Drive).
- **Dynamics Out Jack**: Envelope follower out (**0–5V**).

**TONE**
- **BASS** and **TREB** Sliders: 2-band EQ shaping.
- **Boost**: Pushes bass/treble for extra impact.
- **Tone CV Input**: Modulates both bands simultaneously (**±5V**).

**FBK**
- **FBK Fader**: Sets VCA amount in feedback path.
- **FBK CV**: Controls feedback VCA (**0–5V**).
- **EXT FBK IN Jack**: For routing external FX/device into the feedback loop.
- **Polarity Switch**: Inverts phase of feedback loop.

**X-FADE**
- **X-Fade Fader**: Crossfades between dry (drive) and feedback.
- **X-Fade CV Input**: Controls position of X-fade (**0–5V**).

---

## **Other Controls**
- **Boost (Dynamics)**: Extra punch to envelope effect.
- **Signal/Drive LED**: Shows gain and drive state.
- **Dynamics LED**: Shows envelope activity.

---

## **Quick Start**
1. Patch audio to **Input**, **X-Fade Out** to your mixer.
2. Set **Drive** for desired saturation; use **Hyper** for harder distortion.
3. EQ with **Bass/Treb** sliders.
4. Set **FBK** slider for feedback intensity; try **Polarity** switch for phase effects.
5. Play with **X-Fade** to balance clean vs. effect signal.
6. Modulate **CV inputs** for dynamic, rhythmic, or evolving results.

---

## **Reference Table: Jacks & Controls**

| Label                | Function / CV Range      | Type         | Notes                                   |
|----------------------|-------------------------|--------------|-----------------------------------------|
| **INPUT**            | Audio in                | Input        | Main signal, ±5V                        |
| **DRIVE CV**         | 0–5V                    | Input (CV)   | VCA drive/gain                          |
| **DYNAMICS CV**      | 0–5V                    | Input (CV)   | Envelope VCA amount                     |
| **TONE CV**          | ±5V                     | Input (CV)   | EQ bands                                |
| **FBK CV**           | 0–5V                    | Input (CV)   | Feedback VCA                            |
| **X-FADE CV**        | 0–5V                    | Input (CV)   | Dry/feedback mixer                      |
| **EXT FBK IN**       | Audio in                | Input        | Insert FX or devices into FEEDBACK loop |
| **X-FADE OUT**       | Audio out               | Output       | Mixed output                            |
| **DYNAMICS OUT**     | 0–5V Envelope           | Output (CV)  | Envelope follower                       |

---

## **Tips**
- Use **EXT FBK IN** to route reverb/delay for true "echoes."
- **FBK Polarity** for different phase coloration in feedback path.
- **Dynamics Out** can trigger or modulate other modules in sync with audio.
- Try aggressive **Drive** settings with **Tone** boost for crunchy leads or drums.

---

## **Specs**
- **Power:** +12V: 75mA, -12V: 60mA
- **HP:** 13
- See manual for advanced patch suggestions!

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**
