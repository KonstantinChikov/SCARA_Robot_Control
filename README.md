# README for SCARA Robot Control GUI

This project provides a GUI for controlling a SCARA robot using Processing and Arduino. Below are the instructions to set up and run the system.

---

## **1. Install Required Software**

### **Processing IDE**
- Download and install the [Processing IDE](https://processing.org/).
- Use the Processing IDE to run the `.pde` GUI file.

### **Arduino IDE**
- Ensure the Arduino IDE is installed.
- Upload the SCARA robot’s Arduino code to the microcontroller.

---

## **2. Install Required Libraries**

1. Open the Processing IDE.
2. Navigate to `Sketch > Import Library > Add Library...`.
3. Search for and install the following:
   - **ControlP5**: A library for GUI elements in Processing.
   - **Serial**: This library is included by default in Processing.

---

## **3. Prepare Your Hardware**

### **Connect Your SCARA Robot**
- Connect the Arduino board to your PC via USB.

### **Identify the COM Port**
- Open the Arduino IDE.
- Navigate to `Tools > Port` and note the connected port (e.g., `COM3` or `/dev/ttyUSB0`).

---

## **4. Configure the GUI Code**

1. Open the `.pde` file in the Processing IDE.
2. Locate the line where the serial port is initialized:
   ```java
   myPort = new Serial(this, "COMx", 115200);
   ```
3. Replace `COMx` with your Arduino’s COM port (e.g., `COM3`).
4. Save the file.

