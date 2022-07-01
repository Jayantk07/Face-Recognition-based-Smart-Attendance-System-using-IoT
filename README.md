# Face-Recognition-based-Smart-Attendance-System-using-IoT
Face Recognition using ESP-32 Camera Module and OpenCV 

Clone the project to your localhost and extract the files.

Download and install the latest version of Arduino Software from https://www.arduino.cc/en/software


### Arduino Setup

Open the CameraWebServer1.ino file from the Arduino folder using the Arduino Software application.

Perform the following steps:

  1. Click on File -> Preferences
  2. Copy and paste the following links under the Additional Board Managers URL - ```https://dl.espressif.com/dl/package_esp32_index.json``` & ```https://arduino.esp8266.com/stable/package_esp8266com_index.json```
  3. Under Tools option, Select the ```"AI Thinker ESP32-CAM"``` board under the ESP32 Arduino board.
  4. CPU Frequency - 240MHz
  5. Flash Frequency - 80MHz
  6. Flash Mode - QIO
  7. Partition Scheme - Huge App 3mb
  Leave rest all the same.

  Connect the Arduino Uno board or the FTDI Module to your PC.
  Using the following circuit diagrams, connect your Arduino Uno or the FTDI module with your ESP32 Cam Module.
  <div>
  <img>
  </img>
  <div>

  Within the code, change the ssid and password with the username and password of the wifi you are connected on.
  Save the code and upload it. 

  In the terminal below, you will see initialisation and uploading of code percentage. Once it reaches 100%, disconnect the inter-connected INO and GND wire from each other and press the reset button on the Cam Module.

  Open the Serial Monitor at 115200 Port.

  The Cam Module is initialised and ready to use with the URL provided in the Serial monitor.
  
### Python file

  Open the Attendance.py file and update the camera url with the one you got above.
  Upload your image in the img_fol folder with your name.
  Run the python file and the name will start displaying below in the terminal whenever your face is detected by the camera, hence marking the Attendance in the CSV file as well.
  Press "q" to stop and exit from the camera.
  
  
### Result

