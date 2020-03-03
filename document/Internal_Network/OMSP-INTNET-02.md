# [OMSP-INTNET-02] Base Network/CAN bus
## Description

Controller Area Network (CAN bus) is a communications system commonly used in automotive for the interoperation of the different ECUs (Electronic Control Unit) that control the correct operation of the vehicle. Created by Bosch GmbH in 1983, CAN bus has become a standard maintained by the International Organization for Standardization (ISO) through ISO 11898.

![OMSP](/images/canbus.png)

It is a multi-master communication system, based on a synchronous bus (with different speeds). The implementation of the protocol allows the identification of the issuer, thus providing integrity. However, it does not implement addressing or authentication, so that communication occurs in multicast mode.

![OMSP](/images/canframe.png)

By design, the system presents certain problems from the security perspective:

* **Lack of addressing**: although it allows the identification of the sender, there is no addressing implementation and multicast is used in the connection scheme.
* **Lack of authentication**: does not provide authentication between sender and receiver.
* **Lack of encryption**: information is sent in clear text over the CAN bus.
* **Limited bandwidth**: ease of denial of service attacks.
* **Single entry point**: once the bus is accessed, you get access to all the devices connected to it. It should be noted that access is usually through the OBD-II port.

## How to Test
These weaknesses can be exploited by malicious actors:

### Passive attacks

* **Sniffing**: the architecture and implementation of the system allow to read all the messages present in the bus.

### Active attacks (injection of CAN messages)

* **Replay**: An attacker with access to any of the CAN networks (low speed or high speed) could listen to messages and reproduce them.
* **Denial of service**: An attacker with access to the bus could saturate it with multiple messages. Some manufacturer implementations recognize CAN ID 0000 as a high priority and await the release of the bus to dump their messages.
* **Injection of malicious messages**: An attacker with knowledge of the operating logic of the target ECU could inject specially crafted messages into the bus to obtain a known response. This attack could lead to the takeover of critical systems of the car (acceleration, steering, ABS, injection system, electronic immobilizer, solenoid valves, etc.)

Manufacturers, aware of the weaknesses of the protocol and its implementations, try to introduce several security measures:

* **Robust control logic**: ECUs, before executing any changes in actuators of the car, take into account the state of multiple elements/sensors, so that provoking a specific response from a control unit is usually not trivial. Sometimes it becomes necessary to have control of other passive elements such as sensors.
* **Gateway between networks**: some manufacturers already implement several CAN networks separated by criticality and/or network speed (High Speed CAN network vs. Low Speed CAN network). The interconnection between both networks is done through a gateway that can act as a firewall between networks.
* **Security through obscurity**: architecture and implementation of the control logic of the different ECUs are usually proprietary and not easily accessible, which makes reverse engineering tasks difficult.
* **Signed Firmware**: some manufacturers already sign ECU and gateway firmwares to avoid tampering.

## Tools

- [SocketCAN](https://wiki.linklayer.com/index.php/SocketCAN): SocketCAN is a collection of CAN drivers and networking tools for Linux. It allows interfacing with CAN bus devices in a similar fashion as other network devices. This allows for developers to write code that can support a variety of CAN bus interfaces, including CANtact.
- [CANalyzat0r](https://github.com/schutzwerk/CANalyzat0r): This Python software project is built from scratch with new ideas for analysis mechanisms. It’s released on GitHub and bundles many features of other CAN tools in one place. Also, it’s GUI based and organized with one tab per specific analysis task.
- [How to Build a CAN Sniffer (PiCAN2 CAN-Bus Board)](https://www.karambasecurity.com/blog/2018-01-17-how-to-build-a-can-sniffer): PiCAN2 board to provide CAN-Bus capability for the Raspberry Pi.
- [OBDwiz Automotive Diagnostic Software and ScanTool.net OBD-2 Software](https://www.scantool.net/scantool/downloads/diagnostic-software/): OBDwiz is exclusively free for all the OBDLink and ElmScan 5 customers who purchased their scan tool after May 2010.
- [Industrial Ethernet M12 to RJ45](https://www.amazon.com/m12-rj45/s?k=m12+to+rj45): M12 is an industrial type connector, commonly used in environments where robustness is a requirement due to its reliability in connection. Its behaviour is similar to a RJ45 connector. In many trains is used this type of connector, instead of RJ45, so it will be needed to have hoses that convert M12 to RJ45 to be able to connect to Switches and other devices of the train.


## References

*	["0-days & Mitigations: Roadways to Exploit and Secure Connected BMW Cars". Zhiqiang Cai, Aohui Wang, Wenkai Zhang. Blackhat. 2019](https://i.blackhat.com/USA-19/Thursday/us-19-Cai-0-Days-And-Mitigations-Roadways-To-Exploit-And-Secure-Connected-BMW-Cars-wp.pdf)
*	["Automated Reverse Engineering of Automotive CAN Bus Controls". Charles Barron Kirby and Bryson Payne. KSU Conference on Cybersecurity Education. 2019](https://digitalcommons.kennesaw.edu/ccerp/2019/research/5/)
*	["Intrusion prevention system of automotive network CAN bus". Sam Abbott-McCune and Lisa A. Shay. 2016 IEEE International Carnahan Conference on Security Technology (ICCST). 2016, ISBN 978-1-5090-1072-1](https://ieeexplore.ieee.org/abstract/document/7815711)
*	["Developing a CAN Bus-based Secure System for Automotive Module Connectivity". William Hutchinson Putnam III. University of Aizu. 2018](https://bettercan.readthedocs.io/ja/latest/_downloads/MT.pdf)
*	["CAN Bus Wiring Diagram, a Basics Tutorial". Daniel S. Fowler. Tek Eye. 2017](https://tekeye.uk/automotive/can-bus-cable-wiring)
*	["CAN BUS Gaming Simulator". Leon Bataille. Hackaday. 2015](https://hackaday.io/project/6288-can-bus-gaming-simulator)
*	["Train control system using can protocol". Vinay Sunil Dherage and Mick Vaites. 2016](https://www.mintynet.com/car-hack/chv-44con.pdf)
*	["Car Hacking Village. CAN bus basics with hands on fuzzing". Ian Tabor . 2018](https://www.irjet.net/archives/V3/i1/IRJET-V3I1116.pdf)
