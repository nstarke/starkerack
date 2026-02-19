# Korg — Volca Bass

- [Manual PDF](../../manuals/Korg-Volca-Bass_manual.pdf)

---

It looks like you've attached the manual pages for the **Korg Volca Bass**, which is **not** a Eurorack module but a standalone analog groovebox (though it does feature some connectivity often useful in modular setups!). Still, here is a concise "cheat sheet" for reference, formatted for Eurorack musicians and modular context, and including all requested info.

---
**[Korg Volca Bass Manual PDF](https://cdn.korg.com/user_manuals/volca_bass_OM_EFGSJ1.pdf)**

---

# Korg Volca Bass Cheat Sheet

## Overview
- **Standalone analog bassline groovebox**
- 3 VCOs (saw/square), analog 12dB/oct filter, sequencer, MIDI, and SYNC I/O
- Not a Eurorack-powered module, but can interface with modular/sequencer systems

---

## Inputs & Outputs

| Jack/Terminal          | Type           | Function                                            | Voltage Range      |
|------------------------|----------------|-----------------------------------------------------|--------------------|
| DC 9V                  | Barrel Jack    | Power (use ONLY specified adapter)                  | 9V DC center+      |
| MIDI IN                | 5-pin DIN      | External MIDI note, sync, control                   | MIDI Standard      |
| SYNC IN                | 3.5mm TS (Mono)| Clock Input (step advance)                          | Up to 20V, typically 5V pulses (15ms) |
| SYNC OUT               | 3.5mm TS (Mono)| Clock Output (step pulse: for chaining devices)     | 5V pulse (15ms)    |
| Headphone OUT          | 3.5mm TRS      | Main audio output (also disables speaker)           | Line/headphone     |

> *No CV/Gate inputs for pitch or modulation. Only sync and MIDI input for control!*

---

## Panel Controls

### Knobs:
- **OCTAVE:** Select active keyboard octave
- **TEMPO:** Sequencer tempo
- **VOLUME:** Output level
- **VCO1/2/3 PITCH:** Pitch offset per VCO (+/- 1 octave)
- **CUTOFF (VCF):** Filter cutoff frequency
- **PEAK (VCF):** Filter resonance (emphasis)
- **EG ATTACK:** Envelope attack time
- **EG DECAY/RELEASE:** Envelope decay/release time
- **EG INT:** Envelope-to-filter depth
- **LFO RATE:** LFO speed
- **LFO INT:** LFO depth/intensity

### Buttons:
- **VCO1/2/3:** Toggle/mute active oscillators for editing/playing
- **FUNC:** Hold for accessing parameter/secondary functions
- **MEMORY:** Sequence memory access/save
- **STEP MODE:** Enter step sequencing mode
- **PLAY (►):** Play/Stop sequencer
- **REC (●):** Enter record mode

### Touchpad:
- **Multi-touch Keyboard:** Play notes (used for inputting sequence notes)

### Step Buttons (1-16):
- For sequencer steps, global settings, or saving sequences depending on mode

---

## Voltage/Control Summary

- **SYNC IN:** Accepts 5V clock pulse ("step" clock, not 1V/octave or gate), 15ms or typical modular gates fine
- **SYNC OUT:** Provides 5V clock pulse, 15ms, per step (can mult to modular for clocking)
- **Headphones OUT:** Main audio—can be patched to mixer or external modular effects, line level

---

## Hidden/Advanced Features

- **Step Recording, Active Steps, Slide Editing:** Hold FUNC, press REC/STEP MODE, edit on step buttons
- **Mute VCOs:** Hold FUNC + VCO1/2/3 button
- **Group VCOs:** Hold FUNC + step 1/2/3 (choose unison/chord mode for sequencing)
- **LFO Target:** FUNC + steps 4-6 (amp, pitch, cutoff mod)
- **LFO Shape:** FUNC + step 7 (triangle/square)
- **Oscillator shape per VCO:** FUNC + steps 8-10
- **Envelope Sustain/AMP:** FUNC + steps 11/12

---

## SYNC & Modular Use

- **SYNC IN:** Compatible with modular 5V triggers/gates for clock. Use as a sync'd sequencer or drum-clock source/target.
- **SYNC OUT:** Use as a clock source to chain to other gear, modular clock dividers, sequencers, etc.
- **No direct CV pitch or gate inputs!** Only step advance is supported for modular sync.

---

## Memory & Global Settings

- **Sequence Memory:** 8 slots (select with MEMORY + 1-8)
- **MIDI Channel:** Hold MEMORY while powering on, select 1-16
- **Battery Type/Other Globals:** Hold FUNC while powering on, set with step keys

---

## Reference

- **Audio Output:** Stereo mini-jack; can patch to modular mixers/recorders but may need attenuation
- **Sync Jacks:** Pass modular clocks/triggers directly; can clock from Eurorack modules

---

**[Korg Volca Bass Full Manual PDF](https://cdn.korg.com/user_manuals/volca_bass_OM_EFGSJ1.pdf)**

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)