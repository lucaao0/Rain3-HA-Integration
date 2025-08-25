# Rain3-HA-Integration 🌧️

![GitHub release](https://img.shields.io/github/release/lucaao0/Rain3-HA-Integration.svg) ![License](https://img.shields.io/github/license/lucaao0/Rain3-HA-Integration.svg)

Welcome to the **Rain3-HA-Integration** repository! This project enables seamless integration of the Rain3 pump with Home Assistant, allowing for real-time updates via MQTT. This integration enhances your home automation experience by providing accurate control and monitoring of your irrigation system.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Releases](#releases)

## Features 🌟

- **Real-time Updates**: The integration sends changes from the Rain3 pump directly to Home Assistant using MQTT.
- **Easy Setup**: Simple installation and configuration process.
- **Lightweight**: Built on the ESP32 platform, making it efficient and responsive.
- **HTML Scraping**: Uses DOM parsing for effective data retrieval.
- **IoT Ready**: Fully compatible with IoT devices and platforms.

## Getting Started 🚀

To get started with the Rain3-HA-Integration, you will need the following:

1. **Hardware**: An ESP32 microcontroller.
2. **Software**: Home Assistant installed on your server or Raspberry Pi.
3. **MQTT Broker**: An MQTT broker set up and running (e.g., Mosquitto).

## Installation 🛠️

Follow these steps to install the integration:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/lucaao0/Rain3-HA-Integration.git
   cd Rain3-HA-Integration
   ```

2. **Install Dependencies**:

   Ensure you have Python and the necessary libraries installed. You can install the required libraries using:

   ```bash
   pip install -r requirements.txt
   ```

3. **Upload to ESP32**:

   Use a tool like PlatformIO or Arduino IDE to upload the code to your ESP32.

4. **Configure Home Assistant**:

   Add the necessary configuration in your `configuration.yaml` file in Home Assistant to connect to the MQTT broker.

## Usage 📦

Once you have installed and configured the integration, you can start using it. The Rain3 pump will send updates to Home Assistant, which you can monitor and control through the Home Assistant dashboard.

1. **Monitor Status**: View the status of the Rain3 pump in real-time.
2. **Control Pump**: Turn the pump on or off directly from Home Assistant.
3. **Automation**: Set up automation rules based on the pump's status.

## Configuration ⚙️

To configure the integration, you need to edit the `config.py` file in the repository. Here’s a basic structure of what you need to include:

```python
MQTT_BROKER = "your_mqtt_broker_ip"
MQTT_PORT = 1883
RAIN3_API_URL = "http://your_rain3_api_url"
```

Make sure to replace the placeholders with your actual MQTT broker information and Rain3 API URL.

## Contributing 🤝

We welcome contributions! If you have suggestions or improvements, feel free to open an issue or submit a pull request. Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License 📜

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact 📬

For any questions or support, feel free to reach out:

- **GitHub**: [lucaao0](https://github.com/lucaao0)
- **Email**: lucaao0@example.com

## Releases 📦

To download the latest release, visit the [Releases](https://github.com/lucaao0/Rain3-HA-Integration/releases) section. Make sure to download the appropriate file and execute it to get started.

If you need to check for updates, you can always refer to the [Releases](https://github.com/lucaao0/Rain3-HA-Integration/releases) page.

## Additional Resources 📚

- [Home Assistant Documentation](https://www.home-assistant.io/docs/)
- [MQTT Protocol Overview](https://mqtt.org/)
- [ESP32 Documentation](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/index.html)

## Acknowledgments 🙏

- Thanks to the Home Assistant community for their continuous support and contributions.
- Special thanks to the developers of the libraries used in this project.

## Conclusion 🌈

The Rain3-HA-Integration project aims to provide a simple yet powerful solution for integrating your Rain3 pump with Home Assistant. By using MQTT, you can enjoy real-time updates and control over your irrigation system, making home automation more efficient and effective.

Feel free to explore the code, contribute, and enjoy the benefits of a smart irrigation system!