1. Download Plex Media Server

Open a browser in the Windows VM

Go to the official Plex download page:

https://www.plex.tv/media-server-downloads/?cat=computer&plat=windows

Download the Windows version of Plex Media Server.

2. Create Media Folders

Go to your Desktop

Create a folder called Plex

Inside the Plex folder, create two subfolders:

Movies
TV Shows

3. Install Plex Media Server

Run the Plex Media Server installer from the download folder

Click through the installation prompts

4. Open Plex Web Console

Open a browser

Enter the IP address of your VM followed by the Plex port :32400

Example:

http://192.168.1.10:32400
5. Sign in to Plex

On the Plex setup page, sign in or create an account

Enter your server name and check:

Allow me to access my media server from home

Click Next

6. Add Your Media Libraries

In Media Library section, click Add Library

Choose Movies → Browse to the Movies folder you created → Click Add

Repeat for TV Shows → Browse to the TV Shows folder → Click Add

Click through the rest of the setup

7. Add Media

Download or move your favorite movies and TV shows into the corresponding Plex/Movies and Plex/TV Shows folders.

Plex will automatically index and organize the content.

8. Enable Remote Access

In the Plex web console, click the three dots next to your server

Go to:

Settings → Remote Access

Click Enable Remote Access

Your Plex server is now accessible outside your home network (assuming port 32400 is forwarded in your router).
