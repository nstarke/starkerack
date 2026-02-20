# worng Electronics — Vertex

- [Manual PDF](../../manuals/Vertex manual v1.00.pdf)

---

[Download the WORNG Electronics Vertex Manual (PDF)](attachment:WORNG_Electronics_Vertex_manual.pdf)  

---

# Using the WORNG Electronics Vertex to Build Full-Length Eurorack Songs

The WORNG Electronics Vertex is a unique stereo VCA module that provides deep control over the dynamics and spatial characteristics of your signals. While VCAs are often thought of as utilities for amplitude modulation, Vertex’s ability to alter envelope shapes, enable dynamic panning, and control stereo image opens up creative solutions to a classic modular challenge: turning interesting loops and riffs into structured, evolving full-length songs.

Below, I’ll analyze how you can use the Vertex—in combination with other Eurorack modules—to help your patches evolve and build a sense of “song” structure.

---

## Key Features Recap

- **Stereo linear and exponential VCAs**
- **Voltage-controlled gain and skew (balance/pan)**
- **CV normalization for mono-to-stereo conversion**
- **CV over pan/balance and envelope shaping**
- **All-analog, DC-coupled paths for both audio and CV routing**

---

## Song-Building Strategies with Vertex

### 1. **Dynamic Song Section Transitions (Intro → Verse → Chorus, etc.)**
- **VCAs as Dynamic Song Mixers:** Use Vertex as the last stage for several voices (bass, leads, pads) each routed through separate Vertex modules or sections. With envelope followers, function generators, or automation sources sequencing the gain and pan/skew CVs, you can fade voices in and out, simulate mutes, or bring new parts to the front spatially, much as a DAW automation lane would.
- **CV Macros for “Scenes”:** Mult or sequence scenes of CV into the Gain and Skew inputs to recall different “sections” of your song by dramatically changing which parts are playing and where they sit in the stereo field.

### 2. **Automated Stereo Movement for Evolution**
- **Stereo LFOs/Envelopes:** Automate movement by using an LFO (or random) to the Skew CV, gently swirling pads or leads in the stereo field during chorus or breakdown sections, then snap to center for focused breakdowns.
- **Envelope Shaping for Variation:** Send envelopes with varying lengths or shapes to the Gain CV input per part, and use Skew to exaggerate or tame different sides. With clever envelope sequencing, you can “reshape” parts for different song sections, e.g. wide/long pads in verse, punchy/centered in chorus.

### 3. **Mono-to-Stereo Fill Creation**
- **Mono Signal Injection:** Use the Vertex’s L-to-R normalization to turn a mono voice into a temporary stereo one during fills/breaks, by automating Skew and Gain. Imagine a mono lead that, during a fill, suddenly widens and pans dynamically, creating an ear-catching moment without adding extra gear.

### 4. **Automating Dropouts and Drops**
- **CV-Controlled Mutes and Swells:** Use stepped/random CVs into Gain for sudden mutes, drops, or ramps. For example, an envelope or gate at the transition to a drop mutes all parts by pulling Gain low, then opens up for a full-impact return.
- **Pan “Throws”:** Temporarily automate Skew to hard-left or hard-right, mirroring the “throw” effect in classic studio/DAW mixes for transitions or dramatic breakdowns.

### 5. **Long-Term Evolution With Slow Modulation**
- **Slow Macro LFOs:** Assign a super-slow LFO to the Skew or Gain CV, evolving the stereo spread and dynamics over minutes, not measures. This makes looping patterns feel alive and less repetitive during long song builds.
- **Complex CV Paths:** Use sequencers like the Make Noise Tempi/Rene, vector LFOs (like Batumi or Zadar), or step sequencing modules to send different, section-specific modulation to Vertex’s Skew/Gain.

### 6. **Processing and Layering External Signals**
- **Send DAW/Field Recordings/Ambient Pads:** Use Vertex to bring in and animate external stereo signals in relation to your modular material, crossfading or panning them in and out at key song moments.
- **Live PA/Performance Utility:** Use manual control plus footswitch or expression pedal sources on Skew/Gain CVs for hands-on, performative dynamics in a set—fading, panning, muting, or highlighting as you perform.

---

## Example “Song” Structure Patch Flow Using Vertex

```mermaid
flowchart TD
    A[Sequencer/Drum Machine]
    B[Melodic Voice(s)]
    C[Bass Voice]
    D[Pad/Texture Voice]
    E[Vertex L/R Inputs (Mono/Stereo)]
    F[CV Macro Source(s): LFO, Envelope, Sequencer]
    G[Final Stereo Out/FX]
    
    A --[Drums Mono->L in Vertex 1]--> E
    B --[Lead Mono->L in Vertex 2]--> E
    C --[Bass Mono->L in Vertex 3]--> E
    D --[Pad Stereo->L/R in Vertex 4]--> E

    F --[Gain/Skew CVs by Section or LFO]--> E
    E --[Dynamic, spatial mix of all voices]--> G
```

With this flow, you’d use a combination of sequencer, envelope, and LFO sources to automate how each voice enters, exits, and moves in the stereo field across sections.

---

## Hands-On Tips

- **Scenes with Switches/Sequential Addresses**: Patch different “scene” CVs from a sequential switch to Vertex’s Gain/Skew for verse/chorus/bridge arrangements.
- **Envelope Randomizers**: Use random/trig LFO envelopes to introduce unpredictable panning or level changes, giving a sense of improvisation or “human touch.”
- **Preset Recall**: Advanced setups can use preset or program change modules (e.g., Disting EX, ES-8 with computer control) to modulate Vertex’s CVs for live or studio recall.

---

## Conclusion

The Vertex isn’t just a “utility” VCA—it’s a powerful performance mixing, enveloping, and panning tool for stereo modular setups. With creative CV automation and thoughtful voice routing, you can transform repeating loops into living, breathing full-length songs, packed with dynamic, evolving structure.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)