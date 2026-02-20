# Erica Synths — Sample Drum

- [Manual PDF](../../manuals/FINAL_sample_drum_instrukcija_A4.pdf)

---

[Erica Synths Sample Drum Manual (PDF)](https://www.ericasynths.lv/media/Sample_Drum_Manual.pdf)

---

# Using Erica Synths Sample Drum To Create Full-Length Songs in Eurorack

The **Erica Synths Sample Drum** is a powerful, versatile module for sample playback, slicing, and real-time manipulation—tailor-made for live performance, but also deeply useful for song construction in the modular environment. The common challenge in modular is not building great sounds, but turning them into full musical pieces that evolve, transition, and surprise over time. Here’s how you can leverage the Sample Drum to build full-length songs, in combination with typical Eurorack modules.

## Key Features Recap

- Two independent sample playback channels with CV assignable parameters.
- Manual/auto slicing, 1V/Oct pitch tracking, envelopes, effects.
- Real-time sample recording, editing, and cueing.
- Sample, slice, and project saving and recall for instant arrangement shifting.
- Fast, responsive trigger/playback for rhythmic precision.

## Song Structure: Overcoming the Modular Loop

Let’s break down the problem: In modular, it's easy to build beat-driven grooves or cool melodic fragments, but full tracks need **variation, progression, and arrangement**. Sample Drum’s features—especially dual multi-sample engines, flexible CV assignment, slicing, performance modes, and project recall—are your keys to unlocking full-length arrangements.

### 1. Set Up Song “Scenes” Using Projects

- **Projects** store everything: loaded samples, slicing, envelopes, FX, CV/encoder assignments.
- **Strategy:** Create one project per musical section (Intro, Verse, Chorus, Breakdown, etc.).
- **Recalling Projects:** Manually load these via the encoders, or automate with external triggers through other modules (if using sequenced or hands-on performance workflows).
- **Tip:** DOUBLE projects load both channels; SINGLE lets you swap sections with minimal disruption.

### 2. Evolving Beats & Basslines with Slicing and CV

**Slicing** allows you to chop breaks, melodic loops, or vocal samples into up to 32 slices:
- Assign CV/sequencer/lfo to **SLICE: INDEX** for drum breaks that morph pattern per bar, or for melodic riffs that jump around “slices” of the tune.
- **Performance trick:** Use a sequencer to shift slice position or reset slice order for fills, drops, or variations.

### 3. CV Assign Modulations and Parameter Locks

- Sample Drum allows any CV input to control almost any parameter (pitch, sample select, mode, start/end, FX, envelope).
- Construct long-form builds and variations by patching:
    - **Sequencers** (e.g. Malekko Voltage Block, Make Noise Pressure Points)
    - **LFOs** (for evolving FX, fading in bitcrush, changing reverb, or filter FX)
    - **Random/Chaos sources** (e.g., Wogglebug) for generative textural changes or fills.
- **Example:** Use a step sequencer to switch between Sample Drum’s loaded samples or FX types with every section for instant structural evolution.

### 4. Live Sample Recording & Manipulation for Transitions

- **Capture live loops or riffs** from other modules (using the Sample Drum’s audio input/rec function). Slice these up for improvisational fills or breakdown material.
- Drop in recorded vox or synth parts to instantly flip your arrangement.

### 5. FX and Envelope Automation

- Both FX and envelope parameters are CV-assignable! Use slow envelopes or step sequences to sweep reverb amount, filter settings, fold, or bitcrush.
- For classic song moments (build-ups, breakdowns, drops), automate decay times, morph attack shape, or shift to heavy FX with live controls mapped to Performance Mode encoders.

### 6. The Performance Menu: Your Live Arrangement Hub

- Assign the six main encoders to whatever parameters most need hands-on tweaking per channel in real-time.
- Snap parameters back to their saved state at the push of a button—great for recovering after “crazy” moments or prepping for a new section.
- Manual triggers for one-shots, fills, or hands-on scratching over a groove.

### 7. Using Multiple Sample Drum Modules (or Multitracking)

- Parallel Sample Drums expand tracks: drums+percussion on one, bass+melodics on another, or build stems for later “DAW-like” arrangement.
- Record one channel’s output for further resampling/manipulation.

---

## Example Modular Song-Form Patch

1. **Channel 1:** Sliced breakbeat loop. **CV1** input from sequencer steps slice index for verse, then resets for chorus.
2. **Channel 2:** Melodic or bassline one-shots. **CV2** connects to 1V/Oct sequencer for melodic content.
3. Mix Sample Drum outputs, route to FX modules (e.g., Clouds, Magneto) for space and depth.
4. **Arrange song:** Use performance mode encoders to morph FX, reset slices, bring in new patterns by loading projects, or modulating parameters live.
5. Bring in DAW or external looper if needed to record sections and layer in/out for more traditional arrangement.

---

**Remember**: Structure comes from change—muting, modulating, swapping samples/projects, and bringing in new rhythms or FX. The Sample Drum’s real strength is its flexibility in allowing you to trigger these changes with just CV, external triggers, or hands-on controls.

---

For even more creative automation and live patching tools, check this out:

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)