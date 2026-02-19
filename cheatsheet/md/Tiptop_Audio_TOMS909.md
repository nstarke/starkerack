# Tiptop Audio — TOMS909

- [Manual PDF](../../manuals/Tiptop_Audio_TOMS909_ns.pdf)

---

[Download the TOMS909 Manual PDF](https://www.tiptopaudio.com/909-2)

---

# TOMS909 Cheat Sheet  
**Tiptop Audio | Analog 909 Tom Drums for Eurorack**

---

## **Quickstart**
1. **Patch a gate** (e.g. from a trigger sequencer) to any Tom's `GATE IN`.
2. **Patch each Tom’s `OUT` or the `MIX OUT`** to your sound system.
3. **Set LEVEL & ACCENT** to taste.
4. **Adjust DECAY** for drum body/length.
5. **Adjust TUNE** for pitch.
6. Optionally, patch CV for **VC-TUNE** or **ACCENT IN** for modulation.

---

## **Inputs & Outputs Reference**

### Low Tom (Left Section)
- **LOW GATE IN**: Gate/trig input to trigger Low Tom. (+5V typical, accepts standard modular triggers)
- **LOW OUT**: Audio out for Low Tom (individual)
- **VC-L-TUNE IN**: CV input for Low Tom pitch (TUNE). (CV range: Not 1V/Oct, ±5V recommended)
- **ACCENT IN**: Gate/CV input for dynamic accent. (accepts gates/trigs/CV, +5V typical)

### Mid Tom (Middle Section)
- **MID GATE IN**: Trig input for Mid Tom (+5V typical)
- **MID OUT**: Audio out for Mid Tom
- **VC-M-TUNE IN**: CV for Mid Tom pitch (CV range: ±5V recommended, not 1V/Oct)
- **ACCENT IN**: As above

### High Tom (Right Section)
- **HI GATE IN**: Trig input for High Tom (+5V typical)
- **HI OUT**: Audio out for High Tom
- **VC-H-TUNE IN**: CV for High Tom pitch (CV range: ±5V recommended, not 1V/Oct)
- **ACCENT IN**: As above

### Mixed Output
- **MIX OUT**: Mix of all three Toms for summed output.

---

## **Controls Reference**

- **LEVEL (per Tom):** Drum output volume.
- **ACCENT (per Tom):** Sets max accent gain, and functions as fine gain trim.
- **DECAY (per Tom):** Adjusts drum length from percussive click (CCW) to long tom (CW).
- **TUNE (per Tom):** Sets pitch/timbre.
- **VC-TUNE ATTENUATOR (per Tom):** Scales applied CV for each Tom’s pitch input.

---

## **Voltage Control Details**
- **VC-TUNE IN:** Not 1V/Oct. Responds throughout ±5V. Used for modulation/sequencing of TUNE.
- **ACCENT IN:** Can take gates or CV (up to +5V). When patched, incoming signal sets dynamic accent (volume boost, more attack/noise). ACCENT knob scales the difference.

---

## **Extra Features & Tips**
- **Patch all Toms for polyrhythms:** Use multiple gates/triggers for rhythmic complexity.
- **Patch mixtures:** Individual OUTs for separate processing/panning, or use MIX OUT for classic 909-style sum.
- **Dynamic playing:** Use sequencer CV/gates to modulate ACCENT or TUNE for evolving textures.
- **Audio Rate FM:** Patch audio oscillator (e.g., a VCO) to VC-TUNE INs for metallic, harmonically rich toms.
- **Bus Mixer:** Can be routed to MIXZ module via header.

---

## **Typical Applications**
- Classic 909 toms in your modular rig.
- Dynamic, voltage-controlled tom sounds.
- Sound design: metallic, pitched percussion with FM.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)