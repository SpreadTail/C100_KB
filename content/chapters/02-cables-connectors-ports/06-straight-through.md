# Straight-Through Cables

A **straight-through cable** is the standard cabling configuration used to connect devices of different types, such as connecting a workstation (host) to a network switch. In a straight-through cable, the wire mapping remains consistent across the entire length of the cable; the wire connected to pin 1 on one end of the RJ45 connector is also connected to pin 1 on the other end, and so on.

When operating under the 10BASE-T or 100BASE-T (Fast Ethernet) standards, the transmission process utilizes only two of the four available wire pairs within the UTP cable. One pair is dedicated to transmitting data (Tx), and the second pair is dedicated to receiving data (Rx). The remaining two pairs in the cable are not used for data transmission in these specific older standards, though they are necessary for physical compatibility with the RJ45 interface.

The following illustration demonstrates the concept of the straight-through mapping, where each pin on the Source side corresponds directly to the same pin on the Destination side.

**Illustration: Straight-Through Cable Pinout**

| Pin | Source (RJ45) | Path | Destination (RJ45) |
| :--- | :--- | :--- | :--- |
| 1 | Transmit + | —————————— | Transmit + |
| 2 | Transmit - | —————————— | Transmit - |
| 3 | Receive + | —————————— | Receive + |
| 4 | Unused | —————————— | Unused |
| 5 | Unused | —————————— | Unused |
| 6 | Receive - | —————————— | Receive - |
| 7 | Unused | —————————— | Unused |
| 8 | Unused | —————————— | Unused |