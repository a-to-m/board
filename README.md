About
=====

*a-το-m* is a construction system which serves as a platform for games
and education. It received the [first price][1] in FabCafe’s *2020
Innovative Game Design Challenge.* Find more about a-το-m by looking
at our [entry to the challenge][2].

This repository is about the PCB for an a-το-m building block.


PCB features
============

  * Hexagonal symmetry.

  * MCU, maybe ESP8266/ESP8285. Tasks:
  
      - Program LEDs (see below).
      
      - Communicate via IR (see below).
      
      - Connect to wireless mesh network, for:
    
          + Sending IDs of connected building blocks to base station.
      
          + Receiving from base station how the LEDs should be
            programmed.

  * A few dozen individually addressable LEDs. Not all of them need to
    be RGB.

  * Six IR ports for sending/receiving the block ID to/from the
    connected blocks (super low bandwidth). In previous similar
    projects, [feklee][4] has done this using his library
    [MultiTrans][3], currently only available for the Arduino.

  * Connector for small LiPo battery, allowing the board to run for
    about an hour.

  * Stackable charging connectors, as found in disc shaped restaurant
    pagers.

  * Booster / Voltage regulator for powering the LEDs and the MCU.

  * Charger for the battery.


Design objectives
=================

For now:

  * Target a production run of 25 building blocks. Then we can test
    the product in the wild, with five sets of five blocks.

  * Design for quick PCBA (if using Seeed Fusion, then use their
    OPLs). That allows us to iterate quickly.
    
  * Prefer ease of development over cost.


Base station
============

The base station communicates by Wi-Fi with another device, such as a
phone or a PC. For simplicity it may be possible to use the same PCB
as for a block, but with slightly different firmware, and with a
connector for power.

![Rendering showing blocks stacked on base station, with PCB
exposed](rendering.jpg)

[1]: https://awrd.com/en/award/game-design-challenge-learning/result
[2]: https://awrd.com/en/creatives/detail/9877896
[3]: https://github.com/feklee/MultiTrans/
[4]: https://github.com/feklee
