1. Find the Local IP Address of Your Plex Server

  Identify the local IP address of the machine hosting Plex.

Example:

  192.168.1.10

  Plex typically runs on port:

  32400

  Your Plex web interface may look like:

  http://192.168.1.10:32400

2. Log in to Your Router

  Open a browser

  Enter your router's gateway address

  Common examples:

  192.168.1.1
  192.168.0.1
  192.168.1.254

  Log in using your router's admin credentials.

3. Locate Port Forwarding Settings

  In your router dashboard, find the Port Forwarding section.

4. Create a Port Forwarding Rule

  Add a new rule with the following settings:

  Setting	Value
  Service Name	Plex
  Protocol	TCP
  External Port	32400
  Internal Port	32400
  Internal IP	Your Plex Server IP (e.g., 192.168.1.10)

Example configuration:

Service: Plex
Protocol: TCP
External Port: 32400
Internal Port: 32400
Internal IP: 192.168.1.10

Save or apply the changes.

5. Verify Remote Access in Plex

Open the Plex web interface

Navigate to:

Settings → Remote Access

Click Enable Remote Access

Plex should confirm that your server is fully accessible outside your network.

Optional: Set a Static IP

To prevent the Plex server's IP address from changing, configure either:
