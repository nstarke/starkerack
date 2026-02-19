# Doefper — A-148

- [Manual PDF](../../manuals/A148_man.pdf)

---

[Doepfer A-148 Dual S&H Manual PDF](https://doepfer.de/a100man/a148_man.pdf)

---

# Doepfer A-148 Dual S&H – Cheat Sheet

## Quick Overview
The Doepfer A-148 is a dual Sample & Hold (S&H) and Track & Hold (T&H) module. It can generate random or stepped voltages for controlling other modules. Each of the two identical sections can be independently set to S&H or T&H by internal jumpers (for modules manufactured from Aug 2005 on).

---

## Panel Controls & Features

| Label         | Type    | Function                                                             | Voltage Range            |
|---------------|---------|----------------------------------------------------------------------|--------------------------|
| **Trig In**   | Jack    | Input for the trigger signal (sampling clock)                        | Any A-100 trigs/gates    |
| **Smp In**    | Jack    | Input for the signal to be sampled/held                              | -12V ... +12V            |
| **S&H Out**   | Jack    | Output for the sampled and held (or tracked and held) voltage        | -12V ... +12V            |
| **LEDs**      | Visual  | Shows the polarity of the output voltage (+ LED: positive, - LED: negative) | N/A           |
| **Jumper (int.)** | Header | Sets upper/lower circuit to S&H or T&H mode (default: Upper = S&H, Lower = T&H) | N/A           |

---

## How it Works

- **Sample & Hold (S&H):** At each positive edge on Trig In, the voltage at Smp In is "captured" and held until the next trigger.
- **Track & Hold (T&H):** The output follows the input while Trig In is high; when Trig In goes low, it holds the last value.

---

## Input/Output Reference

### Inputs
- **Trig In**
  - **Type:** Gate/Trigger input
  - **Purpose:** Determines when to sample Smp In
- **Smp In**
  - **Type:** CV/Audio input
  - **Purpose:** Signal to be sampled or tracked
  - **Voltage Range:** -12V to +12V (modules after Aug 2005; previous versions: -8V to +8V)

### Outputs
- **S&H Out**
  - **Type:** CV output
  - **Purpose:** Output the last sampled/tracked value
  - **Voltage Range:** Follows input within -12V to +12V (post-2005)

---

## Typical Patch Examples

1. **Random Arpeggios:**  
   - Patch white noise (A-118) to Smp In, LFO to Trig In, S&H Out to VCO CV.
2. **Glissando:**  
   - Keyboard CV through slew limiter to Smp In, LFO to Trig In, S&H Out to VCO CV.
3. **Random Filter:**  
   - Noise to Smp In, keyboard gate to Trig In, S&H Out to filter CV input.

---

## Version Differences & Jumpers

- **Pre-Aug 2005:** Max input/output voltage range -8V to +8V.
- **Post-Aug 2005:** Full A-100 range, -12V to +12V, and S&H/T&H selectable via jumpers JP2 (upper), JP3 (lower).

---

## Useful Tips
- **LEDs** helpful for monitoring whether the last held voltage is positive or negative.
- **Voltage Range:** Always ensure input voltages are within Doepfer’s -12V to +12V standard.
- **Mode Setting:** Factory default is S&H (upper), T&H (lower).

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**