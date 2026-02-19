# 2hp — Pluck

- [Manual PDF](../../manuals/2hp_Pluck.pdf)

---

[Pluck Manual PDF](#) <!-- Replace "#" with the actual URL if available -->

---

# **Pluck (2hp) Cheat Sheet**

Karplus-Strong string synthesizer with 4-voice polyphony for resonant, percussive, and melodic string timbres in Eurorack.

---

## **Quick Reference**

### **Inputs**
| Jack      | Function                        | Voltage Range | Notes                                   |
|-----------|---------------------------------|---------------|------------------------------------------|
| TRIG      | Trigger input                   | -             | Triggers a new note (up to 4 voices)     |
| DAMP      | Dampening amount CV input       | -5 V to +5 V  | Modulates harmonics/tone on new notes    |
| DECAY     | Decay amount CV input           | -5 V to +5 V  | Modulates decay time on new notes        |
| V/OCT     | 1V/Oct Pitch input              | 0 V and up    | Adds to pitch knob (standard scaling)    |

### **Outputs**
| Jack      | Function                   | Voltage Range | Notes                |
|-----------|----------------------------|---------------|----------------------|
| OUT       | Audio output (main)        | 10 Vpp        | Main module output   |

---

## **Controls**
| Control      | Type        | Description                                                   |
|--------------|-------------|---------------------------------------------------------------|
| DAMP         | Knob        | Sets string dampening (harmonics). Left = dull, right = bright|
| DECAY        | Knob        | Sets decay length. Left = short, right = long                 |
| PITCH        | Knob        | Sets fundamental pitch. Active for latest note, even if sustaining |
| Out LED      | LED         | Visualizes output amplitude                                   |

---

### **How to Use**

1. **Patch TRIG** to a gate/trigger for plucked notes. Each new trigger can play a new polyphonic voice (max 4).
2. **Set DAMP knob/CV**: Left for muted/plucky, right for bright/ringing. CV (-5V to +5V, summed with knob).
3. **Set DECAY knob/CV**: Controls how long each note rings. CV (-5V to +5V, summed with knob).
4. **Tune with PITCH knob/V/OCT**: PITCH knob provides coarse tuning; add V/OCT for external pitch control.
5. **Monitor OUT/LED**: Patch OUT to mixer/audio, use LED for level reference.

---

**Power:** +12V (83.45mA), -12V (4.5mA) | Depth: 42mm | Width: 2hp

---

### **Summary Table**

| Jack/Knob   | Function        | Range/Type                | Notes                 |
|-------------|-----------------|---------------------------|-----------------------|
| TRIG        | Input           | Trigger                   | Create new note       |
| DAMP        | Knob/Input      | Knob / -5V to +5V CV      | Harmonic content      |
| DECAY       | Knob/Input      | Knob / -5V to +5V CV      | Length of note        |
| V/OCT       | Input           | 1V/Oct                    | Standard pitch CV     |
| PITCH       | Knob            | -                         | Set baseline pitch    |
| OUT         | Output          | 10Vpp audio               | Main sound output     |
| Out LED     | Output          | Visual                    | Output amplitude      |

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
