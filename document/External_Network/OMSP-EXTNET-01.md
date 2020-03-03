# [OMSP-EXTNET-01] Cellular Connection
## Description
Any system that needs Internet connectivity in any place and time, must use cellular connectivity technologies (known as 3G, 4G or 5G). More and more elements of vehicles depend on its Internet connection, for example to know the state of the traffic in real-time inside a car or to communicate with a control center in the case of a train. 

However, this Internet connectivity makes these vehicles (that were isolated elements) become potencially reachable from there, increasing the attack surface. 

![OMSP](/images/carmodem.PNG)

Example: Volvo car modem. Source: volvocars.com

## How to Test
When the vehicle need to access the Internet, it stablishes a connection against a base station, similarly to what a smartphone would do. Therefore, the attacks that could be performed against a vehicle would be similar to those against a smartphone, such as base station impersonation or making an IMSI catching attack.

**Rogue Base Station attacks**
* LTE is known to transmit broadcast information in the clear and can be easily sniffed, allowing an attacker to easily configure and set-up a rogue access point. 

## Tools
* [OsmocomBB](http://osmocom.org/projects/baseband/wiki)
* [OsmoBSC](http://osmocom.org/projects/osmobsc/wiki)
* [OsmoMSC](http://osmocom.org/projects/osmomsc/wiki)
* [OsmoHLR](https://osmocom.org/projects/osmo-hlr/wiki/OsmoHLR)

## References

*	["The European Rail Traffic Management System (ERTMS)". Website. 2020](http://www.ertms.net/)
*	["Modelling and Simulation of ERTMS for Current and Future Mobile Technologies". Christian Pinedo and Marina Aguado. International Journal of Vehicular Technology. 2015](https://www.hindawi.com/journals/ijvt/2015/912417/)
*	["Train Topology Discovery Protocol(TTDP) over Dual-Band WLAN-Based Train Communication Network". Shinkwang Kang and Jaehyun Park. The Journal of Korean Institute of Communications and Information Sciences. 2017](http://koreascience.or.kr/article/JAKO201718836884188.page)
