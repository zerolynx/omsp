# [OMSP-CONTROL-01] Distributed Control Core
## Description
Distributed control cores are very common in transport systems. For example, a train has several client and server systems within the network(s) that integrate it, usually with specific systems developed on Linux or, to a lesser extent, on Windows or on proprietary systems, which interact with different services. These devices normally support the HMI (Human-Machine Interface), the control panels used by the driver, operators and other employees, to interact with the different control systems involved, as well as all the software logic that supports the operation of the vehicle.

In the case of cars, there is a great heterogeneity. Unconnected cars, usually based on CAN bus networks, do not have clients/servers as they are conceived in traditional IT networks, but have one or more ECUs that handle all the logic. They have software/firmwares developed at a low level in languages such as C; and to access them, a physical level connection is usually needed. In the case of car sharing vehicles, already treated in the control group [OMSP-SHARE](../Car_Sharing_Systems/README.md), new components that incorporate client and server functionalities are usually integrated.

![OMSP](/images/ecu.jpeg "")

Example: VAG group main ECU

## How to Test
The tests on these systems will be based on port scanning, analysis and exploitation of vulnerable services, elevation of privileges or lateral movement in the network, among others.

## Tools

## References
*	["Security Improvements in Connected Cars". Xinju Ji and Hanwi Cheng. University of Gothenburg (Sweden). 2019](https://odr.chalmers.se/bitstream/20.500.12380/300694/1/CSE%2019-86%20ODR%20Ji%20Cheng.pdf)
