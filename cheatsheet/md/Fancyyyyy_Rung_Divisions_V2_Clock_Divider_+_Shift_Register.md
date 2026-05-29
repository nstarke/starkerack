# Fancyyyyy — Rung Divisions V2 Clock Divider + Shift Register

- [Manual PDF](../../manuals/RungDivisionsManual.pdf)

---

[Manual PDF](attachment)

# Fancyyyyy Rung Divisions — Cheat Sheet

## What it does
A **clock divider + dual gate bus + universal shift register + noise source**.  
Best thought of as a **polyrhythmic gate generator** that also creates **looping / random stepped CV** and can run from **sub-audio up to audio rate**.

Core idea:
- **Clock input** feeds **/2 to /8 dividers**
- Divider outputs are assigned to **Bus1** or **Bus2** with switches
- **Bus1 clocks the shift register**
- **Data input + chance/length/direction logic** determine what enters the shift register
- Shift register produces:
  - **1-Bit gate**
  - **3-Bit CV**
  - **8-Bit CV**

---

## Quick start
1. Set **Length = 8**
2. Set **Chance fully CCW**
3. Put all divider **bus switches to center**
4. Patch a clock to **Clock**
5. Send one divider output, or Clock itself, to **Bus1** using its switch
6. Patch something to **Data** (or use manual write switch)
7. Listen to:
   - **Bus1/Bus2** for gates/polyrhythms
   - **1-Bit** for a gate tied to the register
   - **3-Bit / 8-Bit** for stepped CV
8. Turn **Chance fully CW** to **freeze/loop** the current pattern
9. Press **Direction** or patch a trigger to reverse read direction
10. Modulate **Length**, **Chance**, and **Direction** for evolving patterns

---

## Main behavior
### Clock divider
- Incoming **Clock** is converted to pulses when signal crosses **1V**
- Generates integer divisions: **/2, /3, /4, /5, /6, /7, /8**
- Divider section works from **0–40 kHz**
- **Reset** rising edge resets all counts

### Bus system
- Each divider (and Clock) can be routed by a **3-position switch**:
  - **Left = Bus1**
  - **Center = off**
  - **Right = Bus2**
- **Bus outputs are OR mixes**
- **Bus1 clocks the shift register**

### Shift register
- Universal shift register can read in **either direction**
- **Direction** can be changed by:
  - front panel **button**
  - external **Direction trigger/gate**
- **Length** sets loop point
- **Chance** blends between:
  - **new data**
  - **looped data**
  - **noisy/interference behavior**
- At **Chance fully CW**, the pattern **loops/locks**
- At **Chance fully CCW**, incoming data is XOR’d with internal loop-point logic

---

## Performance tips
- **Simple looping sequence**: write in bits manually, then set **Chance full CW**
- **Pseudo-random sequence**: feed pulses/noise/data into **Data**, set **Chance around middle**
- **Polyrhythms**: mix non-related divisions on **Bus1/Bus2** like **/2 + /5** or **/3 + /7**
- **Audio-rate use**:
  - use divider outputs as subharmonics
  - use **3-Bit / 8-Bit** as digital/noise oscillator CV/audio
- **Chaos patch**:
  - patch **3-Bit** or **8-Bit** back to clock oscillator FM/CV
  - **3-Bit** = more bursty
  - **8-Bit** = more random/strange attractor-like

---

## Controls reference

### Knobs
- **Length**
  - Sets shift register loop length / loop point
  - CV is summed with knob
- **Chance**
  - Sets probability/amount of new data vs looping data
  - Fully CW = loop/hold pattern
  - Fully CCW = stronger influence from external data/XOR logic
  - CV is summed with knob

### Button / switch
- **Direction button**
  - Reverses shift register read direction
- **Data write switch (High / Low)**
  - Manually writes high or low data into the register

### Divider bus switches
For **Clock, /2, /3, /4, /5, /6, /7, /8**:
- **Left** → send to **Bus1**
- **Center** → disconnected
- **Right** → send to **Bus2**

### LEDs
- **8 shift register status LEDs**
  - Show current register bit states

### Rear trimmer
- **Chance trim-pot**
  - Sets response of Chance knob/CV
  - Factory calibrated; usually leave alone

---

## Jack reference

