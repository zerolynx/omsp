# [OMSP-IFACE-02] Touchscreens
## Description
Touchscreens are more and more used as control interfaces in every environment. In more industrial environments, such as a train, it is a system that has been used for a long time. However, nowadays it is normal to find cars with some kind of touchscreen with which to perform some action in the vehicle.

![OMSP](/images/touchscreen.jpg)

Example: Mercedes. Source: welt.de

## How to Test
A wide range of possible attacks against these interfaces is generated, such as try to perform not allowed actions within the interface environment or perform certain actions to modify different elements.

**WRITE operations protection**
* Any WRITE operation done in the system must be authenticated correctly by a password or a physical key.

**CRITICAL operations protection**
* Any CRITICAL operation done in the system must be authenticated and following the standard procedure. Restart and Shutdown operations are considered critical.

## Tools

## References
