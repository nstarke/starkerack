# Rebel Technology — Stoicheia

- [Manual PDF](../../manuals/Stoicheia – Rebel Technology.pdf)

---

**[Stoicheia (Στοιχεῖα) Eurorack Module Manual](https://www.rebeltech.org/product/stoicheia/)**

---

# **Stoicheia: Concise Cheat Sheet**

## **Quick Start**
- **Connect Clock IN A/B:** Plug an LFO or clock into the left/right bottom jack(s).
- **Connect OUT A/B:** Connect left/right OUT jack to your drum or gate-enabled modules.
- **Middle Switch (both rows):** Center for OFF, UP for Trigger, DOWN for Alternating (see Modes).
- **Set Knobs:**
  - Bottom: Fills (# of gates per pattern, CCW=1, Center=50%, CW=all)
  - Middle: Length (steps, 1–16, center=8)
  - Top: Rotation (start position; left/right rotates sequence)

---

## **Panel Controls**

### **Jacks**
- **OUT A/B (top left/right jacks):** Rhythmic gate outputs
  - Low: 0V, High: 5.1V
  - Impedance: < 1.1kΩ
- **RESET (middle jack):** Trigger resets *both* sequences to their start position.
  - Input: > 100kΩ  
- **CLOCK A/B IN (bottom left/right):**  Clock/trigger for left/right sequence.
  - Input: > 100kΩ

### **Knobs (each sequence, left/right columns)**
1. **Top (Rotation):** Step offset/rotation of sequence start
2. **Middle (Length):** 1–16 steps, center=8
3. **Bottom (Fills):** Number of "on" steps (gates), 1–length, center=half, CW=max

### **Switches**
- **Sequence Switch (each sequence, 3-way):**
  - **UP:** Trigger mode—output follows input clock edges, pulse width matches clock
  - **CENTER:** Off
  - **DOWN:** Alternating/Tied mode—output toggles, holding high until next on-beat
- **Chained Mode:** Center switch down enables chaining (A then B, outputs merged)

---

## **Modes**
- **Trigger Mode:** Gate outputs follow the input clock width (UP position)
- **Alternating Mode:** Output toggles on each on-beat (DOWN position)
- **Chained Mode:** Both sequences run consecutively (via center switch DOWN)

---

## **Patterns**
- **E(x,y):** x fills, y steps, auto-Euclidean distribution
  - Example: E(3,4) = [x . x x] (Calypso)
  - E(2,5): [x . x . .] (Take Five, Tchaikovsky)
  - E(5,8): [x . x x . x x .] (Cuban cinquillo, Persian)
  - E(7,12): [x . x x . x x . x . x .]
  - E(9,16): [x . x x . x . x x . x . x . x .]

---

## **Voltage/Current Specs**
- **Power:** +12V <10mA, +5V <25mA, -12V 0mA
- **Output range:** 0V (low), 5.1V (high)

---

## **Reference**
- [Official Manual](https://www.rebeltech.org/product/stoicheia/)
- [Euclidean Patterns Paper by Toussaint (PDF)](http://cgm.cs.mcgill.ca/~godfried/publications/banff.pdf)
- [All source & schematic on Github](https://github.com/pingdynasty/EuclideanSequencer)

---

## **Hacking / Open Hardware**
- **MCU:** ATMega168 (Arduino bootloader, FTDI compatible)
- **Firmware:** Open source, [see repo](https://github.com/pingdynasty/EuclideanSequencer)

---

**Generated With [Eurorack Processor](https://github.com/nstarke/eurorack-processor)**
