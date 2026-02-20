# Doefper — A-148

- [Manual PDF](../../manuals/A148_man.pdf)

---

[Doepfer A-148 Dual S&H System A-100 Manual (PDF)](https://doepfer.de/A100_manual/A148_man.pdf)

---

# Using the Doepfer A-148 Dual S&H to Build Full-Length Songs in Eurorack

The **Doepfer A-148 Dual Sample & Hold (S&H)** is a classic utility module, but its real power lies not just in creating random or stepped voltages, but in creatively "animating" your patch to add arrangement, variation, and motion—key ingredients for turning great loops into full songs. Below are concrete strategies and patch ideas for using the A-148 to break out of "loop hell," introducing structure, theme, variation, and performance elements.

---

## 1. **The S&H and T&H Duality: Beyond Simple Random**
The post-2005 A-148 lets you switch between **Sample & Hold (S&H)** and **Track & Hold (T&H)** modes. Use both modes in a patch to get stepped modulation or "latched" control as well as moments where modulations freely track their source.

- **S&H mode**: Signal is sampled at the rising edge of a trigger and held until the next.
- **T&H mode**: Signal follows the input while the gate is high, then holds when the gate falls low.

### Use-case for Song Arrangement:
- **Verse/Chorus Switching**: Use T&H mode to smoothly automate a parameter only during a "chorus section" (triggered via a performance controller or sequencer), and S&H mode for random or stepped changes elsewhere.
- **Live Arrangement**: Switch modes “on the fly” to mutate patches and accentuate section changes.

---

## 2. **Creating Macro-Variations and Song Sections**
Instead of modulating a single filter or oscillator, send S&H outputs to multiple destinations:

- **Stepwise Key/Root Change:** Patch an S&H output to a quantizer feeding your VCOs. Use another S&H to modulate the offset root note (key), switching between chord progressions or scales with each section, triggered by a clock divider/multiplier for song-length changes.
- **Timed Scene Changes:** Use sequencers or manual gate sources (e.g., from a performance controller, step sequencer, or even manual gate button) to change the S&H "scene" every 16 bars, 8 bars, or when you perform a transition.

#### Example Patch:
```
[Clock Divider] --- (slow triggers) ---> [A-148 Trig In]
[LFO / Random Source / Manual CV] -----> [A-148 Smp In] --->
  --(1)--> [Oscillator Pitch]
  --(2)--> [Filter Cutoff]
  --(3)--> [Effect Send Amount]
```

Change the root, tonality, or character of your whole patch on long time scales.

---

## 3. **Generating Rhythmic & Timbral Motifs**
- **Random Arpeggios:** Send LFO or irregular clocks to Trig In, random noise or stepped voltage to Smp In, and route S&H Out to your VCO Frequency CV. This gives you endless musical phrases, which evolve each time you patch or alter clock speed.
    - Use S&H into a VCF cutoff for evolving sequences.
- **"Theme and Variation":** Use one S&H for repeating melodic/rhythmic content, and the other for randomized counter-melodies, melodies, or modulations. You can clock each from different divisions for swirling, polyrhythmic variation—extendible over long stretches of a song.

---

## 4. **S&H as a Performance Tool**
- **Freeze the State:** In the middle of a song, momentarily stop the trigger clock to both S&H channels—this "locks in" whatever values the patch has. Use this for breakdowns, dropouts, or to arrest modulations, then bring them back for dramatic effect.
- **Manual Resampling:** Use a manual trigger (doepfer A-164-1 Manual Gate, or a momentary switch, or your controller interface) to "capture" a new value at key song moments.

---

## 5. **Glissando and Chord Articulation**
- Use the S&H, as described in the manual, for triggered glissandos or stepped pitch changes. These can act as transitions between song sections, or for expressive chromatic runs, which otherwise are hard to time in a modular setup.

---

## 6. **Randomized, Sync’ed Filter Scenes**
- As shown in the manual, patch S&H out to modulate the cutoff of a filter, but **trigger the S&H with a sync’d gate (e.g., keyboard gate, MIDI clock, or clock divider)**. Each new note or section brings in a new timbral "scene," just like filter sweeps in electronic breakdowns or builds.

---

## 7. **Dynamic Movement During Live Jams**
The module is dual—use both channels for max effect:
- **Channel 1:** High-frequency S&H (clocked with a fast LFO or random source) for quick modulations, "riff" level detail.
- **Channel 2:** Low-frequency S&H (clocked with a divided clock) to control overarching changes or state transitions, creating macrostructure over several song sections.

---

## 8. **Automated FX Scene Switching**
- Modulate FX mix or feedback settings with stepped output. Send different S&H out to different FX/parameters. Each section, triggered by a sequencer or scene controller, "rolls the dice" on new FX landscapes.

---

## 9. **Trigger Sequencing Across the Song**
Patch S&H output to logic or sequential switch modules to change routing, drum patterns, envelope times, or sequencer quantizer sources. This enables high-level song structure without needing a DAW.

---

## 10. **Forcing Movement Away from Loops**
- By building "meta-clocks" with different divisions/timings to the S&H Trig In, you introduce subtle, evolving changes that keep your song from repeating verbatim. Even subtle modulations of reverb, delay times, or waveshaper drive add life to transitions and sections.

---

## Final Tips

- **Combine with sequencers** for traditional note data, using A-148 modulation to bring continuous surprise and natural-sounding evolution.
- **Use externally-synchronized clocks** (MIDI, DAW, drum machine outs) to keep your S&H-based changes in sync with traditional song timelines.
- Tools like muting, mix/compression/eq within the rack can be combined WITH S&H macro modulation for studio-style arrangement options.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
