# K-ACCUMULATOR + Rung Divisions Internal Integration

K-ACCUMULATOR and Rung Divisions can be connected internally using the rear-panel headers, creating a normalized connection between the two modules.

With the supplied **6-to-10-pin rear cable**, K-ACCUMULATOR sends two signals internally to Rung Divisions:

- **K UFG Pulse → Rung Divisions Clock**
- **K MOD oscillator → Rung Divisions Data**

Once the rear cable is installed, you do not need front-panel patch cables for these two fundamental connections.

For the current Rung Divisions, connect the **6-pin end to K-ACCUMULATOR's 6-pin header** and the **10-pin end to the Rung Divisions header marked with three lines**, with the red stripe facing down at both ends.

> The exact rear connection depends on which Rung Divisions revision you own. The connection guide also documents a different wiring procedure for **v1 Rung Divisions**, using a two-wire female-to-female jumper between specific K header pins and the Rung **Bit Seive** header.

---

## What the Internal Connection Does

The internal normalization effectively turns K-ACCUMULATOR and Rung Divisions into a larger feedback/sequencing instrument.

### K UFG → Rung Clock

K's **UFG Pulse** becomes the default clock source for Rung Divisions.

Because the UFG spans sub-audio through audio rates, changing **UFG Time** moves Rung Divisions between:

- Slow sequencing
- Polyrhythmic clocking
- Fast pattern generation
- Audio-rate clock division
- Subharmonic synthesis

Rung Divisions' clock dividers operate from approximately **0–40 kHz**, so they are designed to work in both low-frequency and audio-rate regimes.

### K MOD → Rung Data

K's **MOD oscillator** becomes the default Data source for Rung Divisions.

This means that changes to K's modulation oscillator can directly alter the bitstream being sampled by Rung's shift register.

Useful K controls include:

- **Harmonic**
- **Order**
- **Detune**
- MOD tracking source:
  - Root
  - OSC
  - UFG

Because MOD can move between free pitch offsets, harmonic relationships, and scale-quantized relationships, it can produce very different kinds of data streams for the Rung Divisions shift register.

---

## Practical Integrations

### 1. UFG Time as the Master Rung Rate

Since UFG Pulse is normalized to Rung Clock, the **UFG Time** control effectively becomes the master speed control for Rung Divisions.

At slow rates, this gives you sequencer-like behavior.

At audio rates, Rung Divisions becomes a divider/subharmonic generator.

---

### 2. MOD Harmonic and Order as Pattern Controls

Because MOD feeds Rung Data internally, **Harmonic** and **Order** affect the relationship between the Data waveform and the Rung clock.

This can create different degrees of repetition and variation.

In practice:

- Simple harmonic relationships can produce more obviously repeating patterns.
- More complex or detuned relationships can produce longer, evolving patterns.
- Scale-quantized MOD relationships can create more structured interactions.

This behavior follows from the documented clock/data connection and from how the Rung shift register samples Data on clock edges.

---

### 3. MOD Detune as a Pattern-Evolution Control

Small changes to **MOD Detune** alter the phase relationship between:

- the MOD waveform feeding Rung Data
- the UFG Pulse feeding Rung Clock

Because the shift register reads the Data state when a clock event occurs, small detuning changes can gradually alter which values are captured.

This makes MOD Detune useful for moving between:

- Stable repeating patterns
- Slowly evolving patterns
- More unstable pseudo-random behavior

---

### 4. Rung Chance as a Stability Control

Rung Divisions' **Chance** control determines how much new data can enter the shift register versus how strongly the existing pattern loops.

With MOD supplying Data internally, Chance becomes a useful control over how much influence K's MOD oscillator has on the current pattern.

Use it to move between:

- Locked repeating loops
- Slowly mutating loops
- Highly unstable patterns

---

### 5. Rung Length and Direction as Pattern Reinterpretation

You can change the resulting sequence without changing K at all.

Use:

- **Length** to move the loop point
- **Direction** to reverse the read direction

This lets the same internally generated MOD data produce different repeating structures.

---

## The Front Panel Becomes the Return Path

The internal connection handles:

```text
K UFG Pulse → Rung Clock
K MOD       → Rung Data
```

The front panel can then be used to send Rung's outputs back into K.

For example:

```text
K UFG → Rung Clock
K MOD → Rung Data
Rung 8-Bit → K OSC 1V/TZ
```

This creates a closed system:

1. K generates timing.
2. K generates the binary Data source.
3. Rung converts that into an evolving stepped pattern.
4. The Rung pattern returns to K and controls pitch or modulation.

---

## Rung 8-Bit → K OSC 1V/TZ

A very useful first return patch is:

```text
Rung 8-Bit → K OSC 1V/TZ
```

