✅ Step 1: Select the Installation Option
When you start your VM, you’ll see a boot menu with several options. Choose:

👉 Graphical Install (use the arrow keys to select it, then press Enter).

✅ Step 2: Select Language, Location, and Keyboard Layout
Language: Choose your preferred language (e.g., English).
Location: Select your country or region (e.g., United States).
Keyboard Layout: Choose your keyboard layout (e.g., American English).
✅ Step 3: Configure the Network
Hostname: Enter a name for your system (e.g., debian-vm).

This is your computer's network name.
Domain Name: You can leave this blank unless you’re on a business network.

Root Password:

Enter a strong password for the root user (this is the superuser account with full permissions).
Note: Make sure you remember this password!
Create a New User:

You’ll be asked to create a non-root user for daily use.
Full Name: Enter your name or a username (e.g., CyberMedical).
Username: Enter the same or a shorter version (e.g., cyber).
Password: Enter a strong password for this user.
✅ Step 4: Set Up Time Zone
Select your time zone from the list.
✅ Step 5: Partition the Disk
Choose Guided - Use Entire Disk (recommended for beginners).
Select your virtual hard disk (it will be the only option).
Choose All files in one partition.
Confirm your partition setup and select Finish partitioning.
When asked to write changes to disk, select Yes.
✅ Step 6: Software Selection
You’ll be asked to choose which software packages to install.

Uncheck “Graphical Desktop Environment” if you only need a command-line interface.
Otherwise, leave it checked to install a graphical interface (recommended for beginners).
Make sure standard system utilities are selected.

Proceed with the installation.

✅ Step 7: Install GRUB Boot Loader
When prompted to install the GRUB boot loader, choose Yes.
Select your primary disk (usually /dev/sda).
✅ Step 8: Complete the Installation
Once the installation is complete, you’ll be prompted to reboot the system.
After the VM reboots, log in with the username and password you created earlier.
💻 Next Steps After Setup
Once you're inside your VM:

Update your system:

bash
Copy code
sudo apt update
sudo apt upgrade
Install additional tools if needed, such as:

Git:
bash
Copy code
sudo apt install git
Python:
bash
Copy code
sudo apt install python3
