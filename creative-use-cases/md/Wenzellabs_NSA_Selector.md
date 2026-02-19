# Wenzellabs — NSA Selector

- [Manual PDF](../../manuals/wenzellabs_the_NSA_selector_ the NSA selector eurorack module.pdf)

---

[NSA Selector Manual (PDF format, screenshots)](https://github.com/wenzellabs/the_NSA_selector)

---

# Creative Ways to Use the NSA Selector Eurorack Module

## Overview

The NSA Selector is a highly unusual Eurorack module that bridges Ethernet network traffic and modular synthesis. Featuring two Ethernet jacks (acting as a switch/tap) and one audio output, it converts raw network bitstreams into audio, letting you listen to digital traffic in your patch.

Below are some creative strategies to integrate the NSA Selector into your Eurorack system, both musically and technically.

---

## 1. **Network-Driven Percussion & Rhythms**

**How:**  
Use network pings or controlled bursts of traffic (like scripted ICMP pings, http requests, or file transfers) to create percussive, glitchy signals. The randomness or repetition in network activity translates to rhythmic/noise-based pulses.

**Combinations:**
- **Percussion Modules:** Patch NSA Selector's audio output into a simple VCA, then into a LPG (e.g., Make Noise LxD, Mutable Instruments Ripples in VCA mode) to shape and isolate transients.
- **Envelope Follower:** Use an envelope follower (e.g., Mutable Instruments Ears or Doepfer A-119) to extract CV from the network audio, which can trigger envelopes, drums, or modulate parameters.
- **Random Sources:** External network randomness, processed with a slew limiter (e.g., Make Noise Function) to generate smooth random CV.

---

## 2. **Digital Data as Raw Oscillator Source**

**How:**  
With its 4-bit, 25MS/s output, the NSA Selector acts as a wild, unpredictable oscillator/digital noise source.

**Combinations:**
- **Ring Modulator:** Process its signal with a ring mod (e.g., Doepfer A-114) and another oscillator for metallic, abrasive tones.
- **Waveshapers/Distortion:** Feed into wavefolders or distortion modules (e.g., WMD Geiger Counter, Intellijel µFold) for aggressive textural sounds.
- **Spectral Processors:** Add spectral shapers like the Mutable Instruments Warps for CV-controlled blending with traditional oscillators.

---

## 3. **Audio Visualization of Network Events**

**How:**  
Render network activity as audible events; for example, send files (especially big images in .bmp format) over your local network and "play" these as sound.

**Combinations:**
- **CV & Lights:** Connect to a CV-to-light interface (e.g., Visible Signals Video Mult or LED modules) to visually monitor correlation between data transfer and lighting modulation.
- **Recording/Granular Playback:** Sample the output with a looper (e.g., 4ms Dual Looping Delay, Mutable Instruments Clouds) to chop, freeze, and sequence "data-shaped" textures.

---

## 4. **Sequencer and Live Network Performance**

**How:**  
Coordinate scripted ping/flood traffic as a sequencer, using scripts to control the rhythm and density of network activity.  
With the included "sequencer" Bash script, you can generate timed patterns resembling sequence steps.

**Combinations:**
- **Sequencer Sync:** Use a trigger-to-MIDI interface to sync DAW sequencer patterns with network-triggered audio (e.g., Expert Sleepers ES-8 or MIDI-to-CV modules).
- **Random/Pattern Generators:** Combine with modules like Make Noise Maths or Mutable Instruments Marbles to cross-modulate or "scramble" the NSA Selector's output, influencing network activity and music in both directions.

---

## 5. **Controlled Chaos and Glitch Art**

**How:**  
Over-saturate the network, generate packet loss, or stream plaintext payload for modulated static and noise, leveraging delays and echo-like effects using `tcpdump` and similar commands as detailed in the manual.

**Combinations:**
- **FX Modules:** Send the output through granular processors (Qu-Bit Nebulae, Mutable Instruments Clouds), delays (Chronoblob 2), or stutter/repeater FX (Befaco Rampage) for glitch-art sonic sculptures.
- **VCAs or Switches:** Use it as a modulator/audio-rate CV for dynamic amplitude modulation of other inputs.

---

## 6. **Unconventional MIDI-Controllable Network Traffic**

**How:**  
Develop scripts to control netcat, socat, nmap, or similar tools via software-registered MIDI clients, using external sequencing or generative environments (Max/MSP, Pure Data) to send MIDI notes that trigger network events.

**Combinations:**
- **MIDI-to-CV Interface:** Interface your computer to your rack via a MIDI module (Arturia BeatStep Pro, Doepfer A-190-4). Use MIDI notes to modulate/sequence NSA Selector-driven sound.
- **Logic & Gate Utilities:** Process extracted rhythms using logic modules (Intellijel Plog) for flipping/combining network-derived triggers.

---

## 7. **Live Coding and Network Improv**

**How:**  
Perform live using networked devices—have collaborators send packets/files/streams from their laptops or phones, influencing your Eurorack system in real time.  
Electrons, data, music: all fluid and hackable!

**Combinations:**
- **Audio Mixer:** Patch NSA Selector in with drum machines, synth voices, or mics for spontaneous hybrid jams.
- **Sampler/Looper:** Use modules like the 1010music Bitbox or Bastl Microgranny for capturing and playing back "data beats."

---

## General Module Recommendations

- Envelope follower/preamp (e.g., Mutable Ears, Doepfer A-119)
- VCA, LPG or Gate with modulation input
- Sampler/granular processor (e.g., MI Clouds, Qu-Bit Nebulae)
- Spectral/Waveshaper modules (e.g., Warps, WMD Geiger Counter)
- Logic and clock utility modules
- Sequencers compatible with external clock/reset

---

### More Inspiration

This module's uniqueness comes from its cross-disciplinary fusion of network technology and modular synthesis. Think of it as a "data microphone" for your local network—your challenge is to sculpt its wild output into something musical (or simply appreciate its conceptual weirdness).

---

For full details/actions/scripts, the original **[NSA Selector Manual](https://github.com/wenzellabs/the_NSA_selector)** is a must-read.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)