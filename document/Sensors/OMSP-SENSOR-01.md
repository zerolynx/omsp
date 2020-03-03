# [OMSP-SENSOR-01] Tire-Pressure Monitoring System (TPMS)
## Description
A TPMS is an electronic system designed to monitor the air pressure inside the tires. It reports the tire-pressure to the system. The main goal of a TPMS is avoiding traffic accidents. However, a bad implementation of this protocol could be used to simulate a flat tire, which could lead to a dangerous vehicle stop.

The pentester must check the protocol used is secure and the information transmitted cannot be manipulated.

![OMSP](/images/tpms.jpg)

Source: tirereview.com

## How to Test
The main goal of this control is to simulate fake measures of tire-pressure system in order to alert the driver of a failure in the system.

**Spoofing attacks**
* A spoofing attack consists of emitting a signal in such a way that the receiving system believes that it is communicating with a legitimate system, to which the attacker is supplanting. This signal must be identical at the physical level (frequency, power, etc.) and at the logical level (same protocol, headers, authentication keys if applicable, etc.).

**Jamming attacks**
* A jamming attack consists in inhibiting the legitimate signal of a wireless system through the emission of a random signal (noise) of much greater power and on the same frequency. In this way, the malicious signal "covers" the legitimate one, which cannot be received at destination.

## Tools


## References

* ["TPMS Receiver Hacking". Alexander Arnold and Stephanie Piscitelli. Worcester Polytechnic Institute. 2015](https://web.wpi.edu/Pubs/E-project/Available/E-project-091115-154458/unrestricted/MQP_piscitelli_arnold_2015.pdf)

* ["Security and Privacy Vulnerabilities of In-Car Wireless Networks: A Tire Pressure Monitoring System Case Study. Ishtiaq Rouf. 2010."](https://www.usenix.org/legacy/events/sec10/tech/full_papers/Rouf.pdf)
