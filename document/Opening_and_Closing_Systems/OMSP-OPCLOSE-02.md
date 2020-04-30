# [OMSP-OPCLOSE-02] Radiofrequency
## Description
Since opening doors using a physical key was a slow and uncomfortable method, a natural transition was made to the use of radio frequency devices to open and close the doors of the vehicle.

In the beginning, this technology had no security so opening a vehicle was as simple as replicating the previously obtained signal. Over the years, different security measures have been established, but logical attacks still appear that manage to unlock access to the vehicle.

In the railway environment it is not common to use this type of technology to open the train doors, since safety reasons prevail over comfort.

## How to Test
**Replay Attacks**

The main idea of this attack is to replay a RF signal by capturing the desired transmission. This attack is done a bit 'blindly' as the attacker does not have enough information about the signal. 

**Relay Station Attacks**

In a similar way, we will focus on Relay Station Attacks. Many cars (connected and non connected) have keyless entry systems. This systems allows the owner to open (and start) their car without using a physical key. This attack use a first device to relay received signals to another device. The attacker should be stand close to the original key (generally, near de front door of the house), and the second device will transmit the relayed signal up to the car. 

![OMSP](/images/relaystationattack.png)

The example below shows a real attack shared by West Midlands Police.

[![Example](/images/relaystationattackexample.png)](https://www.youtube.com/watch?v=8pffcngJJq0)

**Disclaimer**: Be sure to use a faraday bag or cage before transmitting any data so you don’t accidentally break any laws by illegally transmitting on regulated frequencies.

## Tools
* [RTL-SDR](https://www.rtl-sdr.com/buy-rtl-sdr-dvb-t-dongles/): Receive only (Frequency range: 500KHz to 1.75GHz)

* [YARD Stick One](https://greatscottgadgets.com/yardstickone/): Receive and Transmit (Frequency range: 300-348MHz, 391-464MHz, and 782-928MHz), Half-Duplex

* [HackRF](https://greatscottgadgets.com/hackrf/): Receive and Transmit (Frequency range: 1 MHz and 6 GHz), Half-Duplex

* [GNURADIO](https://www.gnuradio.org/): GNU Radio is a free software development toolkit that provides signal processing blocks to implement software-defined radios and signal-processing systems.

![OMSP](/images/gnuradio.png)

Source: [GNURADIO](https://www.gnuradio.org/)

## References
* ["Rolljam Attack. How to hack a car". Gonçalo Nespral. 2019](https://hackaday.io/project/164566-how-to-hack-a-car/details)

* ["How To Replay RF Signals Using SDR". Black Hills Infosec. 2020.](https://www.blackhillsinfosec.com/how-to-replay-rf-signals-using-sdr/)

* ["What is a relay attack (with examples) and how can you prevent them?". Penny Hoelscher. 2019](https://www.comparitech.com/blog/information-security/what-is-relay-attack/)
