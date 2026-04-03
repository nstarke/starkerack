# 2hp — Tape

- [Manual PDF](../../manuals/2hp_Tape_Stop.pdf)

---

[Manual PDF](https://www.twohp.com/modules/tape-stop)

# 2hp Tape Stop — Cheat Sheet

**What it does:**  
A **clock-syncable tape stop effect** for audio. It simulates a tape machine slowing down/stopping, with manual or gate triggering and optional clock-synced stop lengths.

## Quick Use
- Patch audio into **IN** and take audio from **OUT**.
- Press **TRIG** or send a gate to the **Trig Gate Input** to start the tape stop effect.
- Set **Trig Toggle**:
  - **Down** = **Momentary**: effect lasts only while held/gate is high
  - **Up** = **Latching**: press/trigger once to start, again to end
- Turn **LAG** to set stop time:
  - **Free mode:** from **instant** up to **4 seconds**
  - **Clocked mode:** patch a clock to **CLOCK** and LAG selects rhythmic divisions/lengths

## Clock-Synced Lag Values
With a clock patched to **CLOCK**, the **LAG** knob sweeps left to right through:

**Instant → 32nd → 16th → 8th → quarter → half → whole → 2 bars → 4 bars → 8 bars → 16 bars**

## 50/50 Mode
- Hold the **TRIG** button while powering on.
- This sets the module to a **50% dry / 50% wet** mix so you still hear the dry signal during tape stopping.

---

## Controls

### TRIG Button
- Starts the tape stop effect.
- In **Momentary** mode, the effect ends when released.
- In **Latching** mode, press again to end.

### Trig Toggle
- **Down:** Momentary
- **Up:** Latching

### LAG Knob
- Sets tape stop length.
- **Unclocked:** instant to **4 seconds**
- **Clocked:** selects synced note/bar durations

### TRIG LED
- Lights when tape stop is active.
- Blinks to show incoming external clock rate when clock is patched.

---

## Inputs / Outputs

### Audio IN
- **Function:** Audio input to be processed
- **Voltage range:** **10 Vpp**

### CLOCK IN
- **Function:** External clock input for syncing tape stop duration
- **Voltage range:** Not specified in manual

### TRIG Gate IN
- **Function:** Gate input to trigger tape stop
- **Threshold:** **0.4 V**

### LAG CV IN
- **Function:** CV control over lag time
- **Voltage range:** **-5 V to +5 V**

### Audio OUT
- **Function:** Processed audio output
- **Voltage range:** **10 Vpp**

---

## Tech Specs
- **Width:** 2 HP
- **Depth:** 46 mm
- **Power:** +12V **101 mA**, -12V **7 mA**, +5V **0 mA**

---

## Practical Tips
- Use **CLOCK IN** when you want tape stops that land musically with your patch.
- Use **Momentary** mode for DJ-style stabs and fills.
- Use **Latching** mode for more performative “drop-out / return” gestures.
- Try slow **LAG** settings on loops, drums, or full mixes for dramatic breakdowns.
- The built-in **50/50 mode** is useful when full wet tape stop feels too extreme.

---

## One-Line Patch Ideas
- **Drum bus → Tape Stop:** rhythmic breakdowns and transitions
- **Sampler/voice → Tape Stop:** classic stop-button effect
- **Clocked sequence + CLOCK IN:** tempo-locked slowdowns
- **CV to LAG:** animated stop times for variation

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)