1. Get the Windows 11 ISO Download Link
Go to the official Microsoft download page:
https://www.microsoft.com/en-gb/software-download/windows11
Copy the Windows 11 ISO download link.

2. Download the ISO in Proxmox
Log in to the Proxmox Web Console
Navigate to your Node → local storage
Select ISO Images
Click Download from URL
Paste the Windows 11 ISO URL
Click Query URL
Click Download
Wait for the download to complete.

3. Download VirtIO Drivers
VirtIO drivers are required for Windows to detect virtual disks and network devices.
Download the latest VirtIO ISO:
https://fedorapeople.org/groups/virt/virtio-win/direct-downloads/archive-virtio/
Find the latest VirtIO driver ISO
Copy the download link
Repeat Step 11 in Proxmox to download it

4. Create the Virtual Machine
In the top-right corner of the Proxmox console, click Create VM
General Tab
Enter a Name for the VM
OS Tab
Set ISO Image → Windows 11 ISO
Enable Add additional drive for VirtIO drivers
Select the VirtIO driver ISO
Continue through the remaining configuration tabs.
Recommended minimum resources for Plex usage:
Disk: 70–90 GB
RAM: 4 GB minimum (8 GB recommended)
CPU: 2+ cores
Adjust based on your hardware.

5. Start the Virtual Machine
Locate the VM in the left sidebar
Double-click it to open the console
Click Start
The Windows 11 installer should appear.

6. Begin Windows Setup
Proceed through the Windows installer.
When prompted:
Product Key
Select:
I don't have a product key
Windows Edition
Select:
Windows 11 Pro
Continue until Windows asks where to install the OS.

7. Load the VirtIO Storage Driver
If no storage device appears:
Click Load Driver
Accept the EULA
Click Browse
Navigate to:
VirtIO Drivers → amd64 → w11
Click OK
Click Install
The virtual disk should now appear.

8. Install Windows
Select the detected virtual disk
Click Next
Windows will now install and the VM will restart multiple times.

9. Bypass Windows Internet Requirement
When the region selection screen appears:
Press:
Shift + F10
Run the command:
OOBE\BYPASSNRO
The VM will restart.
This enables the "I don't have internet" setup option.

10. Complete Initial Windows Setup
Continue through the Windows setup.
When asked for internet:
Select:
I don't have internet
Finish the setup until you reach the Windows desktop.

11. Install the VirtIO Network Driver
The VM will not have internet until the network driver is installed.
Open Device Manager
Right-click Ethernet Controller
Select Update Driver
Choose Browse my computer for drivers
Navigate to:
VirtIO Drivers → NetKVM → w11 → amd64
Click Next
The driver will install and network connectivity will be enabled.

12. Update Windows
Once internet access is working:
Open Windows Settings
Navigate to Windows Update
Install all available updates
