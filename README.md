# Bedew: Automated Greenhouse Nursery System

<p align="center">
  <img src="docs/images/bedew-logo.png" alt="Bedew Logo" width="200"/>
</p>

[![License](https://img.shields.io/github/license/yourusername/bedew)](https://github.com/yourusername/bedew/blob/main/LICENSE)
[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue)](https://www.python.org/downloads/)
[![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-Compatible-green)](https://www.raspberrypi.org/)

**Bedew** is an automated greenhouse nursery system designed to grow healthy plant saplings with minimal human intervention. The system consists of a mobile robot that cares for plants in a greenhouse environment by monitoring conditions, watering plants, seeding new pots, and moving plants as needed.

## 🌱 Features

- **Automated Plant Care**: Water plants based on soil moisture and plant needs
- **Intelligent Monitoring**: Track plant growth, health, and environmental conditions
- **Computer Vision**: Identify plants, assess health, and determine growth stage
- **Environment Control**: Manage temperature, humidity, and lighting for optimal growth
- **Web Interface**: Monitor and control your greenhouse from anywhere
- **Expandable**: Open architecture allows for customization and expansion

## 🏗️ System Overview

The Bedew system consists of two primary components:

1. **Greenhouse Controller**: Manages the greenhouse environment (temperature, humidity, lighting)
2. **Bedew Robot**: A mobile robot that navigates the greenhouse and performs plant care tasks

![System Architecture](docs/images/system-architecture.png)

### Hardware Components

The system is designed to run on:
- **Raspberry Pi 5** (for the robot)
- **Raspberry Pi 4** (for the greenhouse controller)
- Custom PCBs for connecting sensors and actuators
- 3D-printed chassis and mechanical components

See the [Hardware Setup Guide](docs/hardware_setup.md) for detailed specifications and assembly instructions.

## 🚀 Installation

### Prerequisites

- Python 3.7 or higher
- Raspberry Pi OS (Bookworm or newer)
- MQTT broker (Mosquitto)
- Required Python packages

### Basic Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/bedew.git
   cd bedew
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up the configuration:
   ```bash
   python setup.py
   ```

4. Start the system:
   ```bash
   python bedew.py
   ```

For detailed installation instructions, see the [Installation Guide](docs/installation.md).

## 📊 Web Interface

The Bedew system includes a web interface for monitoring and controlling your greenhouse. After starting the system, you can access the web interface at `http://[raspberry-pi-ip]:5000`

![Web Interface](docs/images/web-interface.png)

See the [User Guide](docs/user_guide.md) for detailed usage instructions.

## 🛠️ Development

### Project Structure

The project is organized into several modules:

- `bedew/robot`: Robot control and navigation
- `bedew/greenhouse`: Greenhouse environment control
- `bedew/communication`: Communication between components
- `bedew/web`: Web interface

### Contributing

We welcome contributions to the Bedew project! Please see our [Contributing Guidelines](CONTRIBUTING.md) for more information.

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Special thanks to the open-source community for their invaluable tools and libraries
- Inspired by sustainable agriculture and precision farming practices