## Inputs
| Jack | Type | Voltage / Threshold | Function |
|---|---|---:|---|
| **Clock** | Gate/clock input | accepts any signal crossing **1V** | Master clock for divider |
| **Reset** | Gate/trigger input | rising edge, **700 mV minimum** | Resets divider counts |
| **Data** | Gate/data input | accepts any signal crossing **1V** | External data source for shift register |
| **Direction** | Gate/trigger input | rising edge, **700 mV minimum** | Reverses shift register direction |
| **Length CV** | CV input | **±5V** summed with knob | Modulates loop point/length |
| **Chance CV** | CV input | **±5V** summed with knob | Modulates chance/loop behavior |

## Outputs
| Jack | Type | Voltage Range | Function |
|---|---|---:|---|
| **/2** | Gate output | **0–7V** | Clock divided by 2 |
| **/3** | Gate output | **0–7V** | Clock divided by 3 |
| **/4** | Gate output | **0–7V** | Clock divided by 4 |
| **/5** | Gate output | **0–7V** | Clock divided by 5 |
| **/6** | Gate output | **0–7V** | Clock divided by 6 |
| **/7** | Gate output | **0–7V** | Clock divided by 7 |
| **/8** | Gate output | **0–7V** | Clock divided by 8 |
| **Bus1** | Gate bus output | **0–7V** | OR mix of sources assigned left; also clocks shift register |
| **Bus2** | Gate bus output | **0–7V** | OR mix of sources assigned right |
| **Noise** | Analog noise output | not specified in manual | Noise source |
| **1-Bit** | Gate output | **0–7V** | Gate from first register bit; tracks clock pulse width |
| **3-Bit** | CV output | **±5V** | 3-bit DAC CV, reverse-encoded |
| **8-Bit** | CV output | **±5V** | 8-bit DAC CV, reverse-encoded |

---

## Useful patch recipes

### 1. Basic polyrhythm generator
- Patch clock into **Clock**
- Send **/3** and **/5** to **Bus1**
- Send **/2** and **/7** to **Bus2**
- Use **Bus1** and **Bus2** as two related but different rhythm streams

### 2. Looping stepped CV
- Clock to **Clock**
- Send one division to **Bus1**
- Manually write a few highs using the **Data write switch**
- Set **Chance fully CW**
- Take melody CV from **8-Bit** or **3-Bit**

### 3. Pseudo-random rungler style
- Clock to **Clock**
- Send a division to **Bus1**
- Patch **Noise** or another pulse source to **Data**
- Set **Chance** around noon
- Use **3-Bit** for melodic CV and **1-Bit** for gate/accent

### 4. Evolving sequence length
- Patch slow CV to **Length CV**
- Keep **Chance high**
- Flip **Direction** occasionally
- Produces phrases that appear to reverse or fold

### 5. Audio-rate digital chaos
- Audio oscillator/square into **Clock**
- Patch **8-Bit** back to oscillator FM
- Use **Chance** to tune the amount of chaos
- Monitor **3-Bit**, **8-Bit**, or bus outputs as audio

---

## Important notes
- **Bus1 is the shift register clock**
- Mixing divisions with common factors may have little effect on the bus pattern
- Prime divisions like **/5** and **/7** create more shifting/interference-like rhythms
- Changing **Length** can “lose” stored bits if data has already passed the new loop point
- All major timing functions can operate at **audio rate**

---

## Specs
- **Width:** 12 hp
- **Depth:** 32 mm
- **Power:** +12V **58 mA**, -12V **42 mA**
- **CV outputs:** **±5V**
- **Gate outputs:** **0–7V**
- **Clock/Data input sensitivity:** any signal crossing **1V**
- **Reset/Direction trigger sensitivity:** rising edge, **700 mV minimum**
- **Length/Chance CV inputs:** **±5V** added to knob position

---

## Installation / calibration
- Connect power only to the header labeled **POWER**
- Ribbon cable **red stripe faces down**
- Module has reverse power protection
- Chance trim calibration procedure:
  - send **audio-rate clock** into **Clock**
  - monitor **8-Bit**
  - set **Chance fully CW**
  - adjust trim until pattern no longer changes

---

[Generated With Eurorack Processor](https://github.com/nstarke/eurorack-processor)