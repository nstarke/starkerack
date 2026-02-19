# Korg — Volca FM2

- [Manual PDF](../../manuals/volca-fm2_OM_EFGSCJ3.pdf)

---

It looks like the manual you’ve provided is for the **Korg volca fm2**, which is a *standalone digital FM synthesizer* (not an Eurorack module). However, it features MIDI, analog sync, and 3.5mm jacks which can integrate with modular systems and DAWs via adapters and creative signaling (e.g., with the right analog clocking/conversion and MIDI-to-CV modules).

Below, you’ll find a concise “cheat sheet" for eurorack-style integration and operational use—perfect for modular synth musicians.

---
## [Korg volca fm2 - Digital FM Synthesizer Manual (PDF)](https://www.korg.com/us/support/download/manual/0/529/4663/)  

### Quick Reference Cheat Sheet

#### Inputs & Outputs

| Jack/Port       | Type      | Description & Specs                                                       |
|-----------------|-----------|---------------------------------------------------------------------------|
| **DC 9V**       | Power     | DC power input (use only specified Korg adapter)                           |
| **Headphones**  | 3.5mm TRS | Mini-jack stereo audio output; plugging in mutes the built-in speaker      |
| **SYNC IN**     | 3.5mm TS  | Analog clock in; 20V max input; triggers sequencer steps                   |
| **SYNC OUT**    | 3.5mm TS  | Analog clock out; 5V pulse output at each 16-step sequencer step (15 ms)   |
| **MIDI IN**     | 3.5mm TRS | MIDI - Type A (adapter to DIN needed); accepts note, CC, SYX (DX7)         |
| **MIDI OUT**    | 3.5mm TRS | MIDI - Type A; outputs note/events; use adapter to 5-pin DIN if needed     |

#### Panel Controls

| Control         | Type         | Function                                                                |
|-----------------|--------------|-------------------------------------------------------------------------|
| **POWER**       | Button       | Press to turn on; hold for 1s to turn off                               |
| **TRANSPOSE**   | Slider       | Shifts pitch ±octaves or semitones; semitone mode via FUNC+TRANSPOSE    |
| **VELOCITY**    | Slider       | Sets velocity in Play mode; Value in Edit mode                          |
| **OCTAVE**      | Button (<, >)| Shift keyboard range up/down 1 octave per press; in Edit, select operator|
| **OPERATOR +/-**| Button       | Select FM operator (1-6 or All) in Edit mode                            |
| **PROGRAM**     | Knob         | Selects presaved program (Play); selects FM parameter (Edit)            |
| **ALGRTM**      | Knob         | FM operator algorithm (32 types, DX7 compatible)                        |
| **MEMORY**      | Button       | Hold + 1-16 to load sequence; Func+MEMORY+1-16 to save                  |
| **SAVE/EXPORT** | Button       | Save/Export current program/sequences (see “Exporting” below)           |
| **EDIT**        | Button       | Toggle PLAY/Edit mode                                                   |
| **FUNC**        | Button       | Hold for alt functions (e.g. FX, chain, global config, mode select)      |
| **PLAY**        | Button       | Sequence play/stop                                                      |
| **REC**         | Button       | Sequence record/erase                                                   |
| **STEP KEYS 1-16**| Buttons    | Used as keyboard, step buttons, selector for other functions            |
| **MOD/EG KNOBS**| Knob         | Attack/Decay for Modulator and Carrier ops                              |
| **LFO RATE/P.DEPTH**| Knob     | Controls FM LFO speed and depth                                         |
| **TYPE/DIV**    | Knobs        | Arpeggiator pattern (TYPE) and division (DIV)                           |
| **TEMPO**       | Knob         | Global tempo for seq/arp                                                |
| **VOLUME**      | Knob         | Master output volume                                                    |

#### Global Configuration & Utility

- **Set MIDI Channel:** Power up holding MEMORY, select 1-16 on keyboard.
- **Set Battery Type:** FUNC hold + Power, Key 2 toggles Alkaline/NiMH.
- **Sync Polarity:** FUNC hold + Power, Key 3/4 toggles SYNC direction.
- **Tempo Range:** FUNC hold + Power, Key 5 toggles full/narrow.
- **Restore Defaults:** FUNC+MEMORY hold, power up, REC to confirm (erases all data).

#### Key Functions with FUNC

- **FUNC+ARP ON/OFF:** Toggle arpeggiator
- **FUNC+MONO/UNISON:** Voice modes
- **FUNC+CHORUS/REVERB:** FX, edit level with FUNC+ARP TYPE/DIV
- **FUNC+PROGRAM RANDOM:** Random FM patch
- **FUNC+MOTION SEQ ON/OFF:** Knob automation on/off
- **FUNC+1/1, 1/2, 1/4:** Tempo division for external sync

#### Voltage Ranges (Inputs/Outputs)

| Input/Output     | Voltage Range |
|------------------|--------------|
| **SYNC IN**      | 0–20V Max    |
| **SYNC OUT**     | 5V pulse, 15ms|
| **MIDI In/Out**  | Standard MIDI voltages via TRS or adapter (not analog CV!) |
| **Headphones Out**| Line level audio/standard headphones |

> **NOTE:** This unit does NOT accept standard Eurorack CV/Gate for pitch/trigs! It is clockable via analog clock volts (SYNC IN, 5V or higher trigger) but melodic, modulation CV requires MIDI-to-CV conversion.

### Exporting Patches/Sequences
- **Save:** SAVE/EXPORT, choose slot (PROGRAM knob), press again to save
- **Export:** EDIT mode, SAVE/EXPORT, scroll to desired item, press again to transmit via SYNC OUT

---

## Example Eurorack Integrations

- **Tempo Sync:** Use a Eurorack clock out (5V trigger) to SYNC IN for step-advance, or sync OUT from volca fm to clock external sequencers (with trigger-to-clock conversion if needed).
- **Sequencer Use:** Drive external MIDI modules via MIDI OUT (needs DIN adapter and MIDI-to-CV module).
- **Audio Output:** Patch headphone out into Eurorack line input module.

---

## Reference Links

- [Korg Official Manual PDF (English)](https://www.korg.com/us/support/download/manual/0/529/4663/)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)

---

##### If you have more specific workflow goals (e.g., integrating with MIDI-to-CV, or using sequenced clocks in a patch), just ask!