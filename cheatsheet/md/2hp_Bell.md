# 2hp — Bell

- [Manual PDF](../../manuals/2hp_Bell.pdf)

---

[Download the Bell 2hp Manual (PDF)](https://2hp.com/docs/bell_manual.pdf)  
*(Note: If this is not the official manual location, check the manufacturer's site for most recent version.)*

---

# Bell 2hp Cheat Sheet

**Bell** is a melodic percussion Eurorack module using modal synthesis, with 6 voice polyphony and multiple physical models for metallic and percussive sounds.

---

## Panel Reference

| Label   | Jack/Control Type | Function                                                     | Voltage Range                  |
|---------|-------------------|--------------------------------------------------------------|--------------------------------|
| TRIG    | Input Jack        | Triggers a new note with current settings                    | Gate/Trigger                   |
| MODEL   | Knob + CV In      | Selects 1 of 8 physical models; CV adds to knob              | CV: -5V to +5V (Bipolar)       |
| DAMP    | Knob + CV In      | Sets resonance/decay (damping); CV added to knob             | CV: -5V to +5V (Bipolar)       |
| V/OCT   | CV In             | Pitch control, 1V/Oct standard                              | CV: -1V to +6V                 |
| PITCH   | Knob              | Sets fundamental pitch of current/next note                  |        —                       |
| OUT     | Output Jack       | Audio out, illuminates LED on note trig                      | 10Vpp (peak-to-peak audio)     |

---

## Physical Models (Model Selector):
1. Pure Bell
2. Pure Vibraphone
3. Harmonic Vibraphone
4. Hard Marimba
5. Soft Marimba
6. Tibetan Bowl
7. Wine Glass
8. Redwood Plate

---

## Key Operation Notes

- **TRIG** input fires a new note (up to 6 voice polyphony, oldest replaced).
- **MODEL Knob/CV** morphs or switches through 8 excitor/resonator types.
- **DAMP Knob/CV** modifies decay/resonance for sharp or mellow sounds.
- **V/OCT** provides standard pitch tracking for melodic sequencing.
- **PITCH Knob** sets fundamental, active for the most recent note (pitch bend possible DURING ring-out).
- **OUT** is the mono audio output. LED blinks for ~30ms with each new note.

### Installation
- Requires 2HP width, 45mm depth.
- Power: +12V (86mA), -12V (3mA).
- Red stripe on ribbon cable = -12V.

---

## Typical Patch Example

- Patch sequencer gate to **TRIG**.
- Patch sequencer pitch CV to **V/OCT**.
- Patch audio out from **OUT**.
- Use **MODEL** and **DAMP** for timbre changes.
- Modulate **MODEL** or **DAMP** via CV for evolving metallic textures.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)