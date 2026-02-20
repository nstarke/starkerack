# ADDAC Systems — ADDAC-207 Quantizer

- [Manual PDF](../../manuals/ADDAC_207_Quantizer_REV05.pdf)

---

[ADDAC207 Intuitive Quantizer User’s Guide (PDF)](https://www.addacsystem.com/sites/default/files/files/ADDAC207%20Intuitive%20Quantizer%20Users%20Guide%20REV05.04.2021.pdf)

# How to Use the ADDAC207 Intuitive Quantizer to Create Full-Length Eurorack Songs

Creating jams or short loops in Eurorack is a blast—but ‘songifying’ a patch is a different challenge! The ADDAC207 Intuitive Quantizer is a powerful tool that, when used creatively with other modules, can help build dynamic, evolving, and structured full-length modular songs. Below is an analysis and some concrete ideas for leveraging the ADDAC207 in more “compositional” ways.

---

## Key Features of the ADDAC207 for Song Structure

- **Four independent quantizer channels (“voices”)**  
  Quantize up to four separate CV sources, which can be used for melody, harmony, bass, or other lines. They can share a scale/key or work independently.

- **User-definable & recallable scales, user presets**  
  Switch musical keys, scales, or microtuning on the fly or via CV, ideal for structured pattern changes (verse/chorus/bridge).

- **Assignable CV input for menu control**  
  Morph scales, change quantization type, transpose, alter gate lengths or trigger repeats—all dynamically with external CV for performative and automated changes.

- **Keyboard mode**  
  Use the front-panel buttons as a playable mono keyboard or chord trigger, great for hands-on performance sections.

- **Chord generation via interval assignment**  
  Assign fixed intervals (thirds, fifths, sevenths, etc) to other voices for instant harmonization and chord sequence changes.

- **Preset system**  
  Rapidly recall entire quantizer states.

---

## Song-Building Techniques & Patch Ideas

### 1. **Use Presets for Sections (Verse/Chorus/Bridge, etc.)**

- Save scales, intervals, and gate settings for each section into different ADDAC207 presets.
- Use the assignable CV preset change (assign CV to Preset switching) and trigger with a sequencer, LFO, or footswitch to move through song sections.  
  _**Patch Idea**_: Use a stepped CV sequencer to send different voltages to Preset CV input at each song section.

### 2. **Automate Scale and Key Changes**

- Assign your transpose input or scale CV assignment to an external sequencer for algorithmic/acoustic 'modulation'.
- For key modulations (e.g., up a fourth or down a minor third for bridges), use a precision adder/offset or sequencer to drive the transpose input.
- Use the microtonal features for special sections (e.g., an "otherworldly" bridge).

### 3. **Chord Progressions and Harmonic Evolution**

- Use one sequencer or random CV source for voice 1 (root), and assign intervals (third, fifth, seventh) to voices 2–4 for auto-harmonizing chords.
- Change intervals ‘live’, with assignable CV or gate. For example:  
  - Verse: Voice 2 = third, Voice 3 = fifth  
  - Chorus: Voice 2 = fifth, Voice 3 = seventh—switch with CV.
- Combine with a trigger sequencer to ‘revoice’ chords.

### 4. **Dynamic Arrangement Through Quantization Types**

- Use the “Ignore” mode (quantize only when in scale), “Above”, or “Below” to change melodic feel.
- Assign CV to Quantization Type and automate changes (for example, verse is “Above”, chorus is “Ignore”).

### 5. **Complex Phrasing and Rhythmic Variation**

- Vary Gate Lengths (per section or per voice) via remote control.
- Set up voice inputs to quantize only on incoming gate/trig—combine with rhythmic trigger sequencers or envelope generators for note density control.

### 6. **Create Evolving Melodic Lines or Riffs**

- Use slow, phased, or modulated random LFOs/sequencers for melodic motion into the quantizer, but recall new scales/presets over time to radically shift feel.
- Send clocked random or vector generators into voice 1 for semi-generative melodies, then evolve them by shifting scale or intervals.

### 7. **Performative Approaches**

- Use Keyboard mode to directly ‘play’ in melodies/chords for solos or live overdubs.  
- Combine with a looper or sampler module to record/resample generated motifs for classic “build and release” songwriting.

### 8. **CV-Scene Automation with Other Modules**

- **Sequencers** (e.g., Stillson Hammer, Eloquencer, Metropolis)  
  - Sequence ADDAC207’s Preset or Assign inputs for hands-off song structure changes.
- **Switches/Matrix Mixers** (e.g., Doepfer A-150, XAOC Warna)  
  - Route different CV sources into the quantizer at different song sections.
- **Random/Generative Modules** (e.g., Turing Machine, S&H)  
  - Feed evolving voltages, then steer the musical sense with scale/preset changes.
- **CV Recorders** (e.g., 4ms Looping Delay, Disting EX)  
  - Record dynamic assign CV motions for playback and repeatable ‘song’ automations.
- **Clocked LFOs/Euclidean Rhythms** for evolving trigger/gate patterns.

---

## Example Workflow for a Full-Length Song

1. **Intro**: Use a narrow scale/preset with long gates and slow random CV into one channel for an ambient start.
2. **Verse**: Switch to a full major/minor scale via preset, assign trigger/gate inputs to quantize melodically, use two or three voices for chords.
3. **Bridge**: Morph the scale (harmonic modulation), increase intervals (stack chords more densely), or invoke microtonality.
4. **Chorus**: Wider scale, more harmonies (activate all 4 voices in chord mode), faster gate lengths.
5. **Breakdown**: Change quantizer to “Ignore” type for sparse melodic lines, perhaps switch to Keyboard mode for live play or silence voices for a moment.
6. **Outro**: Return to initial scale/preset or dramatically modulate to an unexpected one for a twist ending.

All section changes can be pre-programmed by using a CV preset controller (e.g., via a sequencer or even manually), keeping your patch intact while the underlying musical structure evolves.

---

## Tips

- **Plan Scenes**: Decide what scales/modes/interval combos you'll use for different sections before you start the patch.
- **CV Animate Everything**: The more you control via assignable CV, the more 'song-like' your modular set will become.
- **Presets are Key**: Use all 11 presets—each can be a scene, moment, or song section.
- **Sync Everything**: Use a master clock and/or reset signal to keep changes and patterns in line.

---

For even more ideas and automation tools, check out eurorack utilities that can create programmatic or performable “scene” or “macro” control over multiple CV destinations.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)