# ALM — ALM005 - Dinky's Taiko

- [Manual PDF](../../manuals/alm005-manual.pdf)

---

[**ALM-005 ‘Dinky’s Taiko’ Manual (PDF)**](https://busycircuits.com/docs/alm005-manual.pdf)

---

# Using ALM-005 ‘Dinky’s Taiko’ to Build Full-Length Eurorack Songs

The **ALM-005 Dinky’s Taiko** is a highly versatile digital drum voice module with richly voltage-controllable parameters, making it capable of far more than just static drum hits. To turn cool grooves into full-length songs and evolving arrangements in a Eurorack environment, you’ll need to combine its strengths with the sequencing, modulation, and mixing capabilities of other modules. Here’s how to get there:

---

## 1. **Understanding What Taiko Can Do**

- **Sound Palette**: Dinky’s Taiko can cover a huge range of percussive, metallic, blip, noise, and synthesized drum sounds—any slot in a conventional drum kit, as well as more experimental percussion and tuned tones.
- **Voltage Control**: Nearly every parameter (except EQ tilt) is voltage-controllable, permitting rich modulation.
- **Choke and Accent**: Unique performance control inputs for dynamic variations per step.

---

## 2. **Moving from Loop to Song**

A single pattern rarely makes a great full-length track. Here's how to expand the Dinky’s Taiko role across an entire song:

### **A. Sequenced Variation & Pattern Changes**

- **Sequencers**: Use a polymorphic or multi-track trigger sequencer (e.g., **ALM Pamela’s PRO Workout**, **Mutable Grids**, **Intellijel Metropolis**) to send both triggers and accents/chokes for evolving patterns.
- **Multiple Patterns**: Program intro, verse, chorus, bridge, breakdown, and fills—send different trigger/accents per song section.
- **Live Pattern Change**: Manually switch patterns or sequence scene/slot changes.

### **B. Modulation Over Time**

- **Precisely Modulate Parameters**: Use LFOs, envelopes, or function generators (like **Make Noise Maths**, **ALM Pam's** or **Malekko Voltage Block**) to sweep or step through parameters such as:
    - **Spectrum**: Morph noise brightness for verse vs. chorus.
    - **Release & Speed**: Shorten/lengthen for breakdowns or fills.
    - **Freq Start/End & Wave**: Move from a standard drum to clangy FM or digital zaps for dramatic changes.
- **Randomization**: Send S&H or random stepped voltages (e.g., **Wogglebug**, **Turing Machine**) to selected inputs for fills or glitchy sections.
- **Visuals as Cues**: The output LED helps check signal change intensity live.

### **C. Macro Arrangement and Performance Techniques**

- **Manual Control**: Fade between Noise and Oscillator sounds using the **Mix** knob (or modulate with CV for automations/build-ups).
- **EQ Tweaks**: Tweak the EQ for brighter/darker sections by hand.
- **Accent/Choke for Dynamics**: Accent to bring attention or hit harder, choke for immediate cuts or gating.

---

## 3. **Interaction With Other Modules**

### **Layering and Multitimbrality**

- **Multiple Dinky’s Taikos**: Chain two or more units for polyphonic percussion or tuned drum melodies.
- **Run Through Effects**: Send outs to reverb, delay, or distortion modules (**ALM MFX**, **Strymon Magneto**, **Desmodus Versio**).
- **Further Processing**: Send into VCAs for external envelopes, or filters for spectral animation.

### **Mixing For Structure**

- **Automated Muting/Cuing**: Use mutes, crossfaders, or voltage-controlled switches/VCAs to drop in/out drums section by section.
- **Submixers**: Blend Dinky’s Taiko with other drums, synth voices, or samples for evolving textures.

### **Melodic Role**

- **Tuned Percussion**: Use CV pitch sequences into **Freq Start/End** for basslines or melodic percussion—the changes don’t track 1v/oct but melodic shape is possible.
- **Wave Scanning**: Sequentially scan through the 24 waveforms with step sequencer or LFO for timbre changes.

---

## 4. **Example Full Site Patch—Building a Track**

```text
- Use Pamela’s PRO Workout to trigger Taiko, sending base rhythm, accents on chorus, and chokes in fills.
- Add an LFO to sweep release or mix over the course of a build-up/transition.
- Sequence Freq End CV for tonal changes in melody/percussion lines during bridge.
- Perform manual EQ/mix tweaks for intro/outro dynamics.
- Use a VCA or mute to drop Taiko out for a breakdown, bring back in for the drop.
- Process output with delay/reverb for larger chorus sections.
- For longer jams, use a CV switch to change between pre-patched LFO/envelope mod sources per song section (verse, chorus, etc.).
```

---

## 5. **Tips for Full-Length Arrangements**

- **Storyboard** your track: plan which parameters and triggers should evolve through the intro, verse, chorus, bridge, and so on.
- **Automate** with slow modulation sources: set sweeping LFOs/envelope generators to ramp or morph sounds over minutes.
- **Utilize Choke** for both rhythm gating and call-and-response phrase structure between percussion elements.
- **Treat Taiko As A Voice**: melodic percussion, noise wash for atmospheres, or spot accent instrument (not just as static drum).

---

## 6. **More Resources**
- [Official ALM-005 ‘Dinky’s Taiko’ Manual (PDF)](https://busycircuits.com/docs/alm005-manual.pdf)
- [ALM Busy Circuits Website](https://busycircuits.com/)
- [Eurorack Songwriting Tips (ModWiggler Forum)](https://modwiggler.com/forum/)
- [Eurorack Patchbook (DivKid)](https://www.youtube.com/playlist?list=PLbKqg5gx1n3h2Hsvphx6wjItYlGlVf3pX)

---

[**Generated With Eurorack Processor**](https://github.com/nstarke/eurorack-processor)