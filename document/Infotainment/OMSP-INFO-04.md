# [OMSP-INFO-04] Screen
## Description
Screens allow to manage, by touch or buttons, different system configurations. These elements are intended to fulfill a specific function. Under the premise that any input of the vehicle can assume a potential risk; throughout this control, it will be reviewed that a user cannot access to other resources of the vehicle, taking advantage of, for example, a bad implementation of the desktop presented to the user.

![OMSP](/images/screen.jpg)

Example: Train screen

## How to Test
There are many known cases in which, through a combination of buttons, or interacting with the edges of a touch screen, it is possible to scale to a higher level in the system. These and other tests will be applicable in this control, where the pentester should focus on bypassing the desktop presented to the user.

Supposing interactive and non-interactive screens in the system, the following controls must be performed in order to grant the estability and resilience of the User Interface.

**Buttons**
* Use of buttons should be disabled or restricted in any way that can bypass the main flow of the application.

**Edges**
* Edges of the presented device should not be interactive if it is not needed. 

**Keyboard**
* If the device needs a keyboard, any keyboard shortcuts should restricted if there are not needed in the flow of the application. Similarly, if they keyboard is Android or iOS based, settings of keyboard should not be accessed by the user.

**Alternative connections**
* Any alternative connection present in the screen should be access restricted by default. If access is needed, capabilities of connection should hardened, in order to avoid any malicious activity.

## Tools


## References

