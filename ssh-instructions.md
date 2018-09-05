---
layout: page
title: Instructions to Connect to a Remote Linux Server and Open a Graphical Program
---

Starting with the first bootcamp session it will be necessary for each participant to connect to Adroit and run remote commands.  In later sessions it will be necessary to run graphical programs.  This page details the steps required to install necessary software and test the configuration.  Please make sure to do this ***before*** the bootcamp.  To request an account on Adroit, fill out the [request form](https://forms.rc.princeton.edu/registration/?q=adroit).



### MacOSX ###
1. Install [XQuartz](http://xquartz.macosforge.org/), the official X server software for Mac
1. Run Applications > Utilities > XQuartz.app
1. Right click on the XQuartz icon in the dock and select Applications > Terminal.  This should bring up a new xterm terminal window.
1. In this xterm window, ssh to a linux server using the -Y argument (secure X11 forwarding).  For example, to log into adroit you would do:  
```
ssh -Y <NetID>@adroit.princeton.edu
```
Note that you will need use your normal NetID and password, plus DUO.  If you receive a message like `ssh_exchange_identification: Connection closed by remote host`, you are likely trying to connect from off-campus and will need to [take additional steps](https://researchcomputing.princeton.edu/faq/why-cant-i-login-to-a-clu).
1. Once you are logged in, you can test the xserver is working correctly by opening an xterm window by typing the `xterm` command. A new window should open with a terminal prompt.  If you get a message similar to "Can't open display:" it is not working correctly.

### Windows ###

1. Install [Xming](https://sourceforge.net/projects/xming/).
1. If you do not already have one, install an ssh client. One popular program is putty.exe.  You can download it from the [PuTTY site](http://www.chiark.greenend.org.uk/~sgtatham/putty/).
1. Run Xming on your PC to start the X server.  You should see the Xming icon in the taskbar if it is running (although you may have to click the little arrow in the taskbar to see it)
1. If using PuTTY configure a new connection as follows:
- Enter the server name in Host Name (e.g. adroit.princeton.edu)
- Make sure the Connection type is set to SSH
- Enable X11 forwarding (Connection > SSH > X11)
- Click Open (note if connecting to adroit you'll need to use your normal NetID and password, plus DUO)
- If you receive a message like `ssh_exchange_identification: Connection closed by remote host`, you are likely trying to connect from off-campus and will need to [take additional steps](https://researchcomputing.princeton.edu/faq/why-cant-i-login-to-a-clu).
1. Once you are logged in, you can test the xserver is working correctly by opening an xterm window by typing the `xterm` command.

### Linux ###

1. Everything should already be installed and ready to go.
1. From a new terminal window, ssh to a linux server using the -Y argument (secure X11 forwarding).  For example, to log into adroit you would do:  
```
ssh -Y <NetID>@adroit.princeton.edu
```
Note that you will need use your normal NetID and password, plus DUO. If you receive a message like `ssh_exchange_identification: Connection closed by remote host`, you are likely trying to connect from off-campus and will need to [take additional steps](https://researchcomputing.princeton.edu/faq/why-cant-i-login-to-a-clu).
1. Once you are logged in, you can test the xserver is working correctly by opening an xterm window by typing the `xterm` command. A new window should open with a terminal prompt.  If you get a message similar to "Can't open display:" it is not working correctly.
