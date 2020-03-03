# [OMSP-SHARE-01] Attacks to expansion kits

## Description
In car sharing vehicles, besides the elements that come standard in the vehicle (such as ECUs), there are usually new devices integrated outside the manufacturing process. They are installed with the aim of providing the car with the necessary functionalities for opening/closure, driving, GPS location or emergency call systems.

These new devices, which are connected to the vehicle network (usually CAN bus), have diagnostic devices to read data from the ECU(s), actuators for opening and closing the doors through mobile apps, devices to allow the car to start, which generally work via Bluetooth and require that the key be in a nearby place (e.g. the glove compartment) or displays to show data to the user, with buttons to perform actions defined by the car sharing platform (such as a emergency button). There are many manufacturers that provide this type of kits, so it will be important to access the manuals with the specifications of each of them, before starting the hacking tests.

![OMSP](/images/mk3edr.jpg)

Example: Texa TMD MK3 edr Fleet tracking (Source: ebay.ie)


## How to Test
Among the possible attacks that a pentester could make, the following are presented:

**Attacks to the opening and starting process**
* Impersonation of the physical key. The attacker removes the key without the vehicle having detected it.
* Impersonation of the NFC card to deactivate the circuit breaker.
* Starting the vehicle with the stolen key.

**Bluetooth-ECU interface hijacking**
* Traffic sniffing.
* Command injection.
* Denial of service that generates a possible vehicle stop.

**Resilience against Internet outage**
* Mobile signal inhibition by removing the SIM from the diagnostic unit while the car is running.

## Tools

## References
