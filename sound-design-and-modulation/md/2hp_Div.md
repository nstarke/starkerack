# 2hp — Div

- [Manual PDF](../../manuals/Div_Manual.pdf)

---

[Link to 2hp Div Manual (PDF)](https://2hp.com/wp-content/uploads/2020/06/Div_manual.pdf)

---

# Creative Modulation Techniques With the 2hp Div

As a Eurorack musician, the 2hp **Div** is a compact but powerful clock divider/multiplier that can be modulated to create wild, kinetic rhythms and textures foundational to modern, gritty electronic music. Below are some focused strategies to harness it for **distorted percussion, aggressive bass, and haunting pads**.

---

## Module Recap & Key Features

- **2 independent clock div/mult channels**
- **Divides/multiplies by 1, 2, 3, 4, 5, 6, 7, 8, or 16**
- **Dedicated division/mult rate knob AND CV per channel**
- **Rate CV inputs: 0-5V**
- **Compact: 2HP**

---

## Modulation Approaches For Unique Sounds

### 1. Distorted Percussive Sounds

**Patch:**
- Use a fast clock or trigger source into `IN`
- Mulitply one channel (e.g., *16) and divide the other (/16); send both outputs to envelope generators or percussive modules
- Run both outputs into different VCAs/waveshapers
- **Rate CV**: Send a random stepped CV (like from a S&H, Turing Machine, or sequencer) to the rate CV input — this causes rapid-fire switching between clock divisions and multiplications, making for unpredictable, glitchy percussion gates

**Tips:**
- Run the outputs through **distortion or wavefolders**
- Use envelope followers to sync other effects to the rhythmic chaos coming from Div

---

### 2. Basslines for Dubstep/Drum & Bass

**Patch:**
- Clock your sequencer from `OUT 1` with a divided clock for halftime feel, and clock a modulation source (LFO or envelope) from `OUT 2` with a multiplied, hyperactive clock
- Modulate the **Rate** (DIV/Mult) for one output with an LFO synced to your DAW/modular clock—a triangle or saw LFO around the range of 0-5V mapped to Rate 1 CV causes shifting subdivisions that make basses "wobble" and gate unpredictably
- Paralleling this with stereo or multi-voice basslines will create complex, polyrhythmic patterns

**Tips:**
- Re-patch the **rate-modulated output** to trigger a VCA or LPG controlling your bass synth’s amplitude or timbre for classic dubstep wobbles or DnB gated bass
- Use both outputs to clock percussion and bass, so they stay “locked” but rhythmically evolving

---

### 3. Haunting Atmospheric Pads

**Patch:**
- Feed a slow clock (e.g., from a clocked LFO) to `IN`
- Send one output (/16) to occasionally trigger a reverb-heavy envelope (for pad gates) and the other (*3, *4, or *5) to modulate a long attack/decay envelope on a filter or VCA
- CV-modulate the **Rate 2** input with a very slow, subtle LFO or sequencer, so the pad “breathes” with irregular intervals

**Tips:**
- Run the different gate intervals through layered noise sources, granular modules, or string synth voices for swelling, unpredictable atmospheres
- Use sub-audio clocks (very slow divisions and multiplications) to build evolving textures—combine with delays and reverbs for ghostly movement

---

### Additional Modulation Ideas

- Send a touch controller, joystick, or random CV generator to the **Rate CV** to improvise in real time
- If you have a sequencer with voltage outs, sequence the Rate CV directly for precise, polyrhythmic pattern changes
- Use a slow envelope or DC-coupled audio signal to dynamically morph from dividers to multipliers mid-performance for morphing grooves

---

## Summary

The 2hp Div’s ability to quickly *and* unpredictably shift clock ratios, especially under CV modulation, is a secret weapon for any modular setup. By modulating its Rate CV inputs with everything from step sequencers to chaotic noise, you turn simple clocks into dynamic sources for evolving beats, morphing bass rhythms, or drifting pads—injecting life and surprise into your patches.

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)