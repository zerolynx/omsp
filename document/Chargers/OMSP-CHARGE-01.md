# [OMSP-CHARGE-01] Car
## Description
Some car models synchronize with charging points to exchange information during the charging process, such as price, charge speed and estimated time to finish. This communication is done through short-range protocols, such as Bluetooth. It will be vital to analyze these communications, in order to verify that they are encrypted and cannot be maliciously manipulated.

![OMSP](/images/carcharger.jpg)

## How to Test
**Encrypted communication**
* Information must be encrypted, otherwise the pentester will not need to obtain the certificates and credentials necessary to decrypt the traffic in order to modify the transmitted information. 

**Integrity of transmitted information**
* Integrity of the information must be guaranteed to avoid being modified on "client" side.

## Tools


## References
* ["ISO 15118: Road vehicles - Vehicle grid communication interface. 2019."](https://www.iso.org/obp/ui/#iso:std:iso:15118:-1:ed-2:v1:en)
* ["EV Charging Systems. Security Requirements. 2016"](http://www.nklnederland.nl/kennisloket/wp-content/uploads/2016/10/Security_Requirements_Charge_Points_v1.0_april2016.pdf)
