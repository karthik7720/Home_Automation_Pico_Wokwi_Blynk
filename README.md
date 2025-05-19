**Home Automation Project**

This repository contains the implementation of a comprehensive Home Automation system using both hardware and virtual simulation. The project is divided into two main parts:

1. **Hardware Implementation:**
   - Components: Raspberry Pi Pico, 4-channel relay module, HC-05 Bluetooth module, and 4 lamps.
   - Control: Custom mobile app developed using MIT App Inventor for controlling the relays via Bluetooth.
     
     
![IMG-20240310-WA0002](https://github.com/user-attachments/assets/f9e106f5-790c-43bb-8935-c5824cdec2eb)




2. **Simulation in Wokwi:**
   - Components: ESP32, relay modules with LEDs, push buttons, 16x2 LCD display.
   - Control: Blynk IoT platform is used to control relay 0, and push buttons are used to control other relays.
     

![Screenshot 2024-03-20 005019](https://github.com/user-attachments/assets/da34d078-9414-4610-909c-0d1d24446df3)

![image](https://github.com/user-attachments/assets/25274aaa-8425-49be-8e39-0c519bc5ece4)


**Hardware Implementation:**

**1. Upload the Code:**

1.1. Open the Thonny IDE on your computer.

1.2. Connect the Raspberry Pi Pico via USB.

1.3. Open the main.ino file in Thonny.

1.4. Ensure the correct COM port is selected in the Thonny settings.

1.5. Click on the Run button to upload the code to the Pico.

**2. Connect Hardware Components:**

2.1. Follow the wiring diagram to connect the hardware components to the Pico:

     2.11. Connect the 4-channel relay module to the Pico GPIO pins as specified in the diagram.

     2.12. Connect the HC-05 Bluetooth module to the Pico for wireless communication.

     2.13. Connect the lamps or other loads to the relay module.

2.2. Double-check connections to prevent short circuits and ensure correct power ratings.

**3. Control via MIT App Inventor App:**

3.1. Open the custom-built mobile app in MIT App Inventor on your smartphone.

3.2. Turn on the Bluetooth module and connect it to the HC-05.

3.3. Once connected, you can control each relay through the app interface.

**Simulation Implementation:**

**1. Open Wokwi Simulator:**

1.1. Visit the Wokwi Simulator.

1.2. Create a new project and import the circuit diagram.

1.3. Arrange components as per the provided wiring diagram:

     1.3.1 ESP32, relay modules (with LEDs), push buttons, and a 16x2 LCD.

**2. Setup Blynk IoT Platform:**

2.1. Register for an account on the Blynk IoT Platform at https://blynk.io/.

2.2. Create a new project and add virtual switches for each relay.

2.3. Copy the following details from the project setup:

      2.3.1 BLYNK_TEMPLATE_ID

      2.3.2 BLYNK_TEMPLATE_NAME

      2.3.3 BLYNK_AUTH_TOKEN

2.4. Paste these values into the main.py code in the Wokwi simulation.

**3. Configure the Web Dashboard:**

3.1. In the Blynk web interface, create a dashboard.

3.2. Add switches and link them to the corresponding virtual pins defined in the code.

**4. Control Relays via Blynk App:**

4.1. Download and install the Blynk IoT App on your smartphone.

4.2. Log in using your Blynk account credentials.

4.3. Select the project and control the relays using the virtual switches.

4.4. The push buttons in the simulation also control the relays, and the relay status is reflected on the Blynk app in real time.
