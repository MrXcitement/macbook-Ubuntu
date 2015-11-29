# MacBook 13" Broadcom Wireless Suspend Fix
## Description
MacBook 13" with Ubuntu 15.10 has a problem where after some unknown period of time suspended, the wireless adapter stays off when the laptop resumes from sleep.

## Solution
Add a new sleep script to the power management directory (/etc/pm/sleep.d) to remove the wireless driver on suspend and reload it on resume. This solution was provided at this web site:
http://askubuntu.com/questions/31826/wifi-stops-working-after-waking-from-suspend-with-a-broadcom-43225

## Install

    $ sudo ./install

