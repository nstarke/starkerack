# Tiptop Audio — MODFX FSU

- [Manual PDF](../../manuals/Tiptop_Audio_fx_manual_MODFX_FSU.pdf)

---

[Tiptop Audio ModFx + FSU Manual PDF](https://tiptopaudio.com/manuals/FSU_MODFX_Manual.pdf)

---

# Using Tiptop Audio MODFX + FSU for Full-Length Eurorack Songs

Eurorack excels at incredible timbres, sequences, and textures—yet structuring these elements into engaging, evolving full-length songs can be a challenge. The Tiptop Audio **MODFX** and **FSU** modules offer a versatile toolkit not just for wild FX but for composition, arrangement, and sonic evolution. Below are strategies and patch ideas for integrating these modules into tracks that unfold dynamically from intro to finale.

---

## 1. **Song Structure via FX States/Scenes**

### A. **Preset Switching as Arrangement**
- Both MODFX and FSU have **8 programs per bank**, and bank changes can act as “scene” or “section” changes in your song.
- **Technique**: Sequence presets (via manual selection, or control with external CV and sequential switch modules) at key points. For example:
    - **Chorus enters:** Switch from a subtle phaser to a lush 6-voice chorus.
    - **Breakdown:** Move to a pitch-shifting granular or freeze effect.
    - **Build-up:** Switch to increasing feedback or drive/distortion for tension.

**External Help:** Modules like the **Malekko Voltage Block**, **Make Noise Pressure Points**, or even a simple **Gate/Trigger sequencer** can automate preset/button presses to change effects in time with your song sections.

---

## 2. **Live Morphing with CV Control**

- Both modules provide **three CV inputs** for continuous control.
- **Automate Dynamics:** Use LFOs, envelopes, random generators, or sequencers to modulate FX parameters in time:
    - Example: Sweep the **Depth** of a flanger in sync with your kick drum pattern for dynamic rhythmic movement.
    - Example: CV control filter cutoff on Tape Filter to simulate a filter sweep break.

**Tip:** Mult CV sources—send the same modulation that opens your bass filter to the depth parameter on MODFX’s chorus for a unified shift in multiple layers at once.

---

## 3. **Transition FX and Builds**

- **FSU’s GLITCH/WARP**: Use Random Grains, Glitch Chorus, or Varispeed to create rises, transitions, or breakdown artifacts.
- **Manual intervention:** Momentarily switch to extreme settings for fills, breaks or “DJ-style” effect sweeps.
- **Sound on Sound Banks:** Loop and degrade elements for breakdowns, then “clear” the buffer for a drop. Use envelope generators to punch the recording in/out at just the right spot for tight transitions.

---

## 4. **Layering and Song Evolution**

### A. **Parallel Processing**
- **Send/Return with Mixer**: Split your signal, process one version through MODFX/FSU for evolving textures, blend back in.
- **Result**: Create lush layers, ghostly echoes, or evolving pads beneath the main line. Animate their presence with the Mix knob (manual or VC).

### B. **Freeze/Looper Techniques**
- **Frozen Plate, SOS Buffer**: Capture a fragment, let it degrade or get modulated. Build motifs or “hold” moments for tension.
- **Manual or CV gate triggers** can punch in/out of looping for live arrangement improvisation.

---

## 5. **Generative & Algorithmic Song Structures**

- Use **random CV** (e.g. from Wogglebug, Turing Machine, or Pamela’s Pro Workout) to modulate effect states, constantly morphing the FX environment.
- Patch **sequencers** like Voltage Block or Hermod to recall specific effect parameter sets at each song section.

---

## 6. **Thematic FX Assignments**

- **Assign specific effects to song roles**:
    - **Intro:** Simple chorus or phaser, sparse “wet” mix.
    - **Verse:** Modest flanging, increased feedback.
    - **Chorus:** Lush 6-Voice Chorus or Tri Stereo Chorus, wide stereo.
    - **Bridge:** Switch banks for FSU’s Glitch/Looper FX for drama and transformation.
    - **Outro:** Sound on Sound looper with Buffer Degrade to slowly disintegrate your final motif.

---

## 7. **Example Song Structure Using ModFx and FSU**

| Section   | Patch / Preset                    | Performance Action |
|-----------|-----------------------------------|--------------------|
| Intro     | ModFx Tape Filter, subtle phaser  | Gradually open Depth with envelope |
| Verse     | ModFx Dual Flange or FSU Tape Sat | CV sweep Rate param for motion |
| Chorus    | ModFx 6-Voice Chorus, max Depth   | Preset switch, wide stereo, raise Mix |
| Break     | FSU Random Grain, Glitch Chorus   | Momentary FX, Engage Freeze/Degrade |
| Build     | ModFx Thru Zero Flanger (mono)    | Rate increases, feedback rises to climax |
| Finale/End| FSU SOS Buffer Degrade, Frozen Plate | Let loop degrade--fade out |

---

## 8. **Performance Tips**

- **Hands-on Play**: Use the illuminated buttons and knobs live for improvisational changes.
- **Sequencing FX**: Pair with gate/CV sequencers to trigger FX parameter shifts or program changes at planned moments.
- **Clocking**: Clock the DSP or mod LFOs from your project’s main clock for tight musical sync.

**Remember:** Songwriting in eurorack is about macro-shaping modulation, effect states, and layers, as much as about drums and melody. MODFX and FSU give you the palette to turn a loop into an evolving, performable track.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)