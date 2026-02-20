# Behringer — 173

- [Manual PDF](../../manuals/QSG_BE_0720-AAL_173 QUAD GATE-MULTIPLES_WW.pdf)

---

[Behringer 173 QUAD GATE/MULTIPLES Manual PDF](https://mediadl.musictribe.com/media/PLM/data/docs/P0EAQ/173_QUAD_GATE_MULTIPLES_QSG_WW.pdf)

---

## How To Use the Behringer 173 QUAD GATE/MULTIPLES to Make Full-Length Eurorack Songs

The Behringer 173 QUAD GATE/MULTIPLES module is a deceptively simple but powerful utility for modular musicians. It provides quad analog gates (with CV control and pass-through) and six sets of passive multiples. While it does not generate sound on its own, it is an extremely helpful tool for structuring, transforming, and expanding your patch—crucial ingredients in turning groovy ideas into cohesive, dynamic songs.

Below, I’ll break down strategies for using the 173 to construct full-length Eurorack tracks, focusing on arrangement, transitions, automation, and performance.

---

### 1. **Song Arrangement & Scene Changes**

#### **A. Muting, Unmuting, and Section Control (Using GATE)**
- Use the Quad Gates to mute/unmute voices (bass, melodies, drums, effects) by routing their trigger/gate/CV signals through the 173.
- Sequence the “GATE IN” inputs from a sequencer or manual controller (e.g., Intellijel Tetrapad, Make Noise Pressure Points).
- Use the “GATE OUT” to pass signals to modules that need to be enabled or disabled at certain parts of your arrangement.
- Example: Gate 1 can mute your drums for a breakdown, Gate 2 brings the hihat in for the chorus, etc. Use your performance controller or DAW to automate this.

#### **B. Live “Drops” and Transitions**
- Use manual gate/CV sources or performance sequencers to trigger transitions (fill, break, drop).
- Pair with voltage-addressable switch modules (e.g., Doepfer A-150, Mutable Instruments Branches) for live section swapping.

### 2. **Automation, Modulation, and Dynamic Patching**

#### **A. Automation of Gate Logic**
- Use LFOs, envelopes, or random/chaos sources (like Mutable Marbles, Wogglebug) patched into GATE CV to dynamically switch elements on/off, creating evolving arrangements.
- Use the inverting/non-inverting logic to create variations (e.g., Gate 3 allows a high gate to let melody through, Gate 4 takes the inverse for an alternate sequence part).

#### **B. Rhythmic Expansion**
- Patch a single gate from your clock divider or sequencer to a MULTIPLE, then send it to several modules for complex polyrhythms.
    - Example: Distribute clock to different percussion voices, or gate-reset signals for sequencers for song sections.

### 3. **Multiples for Macro Control**

- The six sets of 4-way passive multiples make it easy to “fan out” control voltages, triggers, or audio to many destinations:
    - Global modulation (one envelope to multiple filters/VCA for a unified dynamic)
    - Song-wide resets or clock stops/starts for synchronized transitions.
    - Spread melodies or LFOs to several voices for coherent musical phrases or sudden unified modulations (creating breakdown/build-up effects).

### 4. **Build-ups, Breakdowns, and Finales**

- Use the Gates to isolate parts during breakdowns or “drop” sections.
- Use Multiples to instantly route new CVs or triggers during climaxes—for “everything-at-once” moments or for quick changes in the structure.
- Record your performance or automate complex routings with CV sequencing to create an evolving song structure.

### 5. **Performance Tricks**

- Use the module as a “Song Scene Matrix”: pre-patch scenes using gate/CV routings and enable/disable them on the fly with manual gates, step sequencers, MIDI-to-CV controllers, or even external drum pads.
- Combine the 173 with logic modules (AND/OR/XOR) to create complex gating rules that govern song sections and transitions automatically.

---

## Example Song Structure Patch

1. **Intro:** Gates mute drums and bass, only pads are active.
2. **Verse:** Gate CV un-mutes melody; use a multiple to send clock to sequencer and effects.
3. **Chorus:** All gates open, multiple spreads modulation to open all filters, creating a climax.
4. **Breakdown:** Gates dynamically mute different voices, LFO randomizes which voice is active using inverting CV.
5. **Rebuild:** Multiples spread clock, triggers, and modulation, gates open up all channels.
6. **Outro:** Use a single gate to fade sections out in reverse order.

---

## Summary Table

| Feature           | Use In Song | Example Patch |
|-------------------|-------------|--------------|
| QUAD Gate         | Scene muting, transitions | Drum mute, drop, manual fill |
| GATE CV (inv/non-inv) | Arrangement automation | Randomize mutes, swing grooves |
| Multiples         | Spread signals, macro control | Global filter sweep, polyphonic clocks |

---

## Final Tips

- The 173 doesn’t make sound but is a “conductor” for your modular orchestra—perfect for structure, performance, and arrangement.
- Combine with sequential switches, voltage-addressed logic, and step sequencers for maximum effect.
- Think of it as the “arranger’s patchbay”—its true power appears when you want to play a full *song*, not just a loop!

---

### For the original manual PDF:  
[Behringer 173 QUAD GATE/MULTIPLES Manual PDF](https://mediadl.musictribe.com/media/PLM/data/docs/P0EAQ/173_QUAD_GATE_MULTIPLES_QSG_WW.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)