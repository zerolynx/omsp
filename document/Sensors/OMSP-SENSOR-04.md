# [OMSP-SENSOR-04] Security Cameras
## Description
One of the most commonly used physical security elements are security cameras. They have been used for many years on board trains to control the actions and identities of passengers.

Currently, cars begin to add these cameras to control the environment while they are not occupied, as well as the state of traffic while they are in circulation (in order to record possible accidents).

![OMSP](/images/jamming.png)

Source: [Mathworks: Barrage Jammer](https://es.mathworks.com/help/phased/ug/barrage-jammer.html)

## How to Test
This control will focus on attacking these cameras to disable them, or avoiding the warning of attempted theft from reaching its destination.

**Jamming attacks**
* Security cameras must be wired to the network to avoid any jamming attack to the system. Wi-Fi and RF cameras are easy to be disabled by a jamming attack.

**Deauth attacks**
* An attacker can send a deauthentication frame at any time to a wireless access point, with a spoofed address of the security camera. 

## Tools
* [ESP8266 Deauther 2.0](https://github.com/spacehuhn/esp8266_deauther): This software allows you to easily perform a variety of actions to test 802.11 wireless networks by using an inexpensive ESP8266 WiFi SoC.
* [HackRF](https://greatscottgadgets.com/hackrf/): Receive and Transmit (Frequency range: 1 MHz and 6 GHz), Half-Duplex.

## References
