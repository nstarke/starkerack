# Happy Nerding — FM AID

- [Manual PDF](../../manuals/FM-AID-USERS-GUIDE_2020.pdf)

---

[FM AID | 2020 VERSION | USER GUIDE (PDF)](https://happynerding.com/manuals/FM_AID_2020_USER_GUIDE.pdf)

---

# Creative Ways to Use the Happy Nerding FM AID in Your Eurorack System

The Happy Nerding FM AID is an incredibly flexible analog module for through-zero frequency modulation, enabling both classic and experimental synthesis techniques. Here's a detailed exploration into how you can creatively leverage its unique features in your system, including module pairing ideas and workflow inspiration.

---

## 1. **Classic FM Synthesis: Pair with Analog VCOs**

**Modules:**  
- *Intellijel Dixie II+, Doepfer A-110, ALM Busy Circuits MCO, Befaco Even VCO*

**Patch Idea:**  
- Use a sine or sawtooth from a primary VCO as the Carrier input.
- Use a different waveform (tri, sine, complex shape) from a second VCO as the Mod input.
- Experiment with different frequency ratios, such as 1:1, 2:1, or non-integral ratios for more inharmonic results.
- Use the FM AID's multiple outputs (sine, tri, saw, square) to feed a stereo or quad effects chain.

**Why:**  
Achieve classic Yamaha DX-style and metallic or bell-like timbres, but with the warmth and artifacts of analog circuitry.

---

## 2. **Wave Folding & Complex Tone Generation**

**Modules:**  
- *Make Noise Maths, Disting mk4 (in audio rate LFO mode), Mutable Instruments Tides, any wavefolder or wave shaper*

**Patch Idea:**  
- Insert a wavefolder or shaper after the FM AID for further harmonic complexity.
- Use Maths to generate unique shapes or apply an envelope to the Carrier or Modulator for dynamic changes.
- Try cross-patching the outputs into the Mod input (feedback patching) for chaotic digital-esque textures.

---

## 3. **Audio-Rate Modulation for Experimental Results**

**Modules:**  
- *Any audio-rate LFO, Random*Source Serge NTO, Noise Engineering Basimilus Iteritas (as Mod source)*

**Patch Idea:**  
- Patch an LFO running at audio rate into the CV input of FM AID while running VCOs through the Carrier and Mod.
- Alternatively, use a sequencer’s stepped voltage at high speed for "sample & hold" timbres in the modulation.

---

## 4. **Polyphonic or Stereo Patching**

**Modules:**  
- *Polyphonic VCOs (e.g., Suboscillator, Cwejman VCO-2RM), Stereo processing modules (e.g., Strymon Magneto)*

**Patch Idea:**  
- Use two FM AIDs for left and right channels or for two notes in a poly setup.
- Pan the different outputs (sine, tri, saw, square) for stereo width and movement.

---

## 5. **Self-Patching/Feedback for Glitch & Noise Generation**

**Patch Tip from Manual:**  
- Patch the output (try all four shapes) back into the Mod input for natural analog feedback, resulting in digital-esque noise and chaos.
- Modulate the amount of feedback with a VCA, envelope, or LFO.

---

## 6. **Dynamic Timbre Control via CV**

**Modules:**  
- *Envelope Generators (e.g., Intellijel Quadra), Sequencers with velocity output (e.g., Expert Sleepers FH-2, Arturia Keystep Pro)*

**Patch Idea:**  
- Send velocity or note CV to the CV input to dynamically change FM depth.
- Map LFOs or random sources to the CV input for constantly shifting, undulating tones.

---

## 7. **Wave Replacement & Non-Standard Oscillator Inputs**

**Modules:**  
- *Envelope Follower, Drum Modules (e.g., Basimilus Iteritas Alter), Field Recorder, Crosspatch with Effects Returns*

**Patch Idea:**  
- Feed the Mod or Carrier input with external audio (drums, voice, field recordings) for processing sounds in unexpected, FM-tinged ways.
- Use an envelope follower to extract dynamics from an external source and use that as CV to drive FM index in sync with audio.

---

## 8. **Hard Sync Extras**

**Modules:**  
- *Oscillator with Hard Sync (Doepfer A-110-2, Intellijel Dixie II+)*

**Patch Idea:**  
- Sync both the Carrier and Modulator to the same hard sync master to lock them together, then use FM AID to process for stable, punchy FM tones without phase drift (“beating”).

---

## 9. **Morphing Between Waveforms Live**

**Modules:**  
- *VCAs, Matrix Mixer (e.g., Happy Nerding 3xMIA), Morph modules (e.g., Mutable Instruments Blinds)*

**Patch Idea:**  
- Use VCAs to fade between the FM AID sine, saw, and square outputs for dynamic timbral blending.
- Matrix mix the four outputs for custom waveshape creation.

---

## Other Thought Starters

- **Percussive FX:** Try FM audio-rate envelopes or noise bursts for wild drum synthesis.
- **Karplus-Strong/Plucked Sounds:** Patch the FM AID through a delay or physical modeling module, FM modulate the strings for lively, evolving plucks.

---

**Remember:** The FM AID rewards bold experimentation. Any signal can be a modulator or carrier—try everything!

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)
