# Crossover Cables

A crossover cable is a specific type of twisted-pair cabling designed to connect two identical devices directly, such as connecting two computers to each other or linking two network switches. Unlike a straight-through cable, which maintains the same pinout at both ends, a crossover cable reverses the transmit and receive signal paths.

In the 10BASE-T and 100BASE-T standards, devices use pins 1 and 2 to transmit (Tx) and pins 3 and 6 to receive (Rx). If two identical devices were connected using a standard straight-through cable, both would attempt to transmit on pins 1 and 2 and listen on pins 3 and 6, resulting in a signal collision where no communication could occur. The crossover cable solves this by mapping the transmit pins of one connector to the receive pins of the other, ensuring that data sent from one device arrives at the receiving path of the partner device.

The following illustration demonstrates the crossover pinout required to facilitate communication between two identical network devices.

**Illustration: Crossover Cable Pinout (10/100 Mbps)**

| Pin | Connector A | Path | Connector B |
| :--- | :--- | :--- | :--- |
| 1 | Transmit + | — crosses to — | Receive + |
| 2 | Transmit - | — crosses to — | Receive - |
| 3 | Receive + | — crosses to — | Transmit + |
| 4 | Unused | ———————— | Unused |
| 5 | Unused | ———————— | Unused |
| 6 | Receive - | — crosses to — | Transmit - |
| 7 | Unused | ———————— | Unused |
| 8 | Unused | ———————— | Unused |