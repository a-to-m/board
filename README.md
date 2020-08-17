PCB for an a-το-m building block, with:

  * Hexagonal symmetry.

  * MCU, maybe ESP8266/ESP8285. Tasks:
  
      - Program LEDs (see below).
      
      - Communicate via IR (see below).
      
      - Connect to wireless mesh network, for:
    
          + Sending IDs of connected building blocks to base station.
      
          + Receiving from base station how the LEDs should be
            programmed.

  * About two dozen programmable LEDs.

  * Six IR ports for sending/receiving the block ID to/from the
    connected blocks (super low bandwidth).

  * Connector for small LiPo battery, allowing the board to run for
    about an hour.

  * Stackable charging connectors, as found in disc shaped restaurant
    pagers.

  * Booster / Voltage regulator for powering the LEDs and the MCU.

  * Charger for the battery.

The base station communicates by Wi-Fi with another device, such as a
phone or a PC. For simplicity it may be possible to use the same PCB
as for a block, but with slightly different firmware, and with a
connector for power.

![Rendering showing blocks stacked on base station, with PCB
exposed](rendering.jpg)
