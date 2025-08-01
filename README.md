# 🔔 Quiz-Buzzer-System
A digital logic–based buzzer system that latches and displays the first of four buzzer presses using D flip-flops, AND gates, a 7447 BCD-to-7-segment decoder, and a 7-segment display. Upon the first button press, the system locks out subsequent inputs until reset and shows the corresponding player number (1, 2, 4, or 8) on the display.

---

## ⚙️ How It Works

1. Each player's buzzer is connected to a D flip-flop.
2. When a player presses the buzzer:
   - Their corresponding flip-flop latches the input.
   - An AND gate ensures only the first press is acknowledged.
3. The latched output (binary) is sent to a 7447 decoder.
4. The decoder converts it to drive the 7-segment display.
5. A reset button clears all flip-flops to begin a new round.

The displayed output will be:
- `1` for Player 1
- `2` for Player 2
- `4` for Player 3
- `8` for Player 4

These values represent binary encoding (0001, 0010, 0100, 1000)


## 🛠️ Tools & Components Used

- D Flip-Flops (74LS74 or similar)
- AND Gates (74LS08)
- BCD to 7-Segment Decoder (7447)
- Common Anode 7-Segment Display
- Push Buttons (4 – one per team)
- Reset Button
- Power Supply (5V DC)
- Breadboard or PCB
- Connecting wires

---

## 🧠 Skills & Concepts Applied

- Digital Electronics
- Circuit Design

---

## 📁 Project Files

| File Name            | Description                                    |
|---------------------|------------------------------------------------|
| `CircuitDiagram.pdf`| Schematic of the buzzer system (logic gates + decoder) |
| `README.md`         | Project documentation                          |
| `TruthTable.txt`    | Truth table and working logic                  |
| `ComponentsList.txt`| List of components used                        |
| `Simulation.circ`   | (Optional) Logisim or Digital Simulator File   |

---

## 🚀 Future Improvements

- Add sound indicators (buzzers) for the first responder.
- Expand to support more than 4 players.
- Add microcontroller-based scoring and automatic reset.
- Use LEDs to show lock status or team activation.
- Implement wireless buzzers using RF modules.

---
