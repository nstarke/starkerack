# Wenzellabs — NSA Selector

- [Manual PDF](../../manuals/wenzellabs_the_NSA_selector_ the NSA selector eurorack module.pdf)

---

[Manual PDF / Source](https://github.com/wenzellabs/the_NSA_selector)

# the NSA selector — melodic use in a Eurorack system

As a Eurorack musician, I’d treat **the NSA selector** less like a conventional voice module and more like a **data-to-audio sound source / network instrument**. Based on the manual, it is:

- a **4HP** module
- with **2 Ethernet ports**
- **1 audio output**
- internally a **100 Mbps fast ethernet switch**
- with a mirrored internal port feeding a **4-bit DAC + low-pass filter**
- outputting the sound of **raw network traffic**

So this is not an oscillator, sampler, or audio interface in the normal sense. It literally turns packet activity into audio.

## What the module does musically

The key sentence in the manual is essentially:

> any bit on the network will be sent to the audio output

That means your “melody” does not come from pitch CV going into a VCO. Instead, melody emerges from:

- the **timing** of packets
- the **size** of packets
- the **structure** of protocol headers
- the **payload data** being transmitted
- the **rate / density** of traffic on the link

In practice, this gives you a module that can produce:

- clicks
- pulses
- harsh digital tones
- noisy pitched bands
- rhythmic bursts
- repeatable patterns if the network traffic is controlled carefully

## Best ways to create melodic material

## 1. Use the included sequencer script as a pitch/rhythm source

The manual mentions a **sequencer/** folder containing a shell script that “mimics a sequencer by network pings of different size.”

This is probably the most direct melodic use.

### Why it works
Different ping packet sizes create different bit patterns and durations on the wire. Those become distinct audio events at the output. If you send them in a repeating order, you get a crude stepped note sequence.

### Patch idea
- NSA selector audio out → **VCA**
- VCA → **filter** or **wavefolder**
- trigger/gate source → VCA CV input
- optionally NSA selector → **clocked delay / reverb**

### Musical result
- packet sizes become “notes”
- repetition creates a sequence
- VCA gating can sharpen events into plucks
- filtering can emphasize certain resonances, making the sequence feel more tonal

### Performance tip
If you make several ping sizes correspond to several recognizable timbres, you can compose phrases by ordering those sizes like notes in a scale.

## 2. Convert WAV audio into the module’s native network format

The most explicitly melodic feature in the manual is the **upconverter/** tool. It converts a **mono 16-bit 48 kHz WAV** into a **4-bit 25 MHz .nsa file** using delta-sigma style conversion.

This is huge for melody, because it means you can prepare pitched material externally and then “play it” over the network.

### Why it works
Instead of hoping random traffic sounds musical, you intentionally encode:

- single notes
- scales
- arpeggios
- basslines
- melodies
- drones

Then transmit those files over the network so the NSA selector outputs them as audio.

### Strong melodic workflow
1. Create a simple melody in DAW or audio editor
2. Render as mono WAV
3. Convert to `.nsa`
4. Serve/transmit it over the network
5. Patch the output into your Eurorack system

### Patch ideas
- NSA selector → **low-pass filter** → VCA → mixer  
  for taming the harshness into a more playable lead

- NSA selector → **resonant band-pass filter**  
  to isolate partials that behave like a stable pitch center

- NSA selector → **quantizer is not needed on audio**, but use:
  - **envelope follower** from the audio
  - envelope follower CV → filter cutoff or VCA
  - this creates dynamic articulation from the traffic itself

### Musical result
This is your best route to actual recognizably melodic phrases. The quality is intentionally lo-fi and packet-corrupted, but that can sound beautiful in an industrial / glitch / electroacoustic context.

## 3. “Listen to images” for stepped or scanned pseudo-melodies

The manual says uncompressed, unencrypted **BMP** image transfers can be heard, effectively letting you “hear the pixels.”

### Why that matters melodically
Images are organized data. Repeated structures in an image can create:

- repeating frequency zones
- stepped transitions
- scan-like rises/falls
- motif-like bursts

A striped or patterned image can generate surprisingly sequence-like audio.

### Creative melodic trick
Design BMPs intentionally as “graphic scores”:

- horizontal stripes for repeated note-like bands
- diagonal lines for rising/falling gestures
- checkerboards for alternating intervals
- blocks of different brightness for phrase sections

Then transfer the BMP and process the result through your modular.

### Patch idea
- NSA selector → **slew-ish LPG or low-pass gate**
- then into **reverb**
- optionally layer with a tuned oscillator tracking the envelope of the output

This won’t produce equal-tempered notes directly, but it can generate melodic contours and motifs.

## 4. Use traffic saturation and retransmission as ornamentation

The manual notes that saturating the link introduces artifacts, retransmissions, and extra texture.

### Melodic interpretation
Think of this as ornament generation:

- retransmissions = repeats/flams
- congestion = distortion/smear
- header overhead = transient attack content
- link saturation = sustained noisy tone bed

So a clean encoded melody can become expressive when pushed into overload.

### Musical use
Start with a simple converted WAV melody, then:
- intentionally saturate the network
- add simultaneous traffic
- let the melody degrade into glitchy harmonization

This works especially well for:
- IDM
- noise-pop
- electro
- broken transmission ambient
- cyberpunk soundtrack textures

## 5. Create call-and-response with controlled and uncontrolled traffic

The module has two Ethernet jacks and forwards traffic unmodified while tapping it for audio.

That means you can create layers of musical behavior:
- **controlled traffic** = your intended melody
- **ambient traffic** = live counterpoint/noise layer

### Example setup
- one machine sends your `.nsa` melody or ping sequence
- another generates browsing, pings, tcpdump echo, file transfer, or game traffic

The output becomes a hybrid of:
- intentional notes
- accidental accompaniment

### Patch concept
- NSA selector out → **mult**
  - path 1 → dry mixer channel
  - path 2 → distortion/filter/delay

Use the dry channel for articulation and the processed channel for harmonic smear. This can make packet melodies feel bigger and more “composed.”

## 6. Use tcpdump “echo” as a primitive delay for melodic phrases

The manual describes a trick where dumping network traffic to console can effectively double the activity, creating a kind of **echo**.

### Musical use
This is especially useful for melodic phrasing.

If you transmit a short sequence or encoded note phrase, then add:
- `tcpdump -ni eth0`
- or more verbose variants

you can generate repeating or thickened events.

### Result
- short notes become doubled
- sparse phrases become denser
- repeated packet observation adds a primitive feedback feel

It is not tempo-locked delay in the Eurorack sense, but musically it behaves like:
- slapback
- stutter
- burst-repeat
- data haze

## How to combine it with typical Eurorack modules for melody

Because the NSA selector has only **audio out** and no CV inputs, the “using modules together” part is mostly about **what you patch after it**.

## Best companions

### Filter
A resonant filter is probably the most important partner.

Why:
- packet audio is bright and aggressive
- filtering can isolate stable spectral areas
- resonance can emphasize apparent pitch

Use:
- low-pass for smoother lead lines
- band-pass for vowel-like melodic tones
- high resonance for whistle-like digital notes

### VCA + envelope
Helps impose phrasing.

Use a gate source or trigger sequencer to:
- chop continuous network texture into note lengths
- accent certain events
- create rhythmic articulation independent of the traffic itself

### Low-pass gate
Excellent if you want the module to feel more “played” and less like a data stream.

### Delay / reverb
Turns fragmented packet events into melodic ambience.

Especially good for:
- sparse ping sequences
- image-data scans
- short `.nsa` note phrases

### Distortion / wavefolder
Can turn weakly pitched digital noise into richer lead or bass material.

### Envelope follower
A sleeper pairing. Derive CV from the audio amplitude and use it to modulate:
- filter cutoff
- VCA level
- another oscillator’s FM amount

That creates self-animated melodic movement from the network data itself.

### Pitch tracker or PLL-style module
If you have a pitch-tracking utility or PLL, you may be able to extract unstable but interesting pitch CV from the output and use that to drive another oscillator. That gives you:
- NSA selector = chaotic melodic source
- analog/digital VCO = stabilized harmonic shadow

## Practical melodic strategies

## Strategy A: Packet melody voice
- create ping-size sequence
- NSA selector out → filter → VCA → reverb
- use external trigger sequencer for articulation

This gives percussive, glitch-melodic phrases.

## Strategy B: Encoded lead line
- compose WAV melody
- convert to `.nsa`
- transmit file
- NSA selector → resonant filter → stereo FX

This is the clearest path to actual lead melodies.

## Strategy C: Image-score music
- create patterned BMP
- send it through the fileserver setup
- NSA selector → band-pass filter → delay

This gives scanning, abstract melodic contours.

## Strategy D: Dual-layer data harmony
- send `.nsa` melody
- simultaneously add web/file/ping traffic
- output → mult
- one clean, one heavily processed

This creates melody plus noisy accompaniment from the same source.

## What kind of melodies this module is best at

This module is best for:

- **glitch melodies**
- **lo-fi digital leads**
- **harsh arpeggios**
- **rhythmic data motifs**
- **industrial bleeps**
- **cybernetic drones with melodic contour**
- **corrupted sample-like phrases**

It is less suited for:
- clean tonal melodies
- precise 1V/oct playing
- traditional keyboard-style performance
- harmonically pure subtractive synthesis

## Overall musical assessment

The NSA selector is basically a **network sonification voice**. To get melodic results, the trick is to stop thinking like “pitch CV into oscillator” and instead think:

- **packet design = composition**
- **traffic structure = sequencing**
- **network load = timbre**
- **modular processing = articulation and tonal focus**

If I were building a melodic patch around it, my first choice would be:

1. generate a simple `.nsa` phrase from a WAV melody
2. run the output through a resonant filter and VCA
3. add clocked delay/reverb
4. layer with a more stable oscillator for pitch reinforcement

That would give the best mix of:
- recognizable melody
- packet grit
- playable modular dynamics

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)