# Mutable Instruments — Plaits

- [Manual PDF](../../manuals/Mutable Instruments - Plaits.pdf)

---

[Mutable Instruments Plaits Manual (PDF)](https://mutable-instruments.net/modules/plaits/manual.pdf)

---

# Using Mutable Instruments Plaits to Create Full-Length Eurorack Songs

Mutable Instruments Plaits is a versatile macro-oscillator capable of a wide variety of synthesis models, from classic analog waveforms to physical modeling and drum/percussion sounds. While it is easy to create interesting sounds or short patterns with Plaits, building these into a structured, evolving, full-length song requires some planning and integration with other modules. Below are strategies, patching tips, and approaches to using Plaits as the core voice in a complete eurorack performance.

---

## Song Construction Strategies

### 1. **Use Model Morphing for Movement and Theme Evolution**
Plaits is designed for sonic variety. It can morph from melodic synths, chords, through drums and noise:

- **Automate Model Changes**: Use CV sequencers, random sources, or manual Model button changes to switch synthesis models as your song progresses—e.g., starting with a chord/harmonic model for intro, transitioning to percussion models for a beat drop, then moving to formant or noise for a break.
- **Use Trigger Quantization**: Patch the TRIG input so model changes only happen at rhythmic points in your sequence, helping transitions feel musical and deliberate.

### 2. **Exploit CV Modulation for Dynamic Variation**
Inject continuous interest in your patch by modulating Plaits' controls:

- **Sequence the Timbre/Morph/Harmonics**: Route LFOs/envelopes/sequencers to Plaits’ parameters. Use slow, evolving modulation in intros or breakdowns. Use punchy, rhythmic modulation to match beats and fills.
- **Patch Envelopes & FM**: Envelope generators and complex modulations can give each note or phrase new timbral life, essential for long-form musical development.

### 3. **Layer Multiple Plaits (or Voices) for Arrangement**
While a single Plaits can't be truly polyphonic, you can build interest by:

- **Multi-tracking**: If you have more than one Plaits or another voice/module (e.g. Rings, Braids, or analog VCO), split roles between lead, bass, and percussion—each following the evolving song structure.
- **Sampling**: Record Plaits melodic or percussive parts into a sampler and re-use/chop them for new sections.

### 4. **Integrate with Sequencers and Utilities for Structure**
Plaits shines when externally sequenced and modulated:

- **Step/Pattern Sequencers**: Use a Eurorack pattern or gate sequencer (e.g. Pamela’s Pro Workout, Intellijel Metropolix, or a MIDI-to-CV converter) to trigger notes, model changes, or envelopes. Sequence verse/chorus/bridge sections by changing patterns on your sequencer.
- **Switches and Matrix Mixers**: Patch sequencer outputs through voltage-controlled switches (e.g., Doepfer A-150 or similar) to route different controls to Plaits’ CV inputs in different song sections.
- **Logic Modules/Clock Dividers**: Create “song sections” by using logic modules to switch between triggers, modulations, or voice assignments.

### 5. **Take Advantage of Dual Outputs**
- **Layer Aux/Main**: The OUT and AUX outputs give variant flavors of the model (e.g., chord plus root, kick plus snappy snare variant, or main plus sub oscillator). Use a stereo mixer or dual tracks in your DAW to create a larger, more complex soundscape.
- **Parallel Processing**: Process OUT and AUX through different effects (FX, filters, delays), then fade/morph between them for arrangement changes.

### 6. **Performance Controls and Live Interaction**
Perform live tweaks for dynamic arrangements:

- **Manual Model and Range Switching**: Use Plaits’ buttons to trigger model switches, LPG response, or frequency ranges during performance for fills or drops.
- **Modulate Level CV**: Use LFOs, envelopes, or sequencers to rhythmically open/close the internal LPG (Level input), creating automated mutes, fades, or “sidechain” effects.

### 7. **Apply External Effects and Mixing**
- **Evolving FX**: Rout Plaits into stereo effects (e.g., reverb, delay, phaser), modulate FX parameters via CV for swelling intros/builds/drops.
- **Send/Return Automation**: Use VCAs to send more or less of Plaits’ outputs to effects at different song sections.

---

## Example: Song Section Flow

Consider the following arrangement approach:

1. **Intro**: Model set to additive, chord, or granular. Slow LFO to Morph/Timbre for gradual build. Bright FX.
2. **Verse**: Clean analog/wavetable voice, with evolving Harmonics. Structured by sequencer and tight envelope.
3. **Chorus**: Model morph to chords, denser textures. AUX mixes in for stereo width. Filter opens up.
4. **Breakdown**: Switch to formant/noise/drum, minimal melody. Modulate LPG decay for percussive hits.
5. **Drop**: Drum model, aggressive Morph, Model switching by trigger/sequencer, synced to rhythm.
6. **Outro**: Back to granular/additive, reintroduce slow FX modulations, fade Level.

---

## Module Pairing Suggestions

- **Sequencers**: For melody, rhythm, and model automation (e.g., Eloquencer, Rene, Hermod, or simple analog sequencers).
- **Envelope Generators**: For shaping and “animating” Plaits’ parameters.
- **VCAs/Modulation Utilities**: For dynamic patch changes and routing.
- **Switches/Logic**: To create song part “scenes.”
- **FX Units**: For space and drama—dedicate a reverb/delay, modulate wet/dry over time.
- **Samplers/Loopers**: Record/loop Plaits outputs, re-trigger at will.

---

## Tips for Moving Beyond Loops

- **Automate or perform everything**: Use random or evolving CVs, sequenced pattern changes, or hands-on tweaking.
- **Build breaks, fills, and transitions**: Program model & timbre switches, mute/fade parts, introduce FX swells.
- **Record and edit**: Live record your modular jams and refine the best takes into a full “song” in your DAW or via multitrack modules.

---

## Additional Resources

- [Plaits Synthesis Model Demos (YouTube Playlist)](https://youtube.com/playlist?list=PL2OKvuc7x17PuE4-KdvT5lo4-ywBoaiZv)
- [Mutable Instruments Official Site](https://mutable-instruments.net/modules/plaits/)
- [Plaits User Patches and Tricks (Modwiggler Thread)](https://www.modwiggler.com/forum/viewtopic.php?t=227856)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
