# Console Port and Rollover Cables

The console port serves as the dedicated entry point for local, "out-of-band" management of networking hardware. Unlike standard network ports used for data transmission, the console port provides a direct, low-level interface to the device's operating system. This is the primary method used by engineers to perform initial configurations, firmware updates, or password recoveries when a device is not yet reachable via the network.

To connect a terminal or a computer to a Cisco console port, a specific type of cabling known as a **rollover cable** is required. Unlike straight-through cables that maintain the same pin mapping on both ends, a rollover cable reverses the pinout completely. It is named for its internal structure, where the wiring is literally "rolled over" from one end to the other.

This reversal is necessary to align the hardware interfaces correctly between the computer’s serial communication (or USB-to-serial adapter) and the Cisco console port’s pin assignments. By reversing the order, the transmit pins on one end are aligned with the receive pins on the other, establishing a functional serial communication link.

The following table illustrates the pin mapping for a standard rollover cable:

| Pin (End A) | Path | Pin (End B) |
| :--- | :--- | :--- |
| 1 | —————— | 8 |
| 2 | —————— | 7 |
| 3 | —————— | 6 |
| 4 | —————— | 5 |
| 5 | —————— | 4 |
| 6 | —————— | 3 |
| 7 | —————— | 2 |
| 8 | —————— | 1 |