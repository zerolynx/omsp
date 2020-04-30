# [OMSP-OPCLOSE-04] NFC
## Description
In the same way as the emergence of Bluetooth, the data transmission technology at a very short distance is very useful for opening a vehicle, since it requires the user to be next to the car to open the door, with the security that this entails.

These technologies are usually based on cards that are powered by the vehicle itself when they gets close enough, which allows them to activate a small integrated computer inside them, which will be responsible for authenticating the card owner as the legitimate user of the car.

## How to Test
Attacks against NFC will focus on replicating the behavior of the NFC card in order to open the car with a cloned card.
NFC is a branch of High-Frequency (HF) RFID, and it operates at the 13.56 MHz frequency. Nowadays there are some wellknown attacks to some types of cards:

* Known attacks to MIFARE Classic (1K and 4K):
    * Darkside attack
    * Nested attack
    * Hardnested

* Known attacks to MIFARE DESFire:
    * Side-channel leakage
    
![OMSP](/images/teslakeycard.png)

## Tools
* ["Proxmark 3 RDV4"](https://proxmark.com/): Proxmark 3 RDV4 is the latest revision of the Proxmark 3 Platform. It is designed and manufactured by RRG.
* ["PN532 NFC Module"](https://www.nxp.com/docs/en/nxp/data-sheets/PN532_C1.pdf): One of the most common HF NFC chips built in various readers, also used as a research kit sometimes.

## References
* ["Breaking MIFARE DESFire MF3ICD40: Power Analysis and Templates in the Real World". David Oswald. CHES 2011.](https://www.iacr.org/workshops/ches/ches2011/presentations/Session%205/CHES2011_Session5_1.pdf)
* ["Attacks on the curve-based discrete logarithm problem". Universit´e de Versailles Saint-Quentin, Laboratoire PRiSM. 2011](http://ecc2011.loria.fr/slides/summerschool-vitse.pdf)
* ["A 2018 practical guide to hacking NFC/RFID". Sławomir Jasek. 2018](https://smartlockpicking.com/slides/Confidence_A_2018_Practical_Guide_To_Hacking_RFID_NFC.pdf)
* ["Tesla Key Card Protocol". Robert Quattlebaum. 2020](https://gist.github.com/darconeous/2cd2de11148e3a75685940158bddf933)
