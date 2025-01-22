ESP BLE Provisioning with ESP-IDF
Overview
This project demonstrates BLE-based Wi-Fi provisioning using the ESP32 and ESP-IDF. The ESP BLE Provisioning app is used to configure Wi-Fi credentials for the ESP32.

Prerequisites
Hardware
ESP32 development board.
Software
ESP-IDF version 5.1.
ESP BLE Provisioning app (available on Google Play Store).
Installation and Setup
1. Install ESP-IDF
Follow the official ESP-IDF installation guide.

2. Navigate to the Example Project
Go to the wifi_prov_mgr example:cd ~/esp/esp-idf/examples/provisioning/wifi_prov_mgr

3. Build and Flash the Project
Configure the project: idf.py menuconfig

Build the firmware: idf.py build

Flash the firmware to the ESP32: idf.py -p /dev/ttyUSB0 flash

4. Monitor Logs
Start the serial monitor to view logs:idf.py monitor Use Ctrl+] to exit the monitor.

How to Use
Step 1: Open the ESP BLE Provisioning App
Download and install the app from the Google Play Store.
Open the app and scan for BLE devices.
Select your ESP32 from the list of available devices.
Step 2: Provision Wi-Fi Credentials
Enter the Wi-Fi SSID and password in the app.
Send the credentials to the ESP32.
Check the serial monitor logs to confirm successful provisioning.
Outputs and Results
BLE Provisioning Process
The ESP32 is successfully configured to connect to a Wi-Fi network via BLE.
Example Serial Monitor Logs
plaintext I (1234) wifi: Connected to SSID my_wifi I (1234) provisioning: Successfully provisioned.

Demo Video
Include a video demonstrating the following:

BLE provisioning via the app. Similar video : https://www.youtube.com/watch?v=JYtDibqJMs0&t=475s
Credits
Developer: Kiran Mulge
Resources:
ESP-IDF Documentation
BLE Provisioning Example
License
This project is licensed under the MIT License.
