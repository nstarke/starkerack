# 2hp — MMF

- [Manual PDF](../../manuals/2hp_MMF.pdf)

---

[MMF 2HP Multimode Filter Manual PDF](https://2hp.com/manuals/mmf_manual.pdf)

---

# How to Use the 2HP MMF to Create Full-Length Eurorack Songs

The **2HP MMF** is a compact analog multimode filter (low-pass, high-pass, band-pass) with CV control for both cutoff frequency and resonance. While filters are essential for shaping and animating timbres, their real power in modular systems lies in how they can interact with other modules to create evolving, musical structures that last beyond a simple loop.

Here’s how you can use the MMF filter creatively to progress from loops to full tracks:

---

## Key Features of MMF

- **Inputs:** Audio in
- **Freq control:** Manual CV and knob (cutoff frequency)
- **Reso control:** Manual CV and knob (resonance)
- **LP/HP/BP outputs:** Simultaneous 2-pole Low Pass, High Pass, Band Pass
- **Slim design:** Only 2HP wide

---

## Techniques for Full-Length Song Creation

### 1. **Dynamic Filtering for Structure and Progression**

- **Verse/Chorus/Energy Stages:**  
  - Use envelopes, LFOs, or sequenced CV to sweep the cutoff "Freq" knob. Start with the filter closed (low cutoff) for verses and open it for choruses or ‘drops.’
  - Patch a CV sequencer or automation source into the **Freq CV** input so different song sections have distinct timbres.
- **Resonant Peaks for Accents:**  
  - Sequence the "Reso" CV input to add or remove resonance at key moments — for builds, breakdowns, or tension.

### 2. **Multitimbral Layering via Multiple Outputs**

- Simultaneously use the **LP**, **HP**, and **BP** outputs. Route these separately:
    - LP for warm bass or pads
    - HP for bright sizzle or accent layers
    - BP for dynamic mids or additional percussion tones
- **Crossfade or Mix:** Transition between outputs (using VCAs or stereo panners) across song sections to introduce movement and variation without changing your original pattern.

### 3. **Automated Modulation for Evolving Patterns**

- Use random CV sources (e.g., Sample & Hold, Turing Machine) to modulate cutoff/resonance, creating subtle, non-repetitive evolutions.
- Envelope followers can modulate the filter dynamically in response to drums, vocals, or other rhythmic sources—intensifying crescendos or breakdowns.

### 4. **Performance Macros & Manual Interaction**

- Assign the **Freq** or **Reso** CV inputs to macro controllers, multistep sequencers, or even MIDI-to-CV controllers for hands-on, performative filter sweeps and drops.
- Manually perform with the filter in key moments to emphasize transitions, tension, or release.

### 5. **Percussive & Bass Variation**

- For drum lines: Use filters to carve different frequency zones per drum voice and automate their timbres for breaks and fills.
- For basslines: Route the sequence through MMF and automate resonance or cutoff to articulate verse/chorus/fill structure.

### 6. **Sidechaining and Ducking**

- Patch an envelope follower or sidechain CV (e.g., derived from a kick drum) to the filter’s cutoff. This creates space and punch by dynamically filtering out frequencies when the kick hits, resulting in a tighter, more musical mix.

### 7. **Arrangement through Filtering**

- Gradually open the filter cutoff at song start, or close it at the end for organic intros/outros.
- Use voltage-controlled switching/sequential switches to alternate which filter output feeds various effects or destinations for scene changes.

---

## Example Patch Flow for a Song Structure

1. **Intro:** Filter fully closed on LP output, minimal resonance. Gradually open with an envelope, bring in HP output for shimmer.
2. **Verse:** Moderate cutoff on BP output, low resonance for clear articulation of rhythms.
3. **Chorus:** Open LP and HP, add resonance for brightness, possibly modulated with a synced LFO for sweeping effect.
4. **Breakdown:** Drastically sweep cutoff shut, while slowly increasing resonance for tension. Drop certain filter outputs for focus.
5. **Drop:** Snap filter open, introduce all three outputs, automate cutoff for movement.

---

## Complementary Modules To Expand Musicality

- **Sequencers:** For cutoff/resonance modulation (e.g., Pamela’s New Workout, Voltage Block)
- **Function Generators/Envelopes:** For dynamic sweeps and rhythmic filter control (e.g., Maths, Batumi)
- **Random CV/Chaos/Noise:** Source of evolving filter movement
- **VCAs:** For volume/fade automation post-filter
- **Stereo Mixers:** For panning/mixing the different filter outputs
- **Effect Processors:** To add spatial depth to each filter output (delay, reverb, distortion)

---

## Closing Thoughts

By integrating smart modulation, creative routing of multiple filter outputs, and dynamic performance techniques, the MMF becomes a tool for not just timbre shaping, but for crafting the structural, emotional, and energetic progression needed to turn eurorack patches into full-length, expressive songs.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
