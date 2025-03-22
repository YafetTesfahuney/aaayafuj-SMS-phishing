# aaayafuj-SMS-phishing Kali Linux
A phishing tool that can also send SMS alerts.
# AdvPhishing.sh
* It collects phone numbers and can send phishing-based SMS.
![Screenshot 2025-03-21 181826](https://github.com/user-attachments/assets/3eb67ba3-e05c-45bc-99f5-0010ee1501c6)

# To install the tool follow this.
* first open your Terminal, On Kali Linux
* Write or copy then --> Paste
* The commands
  ```
  $ sudo apt update
  $ sudo apt upgrade
  $ nano aaayafuj_phishing_tool.sh
# When you type ☝, Then you have to save the script in *(nano)* down here 
    bash
    $ chmod +x aaayafuj_phishing_tool.sh
    $ bash aaayafuj_phishing_tool.sh
    $ ./aaayafuj_phishing_tool.sh
    $ sudo ./aaayafuj_phishing_tool.sh
  
# when you copy or write ☝ the commands ✔
* Then copy the script 👇
* and paste in "nano"
```
#!/bin/bash

# AdvPhishing Setup Script
# Created by aaayafuj
# To install the tool, follow this:
# First, open your Terminal on Kali Linux.

# AdvPhishing Setup Script for Kali Linux
# Created by aaayafuj

# Summary:
# This script installs and sets up AdvPhishing on Kali Linux, ensuring all dependencies
# are installed before running the tool.

# Update and install necessary dependencies
echo "Updating system and installing dependencies..."
sudo apt update && sudo apt upgrade -y
sudo apt install -y git wget curl php openssh-client

# Clone the AdvPhishing repository
echo "Cloning AdvPhishing repository..."
git clone https://github.com/Ignitetch/AdvPhishing.git

# Navigate to the AdvPhishing directory
cd AdvPhishing || { echo "Failed to enter AdvPhishing directory"; exit 1; }

# Give execution permissions
echo "Setting execution permissions..."
chmod +x *.sh

# Run the script
echo "Starting AdvPhishing..."
bash AdvPhishing.sh


