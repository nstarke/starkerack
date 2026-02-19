# Bastl Instruments — Cinnamon VCF

- [Manual PDF](../../manuals/manual-cinnamon-web-v1.4.pdf)

---

[**Full Manual (PDF) - Bastl Cinnamon State Variable Filter**](https://www.bastl-instruments.com)

---

# Bastl Cinnamon — Quick Reference Cheat Sheet

A **unique-sounding, multi-flavored state-variable filter** module, especially notable for its Drive and Character switches, allowing wild sonic shaping and self-oscillation.

---

## **Front Panel Controls**

### **Knobs:**
| Knob Name    | Function                                                    | Voltage/CV Range      | Notes                                              |
|--------------|-------------------------------------------------------------|-----------------------|----------------------------------------------------|
| Cutoff       | Sets filter cutoff freq (base freq + CVs).                  | —                     | Range determined by CV and pot combined.           |
| Resonance    | Emphasizes cutoff frequency; self-oscillates fully CW.      | —                     | At max, filter will oscillate (sine/alt shapes).   |
| Input Level  | Sets audio gain (0–2 or 0–10 w/Drive switch).               | —                     | Saturates input at high—affected by Drive switch.  |
| FM (Attenuator) | Controls CV amount from Right CV input.                  | —                     | Full CCW = no CV modulation.                       |


### **Switches:**
| Switch Name    | Function                                                    |
|----------------|-------------------------------------------------------------|
| Drive          | Up = overdrive input (gain 0–10), Down = normal (gain 0–2). |
| Char 1         | Alters resonance/oscillation response (see "Character").     |
| Char 2         | Alters resonance/oscillation response (see "Character").     |

---

## **Jacks (Inputs/Outputs):**

| Jack        | Type     | Function                          | Voltage Range              |
|-------------|----------|-----------------------------------|---------------------------|
| Input       | Audio In | Signal to filter                  | Audio levels; gain 0–10    |
| V/OCT       | CV In    | 1V/Oct FM of cutoff (tracking)    | -5V to +5V typical CV      |
| FM (Right)  | CV In    | Additional FM, amount by atten.   | -5V to +5V typical CV      |
| Lowpass     | Audio Out| 12 dB/oct (2-pole) LP out         | Eurorack audio (~±5V)      |
| Bandpass    | Audio Out| 6 dB/oct (1-pole) BP out          | Eurorack audio (~±5V)      |
| Highpass    | Audio Out| 12 dB/oct (2-pole) HP out         | Eurorack audio (~±5V)      |


---

## **Special Functions:**

- **Character Switches:**  
  *Down+Down*: clean sine resonance  
  *Up*: sharper, edgier resonance waveform  
  *Down*: sawtooth-like resonance waveform  
   (*Switches can disrupt V/Oct tracking/osc shape*)

- **Self-Oscillation:**  
  Max resonance → acts as sine/altered wave VCO.  
  (LP = 0°, BP = 90°, HP = 180° phase offset)

---

## **Patch Examples:**

- Routing audio in to Input, take filtered signal from any out (LP, BP, HP).
- Use V/OCT for precision tonal FM (tracking best when Char switches *both OFF*).
- Overdrive/filter for extra harmonics with Drive ON and Input Level up.
- Modulate cutoff with FM input and attenuator for funky sweeps.
- With high resonance, use as a sine/saw/edgy waveform VCO.

---

## **Power Requirements:**
- Width: **5HP**
- Depth: **35mm**
- +12V: <30mA, -12V: <30mA
- PTC fuse and diode protected.

---

## **Reference Links**
- [Bastl Cinnamon Official Page & Video Tutorials](https://www.bastl-instruments.com)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)