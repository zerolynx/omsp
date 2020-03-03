# [OMSP-IFACE-01] Physhical Interfaces
## Description
Traditionally, every human-machine interface has been made using phisical elements as levers or buttons. Although these elements were initially performing mechanical or simple electronic actions (such as activating a power window or turning on a light), today they can be considered as sensors that execute actions within a centralized control system (for example, sending a 'turn on light' instruction that will be processed by the corresponding control system and will generate the 'turn on light' action).

![OMSP](/images/train335.jpg)

Source: trenvista.net

## How to Test
Logic attacks could become possible to be performed on these control systems with some combination of actions that go beyond what is expected in the controller design.

**Replay attacks**
* Systems must have a write protection mechanism to prevent write requests coming from unauthorized nodes in the network.

**Fragmentation attacks**
* Fragmentation attacks are performed by sending specially crafted packets. Some fragmentation attacks are:
  * Ping of Death.
  * TearDrop attack.
  * Zero-Length.
  * Nestea (Linux equivalent to the TearDrop attack)
  * Oshare

## Tools

## References
