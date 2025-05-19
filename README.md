# Home Automation Project

This repository contains the implementation of a comprehensive Home Automation system using both hardware and virtual simulation. The project is divided into two main parts:

1. **Hardware Implementation:**
   - Components: Raspberry Pi Pico, 4-channel relay module, HC-05 Bluetooth module, and 4 lamps.
   - Control: Custom mobile app developed using MIT App Inventor for controlling the relays via Bluetooth.
![IMG-20240310-WA0002](https://github.com/user-attachments/assets/f9e106f5-790c-43bb-8935-c5824cdec2eb)



    

2. **Simulation in Wokwi:**
   - Components: ESP32, relay modules with LEDs, push buttons, 16x2 LCD display.
   - Control: Blynk IoT platform is used to control relay 0, and push buttons are used to control other relays.

## Project Structure:

HomeAutomation_Project/
│── Hardware/
│   ├── MIT_App_Inventor/
│   │   └── HomeAutomation.aia
│   └── Raspberry_Pi_Pico/
│       ├── main.ino
│       └── README.md
│
│── Simulation/
│   └── Wokwi/
│       ├── main.ino
│       ├── Wokwi_Simulation.json
│       └── README.md
│
│── LICENSE
│── README.md
```

## How to Run:
- **Hardware:**
  - Upload the `main.ino` file to the Raspberry Pi Pico using the Arduino IDE or Thonny.
  - Connect the hardware components as per the wiring diagram in the `README.md` file under `Hardware/Raspberry_Pi_Pico`.
  - Open the MIT App Inventor app, connect via Bluetooth to the HC-05 module, and control the relays.

- **Simulation:**
  - Open the Wokwi simulation using the provided `Wokwi_Simulation.json` file.
  - Upload the `main.ino` file to the ESP32 in Wokwi.
  - Control relay 0 via the Blynk IoT app. Push buttons operate relays simultaneously and the status is displayed on the Blynk IoT app..

## License:
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Contributions:
Feel free to fork this repository, open issues, and submit pull requests for improvements and bug fixes.
