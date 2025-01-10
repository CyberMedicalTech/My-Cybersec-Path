### **🖥️ My Cybersecurity Lab Setup Guide**

This is a record of how I set up my personal cybersecurity lab on my new laptop to help me practice hands-on skills and build my GitHub portfolio. I’m documenting each step I take, including:
- ✅ What I installed
- ✅ Commands I ran
- ✅ What I documented in my GitHub
- ✅ Notes I took along the way

---

### **🚀 Step 1: Installing VirtualBox**  
The first step I took was installing VirtualBox, which I needed to create virtual machines (VMs) for running Linux distros and security tools.

### **What I Did:**  
- I downloaded VirtualBox from the official site: [https://www.virtualbox.org](https://www.virtualbox.org).  
- I installed it on my laptop.  
- After the installation, I opened VirtualBox to start creating virtual machines.

---

### **🐧 Step 2: Downloading and Installing Kali Linux**

Next, I set up Kali Linux, which is a popular Linux distribution used for penetration testing and cybersecurity.

### **What I Did:**

- I downloaded the Kali Linux ISO from the official site: https://www.kali.org/downloads/.

- In VirtualBox, I clicked New to create a new VM.

- Used the following settings:

    - Name: Kali Linux

    - Type: Linux

    - Version: Debian (64-bit)

- Allocated at least 2 GB of RAM and 20 GB of storage.

- Attached the Kali Linux ISO to the VM and started the installation.

- Followed the on-screen instructions to complete the installation.

Commands I Ran (Inside Kali):

`sudo apt update`

`sudo apt upgrade`

Notes:

Kali Linux is a virtual work space that can be used for penetration testing and ethical hacking.

Virtualization is important because it allows me to run multiple operating systems on one machine.

The commands `sudo apt update` and `sudo apt upgrade` are used to update the system.

### 🚀 Debian VM Setup
[Click here to view the full guide](./Dabian_Setup.md)
- Launched the Debian VM for the first time.
- Configured the network, users, and partitions.
- Installed and updated the system.

---

### **🛠️ Step 3: Installing Wireshark**

After setting up Kali Linux, I installed Wireshark, a tool used to capture and analyze network traffic.

### **What I Did:**

- In Kali Linux, I opened the terminal.

- I ran the following command to install Wireshark:

`sudo apt install wireshark`

- After the installation, I launched Wireshark and started a capture session to analyze network packets.

Notes:

- Wireshark is a network protocol analyzer that allows me to inspect network traffic in real-time.

- I learned how to start a capture session and review packet data.

- Packet analysis is useful for identifying suspicious activity in a network.

---

### **🔐 Step 4: Installing Wazuh (SIEM Tool)**

Next, I set up Wazuh, an open-source Security Information and Event Management (SIEM) tool to monitor logs and detect threats.

### **What I Did:**

- I followed the official Wazuh installation guide: https://documentation.wazuh.com/.

- I configured Wazuh to monitor logs from my Kali Linux VM.

### **Notes:**

- SIEM tools are essential for log management and threat detection.

- Wazuh provides real-time monitoring and alerts for potential security issues.

- I learned how to set up a SIEM tool and configure it to monitor logs from a virtual machine.

---

### **🐍 Step 5: Installing Python**

Since Python is widely used in cybersecurity for scripting and automation, I installed it on my Kali Linux VM.

### **What I Did:**

- I opened the terminal in Kali Linux.

- I checked if Python was already installed:

`python3 --version`

`sudo apt install python3`

- I also installed pip (Python package manager):

`sudo apt install python3-pip`

### **Notes:**

- Python is great for automating repetitive tasks in cybersecurity.

- Some useful Python libraries for cybersecurity include `scapy`, `requests`, and `os`.

- I wrote a basic Python script to automate log analysis.

---

### **📋 Step 6: Documenting My Journey on GitHub**

Throughout this process, I’ve been documenting my progress in my GitHub repository to keep track of what I’m learning and to showcase my journey to potential employers.


Here’s how I’m structuring my README updates:

### ✅ Week 1
- Installed VirtualBox and set up Kali Linux VM
- Installed Wireshark and captured network traffic
- Installed Wazuh SIEM tool to monitor logs
- Installed Python to automate cybersecurity tasks

🔍 Next Steps in My Learning Journey:

After setting up my lab, I’ll continue learning:

Linux commands (file management, user management, permissions)

Network security concepts (firewalls, VPNs, DNS)

Basic penetration testing with Kali Linux tools like Nmap and Metasploit

🏁 Final Reflections:

Setting up my personal lab has been a crucial first step in my cybersecurity journey. I’ve gained hands-on experience with tools and concepts that will help me continue building my skills and portfolio. I’m excited to keep learning and documenting my progress!

🎯 Goal: By the end of this process, I’ll have a fully functioning cybersecurity lab and a strong foundation to keep building my skills!

