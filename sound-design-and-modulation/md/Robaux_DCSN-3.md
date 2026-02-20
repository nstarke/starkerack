# Robaux — DCSN-3

- [Manual PDF](../../manuals/robauxDCSN3Manual.pdf)

---

[Robaux DCSN3 Decision Tree Module Manual (PDF)](https://robaux.io/assets/modules/dcsn3/DCSN3-Manual.pdf)

---

# Unlocking the Creative Power of the Robaux Decision Tree (DCSN3)

The Robaux DCSN3 Decision Tree is a powerful, performance-friendly randomizer, trigger router, and clock divider for Eurorack. Below is an analysis and set of creative patch ideas to modulate the module for three challenging sound design areas: **distorted percussion**, **crazy basslines (like in dubstep or DnB)**, and **haunting atmospheric pads**.

---

## 1. Distorted Percussive Sounds

### Key Points from the Manual
- DCSN3 can distribute a single trigger/gate randomly or in patterns across up to 12 outputs.  
- Multiple operation modes: mono/poly, latch, clock divider.
- Acts as a complex, multi-channel clock divider with randomization.
- Modes are selectable; division types extend to nonstandard clock ratios (2, 3, 5, spread).

### Creative Modulation Techniques

#### **Chaos Percussion Router**
- **Patch a single gate/trigger or clock source (fast clock) into input a.**
- **Set DCSN3 to Poly/Mono or Poly/Poly mode.**
- **Route several outputs (b–m) to multiple drum modules (even the same one via stackables/switches).**
- Results in "machine-gun," unpredictable percussive bursts across your percussion voices.
- FX: Insert a distortion, wavefolder, or bitcrusher *after* one or more drum modules for maximal grit.

#### **Randomized Clock Division**
- Use DCSN3 clock divider modes (Classic, 2/3/5, Spread) to *trigger distortion or waveshaping modules* at non-regular intervals.
- Patch different division outputs to separate drum triggers or envelope generators for layered, chopped rhythmic complexity.

#### **Gated Saturation/FX**
- Use suboutputs to trigger VCAs opening the audio from a drum or sample *only on certain random steps*—pass signals through resonant filters or distortion, so only slices of the sound are mangled/distorted at random moments.

---

## 2. Crazy Basslines (Dubstep / DnB)

### Key Points from the Manual
- Output routing and mode selection allow for pseudo-random or repeating (16-step pattern) modulation.
- Outputs can be used to drive envelopes, VCA level, filter cutoff, or oscillator FM.

### Creative Modulation Techniques

#### **Bass Movement through Random Routing**
- Set up a fast clock, or clock divided by 2 or 4, into input a.
- Patch **several suboutputs to CV inputs on filter cutoff, waveshaper fold amount, or overdrive level** in your bass voice (not triggers! Use as modulation gates or use S&H to make them CVs).
- Alternatively, use outputs to *reset or re-trigger LFOs* modulating your bass parameters for unpredictable but rhythmic movement.

#### **Random Reset: Glitchy Bassline Generator**
- Use the **hidden reset input** (patch stepped sequencer or random gate into m), so you can force the DCSN3 to jump back to step 1 at non-regular intervals.
- Any modulation chain triggered by DCSN3 (filter, wavetable, sync reset, etc.) will have accents and dropouts that give your bassline a brutally glitched, neuro/DNB-style feel.

#### **Divided Bassline Syncopation**
- Use DCSN3's 2/3/5 or Spread divider modes to create off-grid step sequences.
- Patch multiple outs into *different VCAs* controlling different bass sources.
- Sends polyrhythmic, unrelated triggers to different synth voices, resulting in complex, shifting bass patterns.

---

## 3. Haunting Atmospheric Pads

### Key Points from the Manual
- Subtle randomization and latch modes can create evolving, slowly shifting patterns.
- Switching between random and looped pattern via rotary knob allows improvisational performance.

### Creative Modulation Techniques

#### **Gentle Gate Sprays—Diffuse Drone Textures**
- **Input a slow random pulse (e.g., Turing Machine or S&H clock) to input a.**
- Enable **Latch Poly/Poly mode**—latched gates will stay high until new input, so your pads wash in and out unpredictably.
- Use outs to gate VCAs on long, heavily reverbed/filtered drones or FM voices.

#### **Clock-Driven Pad Swells via Divider**
- Enter Spread mode, provide a slow external clock.
- Patch each output to a separate pad voice, oscillator drone, or VCA.  
- The Spread mode creates slow patterns; as voices fade in/out at different rates, you get organic, otherworldly textures.

#### **Randomized Layering**
- Use the random-to-loop morph function (rotary n) to improvise between “totally random” and “slightly familiar/recurring” combinations—pad layers appear and disappear, creating a narrative, haunted quality.

#### **Atmospheric Random FX**
- Use suboutputs to *randomly trigger slow modulation sources*: sample & hold, slow envelopes, phase shifters, delay send levels.
- Layer the resulting unpredictably-shifting atmospheres for evolving, non-repetitive pads.

---

## **Performance/Advanced Tips**

- **Use the mode switch shortcut**: Hold key o and twist the rotary to morph between mono/poly, latch, or regular trigger.
- **Visual feedback**: Use illuminated output patterns to guide live improvisation ("light sculpture" control).
- **Debug mode**: Check your patch and output assignments fast before a performance.

---

For full details and more creative possibilities, consult the full manual: [Robaux DCSN3 Decision Tree Module Manual (PDF)](https://robaux.io/assets/modules/dcsn3/DCSN3-Manual.pdf)

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)