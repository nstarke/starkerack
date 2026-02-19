# 2hp — Arp

- [Manual PDF](../../manuals/2hp_Arp_Manual_2023.pdf)

---

[Download the 2hp Arp Manual PDF](https://2hp.com/wp-content/uploads/2020/05/2hp_ARP_manual.pdf)

---

# Using 2hp Arp for Hyper-Complex, Densely Rhythmic Percussive Sequences

The 2hp Arp is a gate-driven arpeggiator, not a direct percussive voice or effect, but a CV/gate sequencer specialized in chord-based melodic or pitch information. However, in a creative eurorack environment, especially with percussion modules that can be triggered by pitched CV/gates, the 2hp Arp can be the brain of hyper-complex rhythms and polyrhythms. Here’s how you can leverage the Arp for densely rhythmic, punchy, and unique percussion patterns:

---

## 1. Turn Melodies into Percussion: Pitch-to-Trigger/Drum Synthesis

- **Pitch Sequence to Percussive Module:** Patch the *Output* of the 2hp Arp to a drum module that accepts 1V/Oct CV (e.g., Plonk, Basimilus Iteritas Alter, Erica Synths Pico Drum, etc.)
- **Result:** Each step in the arpeggio sequence hits a different pitch/timbre on your percussive module. Use a *random* or *pendulum* mode to create evolving, dense rhythmic hits.

---

## 2. Gate/Trig Polyrhythms

- **Trig Input as Rhythmic Driver:** Feed the Arp’s *Trig Input* with irregular, fast, or polyrhythmic gate/trigger streams (from a clock divider, trigger sequencer, or burst generator). 
- **Further Complication:** Use different clock divisions or clock sources (e.g., 5 against 4, 7 against 3) to feed the Trig Input, creating inherent polyrhythms in the arpeggio’s playback.
- **Arp as Percussive CV Source:** Route its V/Oct output to a quantizer locked to drum-friendly intervals, or directly drive a percussive voice with highly resonant filters, LPGs, or tuned noise for kick/snare/perc hits.

---

## 3. Chord Complexity as Percussion Source

- **Dense Chord Patterns:** Use more complex chords (especially diminished/augmented and 7ths) for jittery, unstable arpeggios—the rapid succession of intervals maps to wild percussive variation.
- **Live Performance:** Twist the *Chord* and *Root* knobs—or sequence them via CV—for continuously morphing, non-repeating percussive lines.

---

## 4. Playlist of Arpeggio Modes for Structure

- **Mode Knob/Mode CV:** Voltage-control the *Mode* for dynamic switching between ascending/descending/random/pendulum motion, disrupting standard grid repetition.
- **Combine one/two octave modes** to shift the "span" of percussive notes—fast, randomized octave jumps create highly syncopated feel.

---

## 5. Sync & Reset for Pattern Complexity

- **Reset Input for Odd & Asymmetric Loops:** Use reset signals at unusual intervals (non-multiples of your primary clock—prime numbers for example). This constantly restarts the arpeggio at non-obvious rhythmic points—excellent for non-linear rhythms.

---

## 6. Patching Inspiration for Unique, Punchy Sound

- **Wavefolder/Fuzz/Distortion:** Run VCA-controlled percussive modules through aggressive effects, synced to the arpeggiator output, for glitchy, punchy, industrial drum sounds.
- **Amplitude/Filter Modulation:** Use envelope followers, LPGs, or additional VCAs to "sculpt" the percussive hits coming from this melodic stream.
- **Layer Multiple Voices:** Use multiples or buffered mults to split the Arp’s V/Oct out, controlling different percussive voices for instant multi-drum percussion from one pattern.

---

## Example Patch for Hyper Complex Percussion
1. Clock divider #1 (÷5) and #2 (÷7) send triggers to a logic module (XOR or OR), which then triggers the *Trig Input.*
2. Arp's *Output* goes to two voice modules—one pitch-to-drum, one tuned digital metallic voice (like BIA).
3. *Chord CV* input receives a random or LFO signal, slowly morphing the chord over time.
4. Use Pendulum/Random two octave mode for wide variation.
5. *Reset Input* receives a trigger every 13 steps (prime number).
6. All drum voices routed to a shared distortion/wavefolder.

---

By creatively patching the 2hp Arp, you are freed from traditional step sequences, triggering ultra-dense, polyrhythmic, non-repeating, and percussively chaotic patterns.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)