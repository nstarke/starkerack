# Question

Please document how the Fancyyyyy Synthesis K-Accumulator and Rung Divisions can be used together when they are connected internally.  The interal connection documentation can be found here: https://www.fancysynthesis.net/_files/ugd/2321ab_c6527117434d46138fc2b65b06566496.pdf

## Modules In Scope

- Fancyyyyy K-Accumulator Digital Complex Oscillator
- Fancyyyyy Rung Divisions V2 Clock Divider + Shift Register

---

# Answer

I've read both manuals fully, but I was unable to retrieve the internal-connection PDF: WebFetch isn't authorized in this session and network commands via curl were also blocked. Rather than guess at that document's contents, here is what I can document honestly — what each manual actually says about inter-module connection points, and how the two modules pair musically.

# Fancyyyyy K-Accumulator + Rung Divisions: Using Them Together

## ⚠️ A note about the internal connection document

I could not access the linked PDF (`fancysynthesis.net/_files/ugd/2321ab_c6527117434d46138fc2b65b06566496.pdf`) from this environment — web access was not permitted in this session. **Neither of the two manuals I was given describes an internal (behind-the-panel) connection between these two specific modules**, so everything below about the internal link is limited to what the manuals verifiably state, plus front-panel usage that is fully documented. I have not invented details from the unretrievable PDF; please re-run with web access granted (or drop the PDF into the manuals repo) and I can complete that section.

## What the manuals do document about internal connectivity

**Rung Divisions (manual, p.10 "Installation and Calibration"):**
- The module has **four pin headers on the rear**. Only the header labelled "POWER" may receive power — connecting power to any other header can irreversibly damage the module.
- The other headers are labelled in the manual's rear-panel diagram as **"Expander headers 2 & 3"** and **"Expander header 4"**. These are the module's designated internal-connection points.
- The **"Expanders" chapter is a placeholder ("Coming soon")** in this manual revision — the expander/internal-connection protocol is exactly what the separate PDF you linked would cover.

**K-Accumulator (Quickstart v1.02):**
- Requires **two Eurorack power connections** (both headers must be connected). The quickstart does not document any expander/internal header, and notes a full technical manual covering the architecture in depth is still in progress.

So the plausible internal link is Rung Divisions' expander headers connecting behind the panel to the K-Accumulator — but the pinout, cable, and which signals are carried are only in the document I couldn't fetch.

## How the two modules complement each other (documented behavior)

Even without the internal-connection details, the manuals make the intended pairing clear. Rung Divisions is a **poly-rhythmic gate generator and Benjolin/Rungler-derived stepped-CV source**; the K-Accumulator is a **complex oscillator whose every CV input expects exactly this kind of signal**. The natural signal routings (whether made with patch cables or provided by the internal connection) are:

### 1. Rung Divisions as clock/trigger source for the K-Accumulator

| Rung Divisions output | K-Accumulator destination | Result |
|---|---|---|
| Bus1 / Bus2 (mixed clock divisions) | **Δ-Σ Clock input** | Poly-rhythmic stepping of the Δ-Σ pattern generator. Patching this jack breaks the internal UFG normalization, so the pattern generator now steps on Rung Divisions' composite rhythm. |
| /2–/8 divider outputs | **UFG Trig input** | Triggers the function generator in single-shot mode (envelopes/pulsar windows) on any division; the Type button selects hard sync, reversal, or sustain trigger responses. |
| 1-Bit output | **OSC Ext. input (Sync mode)** | The buffered first-bit gate acts as an external damped-sync source, overriding the UFG. |

### 2. Rung Divisions as CV source for the K-Accumulator

| Rung Divisions output | K-Accumulator destination | Result |
|---|---|---|
| 8-Bit output (±5V "sequencer" DAC) | **1V (Root)** or **1V/TZ (OSC)** | Random/looping pitch sequences. The Root input is 1V/Oct calibrated and can be quantised to 21 TET or JI scales — this tames the Rungler's chaos into melodies. The 1V/TZ input auto-detects stepped vs. audio-rate signals, so a sub-audio 8-Bit pattern is treated as pitch CV and an audio-rate one becomes through-zero FM. |
| 3-Bit output ("rungler", contrapuntal reverse-encoded) | **Shift / Depth / Shape / Morph CV inputs** | Stepped animation of the waveshaping matrix. The 3-Bit and 8-Bit outputs move in contrary motion, so using both on different destinations gives complementary voices/timbre motion. |
| Noise output | Any attenuverted CV input | Analogue noise modulation. |

Every OSC-row CV input on the K-Accumulator has an internal normalization from its own UFG or Δ-Σ; **plugging Rung Divisions into any of these jacks overrides that normalization**, replacing internal modulation with Rung Divisions' external patterns.

### 3. K-Accumulator as clock/animator for Rung Divisions

- The **UFG gate output** (pulse width set by Skew) is an ideal clock for Rung Divisions' Clock input — and because Rung Divisions runs from 0–40 kHz, the UFG can sweep it from slow poly-rhythms into audio-rate sub-harmonic/PWM territory. A PWM'd clock (Skew under CV) dynamically changes all gate output lengths, as described in the Rung Divisions Clock Division chapter.
- The **Δ-Σ output** can drive Rung Divisions' Length, Chance, or Direction CV inputs, so the oscillator's pattern generator reshapes the shift register's loop point and randomness in time.

### 4. Cross-feedback (chaos patch)

The Rung Divisions manual explicitly recommends feeding the **3-Bit or 8-Bit output back to a CV input of its clock source**. With the K-Accumulator's UFG clocking Rung Divisions and the 8-Bit output patched to the UFG Time CV (1V/Oct), the pair forms a two-module chaotic system — "burst-like" from the 3-Bit output, more random-with-strange-attractors from the 8-Bit — with the Chance knob dialling in slowly evolving chaotic patterns.

## Summary

The verifiable picture: Rung Divisions exposes dedicated expander headers on its rear PCB for exactly this kind of internal pairing, and the two modules are designed as a rhythmic-brain + complex-voice combination — Rung Divisions supplying clocks, gates, and Rungler CV; the K-Accumulator supplying quantised pitch, envelopes, and audio, with every relevant jack's normalization documented to yield gracefully to the other module's signals. For the exact internal cable pinout and which of these routings the internal connection hard-wires, I'd need access to the linked PDF — happy to fold that in if you can grant web access or add the file to `/home/nick/Documents/git/eurorack-manuals-repo/`.
