# Centreville — PlusMix

- [Manual PDF](../../manuals/PlusMix _ centrevillage.pdf)

---

[**PlusMix Module Manual (PDF)**](https://centrevillage.net/products/PlusMix.html)

---

# Creative Song Arrangement with the PlusMix Eurorack Module

Turning a compelling groove into a **full-length eurorack song** often comes down to adding variation, structure, and performance control. The [**PlusMix**](https://centrevillage.net/products/PlusMix.html) module, though compact, provides unique utilities for arrangement, live mixing, and compositional movement—invaluable for turning loops into narrative musical pieces.

## Key Features Recap

- **3 Inputs (PLS1, PLS2, BASE), 1 Output (MIX)**
- **2 Gate-Controlled Switches (SW1, SW2, with polarity switches SW1PL, SW2PL)**
- **Gate or Manual Control over Signal Mixing**
- **Precision Mixing for CV (pitch-safe)**

## Techniques to Use PlusMix for Structuring Full Songs

### 1. **Dynamic Part Switching**

**Scenario:** You have multiple melody, bass, or modulation lines patched to PLS1 and PLS2.

- **Verse/Chorus Switching:**  
  Use external sequencer or gate sources (e.g., from a sequencer track, clock divider, or manual gate button) to control when PLS1 and PLS2 are mixed in.
  - **PLS1 = Verse Bassline**, **PLS2 = Chorus Bassline**  
  Trigger SW1/SW2 with gates corresponding to your song structure, swapping parts automatically as the song progresses.
- **Manual Song Flow Control:**  
  If you don't patch SW1/SW2, the front panel SW1PL/SW2PL switches act as performance mutes—instantly mute/unmute musical layers live.

### 2. **Subtle Progressions**

- **Ambient/Evolving Textures:**  
  Patch subtle modulations, effects, or underlying melodic lines into PLS1/2. Use slowly modulating gates (from LFOs or function generators) for SW1/SW2, creating evolving, automatic changes in your mix over time—perfect for ambient or cinematic builds.
- **Morphic Transitions:**  
  Toggle gate polarity switches (SW1PL/SW2PL) at key moments to invert when elements come in, creating easy breakdowns, builds, or surprise drops.

### 3. **CV Performance and Variation**

- **Precision Pitch Layering:**  
  Since PlusMix handles pure pitch CV, you can send multiple quantized melodies/arpeggios through PLS1/PLS2 and use PlusMix to dynamically “remix” which pitch lines are in control of a voice at different song sections.
- **Automated Modulation Routing:**  
  Use PlusMix to mix between different CV sources for filter cutoff, effects level, or other mod targets. Use gates or manual switches to morph sound textures in your arrangement.

### 4. **Live Performance & Song Evolution**

- **On-the-fly Muting/Soloing:**  
  By leaving SW1/SW2 unpatched, you gain instant manual mute switches—a powerful hands-on tool for improvising drops, transitions, or introducing layers live.
- **External Gate Sequencing:**  
  Program gates from DAW, MIDI-CV interface, or clock dividers to sequence complex mix changes in time with your song arrangement.

### 5. **Combining With Common Eurorack Modules**

- **Sequencer + PlusMix:**  
  Use a sequencer’s gate tracks or end-of-sequence triggers to switch song sections.
- **Logic/Gate Utilities:**  
  Combine gate logic modules to create even more nuanced arrangement automation (e.g., only bring in PLS2 during both a fill and after 32 bars).
- **Effect Send Control:**  
  Send alternate signals to reverb/delay buses for dramatic transitions and soundstage changes.

## Example Song Flow Patch Idea

1. **Bassline in BASE (always present).**
2. **Melody 1 (PLS1):** Enabled only for Verse using sequencer gate.
3. **Melody 2 (PLS2):** Enabled for Chorus using clock-divided gate.  
4. **Performance:** Use SW1PL/SW2PL switches manually for fills/breakdowns.
5. **Modulation:** Use PlusMix to swap between vibrato and filter-LFO on a lead by mixing their CVs under gate control.

---

> **Tip:** The real power is in both hands-on performance AND automating layering via gate sequencing—making the loops come alive with simple, repeatable structure cues. PlusMix gives you the ability to do big changes, little details, and everything in between, live or pre-programmed.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)