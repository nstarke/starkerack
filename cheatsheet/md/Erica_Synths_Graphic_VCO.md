# Erica Synths — Graphic VCO

- [Manual PDF](../../manuals/graphic_vco_manual_web.pdf)

---

[Erica Synths Graphic VCO User Manual (PDF)](https://www.ericasynths.lv/media/GraphicVCO_manual_2020.pdf)

---

# Erica Synths Graphic VCO  
**Quick Cheat Sheet / Reference**

---

## I. OVERVIEW  
- Eurorack digital VCO with fully programmable/drawable waveforms and FX.
- Morph between two waves, wavetable, and matrix wavetable modes.
- Extensive FX: FM, Phase Distort, Ring Mod, Wavefold, Wavewrap, Bitcrush.
- Save/recall waveforms, wavetables, FX, and full module states ("snapshots").

---

## II. FRONT PANEL CONTROLS

| Label                | Function / Usage                                                                                                 |
|----------------------|-----------------------------------------------------------------------------------------------------------------|
| **LCD SCREEN**       | Visual feedback. Shows menus, waveforms, wavetables, oscilloscope, etc.                                         |
| **Left Encoder**     | Main menu navigation, selects/edits left (A) wave, scrolls through menus or list, confirms by push.              |
| **Right Encoder**    | Secondary settings, selects/edits right (B) wave, FX parameters, oscillators, confirms by push.                 |
| **BACK Button**      | Go back one menu up. Hold 2s to save snapshot.                                                                  |
| **TUNE Knob**        | Master tuning, 16Hz–4kHz (wider range with 1V/oct CV).                                                          |
| **FX Amount Knob**   | Set FX depth or works as CV attenuator if CV patched (unipolar, 0–10V).                                         |
| **FX Param Knob**    | Set FX param (e.g. FM freq). Attenuates FX CV if present (bipolar, -10V–+10V).                                  |
| **MORPH Knob**       | Morph between A & B (or X in matrix), attenuates Morph CV (-10V–+10V).                                          |

---

## III. INPUT/OUTPUT JACKS & VOLTAGE RANGES

| Jack Label             | Function                                   | Voltage Range                 |
|------------------------|--------------------------------------------|-------------------------------|
| **1V/OCT**             | Pitch CV input                             | 0 to +8V (8 octaves)          |
| **FX AMT CV IN**       | FX amount control (unipolar)               | 0 to +10V                     |
| **FX CV IN**           | FX parameter (bipolar)                     | -10V to +10V                  |
| **MORPH CV IN**        | Morph CV (bipolar; matrix = vertical axis) | -10V to +10V                  |
| **MAIN OUT**           | Audio Output (main)                        | 10Vptp                        |
| **SUB/MIX OUT**        | Sub out or mix (configurable)              | 10Vptp                        |

*In matrix mode: FX CV = horizontal (X axis), Morph CV = vertical (Y axis).*

---

## IV. MAIN OPERATING MODES

1. **Morph Mode**  
   - Morph between two waves (A & B).
   - Draw/edit waves or select from presets.
   - Apply FX globally.

2. **Wavetable Mode**  
   - Select/play 16-wave wavetables, morph within.

3. **Wavetable Bank Matrix Mode**  
   - 2D matrix of wavetables (rows) and waves (cols); morph through X/Y or via CV.

---

## V. FX (EFFECTS)

- **Frequency Modulation (FM):** Internal OSC/Ext CV/manual; depth, freq, sync options; amount CV (unipolar: 0–10V), param CV (bipolar: -10V to +10V).
- **Ring Modulator:** Manual/internal/Ext mod; amount/param as above.
- **Phase Distortion:** Depth/amount.
- **Wavefolder/Wavewrapper:** Gain & offset for ext; select FOLD/WRAP.
- **Bitcrush:** Reduces bit/sample rate.
- **Overdrive:** Saturation.
- *FX are applied globally (not suboscillator, except FM).*

---

## VI. WAVETABLE/WAVE DESIGN

- Select, draw, or edit waves with encoders (incl. classic waveforms, line/pencil sketch, partials edit).
- Use morphing for in-between shapes.
- Save waves/wavetables to user memory.
- Manage, rename, delete waves and wavetables via the Manage menu.

---

## VII. SUBOSCILLATOR

- OUT2 outputs configurable suboscillator or mix.
- Parameters: Frequency offset (up to -24 semitones), detune (+-50 cents), mix % (out1 vs out2), assignable waveform.

---

## VIII. SYSTEM MENUS / SNAPSHOTS

- **Snapshots:** Save/load ALL settings (hold BACK 2s to save, menu to recall/delete/rename).
- **Oscilloscope:** Inspect wave, FX, and performance.
- **Device Setup:** CV in gain/bias, display settings, info, firmware update (via USB & Chrome app).

---

## IX. QUICK VOLTAGE REFERENCE

- **1V/Oct Input:** 0 – +8V (8 octaves)
- **FX Amount CV:** 0 – +10V (unipolar)
- **FX Parameter CV:** -10V – +10V (bipolar)
- **Morph CV:** -10V – +10V (bipolar)
- **Audio Outputs:** 10Vptp

---

## X. FIRMWARE UPDATE

- Requires USB mini connection, Chrome app, push both encoders while powering for bootloader.

---

## XI. SAFETY

- Not water resistant.  
- Operates -20° to +50°C.  
- Ship only in original packaging for support/warranty.

---

**For the complete manual, reference the official [Erica Synths PDF](https://www.ericasynths.lv/media/GraphicVCO_manual_2020.pdf).**  
**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**