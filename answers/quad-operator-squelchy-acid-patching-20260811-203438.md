# Question

How can I configure the 'Quad Operator' FM Oscillator to produce squelching melodic acid tones?

## Modules In Scope

- Humble Audio Quad Operator
- Humble Audio Quad Operator Algo Extension

---

# Answer

I've read the full Quad Operator manual (and its Algo expander section). Here's a patch recipe built from the module's actual controls.

# Squelchy Acid Tones on the Humble Audio Quad Operator

The trick to acid sounds on an FM oscillator: there's no filter, so the **"squelch" comes from sweeping the modulation index** — an envelope into a **Gain CV** input stands in for the filter-cutoff envelope of a 303, and **operator feedback** stands in for resonance.

## 1. Start from the manual's "Neutral Position"

Per the *Achieving Harmonic Frequency Modulation Results* section:

- **VCO/LFO switch** → VCO
- **All four operators** → **Lock** state (integer ratios to master tuning — essential for harmonic, melodic results)
- **All Detune knobs** → 12 o'clock
- **All Shape knobs** → full counterclockwise (sine)
- **All Mod sends** → full counterclockwise (no modulation yet)

## 2. Build a two-operator acid voice

Use **Op 1 as the carrier** and **Op 2 as the modulator**:

- **Ratio 1** → ×1 (carrier at the fundamental)
- **Ratio 2** → ×1 or ×2. A 1:1 ratio gives a saw-like spectrum (very 303); 2:1 gives a hollower, square-ish tone
- On **Op 2's row, turn up the "Mod 1" knob** — this is the send from Op 2 into Op 1's frequency. Set it around 10–1 o'clock as your baseline "cutoff" level
- Take your audio from the **Op 1 output** only

Optionally nudge **Shape 1** slightly toward triangle/saw for extra bite, but keep Op 2 a sine — modulating with overtone-rich shapes gets noisy/aliased fast (the manual warns about this).

## 3. The squelch: envelope → Gain 2 CV

This is the key move. From the manual: *"Gain CV — affects both the output level of the operator signal as well as how intensely it modulates other operators via its modulation sends. Normals to gain of 1."*

- Patch a **snappy decay envelope** (fast attack, short-medium decay) into **Gain 2**. Note Gain CV expects **0–5 V**; once patched, it replaces the normalled full gain
- Now every gate closes Op 2's virtual VCA: each note starts bright (high FM index) and sweeps dark as the envelope falls — exactly the wah/squelch of a filter envelope
- **Decay time** = your "cutoff sweep" speed; **Mod 1 send level** = your "cutoff/env amount"
- For **accents**, use a sequencer accent output to raise the envelope level (or mix a second envelope into Gain 2) on accented steps — louder envelope = brighter, harder squelch

Put a regular VCA + amp envelope on the Op 1 output after the module, as usual.

## 4. "Resonance": operator feedback

- On **Op 2's row, also turn up "Mod 2"** — Op 2 modulating itself. Small amounts add a growly, resonant edge that reads like filter resonance; too much tips into noise (easy to ride live)
- Because Gain 2 scales *all* of Op 2's sends, your envelope sweeps the feedback and the carrier modulation together — the squelch and the "resonance" breathe as one, which is very acid
- For more extreme resonance-style effects, the manual suggests the **AR FM input**: take an operator output, process it externally (e.g., through a wavefolder or filter), patch it back into **AR FM**, and use the AR FM row's Mod sends. Watch the red clipping LED and trim the **Gain AR FM** knob

## 5. Melodic sequencing, slides, and consistency

- **Pitch sequence** → the **1V/Oct** input (controls all locked operators together, so the whole FM stack tracks in tune)
- **Slides** (the other half of the acid formula) → use your sequencer's glide/portamento on the 1V/Oct CV; alternatively patch a slewed CV into **LF FM** (±6 semitones) for bend effects
- Patch your gate/trigger into **Reset** to restart operator phase on each note — this keeps the FM transient identical note-to-note for a tight, consistent pluck

## 6. Bonus: Algo expander as a macro "filter knob"

Save a **dark algorithm** (low Mod sends) into slot **A** and a **screaming one** (high sends + feedback) into slot **B**, then use the **Crossfade** knob or its CV input to morph between them — a one-knob acid "cutoff macro" you can sweep or sequence over the pattern, or crossfade against the **Live** knob positions while you tweak.

**Quick summary:** Op 2 (sine, ratio 1–2×, in lock) FMs Op 1 via the Mod 1 send; a fast decay envelope into Gain 2 sweeps the FM index for the squelch; a touch of Mod 2 self-feedback fakes resonance; sequence via 1V/Oct with glide, trigger Reset per note, and take audio from Op 1.
