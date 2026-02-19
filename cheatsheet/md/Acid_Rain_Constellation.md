# Acid Rain — Constellation

- [Manual PDF](../../manuals/Constellation_Manual_Firmware_1.1_4.7.2025.pdf)

---

**[Download: Constellation Firmware V1.1 Manual PDF](sandbox:/mnt/data/Constellation_Firmware_Manual_v1.1.pdf)**

---

# Constellation Eurorack Cheat Sheet

## OVERVIEW
**Constellation** is an 8-channel trigger/gate pattern generator with advanced Euclidean rhythm capabilities, rich logic, pattern modifiers (burst, ratchet, chance), polyrhythmic channel clocks, freely assignable CV modulation, and robust save/load options.

---

## QUICK START

1. **Patch 1–5 Channel Outputs** (top row of module) to drum modules:
   - Ch1: Kick
   - Ch2: Snare/Clap
   - Ch3: Closed Hi-Hat
   - Ch4: Open Hi-Hat
   - Ch5: Rimshot/other sound

2. **Power on:** Plays "4 on the floor" @120 BPM by default.

3. **Press `load`** — select any of the 20 pulsing buttons (central 2 rows) for quick start patterns. Use `live` mode to play/save slots like a keyboard.

4. Patch a slow-moving **0–5 V CV** source into CV Input I for pattern evolution.

---

## INPUT AND OUTPUT JACKS

### Inputs
- **Clock (clk):** External main clock input, expects 0–5V pulse. With cable inserted, switches to external clocking.
- **Reset:** External reset (rising edge = reset).
- **CV Inputs (I–VIII):**
  - **Assignable.** Not fixed to channels; can independently or cascadingly control any parameter on any pattern/channel.
  - **Voltage Ranges:**  
    - `Divide`, `Length`, `Ratchet`: **0–5V (Unipolar)**
    - `Events`, `Rotate`, `Burst`, `Chance`, `Width`, `Mute`, `Load`: **-5V to +5V (Bipolar)**  
    - See details below for modulation ranges.

### Outputs
- **Clock:** +5V/0V digital pulse (either internal or mirrored external clock, depending on clocking).
- **Reset:** +5V pulse on reset event.
- **Channel Outputs (1–8):** +5V when active, 0V inactive — outputting final channel pattern as trigger/gate.

---

## FRONT PANEL CONTROL REFERENCE

### Buttons
- **Top Row:**  
  - `clock`, `reset`, `save`, `load`, `input`, `random`
- **Middle Rows (Horizontal, 8 each):**  
  - Pattern Select (P1–P8), Channel Select (I–VIII), Channel Mute, Live
- **Pattern/Channel Parameter:**  
  - `AND`, `OR`, `XOR`, `flop`, `width`, `burst`, `ratchet`, `chance`, `divide`, `rotate`, `events`, `length`
- **Others:**  
  - Mute, Live, Flop, Logic, Pattern Select, Pattern Parameter

### Encoder
- **Navigation** through channels/patterns/parameters/menus  
- **Adjust** values (press for coarse/fine adjustment)

---

## CHANNEL AND PARAMETER STRUCTURE

- **8 Channels, each with 8 Patterns** (64 patterns total)
    - Each pattern: Divide, Length, Events, Rotate, Burst, Ratchet, Chance
    - Patterns combine via Logic (AND/OR/XOR).  
- **Channel Parameters:**  
    - Logic, Flip-flop (gate vs. trigger behavior), Width

### PATTERN MODIFIERS
- **Burst:** Each trigger = sequence of triggers (one per clock).
- **Ratchet:** Each trigger repeated between clocks (dense cluster).
- **Chance:** 0–100% probabilistic gate per event.

---

## NAVIGATION & MENUS

- **Edit Mode:** Default, full parameter editing.
- **Clock Menu:** BPM (internal clock, tap tempo), main clock div/mult, swing, channel clocks per channel.
    - `width` button: main clock swing (50–90%).
    - `mute` button: stops/starts internal clock.
    - `AND` button: tap tempo.
- **Mute Menu:** Mute channels/patterns; press again to unmute.
- **Save/Load Menu:**  
    - Save/Load any channel/patterns into 20 slots per bank (999 banks).
    - Save/load channel mutes, main clock, input assignments as options.
    - `reset` in load menu: forces re-sync.
- **Live Mode:**  
    - Play save slots "momentarily" (release = revert).
    - Momentarily mute channels.

---

## CV INPUT MODULATION SUMMARY

| Parameter  | Volt. Range    | Behavior                                |
|:-----------|:--------------|:-----------------------------------------|
| Divide     | 0–5V unipolar | 1 to base value (set)                   |
| Length     | 0–5V unipolar | 1 to base value (set)                   |
| Events     | -5V–+5V       | 0 to length, centered at base value      |
| Rotate     | -5V–+5V       | 0 to length, centered at base value      |
| Burst      | -5V–+5V       | 1 to max burst, centered at base value   |
| Ratchet    | 0–5V unipolar | 1 to base value (set)                   |
| Chance     | -5V–+5V       | 0-100%, centered at base value           |
| Width      | -5V–+5V       | 0–100%, centered at base value           |
| Mute       | Gate/Trigger  | Mutes/unmutes on gate/trigger edge       |
| Load       | Gate/Trigger  | Loads selected save slot while high      |

- *CV is sampled once per rising edge of the channel clock.*

---

## TIPS AND UTILITIES

- **Pattern Reset:** Hold pattern button + press reset.
- **CV Inputs Cascade:** Inputs I–VIII cascade L → R for multi-parameter modulation; can disable in settings (`cv_norm = 0`).
- **Save/Load Individual Channels:** In save menu, press only channels to save.
- **Autosave:** Module autosaves every few seconds.
- **Factory Reset:** Delete all bank folders from SD card for blank state.
- **Restore Quickstart Patterns:** Download `000.zip` from Acid Rain website.

---

## LOGIC MODES (Channel):

- **AND:** Only outputs high if all active patterns are high.
- **OR:** Outputs high if any active patterns are high.
- **XOR:** Outputs high if odd number of patterns are high.

---

## FIRMWARE UPDATES

1. Power off, remove/inject micro SD to PC.
2. Download latest firmware; place `FW.BIN` on root.
3. Reinsert SD, power on, wait for update animation.

---

## QUICK REFERENCE: BUTTON SHORTCUTS

| Function              | Action                                     |
|:----------------------|:-------------------------------------------|
| Pattern Reset         | Hold Pattern + Press Reset                 |
| Enter Mute Menu       | Press `mute`                               |
| Save/Load Bank        | `save` / `load`, select bank/slot          |
| Enter Clock Menu      | Press `clock`                              |
| Live Mode             | Press `live`                               |
| Coarse Adjust         | Encoder short press (flashing display)     |
| Randomize Parameter   | Press `random` with parameter selected     |
| Remove CV Assign      | Hold Reset + Input button in Input Menu    |
| Tap Tempo             | Press "AND" button in Clock Menu           |

---

**Manual & Resources:**  
- [Constellation Firmware Manual PDF](sandbox:/mnt/data/Constellation_Firmware_Manual_v1.1.pdf)  
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)