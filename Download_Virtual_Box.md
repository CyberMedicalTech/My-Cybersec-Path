### **✅ Step 1: Download VirtualBox**
1. Go to the official VirtualBox website:
👉 https://www.virtualbox.org

2. Click on the **"Downloads"** button in the menu.

3. Select **"Windows hosts"** to download the Windows installer.

---

### **✅ Step 2: Install VirtualBox**
1. Once the VirtualBox installer is downloaded, open the file (e.g., `VirtualBox-x.x.x-xxxx-Win.exe`

2. The Setup Wizard will open. Click Next to proceed.

3. In the Custom Setup screen:
  - Leave the default options checked (you can install to `C:\\Program Files\\Oracle\\VirtualBox`).
  - **Click Next.**
4. On the **Network Interface Warning** screen, click Yes.
(This will temporarily disconnect your network during installation.)

5. Click **Install** to begin the installation.

6. **Allow any security prompts** from Windows (click **Yes** if prompted).

7. Once the installation completes, click **Finish.**

---

### **✅ Step 3: Download a Virtual Machine (VM) ISO**
You’ll need an ISO file to install a virtual machine. For cybersecurity, I recommend starting with Kali Linux.

👉 Download Kali Linux from the official site:
https://www.kali.org/downloads/

---

### **✅ Step 4: Create a New Virtual Machine in VirtualBox**
1. Open **VirtualBox.**

2. Click the **New** button to create a new VM.

3. In the **Name and Operating System** screen:

- **Name:** Kali Linux
- **Type:** Linux
- **Version:** Debian (64-bit)
4. Click **Next.**

5. Allocate **RAM** for the VM:

- Set at least **2048 MB (2 GB)** of RAM.
- Click **Next**
6. Select **Create a virtual hard disk now** and click **Create.**

7. Choose **VDI (VirtualBox Disk Image)** and click **Next.**

8. Select **Dynamically allocated** and click **Next.**

9. Set the **virtual hard disk size** to at least **20 ** and click **Create.**

---

### **✅ Step 5: Attach the Kali Linux ISO**
1. Select your newly created **Kali Linux VM** in VirtualBox.

2. Click **Settings > Storage.**

3. Under* **Controller: IDE,** click the **Empty** disk icon.

4. Click the **CD icon** on the right, then choose Choose a disk file....

5. Select the **Kali Linux ISO** you downloaded.

6. Click **OK.**

---

### **✅ Step 6: Start the Virtual Machine**
1. Select your **Kali Linux VM** in VirtualBox.

2. Click **Start.**

3. The VM will boot from the ISO file. Follow the on-screen instructions to install Kali Linux.
