# 2hp — Kick

- [Manual PDF](../../manuals/2hp_Kick.pdf)

---

[Download the Kick Module Manual (PDF)](attachment:KICK%20MANUAL.pdf)  
*(replace with actual link if sharing outside this conversation)*

---

# Creative Patch Ideas for the Kick Bass Drum Synthesizer (2hp)

Based on the functions described in the manual, here are some creative ways to patch and utilize the Kick drum module in your Eurorack setup:

## 1. Voltage Sequenced Melodic Kick Basslines

**What you'll need:**  
- Kick module  
- Sequencer (e.g., Make Noise René, Arturia Keystep, or any CV/gate sequencer)  

**How to patch:**  
- Patch your sequencer’s gate output to the **TRIG** input.
- Patch the CV/pitch output to the **V/Oct** input.
- Set Decay to a medium setting.
- Play in a sequence that follows your track’s bassline.

**Creative result:**  
Create punchy, tuned kick drums that follow your song’s bassline. Experiment with microtonal or nonstandard intervals for IDM/glitch vibes.

---

## 2. Kick as a Percussive Lead

**What you'll need:**  
- Kick module  
- Envelope generator (e.g., Maths, Intellijel Quadra)  
- VCA (Voltage Controlled Amplifier)  
- Reverb/Delay module (e.g., Clouds, Mimeophon)

**How to patch:**  
- Use a fast envelope from the EG to modulate **Tone** or **Pitch** via their CV inputs.
- Send the **Out** from Kick to the Reverb/Delay for big room/spacey FX.
- Adjust Decay for long, pipe-like percussive sounds.

**Creative result:**  
By modulating tone/pitch, use the Kick as a synth voice that creates massive, rhythmic pitch-swept toms, sub-basses, or wild metallic thuds.

---

## 3. Glitch & Texture Generation

**What you'll need:**  
- Kick module  
- Random or Sample & Hold module (e.g., Wogglebug, Turing Machine)  
- Modulation source (LFO, stepped random)

**How to patch:**  
- Patch random voltages into the **Tone** and/or **Decay** CV inputs.
- Send **TRIG** input a irregular clock (e.g., Turing Machine’s gate output).
- Optionally, feed the Out to wavefolders or bit-crushing modules.

**Creative result:**  
Generates a constantly changing field of percussive glitch sounds, great for experimental genres. Use wavefolders or effects after the module for even more timbral variety.

---

## 4. Distorted Techno Kicks

**What you'll need:**  
- Kick module  
- VCA or distortion module (e.g., Erica Synths Fusion Distortion, Mutable Instruments Warps)

**How to patch:**  
- Set **Tone** fully left for overdriven sound.
- Send Out to additional analog distortion/saturator.
- Try parallel processing—split the Out signal and process one copy clean, one copy with heavy effects, then mix.

**Creative result:**  
Stack and layer thick, industrial-techno style kicks or add edge to classic 808-style drums with additional drive.

---

## 5. Envelope Follower/Sidechain Compression Effects

**What you'll need:**  
- Kick module  
- Envelope follower (e.g., Mutable Instruments Ears, Befaco Envelope Follower)
- VCA or Compressor module

**How to patch:**  
- Use the envelope follower to convert the Kick’s Out signal into a CV signal.
- Use this CV to modulate the amplitude of another (e.g., pads, bass), creating classic sidechain “pump” effects.

**Creative result:**  
Synchronize the movement of melodic elements to the kick, letting them “breathe” in rhythm with the drum, commonly used in electronic dance music.

---

## Bonus: Automating Decay for Dynamic Beats

Use an LFO or slow random voltage to modulate the **Decay** CV, producing kicks that alternate between tight and boomy throughout a pattern—great for evolving, less-static rhythms.

---

**Module Pairing Highlights:**  
- **Sequencer:** melodic/rhythmic lines
- **Random/S&H:** glitch textures, generative rhythms  
- **Envelope generators:** transient shaping  
- **Effects (Reverb, Delay, Distortion, Wavefolder):** timbral expansion  
- **VCA/Compressor:** sidechaining, amplitude shaping

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)