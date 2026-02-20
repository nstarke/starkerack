# ADDAC Systems — ADDAC-112 Granular Looper

- [Manual PDF](../../manuals/ADDAC112_Granular_E_0.pdf)

---

[ADDAC112 VC Looper & Granular Processor Manual (PDF)](https://media.addacsystem.com/manuals/ADDAC112_manual.pdf)

---

# Using the ADDAC112 VC Looper & Granular Processor to Create Full Length Eurorack Songs

Turning modular jams into **structured, full-length songs** is one of the most challenging aspects of eurorack performance and composition. The ADDAC112 VC Looper & Granular Processor, with its deep real-time sampling, looping, and granular capabilities, offers a unique toolset for breaking the loop-based rut and introducing arrangement, variation, and narrative into modular music.

Below are strategies and patch ideas for integrating the ADDAC112 into full-length songs, especially in coordination with other eurorack modules.

---

## 1. Use Looper Banks & Presets for Song Sections

### **How It Works**
- The ADDAC112 allows you to create *banks* containing up to **99 loops** and **99 presets**.
- Each **preset** captures a state of granular and looper parameters—effectively saving a “scene” or “song section”.

### **Song-Building Technique**
- **Verse/Chorus/Bridge Structure**: Record different loops per section (e.g., loop 1: verse, loop 2: chorus, loop 3: bridge).
- Save relevant granular and processing settings as presets.
- Programmatically switch between **presets** or **loops** using CV or manual knob movement during performance, emulating arrangement changes like in DAWs.

### **With Other Modules**
- Use gate sequencers or footswitches to automate loop or preset changes.
- Combine with voltage-addressable sequencer modules (like SelectBus, Tetrapad, or Nerdseq) to program complex song arrangements.


---

## 2. Evolve Patterns Through Overdub, Granular Processing, and Real-Time Recording

### **How It Works**
- Real-time *overdubbing* with decay—gradually replacing loop material (think live tape experiments).
- Granular engine allows the same source material to be layered and transformed across the song.

### **Song-Building Technique**
- Start with a simple rhythmic or melodic loop; overdub slowly evolving new ideas or textures, allowing the old to fade out (using Overdub Decay).
- Automate or perform granular parameters (density, grain size, pitch, direction) over time—creating textural build-ups, drops, or dramatic moments.
- Use **granular parameters under CV** (from LFOs/envelopes/sequencers) to build or release musical tension.

### **With Other Modules**
- Feed evolving modulation (LFOs, Random, Complex CV) to control granular or looper parameters.
- Sync granular changes to rhythmic events in your patch with clock dividers/multipliers for musical cohesion.


---

## 3. Arrangement Control via CV/Triggers

### **How It Works**
- All parameters (loop select, preset select, playback direction, volume, and most grains parameters) have dedicated CV inputs.

### **Song-Building Technique**
- Use sequencer tracks or manually programmed gates to trigger:
    - **Loop changes (loop select CV)** at designated song moments.
    - **Playback direction reversals** for breakdowns or fills.
    - **Rec New / Play / Stop functions** for creating new sections or drops.
- Automate **grain density**, **panning**, or **pitch** for movement through the song (think dynamic chorus/verse textures).

### **With Other Modules**
- Trigger looper or preset changes from drum patterns, melodies, or synchronized events with clocked logic modules (e.g., Pamela’s New Workout, Tempi).
- CV from performative touch controllers for on-the-fly fills or dynamic structure changes.


---

## 4. Integration with Non-Modular Elements

### **How It Works**
- ADDAC112 accepts stereo line-level inputs—record and manipulate external synths, voices, or even a DAW stem loop.
- Easily save/load banks via SD card for repeatable performances.

### **Song-Building Technique**
- Print modular improvisations/loops into the ADDAC112, then perform song arrangements by morphing, chopping, or re-sequencing them.
- Resample live modular jams to create new evolving backgrounds or “glue” sections together.

### **With Other Modules**
- Use multi-channel MIDI-to-CV (e.g., FH-2, Shuttle Control) to sync with DAWs or drum machines.
- Sample vocals or acoustic instruments, granulate them, and arrange them alongside modular parts for song variation.


---

## 5. Clocked and Quantized Sections

### **How It Works**
- Clocked Mode syncs looper controls to an external clock, allowing hands-free arrangement changes.
- Granular and loop pitch can be **quantized** to musical scales (and scales can be customized).

### **Song-Building Technique**
- Create tight transitions and 'drops' by aligning record/play/clear actions to bars/beats.
- Employ quantized pitch changes for melodically coherent sections and improvisation.


---

## 6. Storing, Saving, and Repeatability

- Save banks, presets, and loops to SD for repeatable live sets. 
- Build songs in scenes, load them between sets, and recall instantly—essential for live performance workflows.

---

## Example Eurorack Full Song Workflow

1. **INTRO:** Record atmospheric texture loop into ADDAC112. Slowly granulate and overdub evolving sounds.
2. **VERSE:** Trigger loop switch to a beat or bassline loop, dry volume up, grains subtle for rhythm.
3. **CHORUS:** Switch preset; grains active and more dense, new loop introduced, pitch up, volume jump.
4. **BREAKDOWN:** Reverse playback, granular size maxed, extreme deviation, automated via CV.
5. **BRIDGE:** Feed external line-level loop (maybe a vocal or field recording), granulate heavily, lower main loop.
6. **OUTRO:** Fade grains and looper, reintroduce intro loop, decrease density and pitch, end.

Sync all structural changes via sequencer CV/gates, or perform them live via manual control.

---

## Key Patch Strategies with Other Modules

- **Programmable Sequencers/Controllers:** Automate song structure and parameter evolution with tracks of changes, not just musical notes.
- **Performance Switches or Touch Controllers:** Use footswitches, Planar, Tetrapad, or similar for hands-on scene switching.
- **Clock/Logic Utilities:** Sync changes to beats using Pamela’s New Workout, Temps Utile, or clocked switch modules.
- **CV Modulation Sources:** LFOs, random, and envelopes to add motion, evolving interest, and transitions.

---

For more, see the full manual:  
[ADDAC112 VC Looper & Granular Processor Manual (PDF)](https://media.addacsystem.com/manuals/ADDAC112_manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)