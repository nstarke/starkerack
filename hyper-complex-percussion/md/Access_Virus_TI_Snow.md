# Access Virus — TI Snow

- [Manual PDF](../../manuals/Virus_TI_Snow_Quickstart.pdf)

---

[Access Virus TI Snow Quickstart Manual PDF](https://www.access-music.de/VirusTI/Downloads/VirusTIQuickstartManual.pdf)

---

## Using the Access Virus TI Snow for Hyper-Complex Percussion and Dense Rhythmic Music

Although the **Virus TI Snow** is not a Eurorack module but a desktop/digital synthesizer, it is an extremely powerful and versatile sound engine, well-suited for integration with modular or DAW setups for futuristic percussion and polyrhythmic complexity. Here’s how you can push it into densely rhythmic, polyrhythmic, and hyper-complex percussion/rhythm, using its features creatively:

### 1. **Multitimbral Percussion Kits (Multi Mode)**
- **4-Part Multitimbrality:** Use each of the four multitimbral parts for different percussive sounds or layers. Assign kick, snare, hat, and a “weird”/FM/percussion element on each part.
- **Split/Layer:** Assign different MIDI channels/zones for each, layering or key-zoning across your MIDI controller or sequencer.

### 2. **Sequencer or Arpeggiator Complex Patterns**
- **Internal Arpeggiator:** Access the [Arp Menu](#) to create intricate patterns. You can assign unique arpeggiator rhythms (up, down, random, chord, user pattern) to each timbre.
    - Select different Patterns per part. There are 64 rhythmic patterns, and the ARP allows for **user pattern editing** in the Virus Control software.
    - Sequence triplets on the snare, 5-step patterns on the hat, and longer cycles (13-step, 7-step) for FM percussion—polyrhythm by mapping *different length arps* to each part.
- **Polyrhythms:** Drive the arpeggiator clock for each part from external MIDI or DAW clock divisions (use different divisions for each part via DAW MIDI routing).
- **Advanced Sequencing:** In DAW mode, sequence each timbre independently, using different time signatures and step counts for complex polyrhythmic layers.

### 3. **LFOs and Modulation for Hyperactive Patterns**
- **Multiple LFOs Per Voice:** The Virus provides 3 LFOs per part, each can be set to independent rates or sync’ed to clock with complex clock divisions.
    - Use LFOs to modulate filter cutoff, pitch, and sample start/end or even effect sends for percussive flutter, pitch modulation, or rhythmic gating.
    - Set LFOs to different clock divisions (e.g., 1/8, 1/5, 1/7, dotted, triplet, etc) across parts for maximal polyrhythm.
- **Envelopes:** Use super-short attack/decay with high filter resonance to create clicky, zappy percussive “pings.” Adjust envelope times for mechanical or organic feel.

### 4. **Oscillator Tricks for Drum Design**
- **HyperSaw in Percussion:** Configure a HyperSaw oscillator with high detune at 1-2 voices for metallic digital hats or clangorous FM bells.
- **FM Amount (Osc 2):** Extreme FM (frequency modulation) can turn the Virus into a wild digital percussion generator.
    - Quick envelope FMs for zaps, laser “pewps,” or conga-like “blips.”
- **Wavetable & Formant:** Modulate the wavetable or formant oscillator index with LFOs at audio rate or with mod envelopes for weird, evolving “machine percussion.”

### 5. **Filters & Distortion for Punch**
- **Aggressive Filtering:** Use serial or parallel filters, sweep cutoff with velocity or envelope for snap and variance.
- **Filter Saturation:** Try the more extreme saturation types for ‘lo-fi’ digital or analog punch.
- **Parallel Filtering:** Route oscillators through different filter circuits for left/right contrast or layered transients.
- **Resonant “Clicks”:** Dial in medium-high resonance with fast cutoff envelope for sharp drum attacks.

### 6. **Effect Processing as Percussive Shaper**
- **Delay:** Use very short clocked delays for comb filtering; adjustable send per part for stereo “bounces.”
- **Phaser/Chorus:** Set to fast modulation for “flam” or “ghost note” feel.
- **Reverb:** Use subtle reverb for space, but go extreme for texture—note that heavy reverb eats polyphony.

### 7. **Automation and Randomization**
- **DAW Automation:** Automate filter types, oscillator FM, and effect sends.
- **Patch Randomization:** Use random LFO phase or manual patch editing for ever-evolving percussion grooves.
- **Mod Wheel/Aftertouch:** Assign these controls to nested modulations (e.g., mod wheel for FM amount & LFO depth).

### 8. **External Integration / Eurorack Cross-Over**
- **Audio Input:** Route modular drum hits into the Virus for further destruction via Virus filters/effects.
- **MIDI-CV Integration:** Use a CV-to-MIDI converter or MIDI-to-CV interface to sequence the Virus from Eurorack sequencers like the Malekko Varigate or Winter Modular Eloquencer.
- **Live Resampling:** Sample Virus percussion into Eurorack samplers (Assimil8or, Morphagene, 1010 Bitbox, etc) for further chopping/granularization.

---

**Summary Patch Construction:**
- **Each Part:** Set up as a percussive voice with different ARP patterns, LFO modulations, and clock sync ratios.
- **Oscillator tricks:** HyperSaw for claps/hats, FM clangors, classic sine for 808ish kicks, wavetables for spooky noise percussion.
- **Filter:** High resonance, fast decay.
- **Amp envelope:** Snappy or long tail for variation.
- **Effects:** Short delays, aggressive phaser, bitcrush on select parts.

---

For deep specifics, consult the [Virus TI Snow Quickstart Manual PDF](https://www.access-music.de/VirusTI/Downloads/VirusTIQuickstartManual.pdf) (see ARP Menu, Multi Mode, LFO Sync, Effects, etc for step-by-step menu navigation).

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)