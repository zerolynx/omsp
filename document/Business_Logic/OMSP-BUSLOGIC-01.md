# [OMSP-BUSLOGIC-01] Unexpected behavior

## Description

Unexpected behaviors occur when a system is not designed or prepared to respond to an unknown event. This control aims to integrate all those vulnerabilities that exploit a functionality that was not designed to be triggered in that way.

For example, if a pentester connects a USB device different to a flash drive in a socket of the vehicle, what would happen? Has the programmer considered it? Or was it just developed to look for music on the drive?

## How to Test

The tests for this control are very different, so the pentester will have to be imaginative and put himself in the shoes of the engineer that has developed the vehicle to try to think which kind of actions are the expected ones, and what other options would be feasible to consider as alternative ways of execution. An interesting rule to use is that if the pentester needs to truly understand the business to understand a bug, we may have a business-logic problem.

Sometimes, in a very complex systems (for example, with several ECUs), the pentester will not have a full understanding of every items of the network. In these cases, it is best to have the client walk the pentester through the elements of the vehicle, so that they may knowed functionality of the different components, before the hacking service begins.

![OMSP](/images/keyboard.png "")

## Tools

- [Rubber Ducky](https://shop.hak5.org/products/usb-rubber-ducky-deluxe): Since 2010 the USB Rubber Ducky has been a very usefull tool for  keystroke injection attacks. It has a simple scripting language, formidable hardware, and covert design.
- Keyboards: A useful tool to escape the window of an application, among other functionalities.

## References

* ["CWE Category: Business Logic Errors". Mitre. 2020](https://cwe.mitre.org/data/definitions/840.html)
