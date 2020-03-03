# [OMSP-INTNET-03] Guest Wi-Fi Network
## Description
Many vehicles such as trains or some cars have a guest Wi-Fi network built-in as standard. With it, they can offer Internet through a physical or virtual SIM included in the vehicle itself, or through a connected smartphone. 

It is the manufacturer's responsibility to provide security to these networks with Internet access. They, unlike corporate networks, do not usually have firewalls with traffic inspection, proxies, or other more traditional security measures. Although trains already tend to contemplate this problem, and isolate the guest Wi-Fi network in a different and controlled network segment; in cars, for reasons of space and budget, it is less common. 

## How to Test
Throughout this control the network must be evaluated, testing that a user is prevented from accessing other networks of the vehicle, and that it is not possible to download malicious files, as if it were a corporate wireless network.

**Password protected**
* A robust password should be implemented.

**Access Protocol**
* A robust access protocol should be implemented.

**Wireless Isolation**
* It prevents a device that is connected to the network by a wireless connection from accessing devices and resources that are connected to the network by a wired connection. It will also prevent one wirelessly connected device from connecting to another one.

## Tools
* [Bettercap](https://github.com/bettercap/bettercap)

## References
* ["A Secure Approach to Deploying Wireless Networks". Joseph Matthews. 2016](https://www.sans.org/reading-room/whitepapers/wireless/secure-approach-deploying-wireless-networks-37342)
