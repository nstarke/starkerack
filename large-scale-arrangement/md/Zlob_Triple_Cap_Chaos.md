# Zlob — Triple Cap Chaos

- [Manual PDF](../../manuals/Zlob Modular - Triple Cap Chaos.pdf)

---

[**Triple Cap Chaos Manual PDF / Product Page**](https://zlobmodular.com/product/triplecapchaos/)

---

# Using the Zlob Modular Triple Cap Chaos for Song Structure in Eurorack 

The **Triple Cap Chaos** from Zlob Modular is a unique chaos-based oscillator, noise source, pseudo ring modulator, and audio mangler. While modules like this often excel at quirky sounds, dirty textures, or wild modulation, it’s easy to relegate them to mere “spice.” However, you can use Triple Cap Chaos as a fundamental building block for composing, structuring, and evolving complete songs in your Eurorack system. Here’s how:

---

## 1. Dynamic Intro/Outro & Texture Shaping

- **Swappable Roles:** Use Triple Cap Chaos as a noisy textural pad or gritty lead at the intro, then bring it back for the outro. This bookends your track with sonic cohesion.
- **Automate Chaos Intensity:** Modulate the *Emanate* and *Width* parameters with envelopes/LFOs or sequenced voltages, ramping up chaos for the climax and toning it down for resolution.

**Example Patch:**
- Feed Triple Cap’s *Y* output through a lowpass gate or filter for evolving noise beds.
- Use a VC-mixer or crossfader to fade Triple Cap in and out during different song sections.

---

## 2. Percussive Elements/Unusual Beats

- **Audio Input Tricks:** Send pulses, gates, or rhythmic audio into the *IN* jack. Triple Cap Chaos will interact with incoming signals to generate wild ring-mod/bit crushed sounds.
- **Freeze/Release with Modulation:** Use a sequencer or clocked random voltage to switch quickly between chaotic and steady modes (by modulating *Emanate* or *Width*) for glitchy fills, pseudo-hi-hats, drums, and breakdowns.

**Example Patch:**
- Mult a drum machine or trigger sequence to the *IN* jack.
- Sequence the *Emanate* CV input (with a random source or S&H).
- Output through a VCA triggered by the same rhythm for synchronized, mangled percussion.

---

## 3. Leads, Basses, and Melodic Variation

- **Lead/Vox:** The *X* output gives windier/smoother sounds, while the *Y* is harsh/aggressive—great for dirty leads, robotic basslines, or formant textures.
- **Melodic Structure:** Instead of tracking pitch with 1V/oct, create melodic variation by switching between chaos levels (fine-tuned with *Width*) or mixing Triple Cap with a traditional VCO for unpredictable harmonics that evolve over time.

**Example Patch:**
- Route *X* or *Y* into a wavefolder or resonant filter.
- Modulate the filter cutoff with a classic envelope for traditional synthesis blended with chaos for movement.
- Sequence *CV* input with random voltage that resets every 4/8 bars for verse/chorus changes.

---

## 4. Transitions & Song Progression

- **Automated Chaos:** Program voltage changes for the *Emanate* or *CV* input to mark transitions (e.g., breakdowns, builds, drops). As these parameters shift, Triple Cap’s sonic signature morphs, helping to signal distinct song sections.
- **Cue Dramatic Moments:** At the end of a phrase (e.g., 16 bars), automate an abrupt parameter change or use stepped voltage to instantly alter the character of the output.

**Example Patch:**
- Use a sequential switch or voltage block to send fixed voltages to the *CV* input at specific song moments.
- Automate fades with voltage-controlled mixers or VCAs to bring Triple Cap Chaos forward or back in the mix for section changes.

---

## 5. Integration with Sequencers, Effects & Other Utilities

- **Self-patching Possibilities:** Take a chaotic output, attenuate and route back into *CV* input, creating feedback that mutates based on other patch elements for unrepeatable patterns section-by-section.
- **Gate Sequencers:** Sequence VCA or filter that processes the Triple Cap so its presence is “played” like another instrument—used for drops, fills, call-and-response with melodic parts.

**Example Patch:**
- Effect process (delay, reverb, warping) the output in parallel, then crossfade effected/clean sounds with VCAs based on your song’s emotional curve.
- Pair with a sample-and-hold/random source driving *CV* input for shifting timbres on chorus or repeats.

---

### **Putting It All Together: Song Blueprint Example**

1. **Intro:** Use Triple Cap’s X-output filtered for soft drones or swells, slowly increasing chaos.
2. **Verse:** Subtler application, or dry/wet crossfade to keep things restrained.
3. **Chorus:** Modulate *Emanate* and *Width* for wild sonics, increase Triple Cap’s presence in the mix.
4. **Breakdown:** Hard switch—use extreme parameter positions for chaos/noise collapse.
5. **Bridge:** Feed melodic content into *IN*, using Triple Cap to obscure or “glitch out” the material.
6. **Finale:** Return Triple Cap to the style/sound of the intro for a full-circle feel.

---

## **Tips for Using Chaos Musically:**

- **Pre-plan Section Timings:** Use voltage presets/scenes for recognized song sections (verse, chorus, etc.).
- **Embrace Randomness:** Let Triple Cap introduce variance where static patterns might get repetitive.
- **Performance Control:** Assign chaos modulation to a controller (manual knob, fader, or foot pedal) for expressive live tweaks.
- **Layering:** Mix chaos with traditional synth voices for a sense of contrast and evolution.

---

**[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)**