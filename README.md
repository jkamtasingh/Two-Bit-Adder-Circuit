# Two-Bit-Adder-Circuit
Used to perform binary addition of two 2 bit numbers, the fundamental part of the Arithmetic Logic Unit within microprocessors.

# Technologies Used
- 3x Red LEDs
- 3x 330Ω Resistors
- 4x 1kΩ Resistors
- 1x 4-Way DIP Switch 
- 1x 74HC86N IC (XOR IC)
- 1x 74HC08N IC (AND IC)
- 1x 74HC32N IC (OR IC)
- Jumper Wires
- Circuitverse software (used to visualize the logic gates on the circuit)

# Features
- The two bit adder circuit accepts two 2-bit binary numbers
  - In my example, the DIP Switch are these inputs: 1 -> B1, 2 -> A1, 3 -> B0, 4 -> A0.
- The Red LEDs produce a 3 bit sum output
  - With my circuit, by reading the LEDs from left to right, the outputs are: Q1, Q0, CO.

# How It Works
The 2-bit adder is built from two stages:
- Bit 0 (Half Adder): A0 and B0 are combined using an XOR gate (produces the sum bit Q0) and an AND gate (produces an internal carry).
- Bit 1 (Full Adder): A1 and B1 must also account for the internal carry generated from bit 0. This stage uses two XOR gates, two AND gates, and an OR gate to produce the sum bit Q1 and the final carry-out, CO.

The internal carry generated from the bit 0 stage feeds directly into the bit 1 stage, allowing the circuit to correctly "carry the 1" the same way you would by hand in decimal addition. The final output is a 3-bit result (Q1, Q0, CO) representing the sum of the two 2-bit binary numbers.

# The Process
To begin, the Circuitverse software was used to combine both a half adder and full adder circuit into a two bit adder circuit.
<img width="1289" height="921" alt="Image" src="https://github.com/user-attachments/assets/6441974d-5263-4dad-8b87-78924a6155b4" />

By using Circuitverse, I was able to visualize where the logic gates will connect together with their respective ICs on the breadboard. 

Next, I recreated the logic gate circuit on a breadboard, using the DIP Switch as the inputs and Red LEDs as outputs. 
<img width="1703" height="1277" alt="Image" src="https://github.com/user-attachments/assets/6c832511-b471-4210-a56b-9a164533640e" />

The finished breadboard circuit is a fully working two bit adder circuit.

# What I learned
Through this project, I learned the important context behind binary addition, reinforced my knowledge with circuit software and familiarized myself with integrated chips. 

# Future Improvements
- As the project is fully functional, my only physical improvement would be cleaning up the wiring on the breadboard.
- I can continue to experiment with two bit adders and find different use cases for them.

# Video Demonstration 
https://github.com/user-attachments/assets/565a40d8-182b-493c-aaf6-6be16f198d36