K's 1V/TZ input automatically distinguishes between stepped control signals and audio-rate modulation.

At low rates, the Rung 8-Bit output behaves as a stepped pitch/modulation sequence.

At audio rates, the same input can move into through-zero FM behavior.

This makes it possible to move continuously between sequencing and audio-rate modulation without changing the basic architecture.

---

## Rung 8-Bit → K Root

A deeper return patch is:

```text
Rung 8-Bit → K Root 1V
```

K's Root can control:

- OSC
- UFG
- both OSC and UFG

MOD can also track Root.

This means one Rung CV pattern can influence much of K's internal frequency structure at once.

With a scale enabled on K, the Root system can also quantize the resulting movement into TET or Just Intonation relationships.

---

## Closed Feedback Patch

A particularly powerful configuration is:

```text
K UFG Pulse → internal → Rung Clock
K MOD       → internal → Rung Data
Rung 8-Bit  → K Root 1V
```

If the UFG is following Root, the feedback path becomes:

```text
K Root
  ↓
K UFG frequency
  ↓
UFG Pulse
  ↓
Rung Clock
  ↓
Rung shift register
  ↓
Rung 8-Bit
  ↓
K Root
```

This creates a feedback system where:

- K sets the Rung clock rate.
- Rung generates the pattern.
- The pattern changes K's Root.
- Root changes the UFG.
- The UFG changes Rung's clock rate again.

This closely matches the feedback architecture described in the Rung Divisions manual, where feeding the 3-Bit or 8-Bit output back to a CV input of the oscillator supplying the clock can generate chaotic behavior.

Useful controls in this patch:

### On K-ACCUMULATOR

- UFG Time
- Root
- Root routing
- Scale
- MOD Harmonic
- MOD Order
- MOD Detune
- Morph
- Shift
- Depth
- Shape

### On Rung Divisions

- Chance
- Length
- Direction
- Bus1 division selection
- Data/write controls

---

## Audio-Rate Integration

Because both modules operate well at audio rates, the rear connection is not limited to sequencing.

With the UFG in the audio range:

```text
K UFG Pulse → Rung Clock
```

Rung's `/2` through `/8` outputs become subharmonic signals.

These can be patched back into K for:

- Sync
- Through-zero FM
- Phase modulation
- Additional rhythmic or audio-rate modulation

Example:

```text
Rung /3 → K TZPM
Rung /5 → K UFG TZFM
Rung Bus1 → K Ext Sync
```

This turns Rung Divisions into an external digital subharmonic and modulation network for K-ACCUMULATOR.

---

## Conceptual Architecture

The intended pairing can be thought of like this:

```text
                     REAR NORMALIZATION

K-ACCUMULATOR                         RUNG DIVISIONS
────────────────                      ──────────────
UFG Pulse ──────────────────────────→ Clock
MOD Oscillator ─────────────────────→ Data


                     FRONT-PANEL RETURNS

Rung /2…/8 ─────────────────────────→ K modulation / sync
Rung Bus1/Bus2 ─────────────────────→ K trigger / sync / modulation
Rung 1-Bit ─────────────────────────→ K trigger / sync
Rung 3-Bit ─────────────────────────→ K pitch / CV / FM
Rung 8-Bit ─────────────────────────→ K Root / pitch / CV / FM
```

The rear cable therefore establishes the **forward path**, while front-panel patching establishes the **return path**.

---

## Recommended Starting Patch

Start simple:

```text
Internal:
K UFG Pulse → Rung Clock
K MOD       → Rung Data

Front panel:
Rung 8-Bit → K OSC 1V/TZ
K sine/cosine → stereo output
```

Then:

1. Set Rung to an 8-step loop.
2. Use Chance to find a stable or slowly evolving pattern.
3. Adjust MOD Harmonic and Order.
4. Make small changes to MOD Detune.
5. Change UFG Time to alter the master rate.
6. Experiment with Rung Direction and Length.
7. Once the pattern is working, add K's Morph, Shift, Depth, and Shape.

This is a good way to hear the internal integration clearly before introducing more complicated feedback paths.

---

## Summary

The rear connection turns the pair into a tightly coupled system:

```text
K UFG Pulse → Rung Clock
K MOD       → Rung Data
```

That makes K-ACCUMULATOR the default source of both **timing** and **binary data**, while Rung Divisions transforms those signals into:

- Clock divisions
- Polyrhythmic gates
- Shift-register patterns
- 1-Bit signals
- 3-Bit stepped CV
- 8-Bit stepped CV

Those outputs can then be patched back into K's:

- Root
- OSC 1V/TZ
- TZPM
- UFG TZFM
- Ext Sync
- Other CV inputs

The result is a system that can move continuously from structured sequencing and harmonic relationships into evolving feedback, subharmonics, and chaotic audio-rate behavior.
