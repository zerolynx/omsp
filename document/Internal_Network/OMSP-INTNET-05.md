# [OMSP-INTNET-05] Network Electronics
## Description
As in any computer network, the networks of a vehicle require switching devices to interconnect every single element in the topology (control devices, sensors, actuators, etc.). Based on the network structure, these elements might be pretty similar to those that can be found in a common IT network, such as Ethernet RJ-45 switches. On other cases, it could be found similar devices with different connectors, such as industrial Ethernet switches with M12 connectors. Finally, it is possible to find pretty rare connectors (from an IT point of view), like CAN bus gateways. 

## How to Test
These network devices must be protected against unwanted connections either closing unused ports (both physically and logically), setting access passwords to the switches management interfaces or disabling all remote management protocols (SSH, Telnet, HTTP, etc.). 

Following these best practices, physical access will be the only accessing way to the target (with a password policy set). On the other hand, it must be established some control mechanism that ensures the legitimacy of every computer connected to the network.

## Tools

## References