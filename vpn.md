# Configuring the VPN for connecting to the LRZ

### Mac Installation
- VPN with Mac OS X
Cisco VPN Client for Mac OS
System requirements:
- OS X 10.11 (El Capitan)

If there are any problems with the AnyConnect client, use the built-in client. A profile for this client is available on the download page.

- OS X 10.10 (Yosemite) , OS X 10.9 (Mavericks) , OS X 10.8 (Mountain Lion) OS X 10.7 (Lion)

Please use the AnyConnect client ( http://www.lrz.de/services/netz/mobil/vpn/anyconnect/ ).

- Mac OS X 10.6 (Snow Leopard).

- Mac OS X 10.6 (Snow Leopard) has a built-in Cisco IPsec client. A profile for this client is available on the download page.

- Mac OS X 10.5 (Leopard) and older:

The Cisco VPN client only runs on the operating system version of Mac OS X 10.1.5. Under the apple there is the menu item About this Mac , with which one can query the version of Mac OS X. For users who still only use Mac OS 9, there is no more client (There was a client of Netlock for $ 114 (as of 08-2003))  

How do I get the VPN client?
The Cisco VPN client and the required lrz.pcf profile can be downloaded from the Leibniz Data Center web server at the following URL: [https://www.lrz.de/services/netz/mobil/vpnclient/] . On this page you have to authenticate yourself with a valid identifier (eg LRZ, MyTUM, CamusLMU) and then get to the download page. Since the installation program is about 14 megabytes in size, we recommend a fast internet connection (estimated download times 56k: 30 min, ISDN: 15 min, DSL: 2 min).  

**Installation of the VPN client:**   
(https://i.imgur.com/6RMI5CL.png)
Double-clicking the mwn-vpnclient-macosx-4.9.01.0180-universal.dmg file (4.9.01.0180 refers to the version number) creates the CiscoVPNClient drive on the Finder Desktop.  

A double-click opens a window containing the installation program (Cisco VPN Client.mpkg) and two folders. Double-clicking Cisco VPN Client.mpkg starts the installation. After installation, the disk image can be ejected and the .dmg file deleted. "  

After authentication to the system, the installation can be started.  

After installation, the Cisco VPN client is in the Applications folder. Double-click to start the VPN client. If there is not the entry lrz, then Profli lrz.pcf , which can be downloaded on the same page as the client can still be installed. To do this extends the window of the VPN client by pressing the keyboard shortcut Command + M . Now you can click the icon Impor t click and lrz.pcf import the file. After pressing Command + M again , the window looks like shown below.  

With the installed profile "LRZ" a secure connection to the VPN server of the Leibniz data center can be established. Click on the profile and choose "Connect".  

After a short negotiation phase, the login mask appears, in which the Internet ID and password must be entered.  

The connection is terminated by clicking on "Disconnect".

 

command line
The client can also be started from the command line

> vpnclient connect lrz

Internet ID and password are queried. The call without parameters provides a short help:

[macclient: ~] vpnclient 
Cisco Systems VPN Client Release 4.9.01 (0030) 
Copyright (C) 1998-2006 Cisco Systems, Inc. All Rights Reserved. 
Client Type (s): Mac OS X 
Running on: Darwin 8.11.0 
Config file directory: / etc / opt / cisco-vpnclient 

Usage: 
```bash
vpnclient connect <profile> [user <username>] [eraseuserpwd | pwd <password>] [nocertpwd] 
vpnclient disconnect 
vpnclient stat [reset] [traffic] [tunnel] [route] [repeat] 
vpnclient notify 
vpnclient verify [autoinitconfig] 
vpnclient autoinit
```
Remove the client

You can remove the client by calling the sudo vpn_uninstall command on the command line.

