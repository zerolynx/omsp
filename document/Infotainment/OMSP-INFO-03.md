# [OMSP-INFO-03] GPS Navigator
## Description
GPS navigators are an indispensable means in today vehicles. Users have been more supportive of the use of external GPS navigators, or the use of their smartphones with application such as Google Maps or Waze, over traditional GPS built-in navigators.

It is increasingly common for vehicles to incorporate this type of GPS navigation software with dynamically updated contents, like traffic, street cuts, current speed, etc.

![OMSP](/images/nmeadatareceived.png)

Source: [Decision support system for collision avoidance at sea. Agnieszka Lazarowska.](https://www.researchgate.net/publication/278123913_Decision_support_system_for_collision_avoidance_at_sea)

## How to Test
In this control, GPS manipulation should be tested trying to modify route destination address, or route itself. Thus altering the normal operation of the system. 

Since GPS data manipulation could be done by different ways, it is necessary to differentiate between:

**GPS Data Level Attacks**
* Data level attacks can vary from modifying pseudo-ranges of satellites in spoofing attacks to produce good, bad and wrong NMEA (National Marine Electronics Association) data trying to crash a receiver.

**GPS Receiver Software Attacks**
* GPS receiver are like computers. Low-end receivers usually run a basic OS stack and simple software. Otherwise, high-end receivers add networking capabilities and complex software. Sofware stack can be compromised, in some cases remotely.

**GPS Dependent System Attacks**
* Higher-level software and systems routinely treat GPS navigation solutions as trusted inputs. An attacker can take advantage of that trust to manipulate positioning, navigation and timing. This kind of attacks can be amplified by manipulating reference stations near the receiver to simulate a real one.

## Tools
* [GPS-SDR-SIM](https://github.com/osqzss/gps-sdr-sim) generates GPS baseband signal data streams, which can be converted to RF using software-defined radio (SDR) platforms, such as ADALM-Pluto, bladeRF, HackRF, and USRP.

## References
* ["All Your GPS Are Belong To Us: Towards Stealthy Manipulation of Road Navigation Systems". Kexion (Curtis) Zeng. ](https://people.cs.vt.edu/gangwang/sec18-gps.pdf)
* ["GPS Software Attacks". Tyler Nighswander. 2012 ](https://users.ece.cmu.edu/~dbrumley/pdf/Nighswander%20et%20al._2012_GPS%20software%20attacks.pdf)
* ["NMEA Reference Manual". Sparkfun.](https://www.sparkfun.com/datasheets/GPS/NMEA%20Reference%20Manual1.pdf)