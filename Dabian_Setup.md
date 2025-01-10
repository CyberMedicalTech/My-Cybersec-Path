### **✅ Step 1: Select the Installation Option**
When you start your VM, you’ll see a boot menu with several options.

Choose:
👉 Graphical Install (use the arrow keys to select it, then press Enter).

---

### **✅ Step 2: Select Language, Location, and Keyboard Layout**
1. Language: Choose your preferred language (e.g., English).
2. Location: Select your country or region (e.g., United States).
3. Keyboard Layout: Choose your keyboard layout (e.g., American English).
  
---

### **✅ Step 3: Configure the Network**
1. Hostname: Enter a name for your system (e.g., `debian-vm`).
  - This is your computer's network name.
2. Domain Name: You can leave this blank unless you’re on a business network.

3. Root Password:
   
  - Enter a strong password for the root user (this is the superuser account with full permissions).
    
Note: Make sure you remember this password!

4. Create a New User:

- You’ll be asked to create a non-root user for daily use.
  
  - Full Name: Enter your name or a username (e.g., `CyberMedical`).
  - Username: Enter the same or a shorter version (e.g., `cyber`).
  - Password: Enter a strong password for this user.
 
---

### **✅ Step 4: Set Up Time Zone**

1. Select your time zone from the list.

---

### **✅ Step 5: Partition the Disk**

1. Choose Guided - Use Entire Disk (recommended for beginners).
   
2. Select your virtual hard disk (it will be the only option).
   
3. Choose All files in one partition.
  
4. Confirm your partition setup and select Finish partitioning.
   
5. When asked to write changes to disk, select Yes.

---

### **✅ Step 6: Software Selection**

1. You’ll be asked to choose which software packages to install.
  - Uncheck “Graphical Desktop Environment” if you only need a command-line interface.
    
  - Otherwise, leave it checked to install a graphical interface (recommended for beginners).
    
2. Make sure standard system utilities are selected.

3. Proceed with the installation.

---

### **✅ Step 7: Install GRUB Boot Loader**

1. When prompted to install the GRUB boot loader, choose Yes.
   
2. Select your primary disk (usually `/dev/sda`).

---

### **✅ Step 8: Complete the Installation**

1. Once the installation is complete, you’ll be prompted to reboot the system.

2. After the VM reboots, log in with the username and password you created earlier.

---

### **💻 Next Steps After Setup**
Once you're inside your VM:

1. Update your system:

`sudo apt update`

`sudo apt upgrade`

2. Install additional tools if needed, such as:

  - Git:
    
`sudo apt install git`

  - Python
    
`sudo apt install python3`
