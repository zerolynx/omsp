# [OMSP-INTNET-04] Bluetooth
## Description
Within the internal network of a vehicle, there are certain sensors and actuators that cannot create a physical data link, either because of their car location or due to motion needs (for example, a sensor located in a wheel). For these cases, data connections must be stablished using a wireless technology that overcomes the restrictions highlighted.  

One of the best technologies that solves these difficulties is Bluetooth. Its range and bandwidth is more than enough to meet any sensor need from anywhere in the car.

## How to Test
Due to the nature of the communication between the sensor and its controller (wireless connections), every attack should be focused on denial of service (known as jamming) or in the impersonation of the sensor. This can be achieved by sending fake data to the controller which could lead into a possible unexpected behavior of the vehicle. 

## Tools

## References
