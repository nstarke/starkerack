# Moog — Labyrinth

- [Manual PDF](../../manuals/Labyrinth Manual.pdf)

---

[**Moog Labyrinth User's Manual (PDF)**](https://www.moogmusic.com//sites/default/files/2024-06/Labyrinth_User_Manual.pdf)

---

# Using the Moog Labyrinth in Eurorack Song Creation

As a modular synthesizer musician, one of the biggest challenges is moving from an engaging loop, riff, or groove into a full-length, evolving composition. The **Moog Labyrinth** is uniquely suited to help overcome this challenge due to its generative dual sequencer, flexible semi-modular patch bay, and deep modulation capabilities. Below, you'll find a synthesis of techniques that leverage Labyrinth's features (and integration with other modules) for complete song structure and progression.

---

## 1. **Generative Sequencing for Continuous Evolution**

**Labyrinth's dual 8-step generative sequencers** can create endlessly evolving melodies, basslines, or rhythmic patterns without repeating exactly, especially with the **CORRUPT** function enabled. This is a powerful solution to “loop fatigue” often experienced in modular music.

**Key Techniques:**
- **Morphing Melodic Content:** Use the CORRUPT knob to slowly and subtly mutate melodies or basslines over time, keeping patterns fresh.
- **Sequence Chaining:** Chain SEQ1 and SEQ2 for up to 16-step sequences. Use different LENGTH settings for polymetric effects.
- **Scene Recall:** You can **lock-in** a generated sequence mid-set using **BUFFER** (hold for 1s) and **recall** it after mutating, simulating verse/chorus transitions.

**Advanced Patch:**
- Sequence the VCO and MOD VCO separately (SEQ1 → VCO, SEQ2 → MOD VCO) to make their evolution asynchronous. Use an external clock divider/multiplier for further rhythmic diversity.

---

## 2. **Performance Macros & "Song" Navigation**

Because Labyrinth doesn't recall full panel presets, you can design **performance macros**:
- **Resetting/Clearing Sequences:** Use the RESET and BUFFER+RESET combos for dramatic section changes (e.g., “drop” everything, re-enter with new material).
- **Manual Tweaks:** Assign large knob movements (VCW FOLD, CUTOFF, BLEND, EG DECAY) for live filtering, timbral transitions, or breakdowns/build-ups.
- **External Control:** Patch other CV sources (modulation sequencers, pressure/joystick, MIDI CC) into key patch points like BLEND, CUTOFF, or VCA CVs for macro automation.

**Example:**
- Use a footswitch or controller to trigger RESET or MUTATE sections for breakdowns or transitions.

---

## 3. **Interfacing & Layering with Other Modules**

Labyrinth shines as both a **centerpiece** and a **sequencer/sound generator** for other voices:
- **Clocking and Sync:** Use Labyrinth’s internal/external clock or MIDI sync. Its clock out can drive other modules (drum sequencers, envelopes, utility sequencers) for synchronized changes.
- **CV/Gate Out:** Patch Labyrinth’s SEQ1 or SEQ2 CV/Trig outs to external oscillators, sampler modules, or other voices to generate harmonically or rhythmically related layers.
- **Processing External Audio:** Use the patch bay’s VCW IN or VCF IN to process drum loops, field recordings, pads, or voices from your other modules, modulating with Labyrinth’s sequencer for evolving FX.

---

## 4. **Song Structure: Dynamic Voice Allocation**

**Split roles** within Labyrinth and externally:
- *Bass/Melody*: Assign the VCO to the bass and the MOD VCO to melodic or percussive lines. Transition between them by crossfading BLEND or switching sequences.
- *Pad/Rhythm Generators*: Use the patch bay utility mixer (U MIX) to create submixes, send them to VCW or VCF for parallel textural layers.
- *Duophony*: Split Labyrinth so SEQ1+VCO handle one “song section,” while SEQ2+MOD VCO handle another, introducing or removing layers as the patch evolves.

---

## 5. **Organic, Evolving Transitions**

**Don’t be afraid of generative "drift":**
- Let one sequencer’s CORRUPT index ramp slowly during a section to create natural, never-fully-repeating progressions.
- Patch envelopes or LFOs from other modules to key parameters (BLEND, VCW FOLD, EG DECAY), so the mix, harmonics, and envelope shapes change gradually and hands-free.
- Use external sequential switch modules to alternate Labyrinth’s outputs through different FX chains or rhythm processors during a set.

---

## 6. **Bridging with MIDI & External Control**

- **MIDI Keyboard Input**: Quantize and transpose Labyrinth’s root (see manual, MIDI Note On behavior) for classic key changes or sudden modulations during a performance.
- **MIDI Clock / Sync**: Sync Labyrinth with drum machines, DAWs, or external sequencers to structure intros, drops, and outros precisely.
- **MIDI CC/Pedal CV**: Map a MIDI or expression pedal to patch points for realtime fades, filter sweeps, or crossfades.

---

## 7. **Preset Morphing (Manual/External)**

Since Labyrinth cannot store presets:
- Use “preset sheets” (see manual) for reference, and quickly dial between prepared states.
- Use modules like CV preset sequencers or manual control voltage sources (e.g., Planar, Pressure Points) to instantly recall specific parameter sets by sending predetermined CV to key patch points.

---

## 8. **Song Example Workout**

**Intro:**  
- Fade in a simple sequence using just the VCO. Slowly adjust BLEND toward the VCF path.
- Gradually turn up SEQ2 and MOD VCO for harmonized lead lines.

**Verse:**  
- Bring in a rhythmic sequence on SEQ2 routed to MOD VCO, with CORRUPT adding melodic changes.

**Chorus:**  
- Chain both sequencers, increase sequence length, and use the utility mixer for richer timbres.
- Use VCW and VCF order switching for new tonal blends.

**Bridge/Breakdown:**  
- Dramatically drop BLEND to one path, increase CORRUPT for randomness, or reset sequences for a moment of silence/restart.

**Outro:**  
- Dim overall VOLUME gradually while increasing filtering or folding, or fade out with EG2 DECAY.

---

### **Combining with Other Modules**

- **Drum Modules:** Use Labyrinth’s clock/sequencer outs to trigger percussion modules (e.g., BIA, Pico Drums).
- **Samplers/Loopers:** Use triggers/CVs to launch samples and change loop speeds or grains for texture changes related to the generative sequences.
- **Switches/FX:** Rout Labyrinth’s audio out through sequential switches or FX pedals/modules for evolving textures and transitions.

---

## **Summary Checklist**
- Use sequencer chain, bit shift, corrupt, and quantize functions for song evolution and sectioning.
- Patch points allow direct morphing, external modulation, clocking, and layering with the rest of your system.
- Take advantage of mutation, crossfade, and voice allocation to move *beyond the loop* into full-form songs.

---

## **References**

- [**Moog Labyrinth User's Manual PDF**](https://www.moogmusic.com//sites/default/files/2024-06/Labyrinth_User_Manual.pdf)
- [Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)