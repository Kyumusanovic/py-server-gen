# Python Persistent Server Reporter 🚀

![Python Version](https://img.shields.io/badge/python-3.6%2B-blue.svg) ![License](https://img.shields.io/badge/license-MIT-green.svg) ![Release](https://img.shields.io/badge/release-latest-orange.svg)

Welcome to the **Python Persistent Server Reporter** repository! This application, developed by Bocaletto Luca, is designed to collect and report system metrics in a reliable and efficient manner. It operates seamlessly across different platforms, making it a versatile tool for system administrators and developers alike.

## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Configuration](#configuration)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)
9. [Releases](#releases)

## Overview

The **Python Persistent Server Reporter** is an application that gathers essential system metrics and sends reports via SMTP. It runs in the background as a Windows Service or a systemd daemon, ensuring that you have continuous access to vital system information. This tool is perfect for monitoring server health and performance, making it a valuable asset for IT professionals.

## Features

- **Cross-Platform Compatibility**: Works on both Windows and Linux systems.
- **System Metrics Collection**: Gathers IP, MAC, hostname, OS, CPU, memory, disk usage, and user information.
- **Configurable Reporting**: Sends reports at user-defined intervals via SMTP.
- **Background Operation**: Runs as a Windows Service or a systemd daemon.
- **Automatic Restart**: The application can restart automatically in case of failure, ensuring minimal downtime.

## Installation

To install the **Python Persistent Server Reporter**, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/Kyumusanovic/py-server-gen.git
   ```

2. Navigate to the project directory:

   ```bash
   cd py-server-gen
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Follow the configuration steps below to set up your environment.

## Usage

After installation, you can start using the **Python Persistent Server Reporter**. 

1. Run the application using the command line:

   ```bash
   python main.py
   ```

2. The application will start collecting metrics and sending reports according to your configuration.

## Configuration

To configure the application, edit the `config.json` file located in the project directory. Here is a sample configuration:

```json
{
  "smtp_server": "smtp.example.com",
  "smtp_port": 587,
  "username": "your_email@example.com",
  "password": "your_password",
  "report_interval": 60,
  "report_recipients": ["recipient@example.com"]
}
```

### Configuration Parameters

- **smtp_server**: The SMTP server address for sending reports.
- **smtp_port**: The port used for the SMTP server (typically 587 for TLS).
- **username**: Your email address for SMTP authentication.
- **password**: Your email password for SMTP authentication.
- **report_interval**: The interval (in seconds) at which reports are sent.
- **report_recipients**: A list of email addresses to receive the reports.

## Contributing

We welcome contributions to the **Python Persistent Server Reporter**! If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your forked repository.
5. Create a pull request detailing your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or support, please reach out to Bocaletto Luca at [your_email@example.com].

## Releases

To download the latest version of the **Python Persistent Server Reporter**, visit the [Releases section](https://github.com/Kyumusanovic/py-server-gen/releases). You can find the necessary files there to download and execute.

For the most up-to-date releases, check the [Releases section](https://github.com/Kyumusanovic/py-server-gen/releases) regularly.

---

Thank you for your interest in the **Python Persistent Server Reporter**! We hope this tool serves you well in monitoring and reporting system metrics effectively.