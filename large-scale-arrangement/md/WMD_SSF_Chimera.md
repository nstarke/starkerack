# WMD SSF — Chimera

- [Manual PDF](../../manuals/Manual_v1.2.pdf)

---

[**Download the WMD Chimera Metallic Percussion Synthesizer Manual (PDF)**](https://wmdevices.com/ChimeraManual.pdf)

---

# Using the WMD Chimera to Create Full Length Eurorack Songs

## Introduction

The **WMD Chimera** is an advanced metallic percussion synthesizer designed for Eurorack. It excels at producing metallic, shimmering, and percussive sounds with deep control over texture, rhythm, and timbre. While adding a striking percussive element to patches is its primary role, thoughtful patching and modulation integration can help you use Chimera as an instrument for building structured, engaging full-length songs.

Below are strategies and patch ideas to move from short patterns into full compositions with Chimera, integrating it as a core voice among your other modules.

---

## 1. **Arranging: Building Song Structure**

Structuring a song requires **variation** over time. In Eurorack, this often means leaving “set-and-forget” patches behind in favor of automation, evolving sequences, and intentional transitions.

### **A. Dynamic Sound Design**
- **Automate SURFACE, DENSITY, & DECAY:**  
  Use sequencers, LFOs, or voltage-controlled random sources to modulate these parameters.  
  - **Intro/Outro:** Fade in with subtle surface types & long decay for a wash, fade out the same way.
  - **Verse/Chorus:** Switch or morph surfaces, add density for energy spikes.
  - **Breakdowns:** Pull DENSITY and DECAY low for minimal, sparse textures.  
  - **Build-ups:** Gradually increase DENSITY or DECAY over 16/32 bar segments.

### **B. FX & Processing Transitions**
- **FX selection & FX AMT:**  
  Automate these with sequential switches or through direct modulation to create dramatic timbral shifts at section changes.

---

## 2. **Groove Variation & Rhythmic Interest**

A repetitive drum pattern can become monotonous, so:

### **A. FEEL Modes for Performance**
- Alternate between FEEL modes for different song sections.  
  - Use FEEL 1 for steady, energetic hits in a chorus.
  - Use FEEL 2 for groovy, syncopated verses and rhythmic interest.
  - Use FEEL 3 for breakdowns, fills, or transitions with unpredictable, “human” metallic hits.

**Modulate FEEL** using switches or CV to jump across song sections without manual knob turning.

### **B. Accent and Choke**
- **ACCENT:** Trigger at specific steps for fills, drops, or “accented” beats in your intended song form.
- **CHOKE:** Use in breakdowns or to punctuate transitions—rapid chokes can make abrupt, dramatic stops.

---

## 3. **Melodic and Tonal Application**

Chimera isn’t just a drum—the **PITCH** and **(PITCH) ENVELOPE** controls let it play melodic or tonal roles:

### **A. Tuned Percussion**
- Sequence the PITCH input using a melodic sequencer or keyboard controller.
- Modulate (PITCH) ENVELOPE for glissando or laser-like effects in breakdowns.
- Combine with conventional drums for hybrid, pitched-groove hooks in your drops or chorus.

---

## 4. **Bringing in External Modulation**

Layering movement and variety is key for a full song:

- **VCA Input:** Dynamically duck or fade the Chimera in/out of the mix, for e.g., sidechain-like punch or gradual buildups.
- **Envelope Followers and LFOs:** Tie Chimera’s controls to CV from modulation sources that track intensity or section changes.
- **Random Generators:** Subtly modulate SURFACE, DENSITY, or FX AMT for constantly evolving textures.

---

## 5. **Arranging with Sequencers and Switches**

- Use sequential switches and clock dividers to reroute trigger, accent, or CV controls to Chimera for different song sections.
- Patch Chimera’s output through VCF, VCA, reverbs, or delays, routing these FX in and out via CV-controlled send/return modules. This lets you “solo” Chimera for fills, breakdowns, or transition effects.

---

## 6. **Practical Song-Building Patch Examples**

- **Intro:** Slow LFO gently raises DENSITY and SURFACE, long DECAY for a granular wash.
- **Verse:** Moderate DENSITY, switch FEEL to 2 for groove, ACCENT on every 8th note.
- **Chorus:** High DENSITY, FEEL 1, apply comb filter FX, increase PITCH slightly.
- **Bridge/Breakdown:** Drastically lower DENSITY, switch FEEL to 3, manual FX sweeps.
- **Fill:** Vary PITCH ENVELOPE for laser-like zaps, trigger ACCENT & CHOKE in sync.

---

## 7. **Integration with Other Modules**

- **Clocked Modulation (Pamela’s New Workout, Zadar):** Send precise, tempo-synced LFOs and envelopes to Chimera’s controls for evolving songscapes.
- **Voltage Addressed Switchers (A-151, Branches):** Send different CV or gates to FEEL, SURFACE, or FX at planned points in a song.
- **Performance Controllers (Tetrapad, Pressure Points):** Trigger fills or transitions on demand.

---

## 8. **Automation & Live Performance**

- Use performance mixers, CV recorders (like Hermod or CV Thing), or DAW integration (via ES-8/ES-9) to automate Chimera’s parameters and FX sends for hands-free, reproducible song sections.

---

## Conclusion

**Chimera shines as both a percussive backbone and a dynamic, performative tool** that can help bridge grooves into fully arranged songs. By automating, sequencing, and modulating Chimera’s many controls in real-time, you transform a chain of repeating patterns into a true progression—ripe for dancefloor, experimental, or cinematic music in the modular world.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)