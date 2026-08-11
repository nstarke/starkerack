# Question

Please document the different configuration modes for the IDUM module and how to access the configuration mode selection UI

## Modules In Scope

- Mystic Circuits IDUM

---

# Answer

# Mystic Circuits IDUM — Configuration (Setup Menu) Modes

The IDUM's hidden configuration options live in its **Setup Menu** (the manual also calls it the "MENU" or "Set Up Mode"). These are global settings, separate from the eight performance modification modes (Bouncing Ball, Rotate, Gate Delay, etc.) selected during normal operation.

## How to Access the Setup Menu

1. **Long press the REMOVE MODE button** (upper-right button, labelled "HOLD 4 MENU" on the panel) to enter the Setup Menu. The MODE ring of LEDs and the LOOP LED switch to displaying the *current configuration* — a lit LED means that option is enabled/selected.
2. **Turn the MODE knob** to point at the option you want to change. Option names are faintly printed on the panel next to each mode LED position (e.g. `PARAM RESOLUTION`, `LENGTH RESOLUTION`, `SLOW CL`, `SPLIT`, `ODD`/`EVEN`/`POW2`).
3. **Short press (tap) REMOVE MODE** to toggle/select the option the dial is pointing at.
4. **Long press REMOVE MODE again** to exit and return to normal operation.

Settings are saved on exiting the menu and **persist across power cycles**.

> ⚠️ **Important:** Unplug (or mute) any modulation patched into the **MODE CV input** before using the menu — mode CV shifts where the processor thinks the dial is pointing, so you could toggle the wrong option.

## Configuration Options

| Option | Sub-settings | Description |
|---|---|---|
| **Parameter Resolution** | ODD / EVEN / POW2 | Restricts the values selectable with the PARAM knob in BURST, MULTIPLY/DIVIDE, and clock-skip modes. **ODD** = any value 1–8; **EVEN** = only 1, 2, 4, 6, 8; **POW2** = only powers of two (1, 2, 4, 8). Useful for keeping tempo-synced manipulations predictable. |
| **Length Resolution** | ODD / EVEN / POW2 | Same restriction scheme, but applied to the LENGTH slider: **ODD** = 1–8, **EVEN** = 1, 2, 4, 6, 8, **POW2** = 1, 2, 4, 8. |
| **Slow Clock** (SLOW CL) | LED on / off | Sets the speed of the clock bursts IDUM uses to re-synchronize sequencers on its clock output. LED **off** = slow bursts — best for slower/digital sequencer modules. LED **on** = fast bursts — best for fast analog sequencers (e.g. Mystic Circuits Tree). If cycle/skipping behavior misbehaves, turn this off. |
| **16 Step** | — | *Unimplemented in firmware v1.0.* Will extend the looper and modification lengths to 16 steps, controlled via the CYCLE switch (labelled "16 STEP" in Setup Mode). |
| **Split** | — | *Unimplemented in firmware v1.0.* Will eventually let each trigger channel choose when it applies a modification, and which one, independently. |
| **Loop** (gate input behavior) | Toggle / Momentary | Press the **LOOP button while inside the Setup Menu** to change how the LOOP gate input behaves. LED **off** = incoming gates *toggle* the looper on/off with each rising edge. LED **on** = gates *momentarily* engage the looper only while the gate input is high. |

## Notes

- In Setup Mode, the **CYCLE switch** is reassigned to the 8-step/16-step selection (labelled "16 STEP") — not yet functional in firmware v1.0.
- The Setup Menu is summarized in the "Getting Started" section (step 8, p. 17) and detailed in the **SETUP MENU** (p. 32) and **SETUP MENU OPTIONS** (p. 34) sections of the manual.
