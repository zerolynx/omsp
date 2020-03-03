# [OMSP-EXTNET-03] Wireless
## Description
Some connected vehicles allow to get connected to wireless networks to access to the Internet, as well as to controlled networks such as a carsharing or logistic base, or a shed in the case of a train. This should be done to synchronize and get different data, as can be updates that would take a lot of time and cost to do using a mobile connection.

Theses wireless receptors, as well as a regular computer, support different technologies such as WEP, WPA or WPA2, and less common, WPA3 and/or RADIUS. 

![OMSP](/images/wireless.png)

Example: Tesla wireless connection.

## How to Test
The pentester will have to check that wireless communications between the vehicle and the access point are safe and that a potential malicious attacker could not take advantage of a protocol weakness to sniff traffic, manipulate it or deny it.

## Tools

## References
*	["Exploiting Wi-Fi Stack on Tesla Model S". Tencent Keen Security Lab. 2020](https://keenlab.tencent.com/en/2020/01/02/exploiting-wifi-stack-on-tesla-model-s/)
