# Pwnbox

![htb screenshot](pwnbox.png?raw=true "Pwnbox")

Want to have your very own pwnbox but don't have VIP?
Create your own!
You can do this all in Parrot OS!

```bash
     ▄▄▄▀▄▄▄
▄▄▀▀▀       ▀▀▄▄▄
█▀▀▄▄         ▄▄▀▀█    █  █         ▐▌     ▄█▄ █          ▄▄▄▄
█    ▀▀▀▄▄▄▀▀▀    █    █▄▄█ ▀▀█ █▀▀ ▐▌▄▀    █  █▀█ █▀█    █▌▄█ ▄▀▀▄ ▀▄▀
█        █        █    █  █ █▄█ █▄▄ ▐█▀▄    █  █ █ █▄▄    █▌▄█ ▀▄▄▀ █▀█
█        █        █
█        █        █    P  E  N   -   T  E  S  T  I  N  G     L  A  B  S
▀▀▄▄     █     ▄▄▀▀
    ▀▀▀▄▄█▄▄▀▀▀
```
## DISCLAIMER
`This has only been done on Parrot OS and is not intended for other systems! Please try so at your own risk`

`p.s: Hackthebox admins. Please don't kill me for making this...`

## Step 1: Open a new Terminal and clone the repo. 

`git clone https://github.com/xxxtentacion/Pwnbox.git`

## Step 2: Start install.sh

`cd Pwnbox`

`chmod +x install.sh`

`./install.sh`

Open a new terminal and then your custom terminal should be there!

> When you connect to your HTB VPN it will appear in your terminal.
---
## Step 3: Selecting theme

Search up "Appearance" in "Menu". Double click "Custom" then click Customize. A new box should appear. Click the "Icons" tab and double click "Pwnbox"


## Step 4: Customising the Panel

On the top panel of your system, right click the three system monitors graphs (the ones with all those lines). Select "Remove from Panel".

### To get the 'ping panel'

Right click on a blank space on the top panel and choose "Add to Panel". In the search bar, type "command", select it and then click add. The time should show on the top panel. Right click on it, click Prefereces and in the command section, paste in `/opt/panel.sh` and change the interval to 5 seconds. It should show "HTB VPN: Disconnected" unless you're on a HTB VPN.

### To get the "processor" menu

Right click on a blank space on the top panel and search for "System monitor". Select it and add it. Right click on the little black box that appeared, select "preferences" and under "System monitor width", update it to "135" pixels, and update "System monitor update interval" "100" milliseconds. Under Monitor Resources. Check Network and Load.

## Step 5: Background

Saving the best for last!

Double click htb.jpg which is inside the github repo we installed. Click the image tab and click "Set as Desktop Background"

## Enjoy!

Hope this tutorial was easy for you!

---

## Common Issues
1.tun0: error fetching interface information: Device not found

This means that you have not connected to hackthebox's VPN. To fix this issue you must connect to the hackthebox vpn or add a # at this line of your .bashrc:

IP=$(ifconfig tun0 | grep "inet " | cut -d " " -f 10)

NOTE: Doing the second one will result in you not being able to see your HTB ip in the terminal.

## More issues?

Report them to any one of these:

Twitter: https://twitter.com/ProjectFeds
Discord Taylor#1337
