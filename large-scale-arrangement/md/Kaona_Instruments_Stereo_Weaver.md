# Kaona Instruments — Stereo Weaver

- [Manual PDF](../../manuals/stereoweaver.pdf)

---

[Download the Stereoweaver Manual (PDF)](https://www.kaona.fr/wp-content/uploads/2024/02/kaona-stereoweaver-manual-en-v1.pdf)

---

# Using Stereoweaver to Create Full-Length Songs in Eurorack

Stereoweaver is a highly creative mono-to-stereo spatial FX module for Eurorack whose unique spatial processing capabilities can transform static or simple patch ideas into dynamic, evolving pieces ideal for full-length tracks. Below, I analyze how to leverage Stereoweaver to overcome common obstacles in evolving modular stereo content, and outline practical patching strategies for song structuring in the modular context.

---

## Key Strengths of Stereoweaver

- **Dynamic Stereo Imaging:** Beyond widening, Stereoweaver introduces movement, micro-delays, phase shifts, and depth.
- **CV Controllability:** Every main parameter (Depth, Phase, Motion, Haas, Width) can be animated via CV, crucial for continual change.
- **Psychoacoustic Prowess:** Employs the Haas effect and phase modulation for organic stereo evolution.
- **Musical Movement:** The Motion control, including a Leslie rotary sim, brings rhythmic modulation to the stereo field.

---

## Turning Patches Into Songs: Concrete Approaches

### 1. Evolving a Static Loop

#### Without Stereoweaver  
A repeating melody/beat becomes fatiguing and static.

#### With Stereoweaver  
- **Automate Depth, Motion, and Width via LFOs or Envelopes:** Fade in more pronounced stereo width and phase animation for choruses, drop them back for verses.
- **Manual Performance:** Perform live modulations on the panel to improvise song structure.

***Patch Example:***  
```
Melody/Bass/Drums (Mono Out) → Stereoweaver IN  
Stereoweaver L/R Outs → Mixer → Effects/Output
LFO1 (slow, synced to bars) → Stereoweaver Width CV
Envelope (from sequencer at section changes) → Depth CV
Ramp LFO → Phase CV (builds tension over time)
```

### 2. Creating Sections (Verse/Chorus/Bridge)

- **Sectional Contrast:** Use Stereoweaver to make clear “sections” by drastically altering stereo scene at section boundaries.
    - Verse = Narrow width, subtle motion
    - Chorus = Wide, animated, Haas engaged, more pronounced depth
    - Bridge = Extreme phase movement or fast rotary effect
- **Scene Transitions via CV:** Connect output from a performance sequencer or a manual controller to change Stereoweaver parameters per section.

***Patch Example:***  
Use preset voltages/attenuators or a Voltage Block (Malekko), or even simple sequential switches to send different CVs to Stereoweaver per song section.

### 3. Filling Out The Arrangement

- **Bring In/Out Elements:** Automated Width can subtly “unmask” new voices or effects when a section changes by shrinking or swelling the image.
- **Cumulative Build:** Start with mono/center-focused sound, use progressive increase in Depth and Motion to "open" the song spatially.

### 4. Organic Movement Over Time

- **Random/LFO CV:** Use Turing Machine/Marbles/other random CV sources to modulate Width/Phase/Motion at slow rates, ensuring that even one-bar loops evolve and feel alive.
- **Performance Controls:** Use big macro knobs or controllers (Intellijel Tetrapad, Faderbank) to sweep Stereoweaver parameters while playing.

### 5. Send Effects / Parallel Processing

- **Aux Send:** Place Stereoweaver on an FX send to “stereoize” dry mono elements (like percussion hits or voice snippets) only at chosen song moments (e.g., breakdown or outro).
- **Switchable Placement:** Use a sequential switch (Doepfer A-151 or similar) to route different sources through Stereoweaver in different song sections.

### 6. Rhythmic or Thematic Emphasis

- **Sync Motion to Master Clock:** Use Clocked LFOs to lock Motion animation to beats or bars, making the stereo effect a coherent structural element.
- **Accentuate Drops or Climax:** Rapidly modulate Haas or Phase for a “slapback” or spatial swirl at key song moments.

---

## Sample Song Structure with Stereoweaver

| Section   | Stereoweaver Settings                                               |
|-----------|---------------------------------------------------------------------|
| Intro     | Narrow width, low Depth, static Motion (centered, focused presence) |
| Verse     | Modest width, Phase modulated slowly, Haas slight, Motion slow      |
| Chorus    | Wide, max Depth, Motion set to rotary, Haas up, pronounced changes  |
| Bridge    | Phase sweeps, chaotic Mode, Width automates back to mono            |
| Outro     | Gradual "collapsing" of stereo image: Width and Left/Right fades    |

By mapping section cues to CV automation (manual, scenes, or sequenced), Stereoweaver helps a patch tell a full story—moving beyond loops, creating dramatic transitions, and making repeated materials feel ever-changing.

---

## Integrating with Other Modules

- **Sequencers:** Use CV output from performance sequencers to modulate Stereoweaver per song part.
- **LFO/Function Generators:** Animate parameters for subtle or dramatic effect across your track's timeline.
- **Switches/Muters:** Change processing routing; bring Stereoweaver in/out for dramatic effect.
- **Effects Chain:** Use Stereoweaver before reverb/delay to create vast, shifting clouds; use after distortion for 3D grit.

---

**Remember:**  
Song progression in modular is about contrast and movement. Stereoweaver is ideal for shaping **spatial contrast** over time, making the difference between "patch" and "track".

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)