# E-BIN: A Smart Garbage System

## Project Overview
E-BIN is a smart waste monitoring and control system designed to enhance waste management in urban environments. By integrating a microcontroller-based system with sensors, LEDs, a buzzer, and an LCD display, E-BIN aims to provide real-time status updates on waste bin levels, promoting efficient waste collection and environmental sustainability.

## Features
- Utilizes **LPC2138** microcontroller for efficient monitoring and control.
- Equipped with **LEDs**, **buzzer**, and **LCD** to provide intuitive feedback on bin status.
- Clear status indications:
  - **Green LED** - Bin is empty
  - **Orange LED** - Bin is nearly full
  - **Red LED + Buzzer** - Bin is full
- Efficiently coded in **Keil uVision4** and simulated in **Proteus**.

## Components Used
- **LPC2138 Microcontroller**
- **LM016L LCD Display**
- **UART Communication Interface**
- **SPST Push Button**
- **Buzzer**
- **LED Indicators**

## Installation Instructions
1. Install **Keil uVision4** IDE and **Proteus** simulator.
2. Clone the repository from GitHub:
   ```bash
   git clone <repository-url>
   ```
3. Open the project file in Keil uVision4.
4. Compile the code and upload it to the LPC2138 microcontroller.
5. Use Proteus to simulate the circuit for testing purposes.

## Code Structure
- **main.c** - Core logic for monitoring and controlling the bin status.
- **lcd.c** - Contains functions for LCD initialization, command execution, and data display.
- **delay.c** - Implements delay functions for timing control.

## Algorithm
1. Initialize hardware components.
2. Initialize the LCD display.
3. Enter an infinite loop for continuous bin status monitoring.
4. For each bin:
   - Display the bin's status on the LCD.
   - Activate LEDs and buzzer accordingly based on the bin's fill level.
5. Introduce a delay to ensure the monitoring loop functions effectively.

## Simulation and Testing
- **Empty Bin:** Displays "EMPTY" with a blinking **Green LED**.
- **Nearly Full Bin:** Displays "NEARLY FULL" with a blinking **Orange LED**.
- **Full Bin:** Displays "FULL" with a blinking **Red LED** and an active **Buzzer**.

## Future Improvements
- Integration of solar panels to power the system for improved sustainability.
- Enhanced communication protocols for remote monitoring capabilities.

## Authors
- **C H Keerthi Vardhan** 
- **D Harsha Vardhan** 
- **L Likhitha Ram** 
- **N Maneeswar Reddy** 

## Faculty Incharge
**C B Rajesh**

## License
This project is licensed under the [MIT License](LICENSE).

## References
- Steve Furber, "ARM System On Chip Architecture," Addison Wesley, 2000.
- [LCD Module Information](https://embeddedcenter.wordpress.com/ece-study-centre/display-module/lcd-16x2-lm016l/)
- [LPC2138 Datasheet](https://www.nxp.com/docs/en/data-sheet/LPC2131_32_34_36_38.pdf)

