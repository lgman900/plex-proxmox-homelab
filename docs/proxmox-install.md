Install Proxmox VE
Follow these steps to install Proxmox Virtual Environment (VE) on your machine.

1. Download the Proxmox VE ISO
Download the latest ISO from the official website:
https://www.proxmox.com/en/downloads

2. Install Balena Etcher
Download and install Balena Etcher, which will be used to create the bootable USB drive.
https://etcher.balena.io/

3. Insert a USB Flash Drive
Insert a USB flash drive into your computer (8GB or larger recommended).

4. Create the Bootable USB
Open Balena Etcher
Click Flash from file
Select the Proxmox VE ISO
Click Select target and choose your USB drive
Click Flash to create the bootable installer

5. Insert USB into the Target Machine
Insert the bootable USB drive into the machine where you want to install Proxmox.

6. Connect Ethernet
Connect an Ethernet cable:
One end → Machine
Other end → Router or network switch
A wired connection is recommended for installation.

7. Boot from the USB Drive
Power on the machine
Enter the Boot Manager / BIOS Boot Menu
Select the External USB Drive
The Proxmox installer should start.

8. Complete the Installation
Follow the installer prompts to configure:
Disk installation location
Root password
Email address
Server hostname
Network configuration

If the machine has an active internet connection, some network settings may be auto-detected.

9. Access the Proxmox Web Interface
After installation finishes, the system will reboot and display a console screen with the server IP address.
Example:

https://192.168.1.10:8006

11. Open the Web Console
Open a browser on your laptop or desktop
Enter the server IP address followed by :8006
Example:
https://192.168.1.10:8006
Log in using:

User: root

Password: (the password you created during installation)

You now have access to the Proxmox Web Management Interface.
