# TAKAAB — Odd Clock Divider

- [Manual PDF](../../manuals/TAKAAB OCD - Odd Clock Divider – Siam Modular.pdf)

---

[TAKAAB OCD - Odd Clock Divider Manual (PDF)](https://siammodular.com/products/takaab-ocd-odd-clock-divider?srsltid=AfmBOopTsJBGyNaC6WtMfJJU3EFzdu1WvzDldMz3y6eA2c-lwQCE1iKj)

---

## Using the TAKAAB OCD Odd Clock Divider to Help Structure Full-Length Eurorack Songs

### Overview

The **TAKAAB OCD** module is a 2HP eurorack clock divider focused on odd and less-common clock divisions, offering you outputs at 1/3, 1/5, 1/7, 1/9 (switchable to 1/6), and 1/10 divisions. Each output is a 6V gate and responds to clock rates up to 10kHz. It also features a reset button/jack for synchronized pattern resets.

Turning loops and patterns into full songs in modular is often about organizing variations, evolving sections, triggering transitions, and introducing generative structure. Having odd divisions (vs. standard binary divisions) unlocks asymmetrical phrasing and unique polyrhythmic relationships—perfect for song length arrangements.

---

### Key Use Cases for Full Song Arrangement

#### 1. **Polyrhythmic Song Sections & Evolution**

By patching a master clock to the OCD, you have five streams of pulses at unusual intervals. Use these to:
- **Trigger different voices:** Connect 1/3 out to your bass drum, 1/5 to a melodic sequencer, 1/7 to modulation events, etc.
- Over time, fade in/out voices or swap outputs between voices to evolve the complexity.
- **Result:** Your basic pattern morphs into intertwined polyrhythmic layers, extending the interest beyond a simple loop.

#### 2. **Algorithmic Section Changes (Song "Scenes")**

- **Send OCD outs to sequential switches** (or logic modules like OR gates) to change which sequencers, drums, or effects get triggered at different divisions.
- **Combine with a manual/automated reset**—for example, send a burst or dedicated reset pulse at bar boundaries to make everything loop together in a musical way, creating distinct numbers of bars per "scene."
- **Result:** Transition between song sections, e.g., 8 bars of polyrhythm, synced breakdown resets, and new builds triggered by OCD resets.

#### 3. **Event and Fill Trigger Generator**

- Use one of the odd divisions (like 1/9 or 1/10) as a fill or break trigger—use a sequential switch, logic, or sample & hold to select new sounds or activate effect sends whenever these rare triggers hit.
- For greater song structure, use a manual or clocked reset to align these fills with your phrasing.

#### 4. **Generative Arrangement Control**

- Patch OCD outs to control the **enable/disable** of sequencers, logic, AND gates, or VCAs that gate entire sub-patches.
- Use the irregular triggers to "mute" or "unmute" layers, so your arrangement organically evolves as rare-gates emerge.
- Combine with quantizers, comparators, or random voltage processors to tie musical changes to rare events.

#### 5. **Synchronizing Other Modulation/Events**

- The reset input (and daisy-chain reset header) allows you to sync multiple clock dividers for complex, multi-part arrangements.
- Use a master manual button or an LFO/clocked pulse to reset all rhythm and modulation sources, creating synchronized phrase resets or drops.

---

### Example Patch Scenario

- **Master Clock → OCD clock in**
- OCD 1/3 out → Bass Drum Trigger (gives a wonky triple meter)
- OCD 1/5 out → Sequencer Advance (odd-meter melody)
- OCD 1/7 out → Envelope for effect modulation (slow, evolving filter sweeps)
- OCD 1/9 out (or 1/6) → Trigger for manual scene/chord change via switch/logic
- OCD Reset in → Gate from performance controller or a slow LFO synced to measure/phrase (song transitions)

By combining, muting, or repatching these over the course of your set, you guide your patches beyond endless loops into structured, evolving full-length tracks.

---

### Bonus Tips

- **Combine with Even Dividers:** Add in a classic clock divider for contrast—alternate between "binary" and "odd" sections by swapping triggers.
- **Automate Resets:** Use step sequencers or clocked random generators to reset the OCD at strategic song points for structured breakdowns or transitions.
- **MIDI/DAW Sync:** Use the OCD in tandem with MIDI clock-to-trigger converters for tight hybrid or synchronized live jams.

---

For advanced programmable arrangements and ideas, check out this resource:  
[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)