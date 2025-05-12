   Face Recognition using ESP32-CAM

This project implements a face recognition the ESP32-CAM module. The system captures facial images and recognizes individuals to mark their attendance automatically. It leverages OpenCV and Visual Studio for face recognition processing.

key Features

- **ESP32-CAM Integration**: Captures images upon detecting a face.
- **OpenCV & Visual Studio**: Processes images for face recognition.
- **Automated Attendance Logging**: Marks attendance for recognized individuals.
- **Real-time Monitoring**: Provides immediate feedback on recognition status.



Hardware used :
  - ESP32-CAM Module
  - FTDI Programmer
  - Jumper Wires
  - Power Supply

Software used :
  - Arduino IDE
  - OpenCV Library
  - Visual Studio



 1. Hardware Setup

- Connect the ESP32-CAM module to your computer using the FTDI programmer.
- Ensure proper connections:
  - **U0R** to **TX**
  - **U0T** to **RX**
  - **GND** to **GND**
  - **5V** to **VCC**

 2. Arduino Configuration

- Open the `esp32cam_face_recognition.ino` file in Arduino IDE.
- Select the appropriate board and port:
  - **Board**: AI Thinker ESP32-CAM
  - **Port**: COM port corresponding to your device
- Upload the code to the ESP32-CAM module.
- 
 3. OpenCV & Visual Studio Setup

- Install OpenCV library and configure it with Visual Studio.
- Open the `face_recognition.py` script in Visual Studio.
- Run the script to start the face recognition process.

 4. Operation

- The ESP32-CAM captures an image when a face is detected.
- The image is sent to the computer where OpenCV processes it.
- If the face matches a registered individual, attendance is marked in `attendance_log.csv`.

 📸 Screenshots
![Screenshot 2025-04-23 113914](https://github.com/user-attachments/assets/a9b29955-5126-4ffd-94f0-7c42027b579b)

![Screenshot 2025-04-23 191133](https://github.com/user-attachments/assets/d7bb7803-0d9b-4ecb-806b-6bbd5e838cce)


- Inspired by the tutorial from [How2Electronics](https://how2electronics.com/face-recognition-based-attendance-system-using-esp32-cam/).


