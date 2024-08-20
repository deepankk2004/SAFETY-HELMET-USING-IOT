

---

# Safety Helmet for Mining Workers Using IoT

## Overview

This project aims to enhance the safety of mining workers through an IoT-enabled smart helmet. The helmet monitors environmental and health conditions and provides real-time alerts to ensure worker safety in hazardous mining environments. The system integrates various sensors and transmits data to a Firebase backend for monitoring and analysis.

## Features

- **Real-Time Monitoring:** Measures environmental conditions such as gas levels, temperature, and humidity.
- **Health Monitoring:** Tracks worker health metrics including emergency alerts triggered by button presses.
- **IoT Integration:** Uses Wi-Fi to send data to Firebase for real-time monitoring and alerts.
- **Helmet Status Detection:** Detects whether the helmet is being worn or not.

## Technologies Used

- **Hardware:** Arduino, MQ2 Gas Sensor, DHT11 Temperature and Humidity Sensor, GPS Module, IR Sensor, Push Button.
- **Software:** C++, FirebaseESP32 library, TinyGPS++ library, DHT library, Wi-Fi for data transmission.

## Getting Started

### Prerequisites

- Arduino IDE
- Firebase account and Firebase Realtime Database setup
- IoT hardware components as listed above

### Installation

1. **Install Required Libraries:**
   - FirebaseESP32
    - TinyGPS++
    - DHT sensor library

     2. **Configure Firebase:**
            - Replace `FIREBASE_HOST` and `FIREBASE_AUTH` with your Firebase project's details.

         3. **Upload Code:**
               - Open `helmet_iot.ino` in the Arduino IDE.
                  - Connect your Arduino board and upload the code.

             4. **Connect Hardware:**
                     - Wire up the sensors and components as defined in the code.

                 ### Usage

                  - **Monitor Data:**
                       - Check the Firebase Realtime Database to view live data from the helmet.

                 - **Emergency Alerts:**
                         - Press the push button on the helmet to trigger an emergency alert, which will be recorded in Firebase.

                - **Helmet Status:**
                           - Ensure that the IR sensor detects whether the helmet is being worn.

                    ## Code Description

                     The provided code initializes the sensors, connects to Wi-Fi, and sends data to Firebase. It also handles real-time monitoring of environmental and health parameters, including:

                    - **Gas Sensor:** Measures the concentration of gases in the environment.
                     - **Temperature and Humidity Sensor:** Reads temperature and humidity data.
                    - **GPS Module:** Provides location data.
                    - **Push Button:** Triggers an emergency alert.
                    - **IR Sensor:** Detects if the helmet is being worn.

                    **Key Functions:**

                    - `setup()`: Initializes the hardware, connects to Wi-Fi, and configures Firebase.
                    - `loop()`: Continuously reads sensor data, updates Firebase, and handles emergency alerts.
                    - `print_ok()` and `print_fail()`: Print status messages for Firebase operations.

                    ## Contributing

                    If you would like to contribute to this project, please fork the repository and submit a pull request with your changes. Ensure that all contributions are well-documented and tested.

                    ## License

                    This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

                    ## Acknowledgments

                    - [Firebase](https://firebase.google.com/)
                    - [Arduino](https://www.arduino.cc/)
                    - [TinyGPS++](https://github.com/mikalhart/TinyGPSPlus)
                    - [DHT Sensor Library](https://github.com/adafruit/DHT-sensor-library)

                     ## Author

                    Deepank Yadav  
                        Email: yadavdeepank6@gmail.com

                    ---
                    Feel free to adjust any details as needed!