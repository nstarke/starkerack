# Doepfer — A-135-1

- [Manual PDF](../../manuals/A135_man.pdf)

---

[Doepfer A-135 VC-Mixer Manual PDF](https://www.doepfer.de/a100man/A135_tec_e.pdf)

---

# Creating Full-Length Songs with the Doepfer A-135 VC-Mixer

The Doepfer A-135 VC-Mixer is a powerful tool not just for mixing individual sounds, but for sculpting evolving, dynamic arrangements—a key process in taking modular sketches and loops into full-length, engaging songs.

Below, I’ll focus on **practical strategies** that leverage this module in combination with other Eurorack gear to move beyond loops and into structured compositions.

## VC-Mixer Features Recap
- Four channel linear VCAs, mixed to a single output.
- Each channel has:
  - Audio input (with attenuator)
  - CV input (with attenuator)
  - Manual gain
- All channels are summed at the output.

---

## Song Structure Strategies Using the A-135

### 1. **Automated Muting and Layer Control**
Instead of simple static mixing, use the A-135’s CV-controlled amplification to bring layers (kick, snare, melody, bass, pads, etc.) in and out either via:
- Sequencers
- Function Generators (ADSR, LFOs)
- Manual controls (for live performance)

**Example:**  
- Use four audio sources (drum loop, bass line, melody, texture).
- Feed different modulation sources (envelope followers, LFOs, scene sequencer like Make Noise Pressure Points, or a MIDI-to-CV interface) into each VCA’s CV in.
- Build a sequence or automation where layers enter/exit the song at different points—giving you “mute automation” like a DAW.

### 2. **Dynamic Volume Fades & Scenes**
Mix parts in/out with evolving shapes, not just on/off. By patching envelopes or LFOs with varied shapes into the VCA CVs, you can:
- Fade elements in for an intro, then out for breakdowns.
- Use random or stepped modulation for stuttered, glitchy arrangements.

**Scene Example:**  
- Patch a slow, looping envelope to fade a pad in gradually over 16 bars.
- Have a stepped random or sample & hold signal (from Doepfer A-148 or similar) bring in percussive fills unpredictably for a bridge.

### 3. **Morphing & Crossfading Between Sections**
Use a controller like Doepfer A-144 Morphing Controller or a macro CV from a sequencer to “slide” between up to four full mixes or sections:
- Each A-135 input could be an entire mix stem (drums, bass, chords, melody).
- The crossfade/morphing CV moves from one section (verse) to another (bridge/chorus), effectively recalling new mix “scenes”.

### 4. **CV-Controlled Effects Routing**
Don’t just use A-135 for raw audio. Patch the outs of various effects (reverb, delay, distortion, filters) to the VC-Mixer, and use its VCAs to blend effects in/out, tempo-synced or modulated for real-time arrangement.

### 5. **Building Drops, Breakdowns, and Returns**
Think of the A-135's channels as structural building blocks. Use gates or envelopes from a sequencer to cut out everything except for bass & drums (drop), or leave only atmosphere and FX (breakdown), then bring all elements back.

**Automate Song Arcs:**
- Pre-program or perform automation curves for each channel’s CV.
- Use a MIDI-to-CV module to control the VCAs from your DAW.

---

## Patch Examples

### **A. Automated Build-Up and Drop**
1. Channel 1: Drums  
2. Channel 2: Bass  
3. Channel 3: Pads  
4. Channel 4: Lead

- Bass, pads, and leads have their VCAs controlled by slow envelopes or sequencer-driven CVs.
- All fade up together for an “intro”; then bass and pads fade out for a “drop”, returning at programmable moments.

### **B. Morphing Arrangement with A-144**
- Feed the A-144’s four morph output CVs to each VCA.
- Single knob or voltage morphs between four full mixes (use linked VCAs for external submixes).
- Automate this morph with a voltage sequencer for evolving song sections.

---

## Overcoming the “Loop-to-Song” Hurdle

The key to using the A-135 for song-length arrangements is **automation and CV control**. By carefully planning how layers, effects, and mix levels evolve (either with performance gestures or sequencer/LFO automation), you transform static loops into dynamic, evolving songs.

**Tips:**
- Use multi-channel MIDI-to-CV modules to automate mix scenes from a DAW.
- Combine sequential switches (e.g., A-151) with the A-135 for more abrupt section changes.
- Utilize voltage memory/recall modules for precise scene morphing.

---

Create patch diagrams using the A-135’s patch sheet templates (in the manual) for each song section. This aids recall when performing or re-creating arrangements.

---

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**