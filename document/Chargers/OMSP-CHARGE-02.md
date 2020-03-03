# [OMSP-CHARGE-02] Charger Points
## Description
The charging point communicates with mobile apps using different protocols. Their security should be checked by acting as a backend server, analyzing network traffic, encryption or sending unexpected data, among other.

![OMSP](/images/charger.png)

## How to Test
**Modify or Disable Power Emergency Settings**
* Power Emergency System must provide resilience to avoid damages to batteries or other EV systems connected.

**Synchronize Timing For Network-Wide Attack**
* This test is capable of create voltage/frequency deviations in the charging process.

**Encrypted communication**
* Information must be encrypted, otherwise the pentester will not need to obtain the certificates and credentials necessary to decrypt the traffic in order to modify the transmitted information. 

**Internet exposure**
* Charger must not be Internet exposed publicly.

## Tools

## References
*	["Charging infrastructure for electric cars: expansion instead of security". Mathias Dalheimer. 34C3. 2018](https://www.youtube.com/watch?v=szYeqOIQ9Bw)
* ["ISO 15118: Road vehicles - Vehicle grid communication interface. 2019."](https://www.iso.org/obp/ui/#iso:std:iso:15118:-1:ed-2:v1:en)
* ["EV Charging Systems. Security Requirements. 2016"](http://www.nklnederland.nl/kennisloket/wp-content/uploads/2016/10/Security_Requirements_Charge_Points_v1.0_april2016.pdf)
