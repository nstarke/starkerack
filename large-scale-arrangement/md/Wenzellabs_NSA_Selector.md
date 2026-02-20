# Wenzellabs — NSA Selector

- [Manual PDF](../../manuals/wenzellabs_the_NSA_selector_ the NSA selector eurorack module.pdf)

---

[NSA Selector Eurorack Module Manual (PDF)](https://github.com/wenzellabs/the_NSA_selector/blob/main/README.md)

---

# Using the NSA Selector to Structure Full-Length Eurorack Songs

As a eurorack modular musician, it’s easy to get stuck in the loop zone—great beats or textures, but no real movement or "song" development. The [NSA Selector module](https://github.com/wenzellabs/the_NSA_selector) is different: it’s a network-to-audio module that converts raw Ethernet traffic ("any bit on the network will be sent to the audio output") into audio signals, introducing a whole new way to bring variety, structure, and unpredictability to your music.

Below, I'll break down creative strategies for using the NSA Selector as a core "arrangement instrument" in a modular setup, helping you move beyond loops and into full-length song territory.

---

## How the NSA Selector Works (Recap)

- **Two Ethernet jacks, one audio output**
- Network packet bits are literally "audified" to the output
- Not a standard audio interface or network protocol player—just raw bit-to-audio tapping
- 4 bit, 25MS/s native format from the PHY MAC MII interface; "network noise" becomes audio
- Add computer-generated or real network traffic to shape the sounds

---

## Strategies for Full-Length Song Creation

### 1. **Section Changes via Network Traffic Modulation**

**How:**
- Use your computer, Raspberry Pi, or another network-capable device to send different types of traffic patterns at different times—like bursts, lulls, pings, file transfers, image transfers, or deliberate "quiet" periods.
- Automate these traffic types using scripts, or MIDI-controllable software (integrate with ping scripts, netcat, socat, etc).
- Use the NSA Selector's audio output as a key source for percussion, noise beds, or glitchy leads that change character over time based on the incoming network patterns.

**Song Structure Use:**
- Verses: Lightweight ping traffic for sparse noise, low rhythm
- Chorus: Dump a bitmap image for intense, noisy bursts
- Bridge: Network quiet or only small packets for minimal sections
- Drop: Flood with HTTP or FTP or gaming traffic for maximum chaos

---

### 2. **Automated Evolutions With Scripts**

**How:**
- The included **sequencer/** shell scripts can "play" sequenced network patterns, e.g., network ping bursts of various sizes.
- Combine with external sequencers that trigger scripts via MIDI-over-USB or network.
- Build up sections that increase or decrease in complexity by controlling the density, duration, and periodicity of network traffic.

**Song Structure Use:**
- Intro: Low-density, simple traffic evolving into more complex patterns
- Buildup: Gradually automate scripts to ramp up the network "sequencer"
- Drop: All scripts firing, high-traffic bursts
- Breakdowns: Back down to minimal scripts, single bursts

---

### 3. **Layered Sampling and Resampling**

**How:**
- Record the NSA Selector’s output during various network traffic states.
- Resample or layer these as loops in a sampler module (e.g., Morphagene, Bitbox, Nebulae).
- Use previously recorded "network jams" as evolving backgrounds, contrasts, or transitions throughout your structure.

**Song Structure Use:**
- Use sampled network audio for intro/outro beds, transitions between song sections, or to create evolving motif elements that reappear across the song ("theme and variation").

---

### 4. **Glitchy Breaks, Fills, and FX**

**How:**
- Use external manipulation (like running tcpdump, flooding traffic, or dropping network interfaces) as a live performance technique to introduce breakdowns, rhythm changes, or sudden noise cuts.
- Automate this with CV-controlled network switches or relays for precise song timing.

**Song Structure Use:**
- Dramatic drops or fills
- Glitch transitions (sudden silence or cacophony, steering the energy flow)
- FX overdubs or one-off noises that mark section changes (like new verse/chorus/break)

---

### 5. **Interactive or Generative Song Structures**

**How:**
- Set up automated or interactive network processes: e.g., control network devices via MIDI, touch interface, or generative code (Max/MSP, Pure Data, Tidalcycles, Supercollider, etc).
- Song evolves based on real-time or "randomized" network interactions.

**Song Structure Use:**
- Self-generating textures that evolve across a full piece
- Use physical network device actions (plug/unplug, Wi-Fi device activity) mapped to key structural moments

---

### 6. **Sync and Layer With Traditional Eurorack Modules**

**How:**
- Layer the NSA Selector output with analog drums, bass, and synths: route its audio through VCAs, filters, effects, and envelopes to keep it musical and dynamic.
- Use envelope followers or comparators to extract triggers or gates from its noisy output, clocking sequencers or modulating other voices for cross-networked modulation over your groove.
- Gate effects, VCAs, or sample switches ("song parts") by voltage derived from the Selector’s output—using the noise bursts to flip sections, mutes, or effects.

---

## Example Patch for Full Song Structure

```
[Network Source(s)] 
     |
     v
[NST Selector Module] --[VCA]--> [Filter/FX] --> [Mixer/Output]
     |                                ^
     |                                |
[Envelope Follower/Comparator] -------|
     |
[Clock/Gate Out] --------> [Sequencer/Drum Machine/FX Trigger]
```

- Pre-program or improvise network scripts for evolving layers over song sections
- Use envelope follower to trigger new drum/bass synth patterns or effects
- Change network traffic types for unique "chorus," "verse," or "bridge" textures

---

## Tips for Creating Complete Songs

- **Plan your network arrangements** like any musical score—time your traffic patterns for distinct sections.
- **Blend with traditional voices:** NSA Selector shines as a textural/arrangement layer; use it to break loops and introduce surprise and movement.
- **Automate, sample, and resample** for further flexibility—network sounds can become motifs!
- **Use live performance of network changes** (muting ports, traffic bursts) for expressive control over your song’s structure.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)