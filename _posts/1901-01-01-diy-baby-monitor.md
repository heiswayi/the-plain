---
title: DIY Baby Monitor
updated: 1901-01-01 00:00
---

My wife and I had a need for a couple of camera baby monitors around the house.  She needed one to check in on the kid she nanny's during the day and I needed one to check on our three dogs while both she and I were out of the house.  I looked at getting a purpose built device like this [one](https://www.amazon.com/Motorola-MBP36S-Wireless-Monitor-3-5-Inch/dp/B00M2F0OYS?th=1) but didn't like how much they were (I'd need to buy two) and how it wasn't an open platform (the device only works locally, there'd be no way to access the video feed on a tablet, smartphone, or remotely). A friend of ours suggested that I pick up a pair of cheap [Foscam IP cameras](https://www.amazon.com/Foscam-FI8910W-Network-Camera-Two-Way/dp/B006ZP8UOW) and use an [iPhone App](https://itunes.apple.com/US/app/id511651356?mt=8) to connect to them. The cost and open nature of the interface had me sold... but there was a catch.

This sort of device is [notoriously insecure](http://www.computerworld.com/article/2878741/hacker-hijacks-wireless-foscam-baby-monitor-talks-and-freaks-out-nanny.html) in it's default state.  I needed to get it secured before I could trust in on my local network.

The immediate steps to do all of that were:

1. Update the device to the [latest firmware](http://foscam.us/firmware).

2. Set a non-default username and password on the device.
...![screenshot](/assets/diy-baby-monitor-user-pass.png)

3. Set the device up to use a non-default port.
...![screenshot](/assets/diy-baby-monitor-network-port.png)

Once I had secured the devices themselves, I moved on to setting up a secure way to access the devices remotely via my home router (running [OpenWRT](https://openwrt.org/)):

1. Setup a static DHCP assignment for each of the devices.
...![screenshot](/assets/diy-baby-monitor-static-dhcp.png)

2. Setup port forwarding for each of the devices to the non-standard port.
...![screenshot](/assets/diy-baby-monitor-port-forward.png)

3. Setup a subdomain hostname override in the local DNS settings (this lets the monitoring devices, when connected to my WiFi, to connect to the cameras via the LAN, and not the internet).
...![screenshot](/assets/diy-baby-monitor-hostname-override.png)
The subdomain used also resolves to my router's IP via a wildcard entry in my dynamic DNS zone file.

What I end up with is a baby monitor that uses off the shelf components, is accessible remotely and locally, and doesn't rely on any third party services.
