# 7 Segments Decoder
![Logic](https://img.shields.io/badge/Logic-Discrete%20ICs-blue?style=flat-square)
![Input](https://img.shields.io/badge/Input-4--bit%20DIP%20Switch-orange?style=flat-square)
![No MCU](https://img.shields.io/badge/No-Microcontroller-red?style=flat-square)
![Open Hardware](https://img.shields.io/badge/Open-Hardware-brightgreen?style=flat-square)

A binary-to-7-segment display decoder built entirely from discrete (and, or, not) logic ICs, no microcontroller, no shortcuts.
---
## How it works
A 4-bit Dip Switch provides a binary number (0–9) to the circuit. The logic then decodes that binary input into the 7 individual segment signals (a–g) that are required to display the correct digit.
## What I learned 
This was one of those projects where you think "how hard can it be? and then spend hours staring at a breadboard full of wires with a multimeter in hand.
The biggest challenge wasn't the logic itself - it was debugging a circuit with this many interconnections and keeping track of which goes where while working on it. 
While working, I decided to **write every connection down on paper as you go**. After it worked for a second and then died, I learned about **floating pins** logic ICs switch so fast that any unconnected input picks up noise and causes random behavior. filling all unused inputs to a defined voltage level fixed it.
## pics
| schema | ICs |
| - | - |
| <img width="447" height="833" alt="image" src="https://github.com/user-attachments/assets/88efa22a-9e7a-49ac-bbae-6ab1723e955f" /> | <img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/4fbd9924-dc8d-43fe-8081-6b0a51e29099" /> |

## BOM
|Part | quantity |
| - | - |
|7-segment display | 1 |
|NOT gate IC (74LS04 or simular) | 1 |
|AND gate IC (74LS08 or simular) | 3 |
|quad input OR gate IC (74LS32 or simular) | 4 |
|4-bit DIP switch | 1 |
|Resistors | 7 |
|Breadboard | 1 |
|Jumper wires | alot |
|5V power supply or powerbank | 1 |

## Tools
- [Logisim Evolution](https://github.com/logisim-evolution/logisim-evolution) - truth table and K-map simplification and logic calculating and simplifying.
- multimeter - testing and debugging
- tweezers - so useful with the small wires
