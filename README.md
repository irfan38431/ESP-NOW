# ESP-NOW Protocol for ESP8266

## Introduction
This repository contains the implementation of the ESP-NOW protocol for the ESP8266 microcontroller. ESP-NOW is a communication protocol developed by Espressif Systems specifically for peer-to-peer communication between ESP8266 and ESP32 devices. It operates on the 2.4GHz band and provides a low-power, low-latency solution for IoT (Internet of Things) applications.

## Getting Started
To use this library in your ESP8266 project, follow these steps:

1. Clone or download this repository.
2. Copy the `ESPNow` folder into the `libraries` folder of your Arduino IDE installation directory.
3. Restart the Arduino IDE.
4. Open the example sketches provided in the `examples` folder to understand how to use the ESP-NOW protocol for various purposes.

## Usage
### Sending Data
To send data using ESP-NOW, follow these steps:

1. Initialize ESP-NOW in sender mode using `ESPNow.begin()`.
2. Add the MAC address of the receiver using `ESPNow.addPeer()`.
3. Send data using `ESPNow.send()`.
4. Handle the data reception on the receiver side.

### Receiving Data
To receive data using ESP-NOW, follow these steps:

1. Initialize ESP-NOW in receiver mode using `ESPNow.begin()`.
2. Register a callback function using `ESPNow.onReceive()`.
3. Handle the received data inside the callback function.

Refer to the provided example sketches for detailed usage.

## Compatibility
This library is compatible with the ESP8266 platform. It may also work with ESP32, but the official ESP-NOW library from Espressif Systems is recommended for ESP32 projects.

## Contributing
Contributions to this project are welcome. If you find any bugs or want to add new features, feel free to open an issue or submit a pull request.

## License
This library is released under the MIT License. See the `LICENSE` file for more details.

## Credits
This library is based on the ESP-NOW implementation by Espressif Systems. Special thanks to the contributors of the ESP-NOW protocol and the Arduino ESP8266 community.

For more information about ESP-NOW, refer to the official documentation by Espressif Systems: [ESP-NOW Protocol Overview](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/network/esp_now.html)
