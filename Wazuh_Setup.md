✅ What is Wazuh?
Wazuh is a Security Information and Event Management (SIEM) tool. It helps you:

Monitor your systems for threats.
Analyze logs from different devices and applications.
Detect security issues in real-time.
Think of it as a central security dashboard to keep track of what's happening in your network.

✅ Step 1: Update Your Kali Linux
Before installing anything, update your system to make sure everything is up-to-date.

🔧 Run this command:
bash
Copy code
sudo apt update && sudo apt upgrade -y
✅ Step 2: Install Required Packages
You need some prerequisite packages for Wazuh.

🔧 Run this command:
bash
Copy code
sudo apt install curl apt-transport-https -y
✅ Step 3: Download the Wazuh Repository Key
The repository key allows Kali Linux to trust the Wazuh package.

🔧 Run this command:
bash
Copy code
curl -s https://packages.wazuh.com/key/GPG-KEY-WAZUH | sudo apt-key add -
✅ Step 4: Add the Wazuh Repository
You need to add the Wazuh repository to your system so you can download the Wazuh packages.

🔧 Run this command:
bash
Copy code
echo "deb https://packages.wazuh.com/4.x/apt stable main" | sudo tee /etc/apt/sources.list.d/wazuh.list
✅ Step 5: Update Your Package List
After adding the Wazuh repository, update the package list to make it available.

🔧 Run this command:
bash
Copy code
sudo apt update
✅ Step 6: Install the Wazuh Manager
The Wazuh Manager is the core part of Wazuh that processes logs and manages alerts.

🔧 Run this command:
bash
Copy code
sudo apt install wazuh-manager -y
✅ Step 7: Start and Enable the Wazuh Service
After installation, you need to start the Wazuh service and set it to start automatically on boot.

🔧 Run these commands:
bash
Copy code
sudo systemctl start wazuh-manager
sudo systemctl enable wazuh-manager
✅ Step 8: Verify Wazuh is Running
To make sure Wazuh Manager is running, check the service status.

🔧 Run this command:
bash
Copy code
sudo systemctl status wazuh-manager
You should see “active (running)” if it’s working correctly.

✅ Optional: Install Wazuh Agent (if you want to monitor the Kali VM itself)
If you want to monitor the same Kali Linux system with Wazuh, install the Wazuh Agent.

🔧 Run this command:
bash
Copy code
sudo apt install wazuh-agent -y
✅ Step 9: Start and Enable the Wazuh Agent
Just like the manager, start the agent service and enable it to start on boot.

🔧 Run these commands:
bash
Copy code
sudo systemctl start wazuh-agent
sudo systemctl enable wazuh-agent
🎯 Summary of Commands:
bash
Copy code
sudo apt update && sudo apt upgrade -y
sudo apt install curl apt-transport-https -y
curl -s https://packages.wazuh.com/key/GPG-KEY-WAZUH | sudo apt-key add -
echo "deb https://packages.wazuh.com/4.x/apt stable main" | sudo tee /etc/apt/sources.list.d/wazuh.list
sudo apt update
sudo apt install wazuh-manager -y
sudo systemctl start wazuh-manager
sudo systemctl enable wazuh-manager
sudo systemctl status wazuh-manager
💡 GitHub Documentation Idea:
Document your Wazuh installation like this:

markdown
Copy code
### 🔐 Installing Wazuh on Kali Linux
- Updated my Kali Linux system.
- Installed required packages for Wazuh.
- Added the Wazuh repository and downloaded the repository key.
- Installed the Wazuh Manager and started the service.
- Verified that Wazuh is running successfully.
