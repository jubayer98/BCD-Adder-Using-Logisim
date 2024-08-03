# BCD Adder Using Logisim

This repository contains the design and simulation of a BCD (Binary-Coded Decimal) adder circuit using Logisim. BCD is a class of binary encodings of decimal numbers where each decimal digit is represented by a fixed number of binary digits, usually four or eight.

## Overview

A BCD adder is a circuit that adds two BCD numbers and produces a BCD result. The BCD adder handles each decimal digit separately and ensures that the sum of each digit pair does not exceed 9 (which is the highest digit in BCD).

## Features

- **BCD Addition Logic**: The circuit includes the logic to handle the addition of two BCD digits.
- **Correction Logic**: When the sum of two digits exceeds 9, the circuit adds 6 (0110) to the result to correct it.
- **Carry Handling**: The circuit correctly handles carries between decimal digits.

## Components

The BCD adder is constructed using the following components in Logisim:

- **4-Bit Binary Adders**: To add the binary representations of the BCD digits.
- **AND, OR, and NOT Gates**: To implement the correction logic.
- **Multiplexers**: To select the correct sum and carry outputs based on the correction logic.

## Design Steps

1. **Basic 4-Bit Adder**: Create a basic 4-bit binary adder using Logisim to handle the addition of two 4-bit numbers.
2. **BCD Correction Logic**: Implement the correction logic to handle cases where the sum of two BCD digits exceeds 9.
3. **Carry Logic**: Add logic to handle the carry out from the addition of two BCD digits.
4. **Simulation**: Simulate the BCD adder circuit in Logisim to verify its functionality with various inputs.

## Simulation

The Logisim project file (`BCDadderCircuit.circ`) contains the complete design and can be used to simulate the BCD adder. The simulation allows you to input BCD numbers and observe the output sum and carry.

## Getting Started

### Prerequisites

- **Logisim**: Download and install Logisim from the [official website](http://www.cburch.com/logisim/).

### Running the Simulation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/jubayer98/BCD-Adder-Using-Logisim.git
   cd BCD-Adder-Using-Logisim
   ```

2. **Open the Project**:
   - Launch Logisim.
   - Open the `BCDadderCircuit.circ` file in Logisim.

3. **Simulate**:
   - Use the input pins to enter BCD numbers.
   - Observe the output sum and carry to verify the correct operation of the BCD adder.

## Usage Example

1. **Input**: BCD numbers `0101` (5) and `0110` (6).
2. **Output**: Sum `0001` (1) with carry `0001` (carry of 1), resulting in `11` (correct BCD result for 5 + 6).

## Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to fork the repository, make your changes, and submit a pull request.

---

Enjoy designing and simulating the BCD adder using Logisim!
