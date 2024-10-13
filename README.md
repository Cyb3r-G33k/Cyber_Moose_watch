
# Cyber Moose Watch  
*Created by Alex Losev*

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Configuration](#configuration)
6. [Web Interface Access](#web-interface-access)
7. [Email Settings](#email-settings)
8. [Logs and Reports](#logs-and-reports)
9. [Development Roadmap](#development-roadmap)
10. [Contributing](#contributing)
11. [License](#license)

---

## Introduction

**Cyber Moose Watch** is a powerful monitoring tool designed for system administrators and cybersecurity enthusiasts. It provides insights into CPU, RAM, disks, GPU, and network usage, while tracking service and process statuses. Additionally, it offers real-time failure detection, automatic service restarts, and email notifications for reports.

---

## Features

- **System Monitoring:** CPU, RAM, Disks, GPU, Network, Service and Process statuses, and average load tracking.
- **Service Management:** Automatic restart for failed services with configurable attempts.
- **Web Interface:** Accessible remotely via IP and port to view system status and manage services.
- **Logs and Reports:** Auto-generated logs and reports in text format.
- **Email Notifications:** Configurable email settings with support for multiple recipients.
- **Process Management:** Drag-and-drop interface to select processes and services to monitor.
- **Multi-host Support:** Ability to add and monitor multiple hosts via the web interface.

---

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Cyb3r-G33k/Cyber_Moose_watch.git
   cd Cyber_Moose_watch
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   python Cyber_Moose_Watch.py
   ```

4. **(Optional) Start the web interface**
   ```bash
   python web_interface.py
   ```

---

## Usage

- **Starting the Application:**  
   Run `Cyber_Moose_Watch.py` to begin monitoring.

- **Web Access:**  
   Use the web interface to view system metrics and manage processes/services.

- **Adding Hosts:**  
   Go to the *Manage Hosts* tab to add a new host with its IP and port.

---

## Configuration

1. **Configuration File:**  
   After the first run, a `config.ini` file will be generated. Use it to:
   - Set default IP and port for the web interface.
   - Configure email settings.
   - Enable or disable automatic service restarts.

2. **Setting Monitoring Parameters:**  
   Go to the *Manage Services* or *Manage Processes* tab in the web interface to select which metrics and processes to monitor.

---

## Web Interface Access

- **Local Access:**  
   Open a web browser and go to:
   ```
   http://localhost:8000
   ```

- **Remote Access:**  
   If running on a different machine, use the host IP and port:
   ```
   http://<host-ip>:<port>
   ```

---

## Email Settings

1. Navigate to the *Settings* tab.  
2. Add the SMTP server, port, email address, and password.  
3. Use the **Test Email** button to verify the connection.  
4. Add multiple recipients by separating their emails with commas.

---

## Logs and Reports

- **Logs:**  
   Logs will be saved in the `/logs` directory in `.txt` format.

- **Reports:**  
   Scheduled reports are automatically generated and sent via email based on the chosen frequency (daily, weekly, or monthly).  
   The report covers system metrics and any alerts triggered during the period.

---

## Development Roadmap

- [x] Core system monitoring functionality  
- [x] Web interface development  
- [ ] Advanced analytics and alerting  
- [ ] Docker support for deployment  
- [ ] Cloud-based monitoring dashboard  

---

## Contributing

We welcome contributions from the community! Follow these steps to contribute:

1. Fork the repository.  
2. Create a new branch:
   ```bash
   git checkout -b feature-branch
   ```
3. Commit your changes:
   ```bash
   git commit -m "Added new feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-branch
   ```
5. Create a pull request.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
