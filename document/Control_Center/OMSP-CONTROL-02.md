# [OMSP-CONTROL-02] Monolithic Control Core
## Description
Monolithic control systems, which use a single main control unit, have been growing in importance over the past decade, taking advantage of the improvement in hardware processing capacity. Manufacturers like Tesla have driven these types of systems, which simplify the manufacturing process greatly. However, most manufacturers have maintained a distributed control architecture based on ECUs.

For example, the main module used in all new Tesla vehicles (which is a Linux based system known as *FSD Computer* or *Hardware 3.0*) includes two custom, 260-sq.-millimeter AI chips. Tesla developed the chips on its own, along with special software designed to complement the hardware. The computer powers the cars self-driving capabilities as well as their advanced in-car "infotainment" system.

![OMSP](/images/TeslaCore.png "")
*Source: https://asia.nikkei.com/*

## How to Test
The tests on these systems will be similar to those in a distributed core: they will be based on port scanning, analysis and exploitation of vulnerable services, elevation of privileges or lateral movement in the network, among others.

## Tools

## References
*	["OVER-THE-AIR: How we remotely compromised the Gateway, BCM and Autopilot ECUs of Tesla cars". Sen Nie, Ling Liu, Yuefeng Du, Wenkai Zhang Keen Security Lab of Tencent. 2016. Blackhat](https://i.blackhat.com/us-18/Thu-August-9/us-18-Liu-Over-The-Air-How-We-Remotely-Compromised-The-Gateway-Bcm-And-Autopilot-Ecus-Of-Tesla-Cars-wp.pdf)
*	["Tesla teardown finds electronics 6 years ahead of Toyota and VW". Nikei Assian Review. 2020](https://asia.nikkei.com/Business/Automobiles/Tesla-teardown-finds-electronics-6-years-ahead-of-Toyota-and-VW2)
