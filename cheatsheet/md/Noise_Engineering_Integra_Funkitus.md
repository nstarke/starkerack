# Noise Engineering — Integra Funkitus

- [Manual PDF](../../manuals/Integra Funkitus - Noise Engineering Documentation.pdf)

---

[**Integra Funkitus Manual (PDF)**](https://manuals.noiseengineering.us/if/)

---

# Integra Funkitus — Cheat Sheet

**Type:** Rhythm Modifier  
**Format:** 8HP Eurorack  
**Depth:** 0.8"  
**Power:** +12 V: 50 mA, -12 V: 11 mA (2x5 header)

---

## Panel Controls and Jacks

### Inputs

| Jack/Control       | Function                                                 | Voltage Range     |
|--------------------|----------------------------------------------------------|-------------------|
| **Part Input 1–4** | Gate input channels. Each receives a separate rhythm.     | Gates > 2 V       |
| **Mod 1–4 Jack**   | CV input for corresponding Mod Knob (1–4). Modulates the modification of that channel. | Typical Euro CV; knob acts as attenuator |

### Outputs

| Jack/Control        | Function                                                  | Voltage Output    |
|---------------------|-----------------------------------------------------------|-------------------|
| **Part Output 1–4** | Gate output channels (modified/combo rhythms).            | 6 V gate signals  |

### Controls

| Control                  | Description                                                                                                    |
|--------------------------|----------------------------------------------------------------------------------------------------------------|
| **Mode Switch**          | 3-way toggle: selects "Trigger" (T), "Gate" (G), or "Logic" (L) mode of operation                             |
| **Mod Knob 1–4**         | Sets probability/combo for corresponding channel (and acts as attenuator for CV input when patched)            |
|                          | - **Trigger Mode (T):** Probability that a rising edge on Input passes to Output (falling edge always passes)  |
|                          | - **Gate Mode (G):** Probability that both rising and falling edges of Input pass to Output                    |
|                          | - **Logic Mode (L):** Which inputs are logically combined for the Output; fully CCW = direct pass, fully CW = mute |
| **Burn Button**          | Instant “fill” — forcibly combines all inputs to all outputs, overriding mode and knob settings                |

---

## Usage Quick Reference

1. **Patch up to four gate signals** into Part Input 1–4 (e.g., clock, rhythm generators like Numeric Repetitor).
2. **Connect Part Outputs 1–4** to drum/percussion modules or other gate destinations.
3. **Set the Mode Switch**:
   - **Trigger (T):** Out = random-per-event gate passes (rising), knob sets probability.
   - **Gate (G):** Out = random-per-edge gate passes (rising + falling), knob sets probability (pulses get longer).
   - **Logic (L):** Out = logical combination of other ins, knob selects combo or mute.
4. **Mod Knobs 1–4**: Select probability/combo for each channel.  
   Or patch CV into Mod 1–4 Jacks for voltage control (knobs become attenuators).
5. **Tap Burn** for instant all-in variation (“fill” effect).

---

## Voltage Summary

- **Inputs (Gate):** >2 V triggers event.
- **Outputs (Gate):** 6 V gates.
- **Mod CV:** Euro CV standard (typically -5 V to +5 V or 0–10 V; manual doesn’t specify but compatible with typical modular voltage ranges).

---

## Tips

- Want simple muting? Turn Logic Mode knob fully clockwise.
- Use CV for evolving, auto-probability changes.
- Combine different modes for evolving, fill-variation percussion lines.
- **Burn** to instantly combine everything for fills/breaks.

---

For more details, see the full [**Integra Funkitus Manual**](https://manuals.noiseengineering.us/if/)  
Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)