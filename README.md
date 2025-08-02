# Description

This repository provides a collection of dependencies and fixes for running Cisco Packet Tracer on Ubuntu 24.04 and later. Simplifies installation by resolving compatibility issues with a few libraries and package on recent Ubuntu releases. 



## Tested ✅
- [x] Ubuntu 25.04
- [x] Ubuntu 24.10
- [x] Ubuntu 24.04
- [x] Debian 13
- [x] Debian 12




## 📋 Prerequisites

Before starting the installation, ensure you have the following:

- A machine running **Ubuntu 24.04** or **Ubuntu 24.10**.
- Basic familiarity with using the terminal/command line.
- **Root (sudo) access** on your machine.



## 🚀 Installation Steps

### Step 1: Clone the Repository

You can start by cloning this repository to your local machine using Git. This will download all the files and installation scripts you'll need.

```bash
git clone https://github.com/farhatizakaria/CiscoPacketTracer-Ubuntu_24.10.git
```

### Step 2: Navigate to the cloned directory
```bash
cd CiscoPacketTracer-Ubuntu_24.10
```
### Step 3: Install Required Dependencies
Before installing Cisco Packet Tracer, install the necessary dependencies for a smooth installation:
```bash
sudo apt update && sudo apt upgrade -y
sudo dpkg -i libgl1-mesa-glx_23.0.4-0ubuntu1~22.04.1_amd64.deb
sudo dpkg -i dialog_1.3-20240101-1_amd64.deb
sudo dpkg -i libxcb-xinerama0-dev_1.15-1ubuntu2_amd64.deb
```
If you encounter any missing dependencies or issues during installation, run:
```bash
sudo apt --fix-broken install
```
### Step 5: Download Cisco Packet Tracer 8.2.2
You can download the Cisco Packet Tracer 8.2.2 .deb package from the official Cisco Networking Academy website. Be sure to log in to your account before downloading.
Visit the [Cisco Networking Academy](https://www.netacad.com/) and download the Packet Tracer 8.2.2 version for Linux.
### Step 6: Install Cisco Packet Tracer
Once you have downloaded the .deb package, navigate to the directory where the .deb file is located. Install Packet Tracer using the following command:
```bash
sudo dpkg -i packettracer_8.2.2_amd64.deb
```

## 🌟 Contributing
Feel free to fork the repository and contribute if you find any additional dependencies or have suggestions for improvement. If you encounter any issues, please create an issue.
