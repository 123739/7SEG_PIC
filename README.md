# 7-Segment Display Using PIC18F4520
This project demonstrates how to interface a 7-segment display with the PIC18F4520 microcontroller. The microcontroller is programmed in C using MPLAB X and the XC8 compiler. The display shows digits from **0 to 9 sequentially**, with appropriate delays, using direct port manipulation.

## Tools & Components Used
- **Microcontroller**: PIC18F4520  
- **Compiler**: MPLAB X IDE with XC8  
- **Simulation**: Proteus (optional)  
- **Display**: 7-Segment Display (Common Cathode/Anode – specify if needed)  
- **Other**: Resistors, Breadboard (if hardware), Connecting Wires

## Key Concepts Covered
- Interfacing 7-segment displays
- Port configuration and bitwise operations
- Timing and delay functions
- Embedded C programming for PIC

## Project Structure
├── 7SEG.c (Source code in MPLAB X)
├── 7SEG_PIC_simulation.mp4 (Circuit simulation)
├── 7SEG_PIC.pdsprj (Proteus file)

## How It Works
Each digit from 0–9 is displayed one at a time by sending the corresponding binary pattern to the output port connected to the 7-segment display. A delay is added between updates to make each number visible to the eye.

If you're using a **common cathode display**, the logic HIGH turns ON the corresponding segment. For **common anode**, the logic is inverted.

## How to Run
1. Clone or download the project.
2. Open `main.c` in MPLAB X.
3. Compile using the XC8 compiler.
4. Load the hex file into Proteus or upload to your PIC18F4520 setup.
5. Observe the 7-segment display counting from 0 to 9 in a loop.

## Notes
- Make sure your PORT direction is set correctly (`TRISx` registers).
- Adjust delay functions if running on actual hardware vs simulation.
- You can modify the digit patterns in `main.c` to display custom sequences.
