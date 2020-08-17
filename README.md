PCB for an a-το-m building block, with:

  * Hexagonal symmetry

  * MCU, maybe ESP8266 (see requirements below)

  * Connectivity to wireless mesh network, maybe ESP-Mesh (to
    communicate with base station)

  * About two dozen programmable LEDs

  * Six IR ports for sending/receiving the ID to/from the connected
    boards (super low bandwidth)

  * Connector for small LiPo battery, allowing the board to run for
    about an hour

  * Stackable charging connectors, as found in disc shaped restaurant
    pagers

  * Booster / Voltage regulator for powering the LEDs and the MCU

  * Charger for the battery

The base station communicates by Wi-Fi with another device, such as a
phone or a PC. For simplicity it may be possible to use the same PCB
as for a block, but with slightly different firmware, and with a
connector for power.

![Rendering showing blocks stacked on base station, with PCB
exposed](rendering.jpg)
