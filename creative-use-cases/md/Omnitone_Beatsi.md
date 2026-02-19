# Omnitone — Beatsi

- [Manual PDF](../../manuals/Beatsi_Information_Package.pdf)

---

[Download the Beatsi Information Package PDF](attachment:file.pdf)

---

# Creative Eurorack Patch Ideas with Beatsi

As a modular synthesist, Beatsi offers a refreshing digital take on modular drum synthesis without relying on samples or physical modeling. Its tight control, seamless kit morphing, and dual assignable/attenuverted CV inputs open up plenty of innovative patch possibilities. Here are some ways to integrate Beatsi into a wider Eurorack setup:

---

## 1. Dynamic Drum Accents with LFOs & Modulation Sources

- **Use Case:** Animate Beatsi’s timbre, decay, or pitch knobs via LFOs (e.g., Malekko ADLFO, ALM Pam’s New Workout, or Make Noise Maths).
- **Technique:** Assign a sine or triangle LFO to **timbre**, slowly morphing between the acoustic, lo-fi, and alien kits for evolving percussive layers within a single pattern.  
- **Advanced:** Modulate **decay** with a stepped random or S&H signal from Mutable Instruments Marbles to randomize drum lengths per hit or pass.

## 2. Sequence-Driven Character Transformation

- **Use Case:** Use a sequencer with CV outs (e.g., Intellijel Metropolix, Erica Synths Black Sequencer) to send sequences to **pitch** or **timbre**.
- **Example:** Assign a sequencer’s CV row to the **pitch** input of the tom, creating tuned drums/basslines or melodic tom sequences.  
- Morph **timbre** with another row for kit switching on snare or hi-hat, adding variation and timbral movement to each bar.

## 3. Performance FX: Manual Kit Morphing and Mutes

- **Use Case:** Take advantage of the real-time mute function (press both parameter & value knobs) in live sets.
- **Tip:** Use a footswitch module (e.g., Befaco Instrument Interface) or external MIDI-to-CV controller (e.g., Arturia Beatstep Pro) to send triggers for mutes or immediate kit changes.

## 4. Envelope Follower and Audio Rate Modulation

- **Use Case:** Patch an envelope follower (Mutable Ears or Doepfer A-119) with external audio or drum loops as a CV source for Beatsi inputs.
- **Result:** The amplitude or transient activity of an incoming loop modulates Beatsi’s timbre or decay in real-time, "sidechaining" modular drum tones to an external groove.

## 5. Additive and Unusual Percussion

- **Use Case:** Combine Beatsi’s OUT with another digital percussion module (e.g., Noise Engineering Basimilus Iteritas Alter, Tiptop One) into a mixer (Intellijel Mixup, WMD Performance Mixer).
- **Result:** Use morphing CV to glue or differentiate Beatsi’s tones from other more static drum sources, or to provide fill-in textures between hits from traditional samplers.

## 6. Generative and Self-Patching Patches

- **Use Case:** Use logic modules (Make Noise Maths, Mutable Kinks, or Intellijel Plog) to generate complex gates/triggers for multi-part rhythms over Beatsi’s various drum triggers.
- **Advanced:** Self-patch Beatsi’s TOM CV output (if present) or envelope outs from other modules back into Beatsi’s CV1/CV2 to create feedback-driven evolving percussion.

## 7. Bitcrush and Glitch FX

- **Use Case:** Since Beatsi’s lo-fi and alien kits already include bit reduction and downsampling, abuse this by patching fast digital noise or stepped random CV (Wogglebug, Turing Machine, Ornament & Crime) into **timbre** or **decay** for broken-glitch digital percussion.

---

## Recommended Generic Modules for Advanced Patch Techniques  

- **CV Modulators:** LFOs, Random Sources, Envelopes, Sequencers  
- **Logic/Utilities:** Clock dividers/multipliers, AND/OR logic, S&H  
- **External Audio Integration:** Envelope Followers, Audio-to-CV  
- **Controllers:** CV/MIDI-to-Gate, Pressure Points/Touch Controllers  
- **Mixers:** For summing and parallel drum sound layering  

---

## General Tips

- **State Saving:** Remember Beatsi’s auto-save after 5 seconds of inactivity; plan your live tweaks accordingly!
- **Attenuversion:** Experiment with negative CV routing to invert envelope contours for offbeat or reversed drum FX.
- **Open/Closed Hats:** Patch creative gate/trigger combos for open and closed hi-hat simulation using other rhythm tools.

---

For further information, and to expand with community-sourced utilities:

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)