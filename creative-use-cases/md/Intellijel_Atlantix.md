# Intellijel — Atlantix

- [Manual PDF](../../manuals/atlantix_manual_2024.09.12.pdf)

---

[Download the Atlantix Manual PDF](sandbox:/mnt/data/Atlantix_Manual_2024_09_12.pdf)

# Creative Patching Ideas: Intellijel Atlantix as a Modular Centerpiece

As an experienced eurorack musician, here's a set of patching strategies and module combinations that exploit Atlantix's architecture, integrating it in novel and musically rewarding ways:

---

## 1. **Complex Thru-Zero FM with External Sources**
Atlantix offers high-quality Thru-Zero (TZFM) linear FM on VCO A. Try patching in audio-rate signals from unconventional oscillators (e.g. Make Noise DPO, Instruō Cš-L, or a digital oscillator like the Mutable Instruments Plaits). This will result in much more complex spectra than using VCO B alone.

- **Patch Example:**  
  - Mult the output of a DPO or Cš-L oscillator and send one copy to Atlantix's FM 1 IN on VCO A (set to TZFM), another to audio, and crossfade between Atlantix and the external oscillator for evolving textures.

---

## 2. **West Coast Synthesis: Wavefolding & LPGs**
Combine Atlantix with a wavefolder (Intellijel Bifold, Tiptop Buchla 258t) or a Low Pass Gate (Make Noise Optomix). Since Atlantix can output raw waveforms (with the expander), send a sine or triangle to a wavefolder then through a LPG.

- **Patch Example:**  
  - Take VCO A sine out (from expander) into Bifold input, output to Optomix, and use Atlantix's envelope as the Optomix CV. You’ll get that classic "pinged" Buchla style West Coast sound with a rich, FM’d core.

---

## 3. **Hybrid Analog-Digital Drum Generator**
Exploit Atlantix’s percussive sync and snappy VCA with a trigger sequencer and external sample players. Use the ENV/GATE switch in Gate mode to turn the VCA into a percussive "hit". Patch gates from a trigger sequencer (e.g. Mutable Grids, or Euclidean Circles).

- **Patch Example:**  
  - Sequence Atlantix’s VCA with fast gates for chiptune drums, while S&H randomizes the pitch for a more organic feel. Parallel patch an external digital drum source and ring modulate with Atlantix for harsh, hybrid percussion.

---

## 4. **Dub Techno Chords With Dual Oscillator Sync**
Patch VCO A and B to slightly detuned intervals and use SYNC tricks (try soft vs. hard) for metallic, lush chords typical of classic dub techno. Process the MIXER output through an external stereo reverb (e.g. Strymon BigSky) and a complex filter (e.g. Mutable Blades).

- **Tip:** Feed VCO B's Square out to Atlantix's AUX 1 to introduce additional harmonic content, and modulate filter Q with an envelope or LFO for swelling chords.

---

## 5. **Self-Patched Generative Systems**
Leverage Atlantix’s rich internal mod matrix and S&H for generative textures, especially with external utilities:

- **Patch Example:**  
  - Use a clock source (Pamela's New Workout, Temps Utile) to advance S&H. Patch S&H OUT to VCO A’s FM, VCF cutoff, or envelope times for evolving, semi-random melodies or timbral shifts.
  - Send Atlantix MOD outputs to external voltage processors (Intellijel Quadrax, Mutable Shades, ALM O/A/x2) to further attenuate, offset, or slew modulations.

---

## 6. **Stereo Applications: Dual Atlantix or Expander**
Pair Atlantix with an external stereo panner (e.g. Happy Nerding PanMix or X-PAN). Use different outputs (main, expander’s filter outs, or post-VCA via external VCAs) for left/right feeds, especially with different waves or filter types (HP on one, LP on the other).

---

## 7. **Waveshaping and Crossfading**
Patch the dedicated oscillator outputs into crossfaders (WORNG SoundStage, Befaco Morphader) for live blending and morphing between shapes. Especially fun when under CV control from Atlantix's Mod X or Y.

---

## 8. **Advanced Ring Modulation**
The ATLX expander provides a passive ring modulator. Try cross-patching wildly disparate signals (e.g., your modular with a dynamic microphone preamped to modular level, or a drum module and Atlantix's oscillator). Use the ring mod output for chaotic, metallic signals perfect for FX or percussion layers.

---

## 9. **Mixer Expansion and Feedback Loops**
Exploit the mixer section’s AUX ins and normals. Use feedback by patching filter outputs back into mixer AUX, and cross-modulate AUX with CVs or audio. Enhance with an external matrix mixer (Doepfer A-138m) for feedback ecosystems.

---

## 10. **Complex Polyphonic Patches with MIDI-to-CV**
Combine Atlantix with a polyphonic MIDI-to-CV interface (Expert Sleepers FH-2, Endorphin.es Shuttle Control). Sequence both VCOs independently for classic two-voice patches, dual bass/lead, or overlapping duophonic arpeggios, and automate envelope, filter, and VCA parameters with external LFOs or Euclidean rhythm generators.

---

### Notable Module Types to Further Expand Possibilities:

- **Random / Chaos:** SSF Ultra-Random Analog, Joranalogue Orbit 3
- **Multi-Effects:** Mutable Instruments Clouds/Beads, Strymon Magneto
- **Sequencers:** Intellijel Metropolix, Winter Modular Eloquencer
- **Granular Processors:** Make Noise Morphagene, Tiptop Audio FSU
- **VCAMixers / CV-Controllable Switches:** Doepfer A-150, Mutable Frames
- **Envelope Followers & Audio-CV Processors:** Befaco A*B+C, Mutable Stages

---

## Summary

Atlantix stands out as a flexible and powerful analog synth voice—its extensive normalization, expander options, and thoughtful modulating architecture make it a superb heart or satellite for any creative eurorack system. Pair it with CV manglers, exotic sound sources, or advanced effect processors for maximum creative discovery.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)