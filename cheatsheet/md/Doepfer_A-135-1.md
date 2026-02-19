# Doepfer — A-135-1

- [Manual PDF](../../manuals/A135_man.pdf)

---

[Doepfer A-135 VC-Mixer Manual (PDF)](https://www.doepfer.de/a100man/A135_anl.pdf)

---

# Doepfer A-135 VC-Mixer (System A-100) Cheat Sheet

The **Doepfer A-135 VC-Mixer** is a 4-channel voltage-controlled mixer combining four linear VCAs and a mixer. It allows voltage-controlled mixing of up to 4 audio signals with individual CV or manual control, suited for both audio and some CV duties.

---

## Inputs & Outputs (Sockets)

| Label       | Type                 | Function                                  | Voltage Range              |
|-------------|----------------------|--------------------------------------------|----------------------------|
| Audio In 1-4 (`!`)  | Input (x4)      | Audio inputs for each VCA channel          | Audio levels (typ. ~10Vpp) |
| Audio Out (`"`)     | Output           | Sum output of all 4 VCAs mixed             | Audio levels (~10Vpp)      |
| ext. CV 1-4 (`§`)   | Input (x4)       | CV input for each VCA                      | 0V (off) to +5V (max gain) |

---

## Controls

| Control      | Per VCA? | Description                                                                              |
|--------------|----------|------------------------------------------------------------------------------------------|
| Audio In     | Yes      | Attenuates the signal at the corresponding Audio In.                                      |
| Gain         | Yes      | Sets manual gain/offset for the channel. 0 = off, increasing gives more base gain.        |
| ext. CV      | Yes      | Attenuates the amount of external control voltage affecting the VCA.                      |

- **Audio In (1-4):** Use the knob to set initial signal level for each audio input.
- **Gain (1-4):** Sets minimum VCA level (offset). Typically set to 0 for unipolar sources (like envelopes); increase for bipolar CV sources (like LFOs) to allow negative swings to have effect.
- **ext. CV (1-4):** Attenuates the external CV input; sets how much modulation affects the VCA.

---

## Reference Notes

- **All VCAs are linear response.**
- **Typical use**: Patch sources (VCOs, samplers, external signals, etc.) into Audio In 1-4. Output to sound system or further processing.
- **CV modulates amplitude**: e.g. use envelopes for dynamics or LFOs/random for movement.
- **0V CV = VCA muted; +5V CV = VCA at max gain.** Control sources include envelopes, LFOs, sequencers, random, etc. (see manual for examples).

---

## Patch Example

1. Plug up to 4 audio sources into Audio In jacks.
2. Optionally patch a control voltage (envelope, LFO, etc.) into ext. CV for one or more channels.
3. Set Audio In and Gain knobs for basic level.
4. Use ext. CV knob to set CV modulation depth.
5. Main output is at Audio Out.

---

### Module Panel Summary

- **Inputs:**  
  `Audio In 1-4` (signal), `ext. CV 1-4` (0-5V, controls VCA)
- **Output:**  
  `Audio Out` (summed/mixed VCA outputs)
- **Knobs per channel:**  
  *Audio In* (attenuator), *Gain* (offset), *ext. CV* (CV attenuator)
- **No buttons, switches, or sliders.**

---

### Additional References

- **CEM3381** VCA chips, high quality, linear response.
- **Voltage range:** For full VCA opening, ext. CV input expects up to +5V (in addition to offset from Gain knob).

---

**For detailed patch diagrams, refer to the Patch-Sheet section in the [full manual (PDF)](https://www.doepfer.de/a100man/A135_anl.pdf).**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)